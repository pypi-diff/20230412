# Comparing `tmp/pyhOn-0.7.0.tar.gz` & `tmp/pyhOn-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhOn-0.7.0.tar", last modified: Tue Apr 11 20:20:25 2023, max compression
+gzip compressed data, was "pyhOn-0.7.2.tar", last modified: Wed Apr 12 00:31:42 2023, max compression
```

## Comparing `pyhOn-0.7.0.tar` & `pyhOn-0.7.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 20:20:12.000000 pyhOn-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-11 20:20:25.138927 pyhOn-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-11 20:20:12.000000 pyhOn-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhOn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 20:20:25.000000 pyhOn-0.7.0/pyhOn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhon/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhon/appliances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/ov.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/td.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/wd.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/appliances/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:25.138927 pyhOn-0.7.0/pyhon/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/connection/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/const.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/hon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 20:20:12.000000 pyhOn-0.7.0/pyhon/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:20:25.138927 pyhOn-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 20:20:12.000000 pyhOn-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.023563 pyhOn-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 00:31:26.000000 pyhOn-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 00:31:42.023563 pyhOn-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-12 00:31:26.000000 pyhOn-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.019563 pyhOn-0.7.2/pyhOn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 00:31:42.000000 pyhOn-0.7.2/pyhOn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.019563 pyhOn-0.7.2/pyhon/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.019563 pyhOn-0.7.2/pyhon/appliances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/ov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/td.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/wd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/appliances/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:42.023563 pyhOn-0.7.2/pyhon/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/connection/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/hon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 00:31:26.000000 pyhOn-0.7.2/pyhon/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:31:42.023563 pyhOn-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 00:31:26.000000 pyhOn-0.7.2/setup.py
```

### Comparing `pyhOn-0.7.0/LICENSE` & `pyhOn-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/PKG-INFO` & `pyhOn-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.0
+Version: 0.7.2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.7.0/README.md` & `pyhOn-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhOn.egg-info/PKG-INFO` & `pyhOn-0.7.2/pyhOn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhOn
-Version: 0.7.0
+Version: 0.7.2
 Summary: Control hOn devices with python
 Author: Andre Basche
 License: MIT
 Project-URL: GitHub, https://github.com/Andre0512/pyhOn
 Project-URL: PyPI, https://pypi.org/project/pyhOn
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyhOn-0.7.0/pyhOn.egg-info/SOURCES.txt` & `pyhOn-0.7.2/pyhOn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/__main__.py` & `pyhOn-0.7.2/pyhon/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/appliance.py` & `pyhOn-0.7.2/pyhon/appliance.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/appliances/ov.py` & `pyhOn-0.7.2/pyhon/appliances/ov.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/commands.py` & `pyhOn-0.7.2/pyhon/commands.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/connection/api.py` & `pyhOn-0.7.2/pyhon/connection/api.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/connection/auth.py` & `pyhOn-0.7.2/pyhon/connection/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import re
 import secrets
 import urllib
 from pprint import pformat
 from urllib import parse
+from urllib.parse import quote
 
 from yarl import URL
 
 from pyhon import const
 from pyhon.exceptions import HonAuthenticationError
 
 _LOGGER = logging.getLogger(__name__)
@@ -82,15 +83,17 @@
             self._called_urls.append((redirect2.status, redirect2.request_info.url))
             if not (
                 url := redirect2.headers.get("Location")
                 + "&System=IoT_Mobile_App&RegistrationSubChannel=hOn"
             ):
                 await self._error_logger(redirect2)
                 return False
-        async with self._session.get(URL(url, encoded=True)) as login_screen:
+        async with self._session.get(
+            URL(url, encoded=True), headers={"user-agent": const.USER_AGENT}
+        ) as login_screen:
             self._called_urls.append(
                 (login_screen.status, login_screen.request_info.url)
             )
             if context := re.findall(
                 '"fwuid":"(.*?)","loaded":(\\{.*?})', await login_screen.text()
             ):
                 fw_uid, loaded_str = context[0]
