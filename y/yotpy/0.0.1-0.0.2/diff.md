# Comparing `tmp/yotpy-0.0.1.tar.gz` & `tmp/yotpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.1.tar", last modified: Tue Apr 11 19:03:48 2023, max compression
+gzip compressed data, was "yotpy-0.0.2.tar", last modified: Wed Apr 12 00:25:11 2023, max compression
```

## Comparing `yotpy-0.0.1.tar` & `yotpy-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      273 2023-04-11 18:47:43.900956 yotpy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.1/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.1/README.md
--rw-r--r--   0        0        0      739 2023-04-11 18:46:02.090290 yotpy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    27460 2023-04-11 18:55:29.432056 yotpy-0.0.1/yotpy.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 yotpy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      298 2023-04-11 23:24:54.329735 yotpy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.2/LICENSE
+-rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.2/README.md
+-rw-r--r--   0        0        0      739 2023-04-11 18:46:02.090290 yotpy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    28334 2023-04-12 00:22:36.216888 yotpy-0.0.2/yotpy.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 yotpy-0.0.2/PKG-INFO
```

### Comparing `yotpy-0.0.1/LICENSE` & `yotpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.1/pyproject.toml` & `yotpy-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.1/yotpy.py` & `yotpy-0.0.2/yotpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 """
 Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 import asyncio
 import aiohttp
+from json import loads as json_loads
 from csv import DictWriter
 from io import StringIO
 from requests import post as requests_post
-from typing import AsyncGenerator, Iterator, Union
+from typing import AsyncGenerator, Iterator, Union, Optional, Callable, Union
 from html import unescape
 from urllib.parse import urlencode
 from math import ceil
 from itertools import chain
 
 
+class SessionNotCreatedError(Exception):
+    """Raised when the aiohttp.ClientSession has not been created before making a request."""
+    def __init__(self, message="Session not created. Please use `async with` context manager to make requests."):
+        super().__init__(message)
+
+
 class PreflightException(Exception):
     pass
 
 class UploadException(Exception):
     pass
 
 class SendException(Exception):
     pass
 
-
+class CustomException(Exception):
+    pass
 
 # TODO: Refactor naming for the below two classes
 class UserIdNotFound(Exception):
     """Raised when the user ID cannot be retrieved."""
     pass
 
 class AppDataNotFound(Exception):
@@ -318,29 +326,44 @@
     A class for interacting with the Yotpo API to fetch app and account information, review data, and send manual review requests.
 
     The YotpoAPIWrapper uses the provided app_key and secret for authentication and constructs the necessary API endpoints for making requests.
 
     Args:
         app_key (str): The Yotpo app key for API authentication.
         secret (str): The client secret to authenticate requests.
+        preferred_uid (Optional[int], optional): The user ID to use for fetching data relating to the Yotpo APP. Defaults to None.
 
     Raises:
         Exception: If either app_key or secret is not provided.
     """
-    def __init__(self, app_key: str, secret: str) -> None:
+    
+    # TODO: Update the explanation of the preferred_uid argument to be more accurate/helpful.
+
+    def __init__(self, app_key: str, secret: str, preferred_uid: Optional[int] = None) -> None:
         if not app_key or not secret:
             raise Exception(f"app_key(exists={bool(app_key)}) and secret(exists={bool(secret)}) are required.")
         
         self._app_key = app_key
         self._utoken = YotpoAPIWrapper._get_user_token(app_key, secret)
+        self.user_id = preferred_uid
         self.app_endpoint = f"https://api.yotpo.com/v1/apps/{app_key}/reviews?utoken={self._utoken}&"
         self.widget_endpoint = f"https://api.yotpo.com/v1/widget/{app_key}/reviews?utoken={self._utoken}&"
         self.write_user_endpoint = f"https://api-write.yotpo.com/users/me?utoken={self._utoken}"
         self.write_app_endpoint = f"https://api-write.yotpo.com/apps"
 
