# Comparing `tmp/KLogLib-0.1.0.tar.gz` & `tmp/KLogLib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KLogLib-0.1.0.tar", last modified: Wed Apr 12 16:10:31 2023, max compression
+gzip compressed data, was "KLogLib-0.1.1.tar", last modified: Wed Apr 12 16:13:00 2023, max compression
```

## Comparing `KLogLib-0.1.0.tar` & `KLogLib-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:10:31.774363 KLogLib-0.1.0/
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:10:31.773525 KLogLib-0.1.0/Handlers/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.1.0/Handlers/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.1.0/Handlers/byte.py
--rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.1.0/Handlers/files_handler.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:10:31.773787 KLogLib-0.1.0/KLog/
--rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.1.0/KLog/KLog.py
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.1.0/KLog/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:10:31.774240 KLogLib-0.1.0/KLogLib.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)     2275 2023-04-12 16:10:31.000000 KLogLib-0.1.0/KLogLib.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 16:10:31.000000 KLogLib-0.1.0/KLogLib.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 16:10:31.000000 KLogLib-0.1.0/KLogLib.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 16:10:31.000000 KLogLib-0.1.0/KLogLib.egg-info/top_level.txt
--rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.1.0/LICENSE
--rw-r--r--   0 javier     (501) staff       (20)     2275 2023-04-12 16:10:31.774428 KLogLib-0.1.0/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.1.0/README.md
--rw-r--r--   0 javier     (501) staff       (20)      191 2023-04-12 16:10:31.774655 KLogLib-0.1.0/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)     2809 2023-04-12 16:10:22.000000 KLogLib-0.1.0/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.794055 KLogLib-0.1.1/
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.793174 KLogLib-0.1.1/Handlers/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.1.1/Handlers/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.1.1/Handlers/byte.py
+-rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.1.1/Handlers/files_handler.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.793423 KLogLib-0.1.1/KLog/
+-rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.1.1/KLog/KLog.py
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.1.1/KLog/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:13:00.793876 KLogLib-0.1.1/KLogLib.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)     2275 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 16:13:00.000000 KLogLib-0.1.1/KLogLib.egg-info/top_level.txt
+-rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.1.1/LICENSE
+-rw-r--r--   0 javier     (501) staff       (20)     2275 2023-04-12 16:13:00.794140 KLogLib-0.1.1/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.1.1/README.md
+-rw-r--r--   0 javier     (501) staff       (20)      191 2023-04-12 16:13:00.794391 KLogLib-0.1.1/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      710 2023-04-12 16:12:50.000000 KLogLib-0.1.1/setup.py
```

### Comparing `KLogLib-0.1.0/Handlers/files_handler.py` & `KLogLib-0.1.1/Handlers/files_handler.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.1.0/KLog/KLog.py` & `KLogLib-0.1.1/KLog/KLog.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.1.0/KLogLib.egg-info/PKG-INFO` & `KLogLib-0.1.1/KLogLib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KLogLib
-Version: 0.1.0
-Home-page: https://github.com/javifriasj/KLog/releases/tag/0.1.0
+Version: 0.1.1
+Home-page: https://github.com/javifriasj/KLog/releases/tag/0.1.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KLog
 
 KLog is a library which aims to bring easy logging in Python
```

### Comparing `KLogLib-0.1.0/LICENSE` & `KLogLib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `KLogLib-0.1.0/PKG-INFO` & `KLogLib-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: KLogLib
-Version: 0.1.0
-Home-page: https://github.com/javifriasj/KLog/releases/tag/0.1.0
+Version: 0.1.1
+Home-page: https://github.com/javifriasj/KLog/releases/tag/0.1.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KLog
 
 KLog is a library which aims to bring easy logging in Python
```

### Comparing `KLogLib-0.1.0/README.md` & `KLogLib-0.1.1/README.md`

 * *Files identical despite different names*

