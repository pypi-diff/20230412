# Comparing `tmp/pyhOn-0.7.2.tar.gz` & `tmp/pyhOn-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.7.2.tar", last modified: Wed Apr 12 00:31:42 2023, max compression
+gzip compressed data, was "pyhOn-0.7.3.tar", last modified: Wed Apr 12 17:19:26 2023, max compression
```

## Comparing `pyhOn-0.7.2.tar` & `pyhOn-0.7.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.023563 pyhOn-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 00:31:26.000000 pyhOn-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 00:31:42.023563 pyhOn-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-12 00:31:26.000000 pyhOn-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.019563 pyhOn-0.7.2/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.019563 pyhOn-0.7.2/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.019563 pyhOn-0.7.2/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.023563 pyhOn-0.7.2/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:31:42.023563 pyhOn-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 00:31:26.000000 pyhOn-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 17:19:14.000000 pyhOn-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 17:19:26.305727 pyhOn-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-12 17:19:14.000000 pyhOn-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.301727 pyhOn-0.7.3/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 17:19:26.000000 pyhOn-0.7.3/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:26.305727 pyhOn-0.7.3/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 17:19:14.000000 pyhOn-0.7.3/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:19:26.305727 pyhOn-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 17:19:14.000000 pyhOn-0.7.3/setup.py
```

### Comparing `pyhOn-0.7.2/LICENSE` & `pyhOn-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/PKG-INFO` & `pyhOn-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.2
+Version: 0.7.3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.7.2/README.md` & `pyhOn-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.7.3/pyhOn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.2
+Version: 0.7.3
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.7.2/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.7.3/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/__main__.py` & `pyhOn-0.7.3/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/appliance.py` & `pyhOn-0.7.3/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/appliances/ov.py` & `pyhOn-0.7.3/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/commands.py` & `pyhOn-0.7.3/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/connection/api.py` & `pyhOn-0.7.3/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/connection/auth.py` & `pyhOn-0.7.3/pyhon/connection/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import urllib
 from pprint import pformat
 from urllib import parse
 from urllib.parse import quote
 
 from yarl import URL
 
-from pyhon import const
-from pyhon.exceptions import HonAuthenticationError
+from pyhon import const, exceptions
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class HonAuth:
     def __init__(self, session, email, password, device) -> None:
         self._session = session
@@ -47,15 +46,15 @@
         result = "hOn Authentication Error\n"
         for i, (status, url) in enumerate(self._called_urls):
             result += f" {i + 1: 2d}     {status} - {url}\n"
         result += f"ERROR - {response.status} - {response.request_info.url}\n"
         result += f"{15 * '='} Response {15 * '='}\n{await response.text()}\n{40 * '='}"
         _LOGGER.error(result)
         if fail:
-            raise HonAuthenticationError("Can't login")
+            raise exceptions.HonAuthenticationError("Can't login")
 
     async def _load_login(self):
         nonce = secrets.token_hex(16)
         nonce = f"{nonce[:8]}-{nonce[8:12]}-{nonce[12:16]}-{nonce[16:20]}-{nonce[20:]}"
         params = {
             "response_type": "token+id_token",
             "client_id": const.CLIENT_ID,
@@ -67,15 +66,19 @@
             "nonce": nonce,
         }
         params = "&".join([f"{k}={v}" for k, v in params.items()])
         async with self._session.get(
             f"{const.AUTH_API}/services/oauth2/authorize/expid_Login?{params}"
         ) as response:
             self._called_urls.append((response.status, response.request_info.url))
-            if not (login_url := re.findall("url = '(.+?)'", await response.text())):
+            text = await response.text()
+            if not (login_url := re.findall("url = '(.+?)'", text)):
+                if "oauth/done#access_token=" in text:
+                    self._parse_token_data(text)
+                    raise exceptions.HonNoAuthenticationNeeded()
                 await self._error_logger(response)
                 return False
         async with self._session.get(login_url[0], allow_redirects=False) as redirect1:
             self._called_urls.append((redirect1.status, redirect1.request_info.url))
             if not (url := redirect1.headers.get("Location")):
                 await self._error_logger(redirect1)
                 return False
@@ -152,14 +155,22 @@
                 except KeyError:
                     _LOGGER.error(
                         "Can't get login url - %s", pformat(await response.json())
                     )
             await self._error_logger(response)
             return ""
 
+    def _parse_token_data(self, text):
+        if access_token := re.findall("access_token=(.*?)&", text):
+            self._access_token = access_token[0]
+        if refresh_token := re.findall("refresh_token=(.*?)&", text):
+            self._refresh_token = refresh_token[0]
+        if id_token := re.findall("id_token=(.*?)&", text):
+            self._id_token = id_token[0]
+
     async def _get_token(self, url):
         async with self._session.get(url) as response:
             self._called_urls.append((response.status, response.request_info.url))
             if response.status != 200:
                 await self._error_logger(response)
                 return False
             url = re.findall("href\\s*=\\s*[\"'](.+?)[\"']", await response.text())
@@ -175,34 +186,17 @@
                 url = re.findall("href\\s*=\\s*[\"'](.*?)[\"']", await response.text())
         url = "/".join(const.AUTH_API.split("/")[:-1]) + url[0]
         async with self._session.get(url) as response:
             self._called_urls.append((response.status, response.request_info.url))
             if response.status != 200:
                 await self._error_logger(response)
                 return False
