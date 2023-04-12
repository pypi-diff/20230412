# Comparing `tmp/yotpy-0.0.2.tar.gz` & `tmp/yotpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.2.tar", last modified: Wed Apr 12 00:25:11 2023, max compression
+gzip compressed data, was "yotpy-0.0.4.tar", last modified: Wed Apr 12 01:04:32 2023, max compression
```

## Comparing `yotpy-0.0.2.tar` & `yotpy-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      298 2023-04-11 23:24:54.329735 yotpy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.2/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.2/README.md
--rw-r--r--   0        0        0      739 2023-04-11 18:46:02.090290 yotpy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    28334 2023-04-12 00:22:36.216888 yotpy-0.0.2/yotpy.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 yotpy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      298 2023-04-12 00:26:21.499743 yotpy-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.4/LICENSE
+-rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.4/README.md
+-rw-r--r--   0        0        0      739 2023-04-11 18:46:02.090290 yotpy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    28570 2023-04-12 01:03:49.147051 yotpy-0.0.4/yotpy.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 yotpy-0.0.4/PKG-INFO
```

### Comparing `yotpy-0.0.2/LICENSE` & `yotpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.2/pyproject.toml` & `yotpy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.2/yotpy.py` & `yotpy-0.0.4/yotpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 """
 
-__version__ = "0.0.2"
+__version__ = "0.0.4"
 
 import asyncio
 import aiohttp
 from json import loads as json_loads
 from csv import DictWriter
 from io import StringIO
 from requests import post as requests_post
@@ -339,33 +339,35 @@
     # TODO: Update the explanation of the preferred_uid argument to be more accurate/helpful.
 
     def __init__(self, app_key: str, secret: str, preferred_uid: Optional[int] = None) -> None:
         if not app_key or not secret:
             raise Exception(f"app_key(exists={bool(app_key)}) and secret(exists={bool(secret)}) are required.")
         
         self._app_key = app_key
-        self._utoken = YotpoAPIWrapper._get_user_token(app_key, secret)
+        self._secret = secret
         self.user_id = preferred_uid
-        self.app_endpoint = f"https://api.yotpo.com/v1/apps/{app_key}/reviews?utoken={self._utoken}&"
-        self.widget_endpoint = f"https://api.yotpo.com/v1/widget/{app_key}/reviews?utoken={self._utoken}&"
+
+    async def __aenter__(self):
+        self.aiohttp_session = aiohttp.ClientSession()
+        self._utoken = await self._get_user_token()
+
+        self.app_endpoint = f"https://api.yotpo.com/v1/apps/{self._app_key}/reviews?utoken={self._utoken}&"
+        self.widget_endpoint = f"https://api.yotpo.com/v1/widget/{self._app_key}/reviews?utoken={self._utoken}&"
         self.write_user_endpoint = f"https://api-write.yotpo.com/users/me?utoken={self._utoken}"
         self.write_app_endpoint = f"https://api-write.yotpo.com/apps"
 
-    async def __aenter__(self):
         if self.user_id is None:
             self.user_id = (await self.get_user())['id']
 
-        self.aiohttp_session = aiohttp.ClientSession()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.aiohttp_session.close()
 
-    @staticmethod
-    def _get_user_token(app_key: str, secret: str) -> str:
+    async def _get_user_token(self) -> str:
         """
         Get the user access token using the provided secret.
 
         Args:
             app_key (str): The target app you want authenticated.
             secret (str): The client secret to authenticate the request.
 
@@ -374,23 +376,19 @@
 
         Raises:
             Exception: If the response status is not OK (200).
         """
         url = "https://api.yotpo.com/oauth/token"
         data = {
             "grant_type": "client_credentials",
-            "client_id": app_key,
-            "client_secret": secret,
+            "client_id": self._app_key,
+            "client_secret": self._secret,
         }
-        # TODO: Replace with aiohttp
-        response = requests_post(url, data=data)
-        if response.ok:
-            return response.json()["access_token"]
 
-        raise Exception(f"Error: {response.status_code} | {response.reason} - {url}")
+        return (await self._post_request(url, data=data, parser=lambda x: x["access_token"]))
 
     async def _options_request(self, url: str, method: str) -> bool:
         """
         Asynchronously sends a preflight OPTIONS request to check if the given method is allowed for the given endpoint.
 
         Args:
             url (str): The API endpoint URL.
@@ -493,23 +491,20 @@
         This function returns various user-related data, such as name, email, display_name, company, position, and other
         metadata like sign_in_count and package details. This data can be useful for understanding user profiles,
         managing access, or customizing the user experience based on the retrieved information.
 
         Returns:
             dict: A dictionary containing user information, including personal details, activity statistics, and package details.
 