+    async def __aenter__(self):
+        if self.user_id is None:
+            self.user_id = (await self.get_user())['id']
+
+        self.aiohttp_session = aiohttp.ClientSession()
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.aiohttp_session.close()
+
     @staticmethod
     def _get_user_token(app_key: str, secret: str) -> str:
         """
         Get the user access token using the provided secret.
 
         Args:
             app_key (str): The target app you want authenticated.
@@ -361,91 +384,111 @@
         # TODO: Replace with aiohttp
         response = requests_post(url, data=data)
         if response.ok:
             return response.json()["access_token"]
 
         raise Exception(f"Error: {response.status_code} | {response.reason} - {url}")
 
-    async def _pages(self, endpoint: str, start_page: int = 1) -> AsyncGenerator[tuple[str, int], None]:
+    async def _options_request(self, url: str, method: str) -> bool:
         """
-        Asynchronously generate URLs for each page of results.
+        Asynchronously sends a preflight OPTIONS request to check if the given method is allowed for the given endpoint.
 
         Args:
-            endpoint (str): The API endpoint to query.
-            start_page (int): The first page to generate.
+            url (str): The API endpoint URL.
 
-        Yields:
-            tuple[str, int] ->
-                str: The URL for the next page of results.
-                int: The current page number.
+        Returns:
+            bool: True if the method is allowed, False otherwise.
         """
-        last_page = ceil((await self.get_total_reviews()) / 100)
-        is_widget = "widget" in endpoint
-        for num in range(start_page, last_page + 1):
-            yield endpoint + urlencode(({("per_page" if is_widget else "count"): 100, "page": num})), num
+        if not hasattr(self, 'aiohttp_session'):
+            raise SessionNotCreatedError()
 
-    # TODO: The use of this method is deprecated. Functionality will be replaced `get_total_reviews`. Possible refactor of this method for better abstractions.
-    # NOTE: Keep for reference until major refactoring is complete.
-    # Use of this function is discouraged. `get_total_reviews` is just better all on metrics.
-    async def get_total_pages(self) -> int:
-        """
-        Asynchronously get the total number of pages of results.
+        # Cheeky way to make sure `method` is at least syntactically correct.
+        if (method := method.upper()) not in ['GET', 'HEAD', 'POST', 'PUT', 'DELETE', 'CONNECT', 'OPTIONS', 'TRACE']:
+            raise Exception("Invalid HTTP method: ", method)
 
-        Returns:
-            int: The total number of pages.
-        """
-        url = self.widget_endpoint + urlencode({"per_page": 1, "page": 1})
-        async with aiohttp.request("GET", url) as response:
+        async with self.aiohttp_session.options(url) as response:
             if response.ok:
-                pagination = (await response.json())['response']['pagination']
-                return ceil(pagination['total'] / 100)
+                allowed_methods = response.headers.get("Allow", "")
+                return method in allowed_methods.split(", ")
+            raise Exception(f"Error: {response.status} {response.reason} - {url}")
 
-            raise Exception(
-                f"Error: {response.status} {response.reason} - {url}")
-    
-    async def get_total_reviews(self) -> int:
+    async def _get_request(self, url: str, parser: Callable[[dict], dict] = None, exception_type: Exception = CustomException, **kwargs) -> dict:
         """
-        Asynchronously fetches the total number of reviews for an app.
+        Asynchronously sends a GET request to the specified URL and parses the response using the provided parser.
 
-        This method first retrieves the user and their user ID, then fetches the app data
-        associated with that user. Finally, it returns the total number of reviews for the app.
+        Args:
+            session (aiohttp.ClientSession): An aiohttp client session for making requests.
+            url (str): The URL to send the request to.
+            parser (Callable[[dict], dict]): A function to parse the response JSON. Defaults to json.loads.
+            exception_type (Union[CustomException, Exception]): The type of exception to raise when an error occurs. Defaults to CustomException.
+            **kwargs: Additional keyword arguments to be passed to the request object.
 
         Returns:
-            int: The total number of reviews for the app.
+            dict: The parsed JSON response.
 
         Raises:
-            UserIdNotFound: If unable to get the user ID.
-            AppDataNotFound: If unable to get the app data.
+            exception_type: If the response status is not 200, an instance of the specified exception_type is raised with an error message.
         """
-        if user_id := (await self.get_user()).get("id") is None:
-            raise UserIdNotFound("Error: Unable to get user id.")
+        if not hasattr(self, 'aiohttp_session'):
+            raise SessionNotCreatedError()
 
-        app = await self.get_app(user_id)
+        async with self.aiohttp_session.get(url, **kwargs) as response:
+            if response.status == 200:
+                raw_data = json_loads(await response.read())
+                if parser is None:
+                    return raw_data
+                return parser(raw_data)
+            raise exception_type(f"Error: {response.status} | {response.reason} - {url}")
 
-        return app['data_for_events']['total_reviews']
- 
-    async def _preflight_request(self, url: str, method : str) -> bool:
+    async def _post_request(self, url: str, data: dict, parser: Callable[[dict], dict] = None, exception_type: Exception = CustomException, **kwargs) -> dict:
         """