-            text = await response.text()
-        if access_token := re.findall("access_token=(.*?)&", text):
-            self._access_token = access_token[0]
-        if refresh_token := re.findall("refresh_token=(.*?)&", text):
-            self._refresh_token = refresh_token[0]
-        if id_token := re.findall("id_token=(.*?)&", text):
-            self._id_token = id_token[0]
+            self._parse_token_data(await response.text())
         return True
 
-    async def authorize(self):
-        if login_site := await self._load_login():
-            fw_uid, loaded, login_url = login_site
-        else:
-            return False
-        if not (url := await self._login(fw_uid, loaded, login_url)):
-            return False
-        if not await self._get_token(url):
-            return False
-        return await self._api_auth()
-
     async def _api_auth(self):
         post_headers = {"id-token": self._id_token}
         data = self._device.get()
         async with self._session.post(
             f"{const.API_URL}/auth/v1/login", headers=post_headers, json=data
         ) as response:
             self._called_urls.append((response.status, response.request_info.url))
@@ -210,14 +204,28 @@
                 json_data = await response.json()
             except json.JSONDecodeError:
                 await self._error_logger(response)
                 return False
             self._cognito_token = json_data["cognitoUser"]["Token"]
         return True
 
+    async def authenticate(self):
+        self.clear()
+        try:
+            if not (login_site := await self._load_login()):
+                raise exceptions.HonAuthenticationError("Can't open login page")
+            if not (url := await self._login(*login_site)):
+                raise exceptions.HonAuthenticationError("Can't login")
+            if not await self._get_token(url):
+                raise exceptions.HonAuthenticationError("Can't get token")
+            if not await self._api_auth():
+                raise exceptions.HonAuthenticationError("Can't get api token")
+        except exceptions.HonNoAuthenticationNeeded:
+            return
+
     async def refresh(self):
         params = {
             "client_id": const.CLIENT_ID,
             "refresh_token": self._refresh_token,
             "grant_type": "refresh_token",
         }
         async with self._session.post(
@@ -227,7 +235,14 @@
             if response.status >= 400:
                 await self._error_logger(response, fail=False)
                 return False
             data = await response.json()
         self._id_token = data["id_token"]
         self._access_token = data["access_token"]
         return await self._api_auth()
+
+    def clear(self):
+        self._session.cookie_jar.clear_domain(const.AUTH_API.split("/")[-2])
+        self._cognito_token = ""
+        self._id_token = ""
+        self._access_token = ""
+        self._refresh_token = ""
```

### Comparing `pyhOn-0.7.2/pyhon/connection/device.py` & `pyhOn-0.7.3/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/connection/handler.py` & `pyhOn-0.7.3/pyhon/connection/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,36 +53,30 @@
         self._device = HonDevice()
         self._email = email
         self._password = password
         if not self._email:
             raise HonAuthenticationError("An email address must be specified")
         if not self._password:
             raise HonAuthenticationError("A password address must be specified")
-        self._request_headers = {}
 
     @property
     def device(self):
         return self._device
 
     async def create(self):
         await super().create()
         self._auth = HonAuth(self._session, self._email, self._password, self._device)
         return self
 
     async def _check_headers(self, headers):
-        if (
-            "cognito-token" not in self._request_headers
-            or "id-token" not in self._request_headers
-        ):
-            if await self._auth.authorize():
-                self._request_headers["cognito-token"] = self._auth.cognito_token
-                self._request_headers["id-token"] = self._auth.id_token
-            else:
-                raise HonAuthenticationError("Can't login")
-        return self._HEADERS | headers | self._request_headers
+        if not (self._auth.cognito_token and self._auth.id_token):
+            await self._auth.authenticate()
+        headers["cognito-token"] = self._auth.cognito_token
+        headers["id-token"] = self._auth.id_token
+        return self._HEADERS | headers
 
     @asynccontextmanager
     async def _intercept(self, method, *args, loop=0, **kwargs):
         kwargs["headers"] = await self._check_headers(kwargs.get("headers", {}))
         async with method(*args, **kwargs) as response:
             if response.status in [401, 403] and loop == 0:
                 _LOGGER.info("Try refreshing token...")
@@ -94,16 +88,14 @@
             elif response.status in [401, 403] and loop == 1:
                 _LOGGER.warning(
                     "%s - Error %s - %s",
                     response.request_info.url,
                     response.status,
                     await response.text(),
                 )
-                self._request_headers = {}
-                self._session.cookie_jar.clear_domain(const.AUTH_API.split("/")[-2])
                 await self.create()
                 async with self._intercept(
                     method, *args, loop=loop + 1, **kwargs
                 ) as result:
                     yield result
             elif loop >= 2:
                 _LOGGER.error(
```

### Comparing `pyhOn-0.7.2/pyhon/helper.py` & `pyhOn-0.7.3/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/hon.py` & `pyhOn-0.7.3/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/pyhon/parameter.py` & `pyhOn-0.7.3/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.2/setup.py` & `pyhOn-0.7.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.7.2",
+    version="0.7.3",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

