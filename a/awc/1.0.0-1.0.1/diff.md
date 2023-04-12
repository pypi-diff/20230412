# Comparing `tmp/awc-1.0.0-py2.py3-none-any.whl.zip` & `tmp/awc-1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 20735 bytes, number of entries: 15
--rw-r--r--  2.0 unx     4516 b- defN 23-Apr-12 19:07 awc/__init__.py
+Zip file size: 21237 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     4516 b- defN 23-Apr-12 20:31 awc/__init__.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Apr-11 16:56 awc/__main__.py
 -rw-r--r--  2.0 unx     3357 b- defN 23-Apr-12 19:44 awc/api.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Apr-12 17:10 awc/const.py
 -rw-r--r--  2.0 unx     1600 b- defN 23-Apr-12 18:57 awc/exc.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 12:49 awc/py.typed
 -rw-r--r--  2.0 unx      845 b- defN 23-Apr-12 18:55 awc/util.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Apr-12 18:58 awc/wrn.py
 -rw-r--r--  2.0 unx     2785 b- defN 23-Apr-12 19:58 awc/sql/__init__.py
 -rw-r--r--  2.0 unx     2062 b- defN 23-Apr-12 19:27 awc/sql/helpers.py
--rw-------  2.0 unx    35107 b- defN 23-Apr-12 20:27 awc-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1790 b- defN 23-Apr-12 20:27 awc-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 20:27 awc-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-12 20:27 awc-1.0.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.0.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-12 20:27 awc-1.0.0.dist-info/RECORD
-15 files, 54156 bytes uncompressed, 19005 bytes compressed:  64.9%
+-rw-------  2.0 unx    35107 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1790 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-11 19:04 awc-1.0.1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Apr-12 20:34 awc-1.0.1.dist-info/RECORD
+16 files, 54905 bytes uncompressed, 19401 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: awc/__init__.py
 Comment: 
 
+Filename: awc/__main__.py
+Comment: 
+
 Filename: awc/api.py
 Comment: 
 
 Filename: awc/const.py
 Comment: 
 
 Filename: awc/exc.py
@@ -21,26 +24,26 @@
 
 Filename: awc/sql/__init__.py
 Comment: 
 
 Filename: awc/sql/helpers.py
 Comment: 
 
-Filename: awc-1.0.0.dist-info/LICENSE
+Filename: awc-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: awc-1.0.0.dist-info/METADATA
+Filename: awc-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: awc-1.0.0.dist-info/WHEEL
+Filename: awc-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: awc-1.0.0.dist-info/top_level.txt
+Filename: awc-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: awc-1.0.0.dist-info/zip-safe
+Filename: awc-1.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: awc-1.0.0.dist-info/RECORD
+Filename: awc-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc/__init__.py

```diff
@@ -7,15 +7,15 @@
 from functools import wraps
 
 import requests
 from furl import furl  # type: ignore
 
 from . import const, exc, util
 
-__version__: typing.Final[str] = "1.0.0"
+__version__: typing.Final[str] = "1.0.1"
 
 
 class Awc:
     """ari-web comments interface"""
 
     __slots__: typing.Tuple[str, ...] = (
         "__instance",
```

## Comparing `awc-1.0.0.dist-info/LICENSE` & `awc-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc-1.0.0.dist-info/METADATA` & `awc-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc
-Version: 1.0.0
+Version: 1.0.1
 Summary: wrapper for ari-web comments API
 Home-page: https://ari-web.xyz/gh/awc
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,comments,api,wrapper,https
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `awc-1.0.0.dist-info/RECORD` & `awc-1.0.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-awc/__init__.py,sha256=zlCd-pGlqGA8vQJOIf-ZVAU2AFRxcxz4OwzsOrXqH8o,4516
+awc/__init__.py,sha256=dQ8CAhDfe8IQaQVlrV_Ey8XTQvKGYDhLrV1PsJy23t0,4516
+awc/__main__.py,sha256=d1UfoKcH5bl9qoqWowmcARIitWbbGsasAZfq8RHHsE4,678
 awc/api.py,sha256=amnyBlHnoO2P7wf4_No0yzvhhnEyLX0yDzON9PbSiIc,3357
 awc/const.py,sha256=Ji-u4yUUmoR2t6OImNx_c8msQqzRXEcXVGxPk8Fo170,292
 awc/exc.py,sha256=ZoaptGrRRHv_dS_22HeiUABLGF6Fd-1eksHrqmqfZ0A,1600
 awc/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 awc/util.py,sha256=jXoXWoh71_lZonB_mA9t_ZLEi6AYdwBGSdRl0GGTeR0,845
 awc/wrn.py,sha256=nBP_fOhh3DBC6-rjNvGpR7RV-JDe7H0kSuD8BRz8UEE,614
 awc/sql/__init__.py,sha256=yMdgaa3vywXhMIJT4qXz9tZEWJdyhtjuD8VfyQ4AaDw,2785
 awc/sql/helpers.py,sha256=IJ-qEBZ39Nq1zhQz5rwHmKnX1En_2u7kNJfhAOL1J50,2062
-awc-1.0.0.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
-awc-1.0.0.dist-info/METADATA,sha256=hoM8IIs2J8msSzQ3aG5mZI95MTOdtqU3qZjDEaidQWM,1790
-awc-1.0.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc-1.0.0.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
-awc-1.0.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc-1.0.0.dist-info/RECORD,,
+awc-1.0.1.dist-info/LICENSE,sha256=nqVIZAIjniFxpDnU4HMUA3KRZ8mFA_JpXMNFVQTHlVI,35107
+awc-1.0.1.dist-info/METADATA,sha256=Dgf45THjGh5j7dG1cBMIBMOvCRUGq8zL1ukbN5N21x4,1790
+awc-1.0.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc-1.0.1.dist-info/top_level.txt,sha256=Xj3P9OwultDU5KrAvJbWKuD3ki2LWL6tSfbMPu28Hck,4
+awc-1.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc-1.0.1.dist-info/RECORD,,
```

