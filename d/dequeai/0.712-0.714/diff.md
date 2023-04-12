# Comparing `tmp/dequeai-0.712.tar.gz` & `tmp/dequeai-0.714.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.712.tar", last modified: Tue Apr 11 21:12:31 2023, max compression
+gzip compressed data, was "dequeai-0.714.tar", last modified: Wed Apr 12 00:43:21 2023, max compression
```

## Comparing `dequeai-0.712.tar` & `dequeai-0.714.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:12:31.794411 dequeai-0.712/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 21:12:31.794411 dequeai-0.712/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:12:31.794411 dequeai-0.712/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.712/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.712/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.712/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.712/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.712/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    21108 2023-04-11 21:03:22.000000 dequeai-0.712/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.712/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.712/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.712/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.712/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 21:12:31.794411 dequeai-0.712/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-11 21:12:31.000000 dequeai-0.712/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-11 21:12:31.000000 dequeai-0.712/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 21:12:31.000000 dequeai-0.712/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-11 21:12:31.000000 dequeai-0.712/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-11 21:12:31.000000 dequeai-0.712/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 21:12:31.794411 dequeai-0.712/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 21:12:18.000000 dequeai-0.712/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:21.449372 dequeai-0.714/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-12 00:43:21.449372 dequeai-0.714/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:21.445372 dequeai-0.714/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.714/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.714/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.714/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.714/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.714/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    21134 2023-04-12 00:42:41.000000 dequeai-0.714/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.714/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.714/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.714/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.714/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 00:43:21.445372 dequeai-0.714/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-12 00:43:20.000000 dequeai-0.714/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-12 00:43:21.000000 dequeai-0.714/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 00:43:21.449372 dequeai-0.714/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-12 00:42:55.000000 dequeai-0.714/setup.py
```

### Comparing `dequeai-0.712/dequeai/datatypes.py` & `dequeai-0.714/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.712/dequeai/dequeai.py` & `dequeai-0.714/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.712/dequeai/dequeai_run.py` & `dequeai-0.714/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
         self._code_logged = False
 
         self._environment_logged = False
 
         self._resources_logged = False
 
-        print(f"Run initialized with project name as {self._project_name} and run id {self._run_id}")
+        print(f"Run initialized with project name as {self._project_name} for user {self.user_name} and run id {self._run_id}")
 
     def _start_parser(self):
         parser = ParsingService()
         parser.receive()
 
     def finish(self):
         self._running = False
```

### Comparing `dequeai-0.712/dequeai/parsing_service.py` & `dequeai-0.714/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.712/dequeai/rest_connect.py` & `dequeai-0.714/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.712/dequeai/util.py` & `dequeai-0.714/dequeai/util.py`

 * *Files identical despite different names*

