# Comparing `tmp/bingbong-0.1.1.tar.gz` & `tmp/bingbong-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingbong-0.1.1.tar", last modified: Wed Apr 12 04:57:44 2023, max compression
+gzip compressed data, was "bingbong-0.1.2.tar", last modified: Wed Apr 12 05:13:57 2023, max compression
```

## Comparing `bingbong-0.1.1.tar` & `bingbong-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.005177 bingbong-0.1.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.1.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      565 2023-04-12 04:57:44.005177 bingbong-0.1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1105 2023-04-11 13:40:02.000000 bingbong-0.1.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 04:57:44.005177 bingbong-0.1.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      796 2023-04-12 04:57:34.000000 bingbong-0.1.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:43.997177 bingbong-0.1.1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.001177 bingbong-0.1.1/src/bingbong.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      565 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      371 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.1.1/src/bingbong.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.005177 bingbong-0.1.1/src/pingpong/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-04-12 04:57:40.000000 bingbong-0.1.1/src/pingpong/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      853 2023-04-12 04:50:42.000000 bingbong-0.1.1/src/pingpong/alpaca.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      583 2023-04-12 04:44:04.000000 bingbong-0.1.1/src/pingpong/gradio.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      662 2023-04-12 04:40:43.000000 bingbong-0.1.1/src/pingpong/pingpong.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.005177 bingbong-0.1.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 03:28:01.000000 bingbong-0.1.1/tests/test_pingpong.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-04-12 04:54:28.000000 bingbong-0.1.1/tests/test_scenarios.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2686 2023-04-12 04:54:13.000000 bingbong-0.1.1/tests/test_strategy.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 05:13:57.063270 bingbong-0.1.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.1.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2458 2023-04-12 05:13:57.063270 bingbong-0.1.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1851 2023-04-12 05:11:48.000000 bingbong-0.1.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 05:13:57.063270 bingbong-0.1.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      971 2023-04-12 05:13:08.000000 bingbong-0.1.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 05:13:57.051270 bingbong-0.1.2/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 05:13:57.055270 bingbong-0.1.2/src/bingbong.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2458 2023-04-12 05:13:56.000000 bingbong-0.1.2/src/bingbong.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      371 2023-04-12 05:13:57.000000 bingbong-0.1.2/src/bingbong.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 05:13:56.000000 bingbong-0.1.2/src/bingbong.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.1.2/src/bingbong.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 05:13:56.000000 bingbong-0.1.2/src/bingbong.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 05:13:57.059270 bingbong-0.1.2/src/pingpong/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-04-12 05:13:27.000000 bingbong-0.1.2/src/pingpong/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      853 2023-04-12 04:50:42.000000 bingbong-0.1.2/src/pingpong/alpaca.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      583 2023-04-12 04:44:04.000000 bingbong-0.1.2/src/pingpong/gradio.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      662 2023-04-12 04:40:43.000000 bingbong-0.1.2/src/pingpong/pingpong.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 05:13:57.063270 bingbong-0.1.2/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 03:28:01.000000 bingbong-0.1.2/tests/test_pingpong.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-04-12 04:54:28.000000 bingbong-0.1.2/tests/test_scenarios.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2686 2023-04-12 04:54:13.000000 bingbong-0.1.2/tests/test_strategy.py
```

### Comparing `bingbong-0.1.1/LICENSE` & `bingbong-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.1/src/pingpong/alpaca.py` & `bingbong-0.1.2/src/pingpong/alpaca.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.1/src/pingpong/gradio.py` & `bingbong-0.1.2/src/pingpong/gradio.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.1/src/pingpong/pingpong.py` & `bingbong-0.1.2/src/pingpong/pingpong.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.1/tests/test_pingpong.py` & `bingbong-0.1.2/tests/test_pingpong.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.1/tests/test_scenarios.py` & `bingbong-0.1.2/tests/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.1/tests/test_strategy.py` & `bingbong-0.1.2/tests/test_strategy.py`

 * *Files identical despite different names*

