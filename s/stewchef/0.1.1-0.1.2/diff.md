# Comparing `tmp/stewchef-0.1.1.tar.gz` & `tmp/stewchef-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stewchef-0.1.1.tar", max compression
+gzip compressed data, was "stewchef-0.1.2.tar", max compression
```

## Comparing `stewchef-0.1.1.tar` & `stewchef-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5654 2023-04-11 15:37:45.191398 stewchef-0.1.1/README.md
--rw-r--r--   0        0        0      489 2023-04-11 15:39:30.183809 stewchef-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.1/stewchef/__init__.py
--rw-r--r--   0        0        0    13090 2023-04-11 14:30:19.267721 stewchef-0.1.1/stewchef/main.py
--rw-r--r--   0        0        0     6390 1970-01-01 00:00:00.000000 stewchef-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5654 2023-04-11 15:37:45.191398 stewchef-0.1.2/README.md
+-rw-r--r--   0        0        0      489 2023-04-12 10:20:18.124101 stewchef-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-06 13:20:00.114249 stewchef-0.1.2/stewchef/__init__.py
+-rw-r--r--   0        0        0    13128 2023-04-12 10:17:17.299510 stewchef-0.1.2/stewchef/main.py
+-rw-r--r--   0        0        0     6390 1970-01-01 00:00:00.000000 stewchef-0.1.2/PKG-INFO
```

### Comparing `stewchef-0.1.1/README.md` & `stewchef-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stewchef-0.1.1/stewchef/main.py` & `stewchef-0.1.2/stewchef/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,16 @@
         else:
             pprint(page_contents)
 
         if save:
             # WARNING: IMPORTANT STEP!
             # Set save_path from None to title
 
-            save_path = page_title.replace(" ", "")
+            if save_path is None:
+                save_path = page_title.replace(" ", "")
 
             if as_html:
                 with open(save_path, "w+") as f:
                     f.write(str(BeautifulSoup(page_contents, features="lxml")))
             else:
                 with open(save_path, "w+") as f:
                     f.write(page_contents)
```

### Comparing `stewchef-0.1.1/PKG-INFO` & `stewchef-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stewchef
-Version: 0.1.1
+Version: 0.1.2
 Summary: A MediaWiki API wrapper for RegiSoup
 Author: pengu5055
 Author-email: urbancmarko1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

