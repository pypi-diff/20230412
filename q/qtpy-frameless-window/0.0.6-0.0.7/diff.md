# Comparing `tmp/QtPy-Frameless-Window-0.0.6.tar.gz` & `tmp/QtPy-Frameless-Window-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.6.tar", last modified: Mon Apr 10 14:24:33 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.0.7.tar", last modified: Wed Apr 12 14:30:51 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.6.tar` & `QtPy-Frameless-Window-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35823 2023-04-10 13:55:10.340365 QtPy-Frameless-Window-0.0.6/LICENSE
--rw-r--r--   0        0        0      868 2023-04-10 14:23:30.646342 QtPy-Frameless-Window-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      334 2023-04-10 13:41:06.835245 QtPy-Frameless-Window-0.0.6/qt_api/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-10 13:55:10.375881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 13:38:09.871612 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-10 13:55:10.375881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource.py
--rw-r--r--   0        0        0      135 2023-04-10 13:38:09.871612 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource.qrc
--rw-r--r--   0        0        0     1471 2023-04-10 13:55:10.376882 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource_rc.py
--rw-r--r--   0        0        0      270 2023-04-10 13:38:09.871612 QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/title_bar/close.svg
--rw-r--r--   0        0        0      457 2023-04-10 13:56:41.474504 QtPy-Frameless-Window-0.0.6/qtframelesswindow/api_differ/windows.py
--rw-r--r--   0        0        0    13288 2023-04-10 14:13:36.743103 QtPy-Frameless-Window-0.0.6/qtframelesswindow/linux/__init__.py
--rw-r--r--   0        0        0     2920 2023-04-10 13:55:10.390882 QtPy-Frameless-Window-0.0.6/qtframelesswindow/linux/window_effect.py
--rw-r--r--   0        0        0    14832 2023-04-10 14:17:48.095834 QtPy-Frameless-Window-0.0.6/qtframelesswindow/mac/__init__.py
--rw-r--r--   0        0        0     4093 2023-04-10 13:55:10.391881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/mac/window_effect.py
--rw-r--r--   0        0        0     4981 2023-04-10 13:55:10.391881 QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/__init__.py
--rw-r--r--   0        0        0     9024 2023-04-10 13:39:48.695927 QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/title_bar_buttons.py
--rw-r--r--   0        0        0      885 2023-04-10 14:01:03.589216 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/__init__.py
--rw-r--r--   0        0        0     9302 2023-04-10 14:05:49.422983 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/linux_utils.py
--rw-r--r--   0        0        0     8330 2023-04-10 14:09:51.608296 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/mac_utils.py
--rw-r--r--   0        0        0     7816 2023-04-10 13:57:02.791321 QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/win32_utils.py
--rw-r--r--   0        0        0     8675 2023-04-10 13:55:10.394880 QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-10 13:55:10.394880 QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/c_structures.py
--rw-r--r--   0        0        0     8979 2023-04-10 13:57:21.082863 QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/window_effect.py
--rw-r--r--   0        0        0     1163 2023-04-10 13:55:10.341348 QtPy-Frameless-Window-0.0.6/README.md
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-12 06:26:37.916046 QtPy-Frameless-Window-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1000 2023-04-12 14:29:59.331412 QtPy-Frameless-Window-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-04-12 06:26:37.920046 QtPy-Frameless-Window-0.0.7/qt_api/__init__.py
+-rw-r--r--   0        0        0     1169 2023-04-12 14:27:18.865226 QtPy-Frameless-Window-0.0.7/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 06:26:37.921076 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/__init__.py
+-rw-r--r--   0        0        0     1471 2023-04-12 14:30:25.601836 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource.py
+-rw-r--r--   0        0        0      135 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource.qrc
+-rw-r--r--   0        0        0     1471 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource_rc.py
+-rw-r--r--   0        0        0      270 2023-04-12 06:26:37.921901 QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/title_bar/close.svg
+-rw-r--r--   0        0        0      457 2023-04-12 08:04:13.929582 QtPy-Frameless-Window-0.0.7/qtframelesswindow/api_differ/windows.py
+-rw-r--r--   0        0        0     4351 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.7/qtframelesswindow/linux/__init__.py
+-rw-r--r--   0        0        0     2920 2023-04-12 08:04:14.020784 QtPy-Frameless-Window-0.0.7/qtframelesswindow/linux/window_effect.py
+-rw-r--r--   0        0        0     4533 2023-04-12 14:27:18.867207 QtPy-Frameless-Window-0.0.7/qtframelesswindow/mac/__init__.py
+-rw-r--r--   0        0        0     4093 2023-04-12 08:04:14.032673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/mac/window_effect.py
+-rw-r--r--   0        0        0     5064 2023-04-12 14:27:18.868207 QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/__init__.py
+-rw-r--r--   0        0        0     9024 2023-04-12 12:28:36.521987 QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/title_bar_buttons.py
+-rw-r--r--   0        0        0      885 2023-04-12 06:26:37.922905 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/__init__.py
+-rw-r--r--   0        0        0     9302 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/linux_utils.py
+-rw-r--r--   0        0        0     8330 2023-04-12 08:04:14.040673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/mac_utils.py
+-rw-r--r--   0        0        0     7816 2023-04-12 08:04:14.041673 QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/win32_utils.py
+-rw-r--r--   0        0        0     8675 2023-04-12 12:00:49.607910 QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-12 06:26:37.924905 QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/c_structures.py
+-rw-r--r--   0        0        0     8979 2023-04-12 08:04:14.052662 QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/window_effect.py
+-rw-r--r--   0        0        0     1156 2023-04-12 14:26:31.626229 QtPy-Frameless-Window-0.0.7/README.md
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.7/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.0.6/LICENSE` & `QtPy-Frameless-Window-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/pyproject.toml` & `QtPy-Frameless-Window-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,28 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.6"
-version = "0.0.6"
+version = "0.0.7"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
 
