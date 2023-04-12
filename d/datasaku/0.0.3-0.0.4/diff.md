# Comparing `tmp/datasaku-0.0.3.tar.gz` & `tmp/datasaku-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasaku-0.0.3.tar", last modified: Wed Apr  5 19:02:46 2023, max compression
+gzip compressed data, was "datasaku-0.0.4.tar", last modified: Wed Apr 12 19:38:51 2023, max compression
```

## Comparing `datasaku-0.0.3.tar` & `datasaku-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-05 19:02:46.593993 datasaku-0.0.3/
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1073 2023-01-10 15:17:32.000000 datasaku-0.0.3/LICENSE
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       21 2023-01-11 16:48:37.000000 datasaku-0.0.3/MANIFEST.in
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2769 2023-04-05 19:02:46.591444 datasaku-0.0.3/PKG-INFO
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1044 2023-01-11 17:00:16.000000 datasaku-0.0.3/README.md
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      910 2023-04-05 19:02:29.000000 datasaku-0.0.3/pyproject.toml
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      330 2023-01-11 15:30:04.000000 datasaku-0.0.3/requirements.txt
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       38 2023-04-05 19:02:46.594327 datasaku-0.0.3/setup.cfg
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-05 19:02:46.570515 datasaku-0.0.3/src/
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-05 19:02:46.585070 datasaku-0.0.3/src/datasaku/
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-01-10 15:17:34.000000 datasaku-0.0.3/src/datasaku/__init__.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      504 2023-01-11 12:03:25.000000 datasaku-0.0.3/src/datasaku/datasaku_calendar.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     5285 2023-01-10 15:17:34.000000 datasaku-0.0.3/src/datasaku/datasaku_geo.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6849 2023-01-10 15:17:34.000000 datasaku-0.0.3/src/datasaku/datasaku_google.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1178 2023-01-10 15:17:34.000000 datasaku-0.0.3/src/datasaku/datasaku_nlp.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1931 2023-01-11 16:56:32.000000 datasaku-0.0.3/src/datasaku/datasaku_pandas.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6170 2023-01-11 12:10:15.000000 datasaku-0.0.3/src/datasaku/datasaku_presto.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     5199 2023-04-05 18:52:30.000000 datasaku-0.0.3/src/datasaku/datasaku_s3.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     2798 2023-01-10 15:17:34.000000 datasaku-0.0.3/src/datasaku/datasaku_snowflake.py
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     1519 2023-01-11 15:43:56.000000 datasaku-0.0.3/src/datasaku/datasaku_starburst.py
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1748 2023-01-10 15:17:35.000000 datasaku-0.0.3/src/datasaku/datasaku_viz.py
-drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-05 19:02:46.589226 datasaku-0.0.3/src/datasaku.egg-info/
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2769 2023-04-05 19:02:46.000000 datasaku-0.0.3/src/datasaku.egg-info/PKG-INFO
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      580 2023-04-05 19:02:46.000000 datasaku-0.0.3/src/datasaku.egg-info/SOURCES.txt
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        1 2023-04-05 19:02:46.000000 datasaku-0.0.3/src/datasaku.egg-info/dependency_links.txt
--rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      330 2023-04-05 19:02:46.000000 datasaku-0.0.3/src/datasaku.egg-info/requires.txt
--rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        9 2023-04-05 19:02:46.000000 datasaku-0.0.3/src/datasaku.egg-info/top_level.txt
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.026108 datasaku-0.0.4/
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1073 2023-01-10 15:17:32.000000 datasaku-0.0.4/LICENSE
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       21 2023-01-11 16:48:37.000000 datasaku-0.0.4/MANIFEST.in
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2779 2023-04-12 19:38:51.025715 datasaku-0.0.4/PKG-INFO
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1054 2023-04-12 19:19:55.000000 datasaku-0.0.4/README.md
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      910 2023-04-12 19:38:39.000000 datasaku-0.0.4/pyproject.toml
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      330 2023-01-11 15:30:04.000000 datasaku-0.0.4/requirements.txt
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)       38 2023-04-12 19:38:51.026200 datasaku-0.0.4/setup.cfg
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.011350 datasaku-0.0.4/src/
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.020273 datasaku-0.0.4/src/datasaku/
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/__init__.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      504 2023-01-11 12:03:25.000000 datasaku-0.0.4/src/datasaku/datasaku_calendar.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     5285 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_geo.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6849 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_google.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1178 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_nlp.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1931 2023-01-11 16:56:32.000000 datasaku-0.0.4/src/datasaku/datasaku_pandas.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     6170 2023-01-11 12:10:15.000000 datasaku-0.0.4/src/datasaku/datasaku_presto.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     4854 2023-04-12 19:34:36.000000 datasaku-0.0.4/src/datasaku/datasaku_s3.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     2798 2023-01-10 15:17:34.000000 datasaku-0.0.4/src/datasaku/datasaku_snowflake.py
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     1519 2023-01-11 15:43:56.000000 datasaku-0.0.4/src/datasaku/datasaku_starburst.py
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)     1748 2023-01-10 15:17:35.000000 datasaku-0.0.4/src/datasaku/datasaku_viz.py
+drwxr-xr-x   0 rhyando.anggoro-adi   (502) staff       (20)        0 2023-04-12 19:38:51.024944 datasaku-0.0.4/src/datasaku.egg-info/
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)     2779 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/PKG-INFO
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)      580 2023-04-12 19:38:51.000000 datasaku-0.0.4/src/datasaku.egg-info/SOURCES.txt
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        1 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/dependency_links.txt
+-rwx------   0 rhyando.anggoro-adi   (502) staff       (20)      330 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/requires.txt
+-rw-r--r--   0 rhyando.anggoro-adi   (502) staff       (20)        9 2023-04-12 19:38:50.000000 datasaku-0.0.4/src/datasaku.egg-info/top_level.txt
```

### Comparing `datasaku-0.0.3/LICENSE` & `datasaku-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/PKG-INFO` & `datasaku-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasaku
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: kurangdoa <rando.bayor@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -53,9 +53,9 @@
 
 Since the package will consist of geo related package so installing gdal is necessary (be patient, takes time)
 ```
 brew install gdal
 ```
 Install the datasaku package using pip
 ```
-pip install datasaku
+pip install datasaku --upgrade
 ```
