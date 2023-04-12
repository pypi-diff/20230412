# Comparing `tmp/python-ubercode-utils-1.0.2.tar.gz` & `tmp/python-ubercode-utils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-ubercode-utils-1.0.2.tar", last modified: Mon Apr  3 13:15:09 2023, max compression
+gzip compressed data, was "dist/python-ubercode-utils-1.0.3.tar", last modified: Wed Apr 12 21:16:31 2023, max compression
```

## Comparing `python-ubercode-utils-1.0.2.tar` & `python-ubercode-utils-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-03 13:15:09.710726 python-ubercode-utils-1.0.2/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/LICENSE
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       43 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/MANIFEST.in
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-03 13:15:09.710726 python-ubercode-utils-1.0.2/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      683 2023-03-06 19:32:30.000000 python-ubercode-utils-1.0.2/README.md
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-03 13:15:09.706726 python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-03 13:15:09.000000 python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      676 2023-04-03 13:15:09.000000 python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-03 13:15:09.000000 python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-03 13:14:56.000000 python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/not-zip-safe
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        9 2023-04-03 13:15:09.000000 python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/top_level.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2023-04-03 13:15:09.710726 python-ubercode-utils-1.0.2/setup.cfg
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      886 2023-04-03 13:14:05.000000 python-ubercode-utils-1.0.2/setup.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-03 13:15:09.710726 python-ubercode-utils-1.0.2/test/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10392 2023-03-09 18:12:52.000000 python-ubercode-utils-1.0.2/test/test_convert.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2712 2023-03-09 19:13:29.000000 python-ubercode-utils-1.0.2/test/test_cursor.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1088 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/test/test_dataframe.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5379 2023-03-20 19:57:36.000000 python-ubercode-utils-1.0.2/test/test_environment.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     3000 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/test/test_json.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2855 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/test/test_logging.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4865 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/test/test_urls.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2144 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/test/test_xml.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-03 13:15:09.710726 python-ubercode-utils-1.0.2/ubercode/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/ubercode/__init__.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-03 13:15:09.710726 python-ubercode-utils-1.0.2/ubercode/utils/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/ubercode/utils/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9473 2023-04-02 15:21:19.000000 python-ubercode-utils-1.0.2/ubercode/utils/convert.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1118 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/ubercode/utils/cursor.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      870 2023-04-03 13:13:43.000000 python-ubercode-utils-1.0.2/ubercode/utils/dataframe.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9704 2023-03-20 20:57:41.000000 python-ubercode-utils-1.0.2/ubercode/utils/environment.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1630 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/ubercode/utils/json.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9199 2023-03-06 22:18:08.000000 python-ubercode-utils-1.0.2/ubercode/utils/logging.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7240 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/ubercode/utils/urls.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2876 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.2/ubercode/utils/xml.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/LICENSE
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       43 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/MANIFEST.in
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      683 2023-03-06 19:32:30.000000 python-ubercode-utils-1.0.3/README.md
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.680824 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      676 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-12 21:16:18.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        9 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/setup.cfg
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      886 2023-04-12 21:14:02.000000 python-ubercode-utils-1.0.3/setup.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/test/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10392 2023-03-09 18:12:52.000000 python-ubercode-utils-1.0.3/test/test_convert.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2712 2023-03-09 19:13:29.000000 python-ubercode-utils-1.0.3/test/test_cursor.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1088 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_dataframe.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5379 2023-03-20 19:57:36.000000 python-ubercode-utils-1.0.3/test/test_environment.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     3000 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_json.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2855 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_logging.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5139 2023-04-12 21:13:14.000000 python-ubercode-utils-1.0.3/test/test_urls.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2144 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_xml.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/ubercode/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/__init__.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/ubercode/utils/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9473 2023-04-02 15:21:19.000000 python-ubercode-utils-1.0.3/ubercode/utils/convert.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1118 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/cursor.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      870 2023-04-03 13:13:43.000000 python-ubercode-utils-1.0.3/ubercode/utils/dataframe.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9704 2023-03-20 20:57:41.000000 python-ubercode-utils-1.0.3/ubercode/utils/environment.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1630 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/json.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9199 2023-03-06 22:18:08.000000 python-ubercode-utils-1.0.3/ubercode/utils/logging.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7557 2023-04-12 21:11:31.000000 python-ubercode-utils-1.0.3/ubercode/utils/urls.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2876 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/xml.py
```

### Comparing `python-ubercode-utils-1.0.2/LICENSE` & `python-ubercode-utils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/PKG-INFO` & `python-ubercode-utils-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ubercode-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Core python utilities for all apps
 Home-page: https://github.com/sstacha/python-ubercode-utils
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # python-ubercode-utils
         Extracting common python utilities re-used between all projects.  The intent is to have minimal dependencies
