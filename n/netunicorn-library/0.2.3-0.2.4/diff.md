# Comparing `tmp/netunicorn-library-0.2.3.tar.gz` & `tmp/netunicorn-library-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netunicorn-library/netunicorn-library/temp/netunicorn/netunicorn-library/dist/.tmp-mem5j2bi/netunicorn-librar", last modified: Fri Mar 17 06:39:14 2023, max compression
+gzip compressed data, was "/home/runner/work/netunicorn-library/netunicorn-library/temp/netunicorn/netunicorn-library/dist/.tmp-urk_wqcb/netunicorn-librar", last modified: Wed Apr 12 21:44:44 2023, max compression
```

## Comparing `netunicorn-library-0.2.3.tar` & `netunicorn-library-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/library/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/heartbleed/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/heartbleed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/heartbleed/heartbleeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/pcapture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/qoe_youtube/
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/qoe_youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/qoe_youtube/watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/speedtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/upload/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-03-17 06:39:02.000000 netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-17 06:39:14.000000 netunicorn-library-0.2.3/src/netunicorn_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/heartbleeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/pcapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/speedtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/top_level.txt
```

### Comparing `netunicorn-library-0.2.3/pyproject.toml` & `netunicorn-library-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-library"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn contrib library"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/basic.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/basic.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/heartbleed/__init__.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/heartbleed/heartbleeder.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/heartbleeder.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/pcapture.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/pcapture.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,18 +74,15 @@
     def run(self):
         signal.signal(signal.SIGCHLD, signal.SIG_IGN)
         pid = self.previous_steps.get(self.capture_task_name, [Failure("Named StartCapture not found")])[-1]
         if isinstance(pid, Failure):
             return pid
 
         pid = pid.unwrap()
-        subprocess.Popen(
-            ["kill", "-w", str(pid)], stdout=subprocess.PIPE, stderr=subprocess.PIPE
-        )
-        return "Successfully killed tcpdump process"
+        return subprocess.check_output(["kill", str(pid)])
 
 
 class StopAllTCPDumps(TaskDispatcher):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.args = args
         self.kwargs = kwargs
```

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/ping.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/ping.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/qoe_youtube/__init__.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/qoe_youtube/watcher.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/speedtest.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/speedtest.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/upload/webdav.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/webdav.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py` & `netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.3/src/netunicorn_library.egg-info/SOURCES.txt` & `netunicorn-library-0.2.4/src/netunicorn_library.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pyproject.toml
 src/netunicorn/library/__init__.py
 src/netunicorn/library/pipelines/__init__.py
 src/netunicorn/library/tasks/__init__.py
 src/netunicorn/library/tasks/basic.py
+src/netunicorn/library/tasks/flags.py
 src/netunicorn/library/tasks/pcapture.py
 src/netunicorn/library/tasks/ping.py
 src/netunicorn/library/tasks/speedtest.py
 src/netunicorn/library/tasks/heartbleed/__init__.py
 src/netunicorn/library/tasks/heartbleed/heartbleeder.py
 src/netunicorn/library/tasks/qoe_youtube/__init__.py
 src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
```

