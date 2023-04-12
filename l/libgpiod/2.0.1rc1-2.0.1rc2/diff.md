# Comparing `tmp/libgpiod-2.0.1rc1.tar.gz` & `tmp/libgpiod-2.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libgpiod-2.0.1rc1.tar", last modified: Wed Apr 12 20:05:42 2023, max compression
+gzip compressed data, was "libgpiod-2.0.1rc2.tar", last modified: Wed Apr 12 20:43:14 2023, max compression
```

## Comparing `libgpiod-2.0.1rc1.tar` & `libgpiod-2.0.1rc2.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-12 20:05:08.000000 libgpiod-2.0.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      299 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/gpiod/
--rw-r--r--   0 root         (0) root         (0)     1419 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10784 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/chip.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/chip_info.py
--rw-r--r--   0 root         (0) root         (0)     1348 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/edge_event.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/gpiod/ext/
--rw-r--r--   0 root         (0) root         (0)     7690 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/ext/chip.c
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/ext/common.c
--rw-r--r--   0 root         (0) root         (0)      729 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/ext/internal.h
--rw-r--r--   0 root         (0) root         (0)     4135 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/ext/line-config.c
--rw-r--r--   0 root         (0) root         (0)     2842 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/ext/line-settings.c
--rw-r--r--   0 root         (0) root         (0)     3601 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/ext/module.c
--rw-r--r--   0 root         (0) root         (0)     8721 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/ext/request.c
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/info_event.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/internal.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/line.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/line_info.py
--rw-r--r--   0 root         (0) root         (0)     6580 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/line_request.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/gpiod/line_settings.py
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 20:05:29.000000 libgpiod-2.0.1rc1/gpiod/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/libgpiod.egg-info/
--rw-r--r--   0 root         (0) root         (0)      299 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/libgpiod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1175 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/libgpiod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/libgpiod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/libgpiod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1764 2023-04-12 20:05:08.000000 libgpiod-2.0.1rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/tests/gpiosim/
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/gpiosim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/gpiosim/chip.py
--rw-r--r--   0 root         (0) root         (0)     6667 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/gpiosim/ext.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:05:42.000000 libgpiod-2.0.1rc1/tests/procname/
--rw-r--r--   0 root         (0) root         (0)      147 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/procname/__init__.py
--rw-r--r--   0 root         (0) root         (0)      817 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/procname/ext.c
--rw-r--r--   0 root         (0) root         (0)     6721 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_chip.py
--rw-r--r--   0 root         (0) root         (0)     1481 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_chip_info.py
--rw-r--r--   0 root         (0) root         (0)     7415 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_edge_event.py
--rw-r--r--   0 root         (0) root         (0)     6789 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_info_event.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_line_info.py
--rw-r--r--   0 root         (0) root         (0)    18442 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_line_request.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_line_settings.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-04-12 20:04:25.000000 libgpiod-2.0.1rc1/tests/tests_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-04-12 20:39:33.000000 libgpiod-2.0.1rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      299 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/gpiod/
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10784 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/chip.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/chip_info.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/edge_event.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/gpiod/ext/
+-rw-r--r--   0 root         (0) root         (0)     7690 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/ext/chip.c
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/ext/common.c
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/ext/internal.h
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/ext/line-config.c
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/ext/line-settings.c
+-rw-r--r--   0 root         (0) root         (0)     3601 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/ext/module.c
+-rw-r--r--   0 root         (0) root         (0)     8721 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/ext/request.c
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/info_event.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/internal.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/line.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/line_info.py
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/line_request.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/gpiod/line_settings.py
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 20:39:42.000000 libgpiod-2.0.1rc2/gpiod/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/libgpiod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      299 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/libgpiod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/libgpiod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/libgpiod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/libgpiod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/tests/
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      481 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/tests/gpiosim/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/gpiosim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/gpiosim/chip.py
+-rw-r--r--   0 root         (0) root         (0)     6667 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/gpiosim/ext.c
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:43:14.000000 libgpiod-2.0.1rc2/tests/procname/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/procname/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/procname/ext.c
+-rw-r--r--   0 root         (0) root         (0)     6721 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_chip.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_chip_info.py
+-rw-r--r--   0 root         (0) root         (0)     7415 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_edge_event.py
+-rw-r--r--   0 root         (0) root         (0)     6789 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_info_event.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_line_info.py
+-rw-r--r--   0 root         (0) root         (0)    18442 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_line_request.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_line_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-04-12 20:38:56.000000 libgpiod-2.0.1rc2/tests/tests_module.py
```

### Comparing `libgpiod-2.0.1rc1/gpiod/__init__.py` & `libgpiod-2.0.1rc2/gpiod/__init__.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/chip.py` & `libgpiod-2.0.1rc2/gpiod/chip.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/edge_event.py` & `libgpiod-2.0.1rc2/gpiod/edge_event.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/ext/chip.c` & `libgpiod-2.0.1rc2/gpiod/ext/chip.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/ext/common.c` & `libgpiod-2.0.1rc2/gpiod/ext/common.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/ext/internal.h` & `libgpiod-2.0.1rc2/gpiod/ext/internal.h`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/ext/line-config.c` & `libgpiod-2.0.1rc2/gpiod/ext/line-config.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/ext/line-settings.c` & `libgpiod-2.0.1rc2/gpiod/ext/line-settings.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/ext/module.c` & `libgpiod-2.0.1rc2/gpiod/ext/module.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/ext/request.c` & `libgpiod-2.0.1rc2/gpiod/ext/request.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/info_event.py` & `libgpiod-2.0.1rc2/gpiod/info_event.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/internal.py` & `libgpiod-2.0.1rc2/gpiod/internal.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/line.py` & `libgpiod-2.0.1rc2/gpiod/line.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/line_info.py` & `libgpiod-2.0.1rc2/gpiod/line_info.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/line_request.py` & `libgpiod-2.0.1rc2/gpiod/line_request.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/gpiod/line_settings.py` & `libgpiod-2.0.1rc2/gpiod/line_settings.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/libgpiod.egg-info/SOURCES.txt` & `libgpiod-2.0.1rc2/libgpiod.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 gpiod/ext/line-settings.c
 gpiod/ext/module.c
 gpiod/ext/request.c
 libgpiod.egg-info/PKG-INFO
 libgpiod.egg-info/SOURCES.txt
 libgpiod.egg-info/dependency_links.txt
 libgpiod.egg-info/top_level.txt
+tests/__init__.py
+tests/__main__.py
+tests/helpers.py
 tests/tests_chip.py
 tests/tests_chip_info.py
 tests/tests_edge_event.py
 tests/tests_info_event.py
 tests/tests_line_info.py
 tests/tests_line_request.py
 tests/tests_line_settings.py
```

### Comparing `libgpiod-2.0.1rc1/setup.py` & `libgpiod-2.0.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/gpiosim/chip.py` & `libgpiod-2.0.1rc2/tests/gpiosim/chip.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/gpiosim/ext.c` & `libgpiod-2.0.1rc2/tests/gpiosim/ext.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/procname/ext.c` & `libgpiod-2.0.1rc2/tests/procname/ext.c`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_chip.py` & `libgpiod-2.0.1rc2/tests/tests_chip.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_chip_info.py` & `libgpiod-2.0.1rc2/tests/tests_chip_info.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_edge_event.py` & `libgpiod-2.0.1rc2/tests/tests_edge_event.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_info_event.py` & `libgpiod-2.0.1rc2/tests/tests_info_event.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_line_info.py` & `libgpiod-2.0.1rc2/tests/tests_line_info.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_line_request.py` & `libgpiod-2.0.1rc2/tests/tests_line_request.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_line_settings.py` & `libgpiod-2.0.1rc2/tests/tests_line_settings.py`

 * *Files identical despite different names*

### Comparing `libgpiod-2.0.1rc1/tests/tests_module.py` & `libgpiod-2.0.1rc2/tests/tests_module.py`

 * *Files identical despite different names*

