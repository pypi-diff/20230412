# Comparing `tmp/KLogLib-0.0.14.tar.gz` & `tmp/KLogLib-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KLogLib-0.0.14.tar", last modified: Wed Apr 12 15:59:17 2023, max compression
+gzip compressed data, was "KLogLib-0.0.15.tar", last modified: Wed Apr 12 16:02:17 2023, max compression
```

## Comparing `KLogLib-0.0.14.tar` & `KLogLib-0.0.15.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:59:17.083762 KLogLib-0.0.14/
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:59:17.082771 KLogLib-0.0.14/Handlers/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.14/Handlers/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.0.14/Handlers/byte.py
--rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.0.14/Handlers/files_handler.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:59:17.083036 KLogLib-0.0.14/KLog/
--rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.0.14/KLog/KLog.py
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.14/KLog/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:59:17.083618 KLogLib-0.0.14/KLogLib.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      210 2023-04-12 15:59:17.000000 KLogLib-0.0.14/KLogLib.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      265 2023-04-12 15:59:17.000000 KLogLib-0.0.14/KLogLib.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 15:59:17.000000 KLogLib-0.0.14/KLogLib.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 15:59:17.000000 KLogLib-0.0.14/KLogLib.egg-info/top_level.txt
--rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.14/LICENSE
--rw-r--r--   0 javier     (501) staff       (20)      210 2023-04-12 15:59:17.083853 KLogLib-0.0.14/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.0.14/README.md
--rw-r--r--   0 javier     (501) staff       (20)      548 2023-04-12 15:53:02.000000 KLogLib-0.0.14/README.rst
--rw-r--r--   0 javier     (501) staff       (20)      206 2023-04-12 15:59:17.084113 KLogLib-0.0.14/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      732 2023-04-12 15:48:47.000000 KLogLib-0.0.14/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:02:17.931284 KLogLib-0.0.15/
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:02:17.930465 KLogLib-0.0.15/Handlers/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.15/Handlers/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.0.15/Handlers/byte.py
+-rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.0.15/Handlers/files_handler.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:02:17.930712 KLogLib-0.0.15/KLog/
+-rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.0.15/KLog/KLog.py
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.15/KLog/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 16:02:17.931158 KLogLib-0.0.15/KLogLib.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      139 2023-04-12 16:02:17.000000 KLogLib-0.0.15/KLogLib.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 16:02:17.000000 KLogLib-0.0.15/KLogLib.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 16:02:17.000000 KLogLib-0.0.15/KLogLib.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 16:02:17.000000 KLogLib-0.0.15/KLogLib.egg-info/top_level.txt
+-rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.15/LICENSE
+-rw-r--r--   0 javier     (501) staff       (20)      139 2023-04-12 16:02:17.931341 KLogLib-0.0.15/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.0.15/README.md
+-rw-r--r--   0 javier     (501) staff       (20)       82 2023-04-12 16:02:17.931542 KLogLib-0.0.15/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)     2809 2023-04-12 16:01:55.000000 KLogLib-0.0.15/setup.py
```

### Comparing `KLogLib-0.0.14/Handlers/files_handler.py` & `KLogLib-0.0.15/Handlers/files_handler.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.14/KLog/KLog.py` & `KLogLib-0.0.15/KLog/KLog.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.14/LICENSE` & `KLogLib-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.14/README.md` & `KLogLib-0.0.15/README.md`

 * *Files identical despite different names*

