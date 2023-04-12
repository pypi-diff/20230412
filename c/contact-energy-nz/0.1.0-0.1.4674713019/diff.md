# Comparing `tmp/contact-energy-nz-0.1.0.tar.gz` & `tmp/contact-energy-nz-0.1.4674713019.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-energy-nz-0.1.0.tar", last modified: Tue Apr 11 11:51:02 2023, max compression
+gzip compressed data, was "contact-energy-nz-0.1.4674713019.tar", last modified: Wed Apr 12 04:52:02 2023, max compression
```

## Comparing `contact-energy-nz-0.1.0.tar` & `contact-energy-nz-0.1.4674713019.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:51:02.158925 contact-energy-nz-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-11 11:51:02.158925 contact-energy-nz-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:51:02.158925 contact-energy-nz-0.1.0/contact_energy_nz/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/contact_energy_nz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/contact_energy_nz/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/contact_energy_nz/contact_energy_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/contact_energy_nz/usage_datum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:51:02.158925 contact-energy-nz-0.1.0/contact_energy_nz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-11 11:51:02.000000 contact-energy-nz-0.1.0/contact_energy_nz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 11:51:02.000000 contact-energy-nz-0.1.0/contact_energy_nz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:51:02.000000 contact-energy-nz-0.1.0/contact_energy_nz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 11:51:02.000000 contact-energy-nz-0.1.0/contact_energy_nz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:51:02.158925 contact-energy-nz-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:51:02.158925 contact-energy-nz-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 11:50:46.000000 contact-energy-nz-0.1.0/tests/test_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:52:02.158571 contact-energy-nz-0.1.4674713019/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 04:52:02.158571 contact-energy-nz-0.1.4674713019/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:52:02.158571 contact-energy-nz-0.1.4674713019/contact_energy_nz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz/contact_energy_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz/usage_datum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:52:02.158571 contact-energy-nz-0.1.4674713019/contact_energy_nz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 04:52:02.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 04:52:02.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:52:02.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 04:52:02.000000 contact-energy-nz-0.1.4674713019/contact_energy_nz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:52:02.158571 contact-energy-nz-0.1.4674713019/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:52:02.158571 contact-energy-nz-0.1.4674713019/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 04:51:47.000000 contact-energy-nz-0.1.4674713019/tests/test_integration.py
```

### Comparing `contact-energy-nz-0.1.0/LICENSE` & `contact-energy-nz-0.1.4674713019/LICENSE`

 * *Files identical despite different names*

### Comparing `contact-energy-nz-0.1.0/contact_energy_nz/contact_energy_connector.py` & `contact-energy-nz-0.1.4674713019/contact_energy_nz/contact_energy_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,34 +2,32 @@
 API Interface Module
 """
 import datetime
 from typing import Any
 import aiohttp
 import logging
 
-from contact_energy_nz.usage_datum import UsageDatum
-from contact_energy_nz.consts import API_BASE_URL, API_KEY
+from .usage_datum import UsageDatum
+from .consts import API_BASE_URL, API_KEY
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AuthException(Exception):
     """Error to indicate we cannot authenticate to API."""
 
-class ContactEnergyConnector:
+class ContactEnergyApi:
     """Contact Energy auth and data poller."""
 
     def __init__(
         self, username: str = None, password: str = None, token: str = None
     ) -> None:
         self.username = username
         self.password = password
         self.token = token
-        self.accounts = None
-        self.usage = None
         self.contract_id = None
         self.account_id = None
 
     @classmethod
     async def from_credentials(cls, username: str, password: str):
         """Construct instance of ContactEnergyConnector from username and password. Fetches API token"""
         instance = cls(username, password)
@@ -59,74 +57,59 @@
 
         return {
             "x-api-key": API_KEY,
             "session": self.token,
             "authorization": self.token,
         }
 
-    async def _try_fetch_data(self, url) -> Any:
+    async def _try_fetch_data(self, url, method = "get") -> Any:
         try:
             async with aiohttp.ClientSession() as session:
-                async with session.get(url, headers=self._set_headers()) as response:
+                fn = session.get if method == "get" else session.post
+                async with fn(url, headers=self._set_headers()) as response:
                     if response.status == 401:
                         _LOGGER.warning("Unauthorized access: %s", response.reason)
                         raise AuthException(response.reason)
                     elif response.status == 403:
                         _LOGGER.warning("Access forbidden: %s", response.reason)
                         raise AuthException(response.reason)
                     else:
                         return await response.json()
         except aiohttp.ClientError as error:
             _LOGGER.error("Error fetching data from server: %s", error)
             raise
 
     async def account_summary(self):
         """Helper method to query account summary and determine account/contract id"""
-        self.accounts = await self._try_fetch_data(f"{API_BASE_URL}/accounts?ba=")       
-
-    async def get_usage(self) -> list[UsageDatum]:
-        """Query latest available hourly usage stats. These are likely going to always be couple days old"""
-        async with aiohttp.ClientSession() as session:
-            today = datetime.date.today()
-            first_day = today.replace(day=1)
-            last_day = today.replace(
-                day=(
-                    datetime.date(today.year, today.month + 1, 1)
-                    - datetime.timedelta(days=1)
-                ).day
-            )
-
-            formatted_start_date = first_day.strftime("%Y-%m-%d")
-            formatted_end_date = last_day.strftime("%Y-%m-%d")
-            url = f"{API_BASE_URL}/usage/{self.contract_id}?ba={self.account_id}&interval=daily&from={formatted_start_date}&to={formatted_end_date}"
-            async with session.post(url, headers=self._set_headers()) as response:
-                if response.status == 401:
-                    _LOGGER.warning("Unauthorized access: %s", response.reason)
-                    raise AuthException(response.reason)
-                elif response.status == 403:
-                    _LOGGER.warning("Access forbidden: %s", response.reason)
-                    raise AuthException(response.reason)
-                else:
-                    daily_stats = await response.json()
-
-            sorted_daily_stats = sorted(
-                daily_stats, key=lambda x: x["date"], reverse=True
-            )
-            last_available_day = datetime.datetime.strptime(
-                sorted_daily_stats[0]["date"], "%Y-%m-%dT%H:%M:%S.%f%z"
-            )
-            formatted_last_available_day = last_available_day.strftime("%Y-%m-%d")
-
-            url = f"{API_BASE_URL}/usage/{self.contract_id}?ba={self.account_id}&interval=hourly&from={formatted_last_available_day}&to={formatted_last_available_day}"
-            async with session.post(url, headers=self._set_headers()) as response:
-                if response.status == 401:
-                    _LOGGER.warning("Unauthorized access: %s", response.reason)
-                    raise AuthException(response.reason)
-                elif response.status == 403:
-                    _LOGGER.warning("Access forbidden: %s", response.reason)
-                    raise AuthException(response.reason)
-                else:
-                    usage_response = await response.json()
-                    return sorted(
-                        [UsageDatum(item) for item in usage_response],
-                        key=lambda x: x.date,
-                    )
+        accounts = await self._try_fetch_data(f"{API_BASE_URL}/accounts?ba=")       
+        self.account_id = accounts["accountsSummary"][0]["id"]
+        self.contract_id = accounts["accountsSummary"][0]["contracts"][0]["contractId"]
+
+    async def get_latest_usage(self) -> list[UsageDatum]:
+        """Query latest available monthly usage stats"""
+        today = datetime.date.today()
+        first_day = today.replace(day=1)
+        last_day = today.replace(
+            day=(
+                datetime.date(today.year, today.month + 1, 1)
+                - datetime.timedelta(days=1)
+            ).day
+        )
+
+        if first_day > today:
+            raise ValueError("Date cannot be in the future") 
+        
+        return (await self.get_usage(first_day, last_day))[0]
+
+    async def get_usage(self, start_date: datetime, end_date: datetime) -> list[UsageDatum]:
+        """Query monthly usage stats for given range"""
+
+        formatted_start_date = start_date.strftime("%Y-%m-%d")
+        formatted_end_date = end_date.strftime("%Y-%m-%d")
+
+        url = f"{API_BASE_URL}/usage/{self.contract_id}?ba={self.account_id}&interval=monthly&from={formatted_start_date}&to={formatted_end_date}"
+        monthly_stats = await self._try_fetch_data(url, "post")
+        return sorted(
+                    [UsageDatum(item) for item in monthly_stats],
+                    key=lambda x: x.date,
+                    reverse=True
+                )
```

### Comparing `contact-energy-nz-0.1.0/contact_energy_nz/usage_datum.py` & `contact-energy-nz-0.1.4674713019/contact_energy_nz/usage_datum.py`

 * *Files identical despite different names*

### Comparing `contact-energy-nz-0.1.0/pyproject.toml` & `contact-energy-nz-0.1.4674713019/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "contact-energy-nz"
-version = "0.1.0"
+version = "0.1.4674713019"
 description = "API Connector to fetch usage data from Contact Energy NZ utilities provider"
 authors = [
     {name = "Tkhadimullin", email = "hello@wiseowls.co.nz"}
 ]
 license = {text = "MIT"}
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 aiohttp = "^3.7.4"
 
 [tool.poetry.dev-dependencies]
 black = "^21.12b0"
 pylint = "^2.11.1"
 pytest = "^6.2.5"
+pytest-asyncio = "^0.21.0"
 aioresponses = "^0.7.4"
+python-dotenv = "^1.0.0"
 
 [tool.black]
 line-length = 79
 target-version = ['py38']
 
 [tool.pytest]
 testpaths = [
```