```

### Comparing `datasaku-0.0.3/README.md` & `datasaku-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 
 Since the package will consist of geo related package so installing gdal is necessary (be patient, takes time)
 ```
 brew install gdal
 ```
 Install the datasaku package using pip
 ```
-pip install datasaku
+pip install datasaku --upgrade
 ```
```

### Comparing `datasaku-0.0.3/pyproject.toml` & `datasaku-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datasaku"
 dynamic = ["dependencies"]
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="kurangdoa", email="rando.bayor@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_geo.py` & `datasaku-0.0.4/src/datasaku/datasaku_geo.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_google.py` & `datasaku-0.0.4/src/datasaku/datasaku_google.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_nlp.py` & `datasaku-0.0.4/src/datasaku/datasaku_nlp.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_pandas.py` & `datasaku-0.0.4/src/datasaku/datasaku_pandas.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_presto.py` & `datasaku-0.0.4/src/datasaku/datasaku_presto.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_s3.py` & `datasaku-0.0.4/src/datasaku/datasaku_s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,20 @@
     """Class for S3"""
     def __init__(self, aws_access_key_id, aws_secret_access_key, aws_session_token=None):
         self.aws_id =  aws_access_key_id
         self.aws_key = aws_secret_access_key
         self.aws_token = aws_session_token
 
         # create session
-        if (self.aws_id is not None) & (self.aws_key is not None) & (self.aws_token is not None):
-            if self.aws_token is not None:
-                self.s3_session = boto3.Session(
-                    aws_access_key_id = self.aws_id,
-                    aws_secret_access_key = self.aws_key,
-                    aws_session_token = self.aws_token
-                ) # create aws session if there is aws credential defined
-            else:
-                self.s3_session = boto3.Session(
-                    aws_access_key_id = self.aws_id,
-                    aws_secret_access_key = self.aws_key,
-                ) # create aws session if there is aws credential defined
+        if (self.aws_id is not None) & (self.aws_key is not None):
+            self.s3_session = boto3.Session(
+                aws_access_key_id = self.aws_id,
+                aws_secret_access_key = self.aws_key,
+                aws_session_token = self.aws_token,
+            ) # create aws session if there is aws credential defined
         else:
             self.s3_session = boto3.Session() # create aws session using using environment detail 
 
     def s3_list_bucket(self):
         """list bucket inside s3"""
         s3_resource = self.s3_session.resource('s3') # create s3 resource
         buckets = [bucket.name for bucket in s3_resource.buckets.all()] # list down the bucket
```

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_snowflake.py` & `datasaku-0.0.4/src/datasaku/datasaku_snowflake.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_starburst.py` & `datasaku-0.0.4/src/datasaku/datasaku_starburst.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku/datasaku_viz.py` & `datasaku-0.0.4/src/datasaku/datasaku_viz.py`

 * *Files identical despite different names*

### Comparing `datasaku-0.0.3/src/datasaku.egg-info/PKG-INFO` & `datasaku-0.0.4/src/datasaku.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasaku
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: kurangdoa <rando.bayor@gmail.com>
 License: Copyright (c) 2022 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -53,9 +53,9 @@
 
 Since the package will consist of geo related package so installing gdal is necessary (be patient, takes time)
 ```
 brew install gdal
 ```
 Install the datasaku package using pip
 ```
-pip install datasaku
+pip install datasaku --upgrade
 ```
```

### Comparing `datasaku-0.0.3/src/datasaku.egg-info/SOURCES.txt` & `datasaku-0.0.4/src/datasaku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

