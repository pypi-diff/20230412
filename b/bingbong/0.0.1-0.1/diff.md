# Comparing `tmp/bingbong-0.0.1.tar.gz` & `tmp/bingbong-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingbong-0.0.1.tar", last modified: Wed Apr 12 01:31:19 2023, max compression
+gzip compressed data, was "bingbong-0.1.tar", last modified: Wed Apr 12 01:31:44 2023, max compression
```

## Comparing `bingbong-0.0.1.tar` & `bingbong-0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:19.635246 bingbong-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      565 2023-04-12 01:31:19.631246 bingbong-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1105 2023-04-11 13:40:02.000000 bingbong-0.0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 01:31:19.635246 bingbong-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      796 2023-04-12 01:31:16.000000 bingbong-0.0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:19.627246 bingbong-0.0.1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:19.631246 bingbong-0.0.1/src/bingbong.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      565 2023-04-12 01:31:19.000000 bingbong-0.0.1/src/bingbong.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      347 2023-04-12 01:31:19.000000 bingbong-0.0.1/src/bingbong.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.0.1/src/bingbong.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.0.1/src/bingbong.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 01:31:19.000000 bingbong-0.0.1/src/bingbong.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:19.631246 bingbong-0.0.1/src/pingpong/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-04-12 01:23:48.000000 bingbong-0.0.1/src/pingpong/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-04-11 23:29:23.000000 bingbong-0.0.1/src/pingpong/alpaca.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      471 2023-04-11 14:52:10.000000 bingbong-0.0.1/src/pingpong/gradio.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-04-11 23:32:31.000000 bingbong-0.0.1/src/pingpong/pingpong.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:19.631246 bingbong-0.0.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 01:05:54.000000 bingbong-0.0.1/tests/test_pingpong.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1909 2023-04-12 01:05:44.000000 bingbong-0.0.1/tests/test_strategy.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.815587 bingbong-0.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      563 2023-04-12 01:31:44.815587 bingbong-0.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1105 2023-04-11 13:40:02.000000 bingbong-0.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 01:31:44.815587 bingbong-0.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      794 2023-04-12 01:31:34.000000 bingbong-0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.807587 bingbong-0.1/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.811587 bingbong-0.1/src/bingbong.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      563 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      347 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.1/src/bingbong.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.815587 bingbong-0.1/src/pingpong/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2023-04-12 01:31:41.000000 bingbong-0.1/src/pingpong/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-04-11 23:29:23.000000 bingbong-0.1/src/pingpong/alpaca.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      471 2023-04-11 14:52:10.000000 bingbong-0.1/src/pingpong/gradio.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-04-11 23:32:31.000000 bingbong-0.1/src/pingpong/pingpong.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.815587 bingbong-0.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 01:05:54.000000 bingbong-0.1/tests/test_pingpong.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1909 2023-04-12 01:05:44.000000 bingbong-0.1/tests/test_strategy.py
```

### Comparing `bingbong-0.0.1/LICENSE` & `bingbong-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bingbong-0.0.1/PKG-INFO` & `bingbong-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.0.1
+Version: 0.1
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bingbong-0.0.1/README.md` & `bingbong-0.1/README.md`

 * *Files identical despite different names*

### Comparing `bingbong-0.0.1/setup.py` & `bingbong-0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bingbong',
-    version='0.0.1',
+    version='0.1',
     description='Ping pong management library for LLM applied application',
     author='chansung park',
     author_email='deep.diver.csp@gmail.com',
     url='https://github.com/deep-diver/PingPong',
     install_requires=[],
     packages=['pingpong'],
     package_dir={'':'src'},
```

### Comparing `bingbong-0.0.1/src/bingbong.egg-info/PKG-INFO` & `bingbong-0.1/src/bingbong.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.0.1
+Version: 0.1
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bingbong-0.0.1/src/pingpong/alpaca.py` & `bingbong-0.1/src/pingpong/alpaca.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.0.1/src/pingpong/pingpong.py` & `bingbong-0.1/src/pingpong/pingpong.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.0.1/tests/test_pingpong.py` & `bingbong-0.1/tests/test_pingpong.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.0.1/tests/test_strategy.py` & `bingbong-0.1/tests/test_strategy.py`

 * *Files identical despite different names*

