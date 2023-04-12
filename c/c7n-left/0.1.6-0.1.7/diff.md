# Comparing `tmp/c7n_left-0.1.6-py3-none-any.whl.zip` & `tmp/c7n_left-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 19616 bytes, number of entries: 15
+Zip file size: 19614 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     2977 b- defN 80-Jan-01 00:00 c7n_left/cli.py
 -rw-r--r--  2.0 unx    11560 b- defN 80-Jan-01 00:00 c7n_left/core.py
 -rw-r--r--  2.0 unx      142 b- defN 80-Jan-01 00:00 c7n_left/entry.py
 -rw-r--r--  2.0 unx     4315 b- defN 80-Jan-01 00:00 c7n_left/filters.py
 -rw-r--r--  2.0 unx    11802 b- defN 80-Jan-01 00:00 c7n_left/output.py
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/__init__.py
 -rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/graph.py
 -rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/provider.py
 -rw-r--r--  2.0 unx      945 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/resource.py
 -rw-r--r--  2.0 unx     7208 b- defN 80-Jan-01 00:00 c7n_left/test.py
 -rw-r--r--  2.0 unx      732 b- defN 80-Jan-01 00:00 c7n_left/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    12065 b- defN 16-Jan-01 00:00 c7n_left-0.1.6.dist-info/METADATA
-?rw-------  2.0 unx     1206 b- defN 23-Apr-11 08:33 c7n_left-0.1.6.dist-info/RECORD
-15 files, 58040 bytes uncompressed, 17634 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12065 b- defN 16-Jan-01 00:00 c7n_left-0.1.7.dist-info/METADATA
+?rw-------  2.0 unx     1206 b- defN 23-Apr-12 11:00 c7n_left-0.1.7.dist-info/RECORD
+15 files, 58040 bytes uncompressed, 17632 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: c7n_left/test.py
 Comment: 
 
 Filename: c7n_left/utils.py
 Comment: 
 
-Filename: c7n_left-0.1.6.dist-info/WHEEL
+Filename: c7n_left-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_left-0.1.6.dist-info/entry_points.txt
+Filename: c7n_left-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_left-0.1.6.dist-info/METADATA
+Filename: c7n_left-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: c7n_left-0.1.6.dist-info/RECORD
+Filename: c7n_left-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_left-0.1.6.dist-info/METADATA` & `c7n_left-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c7n-left
-Version: 0.1.6
+Version: 0.1.7
 Summary: Custodian policies for IAAC definitions
 Home-page: https://cloudcustodian.io
 License: Apache-2
 Author: Cloud Custodian Project
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: c7n (==0.9.25) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: c7n (==0.9.26) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: boto3 (==1.26.109) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: jsonschema (==4.17.3) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: argcomplete (==3.0.5) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: python-dateutil (==2.8.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pyyaml (==6.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: tabulate (==0.9.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: importlib-metadata (==5.2.0) ; python_version >= "3.7" and python_version < "3.8"
```

## Comparing `c7n_left-0.1.6.dist-info/RECORD` & `c7n_left-0.1.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 c7n_left/output.py,sha256=aeaPfPFzLhQyc3HRnXY5l88HXUtIkmxPloAleEK2qVM,11802
 c7n_left/providers/terraform/__init__.py,sha256=BPUsPHvPInkb9N5fqhYccTRt_dWnFsdSEkFSDwgAFlY,121
 c7n_left/providers/terraform/graph.py,sha256=b47aqwKM6QCjdfRwWwteciplflNER-WKw86JTB-F1Gc,3282
 c7n_left/providers/terraform/provider.py,sha256=5etOLvG-3nssOsfw1Dfs08QPTmujiBb6RvfZ1v_7Ve4,1552
 c7n_left/providers/terraform/resource.py,sha256=6sZhzlHrZ8unJKJViHsQkalQAspCzUyMAL8mjzngR98,945
 c7n_left/test.py,sha256=iOW7nQLjCk9Luk4LhjAqKfKBnoy_tJCUrMPO9qKW20I,7208
 c7n_left/utils.py,sha256=V8yRbNRjKmuz24ZrfYwtYSLdyLMlZ0MVIhAkZdMwFbQ,732
-c7n_left-0.1.6.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
-c7n_left-0.1.6.dist-info/entry_points.txt,sha256=BP7MM3oxRCtY3qaC9GsUqrYj3962epelsmHx4XkQ6pY,45
-c7n_left-0.1.6.dist-info/RECORD,,
-c7n_left-0.1.6.dist-info/METADATA,sha256=Uz4LdIO9V--nSuTpor_06G4UyqgxxJ5_UQmpgN-7rTo,12065
+c7n_left-0.1.7.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
+c7n_left-0.1.7.dist-info/entry_points.txt,sha256=BP7MM3oxRCtY3qaC9GsUqrYj3962epelsmHx4XkQ6pY,45
+c7n_left-0.1.7.dist-info/RECORD,,
+c7n_left-0.1.7.dist-info/METADATA,sha256=ktOHViWiooXV9QPjXfIw1fENbJIMNKQsMnDYrogOQf4,12065
```