@@ -107,16 +110,16 @@
             "message": {
                 "actions": [
                     {
                         "id": "79;a",
                         "descriptor": "apex://LightningLoginCustomController/ACTION$login",
                         "callingDescriptor": "markup://c:loginForm",
                         "params": {
-                            "username": self._email,
-                            "password": self._password,
+                            "username": quote(self._email),
+                            "password": quote(self._password),
                             "startUrl": parse.unquote(
                                 login_url.split("startURL=")[-1]
                             ).split("%3D")[0],
                         },
                     }
                 ]
             },
```

### Comparing `pyhOn-0.7.0/pyhon/connection/device.py` & `pyhOn-0.7.2/pyhon/connection/device.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/connection/handler.py` & `pyhOn-0.7.2/pyhon/connection/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 from pyhon.exceptions import HonAuthenticationError
 
 
 class HonBaseConnectionHandler:
     _HEADERS = {"user-agent": const.USER_AGENT, "Content-Type": "application/json"}
 
     def __init__(self, session=None):
+        self._create_session = session is None
         self._session = session
         self._auth = None
 
     async def __aenter__(self):
         return await self.create()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
 
     async def create(self):
-        self._session = aiohttp.ClientSession(headers=self._HEADERS)
+        if self._create_session:
+            self._session = aiohttp.ClientSession()
         return self
 
     @asynccontextmanager
     async def _intercept(self, method, *args, loop=0, **kwargs):
         raise NotImplementedError
 
     @asynccontextmanager
@@ -37,15 +39,16 @@
 
     @asynccontextmanager
     async def post(self, *args, **kwargs):
         async with self._intercept(self._session.post, *args, **kwargs) as response:
             yield response
 
     async def close(self):
-        await self._session.close()
+        if self._create_session:
+            await self._session.close()
 
 
 class HonConnectionHandler(HonBaseConnectionHandler):
     def __init__(self, email, password, session=None):
         super().__init__(session=session)
         self._device = HonDevice()
         self._email = email
@@ -71,15 +74,15 @@
             or "id-token" not in self._request_headers
         ):
             if await self._auth.authorize():
                 self._request_headers["cognito-token"] = self._auth.cognito_token
                 self._request_headers["id-token"] = self._auth.id_token
             else:
                 raise HonAuthenticationError("Can't login")
-        return headers | self._request_headers
+        return self._HEADERS | headers | self._request_headers
 
     @asynccontextmanager
     async def _intercept(self, method, *args, loop=0, **kwargs):
         kwargs["headers"] = await self._check_headers(kwargs.get("headers", {}))
         async with method(*args, **kwargs) as response:
             if response.status in [401, 403] and loop == 0:
                 _LOGGER.info("Try refreshing token...")
@@ -91,14 +94,16 @@
             elif response.status in [401, 403] and loop == 1:
                 _LOGGER.warning(
                     "%s - Error %s - %s",
                     response.request_info.url,
                     response.status,
                     await response.text(),
                 )
+                self._request_headers = {}
+                self._session.cookie_jar.clear_domain(const.AUTH_API.split("/")[-2])
                 await self.create()
                 async with self._intercept(
                     method, *args, loop=loop + 1, **kwargs
                 ) as result:
                     yield result
             elif loop >= 2:
                 _LOGGER.error(
```

### Comparing `pyhOn-0.7.0/pyhon/helper.py` & `pyhOn-0.7.2/pyhon/helper.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/hon.py` & `pyhOn-0.7.2/pyhon/hon.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/pyhon/parameter.py` & `pyhOn-0.7.2/pyhon/parameter.py`

 * *Files identical despite different names*

### Comparing `pyhOn-0.7.0/setup.py` & `pyhOn-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyhOn",
-    version="0.7.0",
+    version="0.7.2",
     author="Andre Basche",
     description="Control hOn devices with python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "GitHub": "https://github.com/Andre0512/pyhOn",
         "PyPI": "https://pypi.org/project/pyhOn",
```