```

### Comparing `python-ubercode-utils-1.0.2/README.md` & `python-ubercode-utils-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/PKG-INFO` & `python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ubercode-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Core python utilities for all apps
 Home-page: https://github.com/sstacha/python-ubercode-utils
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # python-ubercode-utils
         Extracting common python utilities re-used between all projects.  The intent is to have minimal dependencies
```

### Comparing `python-ubercode-utils-1.0.2/python_ubercode_utils.egg-info/SOURCES.txt` & `python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/setup.py` & `python-ubercode-utils-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='python-ubercode-utils',
-      version='1.0.2',
+      version='1.0.3',
       description='Core python utilities for all apps',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/sstacha/python-ubercode-utils',
       author='Steve Stacha',
       author_email='sstacha@gmail.com',
       license='MIT',
```

### Comparing `python-ubercode-utils-1.0.2/test/test_convert.py` & `python-ubercode-utils-1.0.3/test/test_convert.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/test/test_cursor.py` & `python-ubercode-utils-1.0.3/test/test_cursor.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/test/test_dataframe.py` & `python-ubercode-utils-1.0.3/test/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/test/test_environment.py` & `python-ubercode-utils-1.0.3/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/test/test_json.py` & `python-ubercode-utils-1.0.3/test/test_json.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/test/test_logging.py` & `python-ubercode-utils-1.0.3/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/test/test_urls.py` & `python-ubercode-utils-1.0.3/test/test_urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 from contextlib import redirect_stdout
 from io import StringIO
 
 from ubercode.utils.urls import ParsedUrl
+from ubercode.utils.urls import ParsedQueryString
 
 
 class TestUrls(unittest.TestCase):
 
     # -------- ParsedUrl class ----------
 
     # --- constructor defaults
@@ -83,11 +84,16 @@
         # test updates if there
         parsed_url.set_param("u", "2")
         self.assertEqual("//test.local.net:8000/test/index.html?z=1&u=2&v=4#test2", str(parsed_url))
         # test removing a param
         parsed_url.del_param("u")
         self.assertEqual("//test.local.net:8000/test/index.html?z=1&v=4#test2", str(parsed_url))
 
+        # bugfix #1: test that we don't truncate data if there is an = in the data
+        test_qs = "id=1&b=2&x=1234=56&z=3"
+        parsed_qs = ParsedQueryString(test_qs)
+        self.assertEqual(test_qs, str(parsed_qs))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-ubercode-utils-1.0.2/test/test_xml.py` & `python-ubercode-utils-1.0.3/test/test_xml.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/convert.py` & `python-ubercode-utils-1.0.3/ubercode/utils/convert.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/cursor.py` & `python-ubercode-utils-1.0.3/ubercode/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/dataframe.py` & `python-ubercode-utils-1.0.3/ubercode/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/environment.py` & `python-ubercode-utils-1.0.3/ubercode/utils/environment.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/json.py` & `python-ubercode-utils-1.0.3/ubercode/utils/json.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/logging.py` & `python-ubercode-utils-1.0.3/ubercode/utils/logging.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/urls.py` & `python-ubercode-utils-1.0.3/ubercode/utils/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 from urllib.parse import urlsplit
+from ubercode.utils.convert import to_str
 
 
 class ParsedQueryString:
     """
     Encapsulates the parsing and setting of query string parameters
     """
     def __init__(self, query_string):
@@ -12,17 +13,27 @@
         # strip off the ? if still there
         if self.qs.startswith("?"):
             self.qs = self.qs[1:]
         # split each param based on & (should be x=xval, y=yval etc)
         exp_params = self.qs.split("&")
         self.params = {}
         for exp_param in exp_params:
-            items = exp_param.split("=")
-            if len(items) >= 2:
-                self.params[items[0]] = items[1]
+            param = to_str(exp_param)
+            key = ""
+            value = ""
+            pos = param.find("=")
+            if pos > -1:
+                key = param[:pos]
+                if len(param) > pos + 1:
+                    value = param[pos + 1:]
+            else:
+                if param:
+                    key = param
+            if key:
+                self.params[key] = value
 
     def __str__(self):
         """
         By default, the query string will be the params dict put back together without the ?
         :return:
         """
         qs = ""
```

### Comparing `python-ubercode-utils-1.0.2/ubercode/utils/xml.py` & `python-ubercode-utils-1.0.3/ubercode/utils/xml.py`

 * *Files identical despite different names*

