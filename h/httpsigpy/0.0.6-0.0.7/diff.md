# Comparing `tmp/httpsigpy-0.0.6.tar.gz` & `tmp/httpsigpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpsigpy-0.0.6.tar", last modified: Fri Aug 26 02:05:48 2022, max compression
+gzip compressed data, was "httpsigpy-0.0.7.tar", last modified: Wed Apr 12 18:21:21 2023, max compression
```

## Comparing `httpsigpy-0.0.6.tar` & `httpsigpy-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jricher    (501) staff       (20)        0 2022-08-26 02:05:48.306159 httpsigpy-0.0.6/
--rw-r--r--   0 jricher    (501) staff       (20)     1090 2022-05-08 09:29:12.000000 httpsigpy-0.0.6/LICENSE
--rw-r--r--   0 jricher    (501) staff       (20)     2965 2022-08-26 02:05:48.305941 httpsigpy-0.0.6/PKG-INFO
--rw-r--r--   0 jricher    (501) staff       (20)     2539 2022-07-27 17:33:16.000000 httpsigpy-0.0.6/README.md
-drwxr-xr-x   0 jricher    (501) staff       (20)        0 2022-08-26 02:05:48.304505 httpsigpy-0.0.6/httpsig/
--rw-r--r--   0 jricher    (501) staff       (20)    15060 2022-08-26 01:54:21.000000 httpsigpy-0.0.6/httpsig/__init__.py
-drwxr-xr-x   0 jricher    (501) staff       (20)        0 2022-08-26 02:05:48.305620 httpsigpy-0.0.6/httpsigpy.egg-info/
--rw-r--r--   0 jricher    (501) staff       (20)     2965 2022-08-26 02:05:48.000000 httpsigpy-0.0.6/httpsigpy.egg-info/PKG-INFO
--rw-r--r--   0 jricher    (501) staff       (20)      178 2022-08-26 02:05:48.000000 httpsigpy-0.0.6/httpsigpy.egg-info/SOURCES.txt
--rw-r--r--   0 jricher    (501) staff       (20)        1 2022-08-26 02:05:48.000000 httpsigpy-0.0.6/httpsigpy.egg-info/dependency_links.txt
--rw-r--r--   0 jricher    (501) staff       (20)        8 2022-08-26 02:05:48.000000 httpsigpy-0.0.6/httpsigpy.egg-info/top_level.txt
--rw-r--r--   0 jricher    (501) staff       (20)       38 2022-08-26 02:05:48.306231 httpsigpy-0.0.6/setup.cfg
--rw-r--r--   0 jricher    (501) staff       (20)      641 2022-08-25 21:52:30.000000 httpsigpy-0.0.6/setup.py
+drwxr-xr-x   0 jricher    (501) staff       (20)        0 2023-04-12 18:21:21.149460 httpsigpy-0.0.7/
+-rw-r--r--   0 jricher    (501) staff       (20)     1090 2022-05-08 09:29:12.000000 httpsigpy-0.0.7/LICENSE
+-rw-r--r--   0 jricher    (501) staff       (20)     2965 2023-04-12 18:21:21.149179 httpsigpy-0.0.7/PKG-INFO
+-rw-r--r--   0 jricher    (501) staff       (20)     2539 2022-07-27 17:33:16.000000 httpsigpy-0.0.7/README.md
+drwxr-xr-x   0 jricher    (501) staff       (20)        0 2023-04-12 18:21:21.147542 httpsigpy-0.0.7/httpsig/
+-rw-r--r--   0 jricher    (501) staff       (20)    14678 2023-04-12 18:16:47.000000 httpsigpy-0.0.7/httpsig/__init__.py
+drwxr-xr-x   0 jricher    (501) staff       (20)        0 2023-04-12 18:21:21.148870 httpsigpy-0.0.7/httpsigpy.egg-info/
+-rw-r--r--   0 jricher    (501) staff       (20)     2965 2023-04-12 18:21:21.000000 httpsigpy-0.0.7/httpsigpy.egg-info/PKG-INFO
+-rw-r--r--   0 jricher    (501) staff       (20)      178 2023-04-12 18:21:21.000000 httpsigpy-0.0.7/httpsigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jricher    (501) staff       (20)        1 2023-04-12 18:21:21.000000 httpsigpy-0.0.7/httpsigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jricher    (501) staff       (20)        8 2023-04-12 18:21:21.000000 httpsigpy-0.0.7/httpsigpy.egg-info/top_level.txt
+-rw-r--r--   0 jricher    (501) staff       (20)       38 2023-04-12 18:21:21.149536 httpsigpy-0.0.7/setup.cfg
+-rw-r--r--   0 jricher    (501) staff       (20)      641 2023-04-12 17:30:39.000000 httpsigpy-0.0.7/setup.py
```

### Comparing `httpsigpy-0.0.6/LICENSE` & `httpsigpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `httpsigpy-0.0.6/PKG-INFO` & `httpsigpy-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpsigpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: HTTP Message Signatures
 Home-page: https://github.com/bspkio/httpsigpy
 Author: Justin Richer
 Author-email: python@justin.richer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `httpsigpy-0.0.6/README.md` & `httpsigpy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `httpsigpy-0.0.6/httpsig/__init__.py` & `httpsigpy-0.0.7/httpsig/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 try:
     from http_parser.parser import HttpParser
 except ImportError:
     from http_parser.pyparser import HttpParser
 
 import http_sfv
-from urllib.parse import parse_qs
+from urllib.parse import parse_qs, quote
 import base64
 from Cryptodome.Signature import pss
 from Cryptodome.Signature import pkcs1_15
 from Cryptodome.Signature import DSS
 from Cryptodome.Hash import SHA512
 from Cryptodome.Hash import SHA256
 from Cryptodome.Hash import HMAC
@@ -232,32 +232,20 @@
                 cid = http_sfv.Item('@query-param')
                 cid.params['name'] = q
                 response['derived'].append(
                     {
                         'id': cid.value,
                         'cid': str(cid),
                         'name': q,
-                        'val': v[0]
+                        'val': quote(v[0].encode('utf-8')) # value is the quoted version, after parsing
                     }
                 )
             elif len(v) > 1:
                 # Multiple values, undefined behavior?
-                for i in range(len(v)):
-                    cid = http_sfv.Item('@query-param')
-                    cid.params['name'] = q
-                    response['derived'].append(
-                        {
-                            'id': cid.value,
-                            'cid': str(cid),
-                            'name': q,
-                            'val': v[i],
-                            'idx': i
-                        }
-                    )
-        
+                nop
         if req:
             for d in response['derived']:
                 i = http_sfv.Item()
                 i.parse(d['cid'].encode('utf-8'))
                 i.params['req'] = True
                 d['req'] = True
                 d['cid'] = str(i)
```

### Comparing `httpsigpy-0.0.6/httpsigpy.egg-info/PKG-INFO` & `httpsigpy-0.0.7/httpsigpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpsigpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: HTTP Message Signatures
 Home-page: https://github.com/bspkio/httpsigpy
 Author: Justin Richer
 Author-email: python@justin.richer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `httpsigpy-0.0.6/setup.py` & `httpsigpy-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="httpsigpy",
-    version="0.0.6",
+    version="0.0.7",
     author="Justin Richer",
     author_email="python@justin.richer.org",
     description="HTTP Message Signatures",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bspkio/httpsigpy",
     packages=setuptools.find_packages(),
```