-        Asynchronously sends a preflight OPTIONS request to check if the given method is allowed for the given endpoint.
+        Asynchronously sends a POST request to the specified URL and parses the response using the provided parser.
 
         Args:
-            url (str): The API endpoint URL.
+            session (aiohttp.ClientSession): An aiohttp client session for making requests.
+            url (str): The URL to send the request to.
+            data (dict): The data to send in the request body.
+            parser (Callable[[dict], dict]): A function to parse the response JSON. Defaults to json.loads.
+            exception_type (Union[CustomException, Exception]): The type of exception to raise when an error occurs. Defaults to CustomException.
+            **kwargs: Additional keyword arguments to be passed to the request object.
 
         Returns:
-            bool: True if the method is allowed, False otherwise.
+            dict: The parsed JSON response.
+
+        Raises:
+            exception_type: If the response status is not 200, an instance of the specified exception_type is raised with an error message.
         """
-        # Cheeky way to make sure `method` is at least syntactically correct.
-        if (method := method.upper()) not in ['GET', 'HEAD', 'POST', 'PUT', 'DELETE', 'CONNECT', 'OPTIONS', 'TRACE']:
-            raise Exception("Invalid HTTP method: ", method)
+        if not hasattr(self, 'aiohttp_session'):
+            raise SessionNotCreatedError()
 
-        async with aiohttp.request(method, url) as response:
-            if response.ok:
-                allowed_methods = response.headers.get("Allow", "")
-                return "POST" in allowed_methods.split(", ")
-            raise Exception(f"Error: {response.status} {response.reason} - {url}")
+        async with self.aiohttp_session.post(url, data=data, **kwargs) as response:
+            if response.status == 200:
+                raw_data = json_loads(await response.read())
+                if parser is None:
+                    return raw_data
+                return parser(raw_data)
+            raise exception_type(f"Error: {response.status} | {response.reason} - {url}")
+
+    async def _pages(self, endpoint: str, start_page: int = 1) -> AsyncGenerator[tuple[str, int], None]:
+        """
+        Asynchronously generate URLs for each page of results.
+
+        Args:
+            endpoint (str): The API endpoint to query.
+            start_page (int): The first page to generate.
+
+        Yields:
+            tuple[str, int] ->
+                str: The URL for the next page of results.
+                int: The current page number.
+        """
+        last_page = ceil((await self.get_total_reviews()) / 100)
+        is_widget = "widget" in endpoint
+        for num in range(start_page, last_page + 1):
+            yield endpoint + urlencode(({("per_page" if is_widget else "count"): 100, "page": num})), num
 
     async def get_user(self) -> dict:
         """
         Asynchronously fetches user data from the user endpoint.
 
         This function returns various user-related data, such as name, email, display_name, company, position, and other
         metadata like sign_in_count and package details. This data can be useful for understanding user profiles,
@@ -456,34 +499,29 @@
 
         Note:
             Mostly you will only need to retrieve the id from the user endpoint, and then use it to fetch the app.
 
         Example:
             ```python
             >>> yotpo = YotpoAPIWrapper(app_key, secret)
-            >>> user_id = (await yotpo.get_user())['id']
-            >>> app = await yotpo.get_app(user_id)
+            >>> async with yotpo as yp:
+            >>>     user_id = (await yp.get_user())['id']
+            >>>     app = await yp.get_app(user_id)
             ```
 
         Raises:
             Exception: If the request to the user endpoint returns a non-OK status.
         """
         url = self.write_user_endpoint
         
-        async with aiohttp.request("GET", url) as response:
-            if response.ok:
-                return (await response.json())['response']['user']
-            raise Exception(f"Error: {response.status} | {response.reason} - {url}")
+        return await self._get_request(url, parser=lambda data: data['response']['user'])
 
-    async def get_app(self, user_id: str | int) -> dict:
+    async def get_app(self) -> dict:
         """
