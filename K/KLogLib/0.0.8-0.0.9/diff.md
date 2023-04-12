# Comparing `tmp/KLogLib-0.0.8.tar.gz` & `tmp/KLogLib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KLogLib-0.0.8.tar", last modified: Wed Apr 12 15:49:00 2023, max compression
+gzip compressed data, was "KLogLib-0.0.9.tar", last modified: Wed Apr 12 15:49:58 2023, max compression
```

## Comparing `KLogLib-0.0.8.tar` & `KLogLib-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:00.831619 KLogLib-0.0.8/
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:00.830810 KLogLib-0.0.8/Handlers/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.8/Handlers/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.0.8/Handlers/byte.py
--rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.0.8/Handlers/files_handler.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:00.831047 KLogLib-0.0.8/KLog/
--rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.0.8/KLog/KLog.py
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.8/KLog/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:00.831514 KLogLib-0.0.8/KLogLib.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:49:00.000000 KLogLib-0.0.8/KLogLib.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      265 2023-04-12 15:49:00.000000 KLogLib-0.0.8/KLogLib.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 15:49:00.000000 KLogLib-0.0.8/KLogLib.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 15:49:00.000000 KLogLib-0.0.8/KLogLib.egg-info/top_level.txt
--rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.8/LICENSE
--rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:49:00.831680 KLogLib-0.0.8/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.0.8/README.md
--rw-r--r--   0 javier     (501) staff       (20)     2095 2023-04-12 15:43:58.000000 KLogLib-0.0.8/README.txt
--rw-r--r--   0 javier     (501) staff       (20)       81 2023-04-12 15:49:00.831885 KLogLib-0.0.8/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      732 2023-04-12 15:48:47.000000 KLogLib-0.0.8/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:58.162665 KLogLib-0.0.9/
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:58.161611 KLogLib-0.0.9/Handlers/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.9/Handlers/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.0.9/Handlers/byte.py
+-rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.0.9/Handlers/files_handler.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:58.161941 KLogLib-0.0.9/KLog/
+-rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.0.9/KLog/KLog.py
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.9/KLog/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:49:58.162530 KLogLib-0.0.9/KLogLib.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:49:58.000000 KLogLib-0.0.9/KLogLib.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      265 2023-04-12 15:49:58.000000 KLogLib-0.0.9/KLogLib.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 15:49:58.000000 KLogLib-0.0.9/KLogLib.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 15:49:58.000000 KLogLib-0.0.9/KLogLib.egg-info/top_level.txt
+-rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.9/LICENSE
+-rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:49:58.162733 KLogLib-0.0.9/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.0.9/README.md
+-rw-r--r--   0 javier     (501) staff       (20)      548 2023-04-12 15:49:48.000000 KLogLib-0.0.9/README.txt
+-rw-r--r--   0 javier     (501) staff       (20)       81 2023-04-12 15:49:58.162957 KLogLib-0.0.9/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      732 2023-04-12 15:48:47.000000 KLogLib-0.0.9/setup.py
```

### Comparing `KLogLib-0.0.8/Handlers/files_handler.py` & `KLogLib-0.0.9/Handlers/files_handler.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.8/KLog/KLog.py` & `KLogLib-0.0.9/KLog/KLog.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.8/LICENSE` & `KLogLib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.8/README.md` & `KLogLib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.8/setup.py` & `KLogLib-0.0.9/setup.py`

 * *Files identical despite different names*

