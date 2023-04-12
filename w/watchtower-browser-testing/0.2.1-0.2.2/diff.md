# Comparing `tmp/watchtower_browser_testing-0.2.1.tar.gz` & `tmp/watchtower_browser_testing-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.2.1.tar", last modified: Wed Apr 12 10:20:11 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.2.2.tar", last modified: Wed Apr 12 10:28:07 2023, max compression
```

## Comparing `watchtower_browser_testing-0.2.1.tar` & `watchtower_browser_testing-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:20:11.039967 watchtower_browser_testing-0.2.1/
--rw-rw-rw-   0        0        0      310 2023-04-12 10:20:11.039967 watchtower_browser_testing-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 10:20:11.040968 watchtower_browser_testing-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:20:11.031966 watchtower_browser_testing-0.2.1/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      522 2023-04-12 09:47:53.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     9931 2023-04-12 10:19:44.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-12 10:19:44.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:20:11.037966 watchtower_browser_testing-0.2.1/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-12 10:20:10.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-04-12 10:20:10.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:20:10.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 10:20:10.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-12 10:20:10.000000 watchtower_browser_testing-0.2.1/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 10:28:07.303743 watchtower_browser_testing-0.2.2/
+-rw-rw-rw-   0        0        0      310 2023-04-12 10:28:07.302779 watchtower_browser_testing-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:28:07.303743 watchtower_browser_testing-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:28:07.293744 watchtower_browser_testing-0.2.2/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-04-12 09:47:53.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0    10014 2023-04-12 10:27:57.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-12 10:27:57.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:28:07.300742 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.2.1/setup.py` & `watchtower_browser_testing-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.1/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.2.2/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.1/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.2.2/watchtower_browser_testing/testsuite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 import glob
 import importlib.util
 import inspect
 import sys
 import types
+import functools
 
 from playwright.sync_api import sync_playwright
 
 from watchtower_browser_testing.tracking_validation import EventQueue, RequestValidator
 from watchtower_browser_testing import exceptions
 from watchtower_browser_testing import config
 
@@ -70,18 +71,18 @@
             'event': self.event,
             'browser': self.browser,
             'ok': self.ok,
             'errors': self.errors,
             'data': self.data
         }
 
-def new_page_from_gtm(self, *args, **kwargs):
+def new_page_from_gtm(self, ta_page, *args, **kwargs):
 
-    with self.ta_page.expect_popup() as page_info:
-        self.ta_page.get_by_role("button", name="Reopen").click()
+    with ta_page.expect_popup() as page_info:
+        ta_page.get_by_role("button", name="Reopen").click()
     return page_info.value
 
 
 class TrackingTest(object):
 
     browsers = config.DEFAULT_BROWSERS
 
@@ -112,15 +113,16 @@
             self.ta_page = self.context.new_page()
             self.ta_page.goto(gtm_preview_link)
             with self.ta_page.expect_popup() as page_info:
                 self.ta_page.get_by_role("button", name="Connect").click()
             self.page = page_info.value
             self.ta_page.get_by_role("button", name="Continue", exact=True).click()
             self.page.close()
-            self.context.new_page = types.MethodType(new_page_from_gtm, self.context)
+            func = functools.partial(new_page_from_gtm, ta_page=self.ta_page)
+            self.context.new_page = types.MethodType(func, self.context)
 
         else:
             self.browser = self.app.launch(headless=headless)
             self.context = self.browser.new_context()
 
         self.data_context = TestContext()
```

### Comparing `watchtower_browser_testing-0.2.1/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.2.2/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.1/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