-        Asynchronously fetches app data for the app associated with the given user ID.
-
-        Args:
-            user_id (str | int): The user ID for which to fetch app data.
+        Asynchronously fetches app data for the app associated with the preferred user ID.
 
         Returns:
             dict: A dictionary containing app information derived from the specified user. The app information includes
             details such as app_key, domain, name, url, account type, users, reminders, custom design, created
             and updated timestamps, tracking code status, account emails, package details, enabled product
             categories, features usage summary, data for events, category, installed status, organization,
             and associated apps.
@@ -493,104 +531,89 @@
         """
         # NOTE: The user_id does not appear to actually matter at all, as it still returns data even if it is not a valid user ID.
         # I suspect `user_id` is just used to track which user is making the request.
 
         # TODO: If the above is true, we can probably abstract away the `user_id` parameter and just use the user ID from the user endpoint.
         # And if need be we can add some configuration to allow the user to specify a user ID if they want to.
 
-        url = f"https://api-write.yotpo.com/apps/{self._app_key}?user_id={user_id}&utoken={self._utoken}"
+        url = f"https://api-write.yotpo.com/apps/{self._app_key}?user_id={self.user_id}&utoken={self._utoken}"
 
-        async with aiohttp.request("GET", url) as response:
-            if response.ok:
-                return (await response.json())['response']['app']
-            raise AppDataNotFound(f"Error: {response.status} | {response.reason} - {url}")
-        
-    async def fetch(self, session: aiohttp.ClientSession, url: str, page_num : int) -> list[dict]:
+        return await self._get_request(url, parser=lambda data: data['response']['app'], exception_type=AppDataNotFound)
+
+    async def get_total_reviews(self) -> int:
         """
-        Asynchronously fetch the contents of a URL.
+        Asynchronously fetches the total number of reviews for an app.
 
-        Args:
-            session (aiohttp.ClientSession): The aiohttp client session to use for the request.
-            url (str): The URL to fetch.
-            page_num (int): For tracking purposes.
+        This method first retrieves the user and their user ID, then fetches the app data
+        associated with that user. Finally, it returns the total number of reviews for the app.
 
         Returns:
-            list[dict]: A list of reviews.
+            int: The total number of reviews for the app.
 
         Raises:
-            Exception: If the response status is not 200.
+            UserIdNotFound: If unable to get the user ID.
+            AppDataNotFound: If unable to get the app data.
         """
-        # TODO: Generalize this, so that it can be used for other endpoints.
-        # TODO: Add return parser function as an argument.
-        print(f"Fetching URL: {url}")
-        is_widget = "widget" in url
-        # TODO: remove "page_number" metadata from reviews.
-        # It's use is now deprecated. Remove when convenient.
-        async with session.get(url) as response:
-            if response.status == 200:
-                json = await response.json()
-                page = json['response']['reviews'] if is_widget else json['reviews']
-                return [dict(review, **{"page_number": page_num}) for review in page]
+        if user_id := (await self.get_user()).get("id") is None:
+            raise UserIdNotFound("Error: Unable to get user id.")
 
-            raise Exception(
-                f"Error: {response.status} {response.reason} - {url}")
+        app = await self.get_app(user_id)
 
-    async def batch_fetch(self, endpoint: str, start_page : int = 1) -> list[dict]:
+        return app['data_for_events']['total_reviews']
+    
+    async def get_templates(self) -> dict:
+        user_id = (await self.get_user())['id']
+        app = await self.get_app(user_id)
+        templates = app['account_emails']
+        return templates
+        
+    async def fetch_review_page(self, url: str) -> list[dict]:
         """
-        Asynchronously fetch all pages of results for an API endpoint.
+        Asynchronously fetch the contents of a review URL.
 
         Args:
-            endpoint (str): The API endpoint to query.
-            start_page (int): The first page to generate.
+            url (str): The URL to fetch.
 
         Returns:
-            list: A list of response json and an integer indicating the number of pages queried.
+            list[dict]: A list of reviews.
 
         Raises:
