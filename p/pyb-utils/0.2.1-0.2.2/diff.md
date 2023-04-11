# Comparing `tmp/pyb_utils-0.2.1.tar.gz` & `tmp/pyb_utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyb_utils-0.2.1.tar", max compression
+gzip compressed data, was "pyb_utils-0.2.2.tar", max compression
```

## Comparing `pyb_utils-0.2.1.tar` & `pyb_utils-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-03-01 18:44:35.352445 pyb_utils-0.2.1/pyb_utils/__init__.py
--rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.2.1/pyb_utils/camera.py
--rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.2.1/pyb_utils/collision.py
--rw-r--r--   0        0        0     1425 2023-03-01 18:44:35.356445 pyb_utils-0.2.1/pyb_utils/frame.py
--rw-r--r--   0        0        0     4588 2023-03-01 18:44:35.356445 pyb_utils-0.2.1/pyb_utils/ghost.py
--rw-r--r--   0        0        0      729 2023-03-01 18:44:35.356445 pyb_utils-0.2.1/pyb_utils/math.py
--rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.2.1/pyb_utils/robots.py
--rw-r--r--   0        0        0      577 2023-03-01 18:45:07.728466 pyb_utils-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 pyb_utils-0.2.1/setup.py
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 pyb_utils-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2011 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/pyb_utils/__init__.py
+-rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.2.2/pyb_utils/camera.py
+-rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/collision.py
+-rw-r--r--   0        0        0     1425 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/frame.py
+-rw-r--r--   0        0        0     4588 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/ghost.py
+-rw-r--r--   0        0        0      729 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/math.py
+-rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.2.2/pyb_utils/robots.py
+-rw-r--r--   0        0        0      598 2023-04-11 22:44:18.290567 pyb_utils-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 pyb_utils-0.2.2/setup.py
+-rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 pyb_utils-0.2.2/PKG-INFO
```

### Comparing `pyb_utils-0.2.1/LICENSE` & `pyb_utils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.1/pyb_utils/camera.py` & `pyb_utils-0.2.2/pyb_utils/camera.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.1/pyb_utils/collision.py` & `pyb_utils-0.2.2/pyb_utils/collision.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.1/pyb_utils/frame.py` & `pyb_utils-0.2.2/pyb_utils/frame.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.1/pyb_utils/ghost.py` & `pyb_utils-0.2.2/pyb_utils/ghost.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.1/pyb_utils/math.py` & `pyb_utils-0.2.2/pyb_utils/math.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.1/pyb_utils/robots.py` & `pyb_utils-0.2.2/pyb_utils/robots.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.2.1/pyproject.toml` & `pyb_utils-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.black]
 line-length = 80
 
 [tool.poetry]
 name = "pyb_utils"
-version = "0.2.1"
+version = "0.2.2"
 description = "Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras."
 authors = ["Adam Heins <mail@adamheins.com>"]
 license = "MIT"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 numpy = "^1.21.5"
 pybullet = "^3.2.1"
 spatialmath-python = ">=1.0.0"
 Pillow = "^9.0.0"
```