+[project.optional-dependencies]
+pyqt = [
+    "pyside2>=5.15.2.1",
+    "pyside6>=6.5.0",
+    "pyqt5>=5.15.9",
+    "pyqt6>=6.4.2",
+]
+
 [build-system]
 build-backend = "pdm.pep517.api"
 requires = [
     "pdm-pep517>=1.0.0",
 ]
```

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/_rc/resource_rc.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/_rc/resource_rc.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/linux/window_effect.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/mac/window_effect.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/__init__.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -113,18 +113,20 @@
         self.hBoxLayout.insertSpacing(0, 10)
         self.hBoxLayout.insertWidget(1, self.iconLabel, 0, Qt.AlignLeft)
         self.window().windowIconChanged.connect(self.setIcon)
 
         # add title label
         self.titleLabel = QLabel(self)
         self.hBoxLayout.insertWidget(2, self.titleLabel, 0, Qt.AlignLeft)
+        # change color to black due to qt6 is white
         self.titleLabel.setStyleSheet("""
             QLabel{
                 background: transparent;
                 font: 13px 'Segoe UI';
+                color:black;
                 padding: 0 4px
             }
         """)
         self.window().windowTitleChanged.connect(self.setTitle)
 
     def setTitle(self, title):
         """ set the title of title bar
```

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/titlebar/title_bar_buttons.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/__init__.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/linux_utils.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/mac_utils.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/utils/win32_utils.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/__init__.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/c_structures.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/qtframelesswindow/windows/window_effect.py` & `QtPy-Frameless-Window-0.0.7/qtframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.6/README.md` & `QtPy-Frameless-Window-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 To install use pip:
 ```shell
 pip install QtPy-Frameless-Window
 ```
 Or clone the repo:
 ```shell
 git clone https://github.com/TaoChenyue/QtPy-Frameless-Window.git
-python setup.py install
+pip install -e .
 ```
 
 ## FQ
 + Q: Why acrylic window response slowly when dragging its edge on Windows platform?<br>
 A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
```

### Comparing `QtPy-Frameless-Window-0.0.6/PKG-INFO` & `QtPy-Frameless-Window-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.6
+Version: 0.0.7
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Provides-Extra: pyqt
 Project-URL: Homepage, https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # QtPy-Frameless-Window
 
@@ -30,14 +31,14 @@
 To install use pip:
 ```shell
 pip install QtPy-Frameless-Window
 ```
 Or clone the repo:
 ```shell
 git clone https://github.com/TaoChenyue/QtPy-Frameless-Window.git
-python setup.py install
+pip install -e .
 ```
 
 ## FQ
 + Q: Why acrylic window response slowly when dragging its edge on Windows platform?<br>
 A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
```