-        Note:
-            Mostly you will only need to retrieve the id from the user endpoint, and then use it to fetch the app.
 
         Example:
             ```python
             >>> yotpo = YotpoAPIWrapper(app_key, secret)
             >>> async with yotpo as yp:
-            >>>     user_id = (await yp.get_user())['id']
-            >>>     app = await yp.get_app(user_id)
+            >>>     user = await yp.get_user()
             ```
 
         Raises:
             Exception: If the request to the user endpoint returns a non-OK status.
         """
         url = self.write_user_endpoint
         
@@ -546,75 +541,82 @@
         This method first retrieves the user and their user ID, then fetches the app data
         associated with that user. Finally, it returns the total number of reviews for the app.
 
         Returns:
             int: The total number of reviews for the app.
 
         Raises:
-            UserIdNotFound: If unable to get the user ID.
             AppDataNotFound: If unable to get the app data.
         """
-        if user_id := (await self.get_user()).get("id") is None:
-            raise UserIdNotFound("Error: Unable to get user id.")
-
-        app = await self.get_app(user_id)
+        app = await self.get_app()
 
         return app['data_for_events']['total_reviews']
     
     async def get_templates(self) -> dict:
-        user_id = (await self.get_user())['id']
-        app = await self.get_app(user_id)
+        app = await self.get_app()
         templates = app['account_emails']
         return templates
         
     async def fetch_review_page(self, url: str) -> list[dict]:
         """
-        Asynchronously fetch the contents of a review URL.
+        Asynchronously fetch a single review page from the specified URL.
+
+        This function fetches review data from the provided URL and parses the response based on whether
+        the URL is for the widget endpoint or not.
 
         Args:
-            url (str): The URL to fetch.
+            url (str): The URL from which to fetch review data.
 
         Returns:
-            list[dict]: A list of reviews.
+            list[dict]: A list of review dictionaries.
 
-        Raises:
-            Exception: If the response status is not 200.
         """
         is_widget = "widget" in url
         return await self._get_request(url, parser=lambda data: data['response']['reviews'] if is_widget else data['reviews'])
 
-    async def fetch_all_reviews(self, endpoint: str) -> list[dict]:
+
+    async def fetch_all_reviews(self, published: bool = True) -> list[dict]:
         """
-        Asynchronously fetch all the reviews of a given review endpoint.
+        Asynchronously fetch all reviews from the specified endpoints.
+
+        This function fetches review data from the app and widget endpoints if `published` is set to True, 
+        and only from the app endpoint if `published` is set to False. The fetched reviews are then merged
+        based on their "id" attribute.
 
         Args:
-            endpoint (str): The API endpoint to query.
+            published (bool, optional): Determines if the function should fetch reviews from both
+                                         the app and widget endpoints or just the app endpoint.
+                                         Defaults to True.
 
         Returns:
-            list: A list of response json and an integer indicating the number of pages queried.
+            list[dict]: A list of merged review dictionaries.
 
         Raises:
-            Exception: If any response status is not 200.
+            Exception: If one or more requests fail.
         """
-        
-        review_requests = []
-        async for url, _ in self._pages(endpoint):
-            task = asyncio.create_task(self.fetch_review_page(url))
-            review_requests.append(task)
-        
-        print(f"Gathering {len(review_requests)} review requests...")
-        results = await asyncio.gather(*review_requests, return_exceptions=True)
+        reviews = []
+        for endpoint in ([self.app_endpoint, self.widget_endpoint] if published else [self.app_endpoint]):
+            review_requests = []
+            async for url, _ in self._pages(endpoint):
+                task = asyncio.create_task(self.fetch_review_page(url))
+                review_requests.append(task)
+            
+            print(f"Gathering {len(review_requests)} review requests from {endpoint}...")
+            results = await asyncio.gather(*review_requests, return_exceptions=True)
 
-        if any([isinstance(result, Exception) for result in results]):
-            raise Exception("One or more requests failed.")
-        else:
-            # Flatten the list of lists into one big list using itertools.chain
-            results = list(chain.from_iterable(results))
-            return results
-    
+            if any([isinstance(result, Exception) for result in results]):
+                raise Exception("One or more requests failed.")
+            else:
+                # Flatten the list of lists into one big list using itertools.chain
+                results = list(chain.from_iterable(results))
+                reviews.append(results)
+            
+        return JSONTransformer.merge_on_key("id", *reviews)
+
+        
     async def send_review_request(self, template_id: int | str, csv_stringio: StringIO, spam_check: bool = False):
         """
         Asynchronously send a "manual" review request to Yotpo using a specific email template.
 
         This method takes a template_id, a CSV formatted StringIO object containing the review
         request data, and an optional spam_check flag. It uploads the review data to Yotpo and
         sends the review request using the specified email template.
```

### Comparing `yotpy-0.0.2/PKG-INFO` & `yotpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.2
+Version: 0.0.4
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

