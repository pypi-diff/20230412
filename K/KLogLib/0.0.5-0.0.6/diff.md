# Comparing `tmp/KLogLib-0.0.5.tar.gz` & `tmp/KLogLib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KLogLib-0.0.5.tar", last modified: Wed Apr 12 15:38:31 2023, max compression
+gzip compressed data, was "KLogLib-0.0.6.tar", last modified: Wed Apr 12 15:40:21 2023, max compression
```

## Comparing `KLogLib-0.0.5.tar` & `KLogLib-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:38:31.463617 KLogLib-0.0.5/
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:38:31.462627 KLogLib-0.0.5/Handlers/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.5/Handlers/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.0.5/Handlers/byte.py
--rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.0.5/Handlers/files_handler.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:38:31.462971 KLogLib-0.0.5/KLog/
--rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.0.5/KLog/KLog.py
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.5/KLog/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:38:31.463496 KLogLib-0.0.5/KLogLib.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:38:31.000000 KLogLib-0.0.5/KLogLib.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 15:38:31.000000 KLogLib-0.0.5/KLogLib.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 15:38:31.000000 KLogLib-0.0.5/KLogLib.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 15:38:31.000000 KLogLib-0.0.5/KLogLib.egg-info/top_level.txt
--rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.5/LICENSE
--rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:38:31.463679 KLogLib-0.0.5/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.0.5/README.md
--rw-r--r--   0 javier     (501) staff       (20)      103 2023-04-12 15:38:31.463902 KLogLib-0.0.5/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      740 2023-04-12 15:30:17.000000 KLogLib-0.0.5/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:40:21.757517 KLogLib-0.0.6/
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:40:21.756691 KLogLib-0.0.6/Handlers/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.6/Handlers/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.0.6/Handlers/byte.py
+-rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.0.6/Handlers/files_handler.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:40:21.756941 KLogLib-0.0.6/KLog/
+-rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.0.6/KLog/KLog.py
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.6/KLog/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:40:21.757391 KLogLib-0.0.6/KLogLib.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      146 2023-04-12 15:40:21.000000 KLogLib-0.0.6/KLogLib.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 15:40:21.000000 KLogLib-0.0.6/KLogLib.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 15:40:21.000000 KLogLib-0.0.6/KLogLib.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 15:40:21.000000 KLogLib-0.0.6/KLogLib.egg-info/top_level.txt
+-rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.6/LICENSE
+-rw-r--r--   0 javier     (501) staff       (20)      146 2023-04-12 15:40:21.757594 KLogLib-0.0.6/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.0.6/README.md
+-rw-r--r--   0 javier     (501) staff       (20)      129 2023-04-12 15:40:21.757811 KLogLib-0.0.6/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      740 2023-04-12 15:30:17.000000 KLogLib-0.0.6/setup.py
```

### Comparing `KLogLib-0.0.5/Handlers/files_handler.py` & `KLogLib-0.0.6/Handlers/files_handler.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.5/KLog/KLog.py` & `KLogLib-0.0.6/KLog/KLog.py`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.5/LICENSE` & `KLogLib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.5/README.md` & `KLogLib-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.5/setup.py` & `KLogLib-0.0.6/setup.py`

 * *Files identical despite different names*

