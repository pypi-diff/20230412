# Comparing `tmp/QtPy-Frameless-Window-0.0.7.tar.gz` & `tmp/QtPy-Frameless-Window-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.7.tar", last modified: Wed Apr 12 14:30:51 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.0.8.tar", last modified: Wed Apr 12 15:00:20 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.7.tar` & `QtPy-Frameless-Window-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    35823 2023-04-12 06:26:37.916046 QtPy-Frameless-Window-0.0.7/LICENSE
--rw-r--r--   0        0        0     1000 2023-04-12 14:29:59.331412 QtPy-Frameless-Window-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      334 2023-04-12 06:26:37.920046 QtPy-Frameless-Window-0.0.7/qt_api/__init__.py
--rw-r--r--   0        0        0     1169 2023-04-12 14:27:18.865226 QtPy-Frameless-Window-0.0.7/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 06:26:37.921076 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/__init__.py
--rw-r--r--   0        0        0     1471 2023-04-12 14:30:25.601836 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource.py
--rw-r--r--   0        0        0      135 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource.qrc
--rw-r--r--   0        0        0     1471 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource_rc.py
--rw-r--r--   0        0        0      270 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/title_bar/close.svg
--rw-r--r--   0        0        0      457 2023-04-12 08:04:13.929582 QtPy-Frameless-Window-0.0.7/qtframelesswindow/api_differ/windows.py
--rw-r--r--   0        0        0     4351 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.7/qtframelesswindow/linux/__init__.py
--rw-r--r--   0        0        0     2920 2023-04-12 08:04:14.020784 QtPy-Frameless-Window-0.0.7/qtframelesswindow/linux/window_effect.py
--rw-r--r--   0        0        0     4533 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.7/qtframelesswindow/mac/__init__.py
--rw-r--r--   0        0        0     4093 2023-04-12 08:04:14.032673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/mac/window_effect.py
--rw-r--r--   0        0        0     5064 2023-04-12 14:27:18.868207 QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/__init__.py
--rw-r--r--   0        0        0     9024 2023-04-12 12:28:36.521987 QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/title_bar_buttons.py
--rw-r--r--   0        0        0      885 2023-04-12 06:26:37.922905 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/__init__.py
--rw-r--r--   0        0        0     9302 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/linux_utils.py
--rw-r--r--   0        0        0     8330 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/mac_utils.py
--rw-r--r--   0        0        0     7816 2023-04-12 08:04:14.041673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/win32_utils.py
--rw-r--r--   0        0        0     8675 2023-04-12 12:00:49.607910 QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-12 06:26:37.924905 QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/c_structures.py
--rw-r--r--   0        0        0     8979 2023-04-12 08:04:14.052662 QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/window_effect.py
--rw-r--r--   0        0        0     1156 2023-04-12 14:26:31.626229 QtPy-Frameless-Window-0.0.7/README.md
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-12 06:26:37.916046 QtPy-Frameless-Window-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1000 2023-04-12 14:59:07.447897 QtPy-Frameless-Window-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-12 06:26:37.920046 QtPy-Frameless-Window-0.0.8/qt_api/__init__.py
+-rw-r--r--   0        0        0     1169 2023-04-12 14:27:18.865226 QtPy-Frameless-Window-0.0.8/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:26:37.921076 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/__init__.py
+-rw-r--r--   0        0        0     1468 2023-04-12 14:50:14.195223 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/resource.py
+-rw-r--r--   0        0        0      135 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/resource.qrc
+-rw-r--r--   0        0        0      270 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/title_bar/close.svg
+-rw-r--r--   0        0        0      457 2023-04-12 08:04:13.929582 QtPy-Frameless-Window-0.0.8/qtframelesswindow/api_differ/windows.py
+-rw-r--r--   0        0        0     4351 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.8/qtframelesswindow/linux/__init__.py
+-rw-r--r--   0        0        0     2920 2023-04-12 08:04:14.020784 QtPy-Frameless-Window-0.0.8/qtframelesswindow/linux/window_effect.py
+-rw-r--r--   0        0        0     4533 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.8/qtframelesswindow/mac/__init__.py
+-rw-r--r--   0        0        0     4093 2023-04-12 08:04:14.032673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/mac/window_effect.py
+-rw-r--r--   0        0        0     5064 2023-04-12 14:27:18.868207 QtPy-Frameless-Window-0.0.8/qtframelesswindow/titlebar/__init__.py
+-rw-r--r--   0        0        0     9024 2023-04-12 12:28:36.521987 QtPy-Frameless-Window-0.0.8/qtframelesswindow/titlebar/title_bar_buttons.py
+-rw-r--r--   0        0        0      885 2023-04-12 06:26:37.922905 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/__init__.py
+-rw-r--r--   0        0        0     9302 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/linux_utils.py
+-rw-r--r--   0        0        0     8330 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/mac_utils.py
+-rw-r--r--   0        0        0     7816 2023-04-12 08:04:14.041673 QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/win32_utils.py
+-rw-r--r--   0        0        0     8675 2023-04-12 12:00:49.607910 QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-12 06:26:37.924905 QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/c_structures.py
+-rw-r--r--   0        0        0     8979 2023-04-12 08:04:14.052662 QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/window_effect.py
+-rw-r--r--   0        0        0     1156 2023-04-12 14:26:31.626229 QtPy-Frameless-Window-0.0.8/README.md
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.8/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.0.7/LICENSE` & `QtPy-Frameless-Window-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/pyproject.toml` & `QtPy-Frameless-Window-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.6"
-version = "0.0.7"
+version = "0.0.8"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
```

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/__init__.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/_rc/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Resource object code (Python 3)
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 6.5.0
 # WARNING! All changes made in this file will be lost!
 
-from PySide6 import QtCore
+from qtpy import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x01\x0e\
 <\
 svg width=\x2245pt\x22\
  height=\x2230pt\x22 v\
 ersion=\x221.1\x22 vie\
```

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/linux/__init__.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/linux/window_effect.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/mac/__init__.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/mac/window_effect.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/__init__.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/title_bar_buttons.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/__init__.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/linux_utils.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/mac_utils.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/win32_utils.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/__init__.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/c_structures.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/window_effect.py` & `QtPy-Frameless-Window-0.0.8/qtframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/README.md` & `QtPy-Frameless-Window-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.7/PKG-INFO` & `QtPy-Frameless-Window-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.7
+Version: 0.0.8
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