-            Exception: If any response status is not 200.
+            Exception: If the response status is not 200.
         """
-        async with aiohttp.ClientSession() as session:
-            tasks = []
-            async for url, num in self._pages(endpoint, start_page):
-                task = asyncio.create_task(self.fetch(session, url, num))
-                tasks.append(task)
-            results = await asyncio.gather(*tasks, return_exceptions=True)
-            if any([isinstance(result, Exception) for result in results]):
-                raise Exception("One or more requests failed.")
-            else:
-                # Flatten the list of lists into one big list using itertools.chain
-                results = list(chain.from_iterable(results))
-                return results
+        is_widget = "widget" in url
+        return await self._get_request(url, parser=lambda data: data['response']['reviews'] if is_widget else data['reviews'])
 
-    async def _post_request(self, session, url, data, as_form_data=False):
+    async def fetch_all_reviews(self, endpoint: str) -> list[dict]:
         """
-        Send an asynchronous POST request to the specified URL with the given data using the provided aiohttp session, data will be formatted as `aiohttp.FormData` if specified .
+        Asynchronously fetch all the reviews of a given review endpoint.
 
         Args:
-            session (aiohttp.ClientSession): The aiohttp client session to use for sending the request.
-            url (str): The URL to send the POST request to.
-            data (dict): A dictionary containing the data to be sent in the request.
-            as_form_data (bool, optional): Whether or not to format the data as `aiohttp.FormData`. Defaults to False.
+            endpoint (str): The API endpoint to query.
 
         Returns:
-            dict: A dictionary containing the JSON response data.
+            list: A list of response json and an integer indicating the number of pages queried.
 
         Raises:
-            Exception: If the response status code is not 200.
+            Exception: If any response status is not 200.
         """
-        if as_form_data:
-            form_data = aiohttp.FormData()
-            for key, value in data.items():
-                form_data.add_field(key, value)
+        
+        review_requests = []
+        async for url, _ in self._pages(endpoint):
+            task = asyncio.create_task(self.fetch_review_page(url))
+            review_requests.append(task)
+        
+        print(f"Gathering {len(review_requests)} review requests...")
+        results = await asyncio.gather(*review_requests, return_exceptions=True)
 
-        async with session.post(url, data=data) as response:
-            if response.status == 200:
-                return await response.json()
-            else:
-                raise Exception(f"Error: {response.status} {response.reason} - {url}")
+        if any([isinstance(result, Exception) for result in results]):
+            raise Exception("One or more requests failed.")
+        else:
+            # Flatten the list of lists into one big list using itertools.chain
+            results = list(chain.from_iterable(results))
+            return results
     
     async def send_review_request(self, template_id: int | str, csv_stringio: StringIO, spam_check: bool = False):
         """
         Asynchronously send a "manual" review request to Yotpo using a specific email template.
 
         This method takes a template_id, a CSV formatted StringIO object containing the review
         request data, and an optional spam_check flag. It uploads the review data to Yotpo and
@@ -607,19 +630,17 @@
 
         Raises:
             Exception: If any response status is not 200.
             UploadException: If the uploaded file is not valid.
         """
         upload_url = f"{self.write_app_endpoint}/{self._app_key}/account_emails/{template_id}/upload_mailing_list"
         send_url = f"{self.write_app_endpoint}/{self._app_key}/account_emails/{template_id}/send_burst_email"
+        
+        upload_response = await self._post_request(upload_url, {"file": csv_stringio, "utoken": self._utoken})
+        upload_data = upload_response['response']['response']
 
-        async with aiohttp.ClientSession() as session:
-            # Upload data needs to be sent as form data.
-            upload_response = await self._post_request(session, upload_url, {"file": csv_stringio, "utoken": self._utoken}, as_form_data=True)
-            upload_data = upload_response['response']['response']
-
-            if upload_data['is_valid_file']:
-                send_response = await self._post_request(session, send_url, {"file_path": upload_data['file_path'], "utoken": self._utoken, "activate_spam_limitations": spam_check})
-            else:
-                raise UploadException("Error: Uploaded file is not valid")
+        if upload_data['is_valid_file']:
+            send_response = await self._post_request(send_url, {"file_path": upload_data['file_path'], "utoken": self._utoken, "activate_spam_limitations": spam_check})
+        else:
+            raise UploadException("Error: Uploaded file is not valid")
 
         return {"upload": upload_response, "send": send_response}
```

### Comparing `yotpy-0.0.1/PKG-INFO` & `yotpy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

