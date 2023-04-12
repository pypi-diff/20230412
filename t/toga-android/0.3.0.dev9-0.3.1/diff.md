# Comparing `tmp/toga-android-0.3.0.dev9.tar.gz` & `tmp/toga-android-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-android-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:21 2018, max compression
+gzip compressed data, was "toga-android-0.3.1.tar", last modified: Wed Apr 12 01:58:28 2023, max compression
```

## Comparing `toga-android-0.3.0.dev9.tar` & `toga-android-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,90 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     2302 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/tests/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-android-0.3.0.dev9/tests/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      277 2017-12-22 11:14:30.000000 toga-android-0.3.0.dev9/tests/test_implementation.py
--rw-r--r--   0 rkm        (501) staff       (20)      115 2017-12-22 11:14:05.000000 toga-android-0.3.0.dev9/MANIFEST.in
--rw-r--r--   0 rkm        (501) staff       (20)     1657 2018-07-07 05:52:00.000000 toga-android-0.3.0.dev9/setup.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     2302 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)      653 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)       22 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)       19 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android.egg-info/dependency_links.txt
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/setup.cfg
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android/hardware/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2018-05-26 09:29:22.000000 toga-android-0.3.0.dev9/toga_android/hardware/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     2103 2018-06-10 23:51:35.000000 toga-android-0.3.0.dev9/toga_android/window.py
--rw-r--r--   0 rkm        (501) staff       (20)     2042 2017-12-23 03:47:56.000000 toga-android-0.3.0.dev9/toga_android/layout.py
--rw-r--r--   0 rkm        (501) staff       (20)      351 2018-05-17 17:50:36.000000 toga-android-0.3.0.dev9/toga_android/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1575 2018-01-25 04:51:21.000000 toga-android-0.3.0.dev9/toga_android/factory.py
--rw-r--r--   0 rkm        (501) staff       (20)     1345 2018-07-07 05:52:00.000000 toga-android-0.3.0.dev9/toga_android/app.py
--rw-r--r--   0 rkm        (501) staff       (20)      922 2018-01-25 04:51:21.000000 toga-android-0.3.0.dev9/toga_android/dialogs.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-android-0.3.0.dev9/toga_android/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)       81 2017-12-22 11:14:05.000000 toga-android-0.3.0.dev9/toga_android/widgets/box.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-android-0.3.0.dev9/toga_android/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1545 2018-01-25 04:51:21.000000 toga-android-0.3.0.dev9/toga_android/widgets/textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     1525 2018-01-25 04:51:21.000000 toga-android-0.3.0.dev9/toga_android/widgets/button.py
--rw-r--r--   0 rkm        (501) staff       (20)     1330 2018-01-18 21:56:40.000000 toga-android-0.3.0.dev9/toga_android/widgets/label.py
--rw-r--r--   0 rkm        (501) staff       (20)      177 2018-05-26 09:29:22.000000 toga-android-0.3.0.dev9/toga_android/widgets/passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     1453 2018-05-26 09:29:22.000000 toga-android-0.3.0.dev9/toga_android/widgets/base.py
--rw-r--r--   0 rkm        (501) staff       (20)     1097 2017-12-22 11:14:05.000000 toga-android-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.140164 toga-android-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:57:45.000000 toga-android-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:57:45.000000 toga-android-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 01:57:45.000000 toga-android-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-12 01:58:28.140164 toga-android-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-12 01:57:45.000000 toga-android-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 01:57:45.000000 toga-android-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 01:58:28.140164 toga-android-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-12 01:57:45.000000 toga-android-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.116164 toga-android-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.128164 toga-android-0.3.1/src/toga_android/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.132164 toga-android-0.3.1/src/toga_android/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.132164 toga-android-0.3.1/src/toga_android/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/activity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.136164 toga-android-0.3.1/src/toga_android/libs/android/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/android/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.136164 toga-android-0.3.1/src/toga_android/libs/androidx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/androidx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/libs/androidx/swiperefreshlayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.140164 toga-android-0.3.1/src/toga_android/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/datepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/imageview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.140164 toga-android-0.3.1/src/toga_android/widgets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/internal/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/timepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-12 01:57:45.000000 toga-android-0.3.1/src/toga_android/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.132164 toga-android-0.3.1/src/toga_android.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-12 01:58:27.000000 toga-android-0.3.1/src/toga_android.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-12 01:58:28.000000 toga-android-0.3.1/src/toga_android.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:27.000000 toga-android-0.3.1/src/toga_android.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 01:58:27.000000 toga-android-0.3.1/src/toga_android.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:12.000000 toga-android-0.3.1/src/toga_android.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 01:58:27.000000 toga-android-0.3.1/src/toga_android.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 01:58:27.000000 toga-android-0.3.1/src/toga_android.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.140164 toga-android-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.140164 toga-android-0.3.1/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:28.140164 toga-android-0.3.1/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 01:57:45.000000 toga-android-0.3.1/tests_backend/widgets/textinput.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-android-0.3.0.dev9/toga_android/window.py` & `toga-android-0.3.1/src/toga_android/widgets/timepicker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,64 @@
+from datetime import time
 
-class AndroidViewport:
-    def __init__(self, native):
-        self.native = native
-        self.dpi = 96  # FIXME This is almost certainly wrong...
-        # self.dpi = ... self.interface.app._impl.device_scale
-
-    @property
-    def width(self):
-        return self.native.ClientSize.Width
-
-    @property
-    def height(self):
-        return self.native.ClientSize.Height
-
-
-class Window:
-    def __init__(self, interface):
-        self.interface = interface
-        self.interface._impl = self
-        self.create()
+from ..libs.android import R__drawable
+from ..libs.android.widget import (
+    TimePickerDialog,
+    TimePickerDialog__OnTimeSetListener as OnTimeSetListener,
+)
+from .internal.pickers import PickerBase
+
+
+class TimePickerListener(OnTimeSetListener):
+    def __init__(self, picker_impl):
+        super().__init__()
+        self.picker_impl = picker_impl
+
+    def onTimeSet(self, _, *args):
+        new_value = time(*args)
+
+        self.picker_impl._dialog = None
+        self.picker_impl.interface.value = new_value
+        if self.picker_impl.interface.on_change:
+            self.picker_impl.interface.on_change(self.picker_impl)
+
+
+class TimePicker(PickerBase):
+    @classmethod
+    def _get_icon(cls):
+        return R__drawable.ic_menu_recent_history
+
+    @classmethod
+    def _get_hint(cls):
+        return "HH:MM"
 
     def create(self):
-        pass
-
-    def set_app(self, app):
-        self._create()
-
-    def set_content(self, widget):
-        if self.native is None:
-            widget.native = TogaLayout(self.app.native, widget)
-
-        # Add all children to the content widget.
-        for child in widget.interface.children:
-            child._impl.container = widget
-
-        self.app._impl.setContentView(self._container._impl)
-
-    def set_title(self, title):
-        pass
-
-    def set_position(self, position):
-        pass
-
-    def set_size(self, size):
-        pass
-
-    def set_app(self, app):
-        pass
-
-    def create_toolbar(self):
-        pass
+        return super().create()
 
-    def show(self):
+    def set_on_change(self, handler):
+        # nothing to do here, but it just has to exist
         pass
 
-    def set_full_screen(self, is_full_screen):
-        self.interface.factory.not_implemented('Window.set_full_screen()')
-
-    def info_dialog(self, title, message):
-        self.interface.factory.not_implemented('Window.info_dialog()')
-
-    def question_dialog(self, title, message):
-        self.interface.factory.not_implemented('Window.question_dialog()')
-
-    def confirm_dialog(self, title, message):
-        self.interface.factory.not_implemented('Window.confirm_dialog()')
-
-    def error_dialog(self, title, message):
-        self.interface.factory.not_implemented('Window.error_dialog()')
-
-    def stack_trace_dialog(self, title, message, content, retry=False):
-        self.interface.factory.not_implemented('Window.stack_trace_dialog()')
+    def get_value(self):
+        return self._value
 
-    def save_file_dialog(self, title, suggested_filename, file_types):
-        self.interface.factory.not_implemented('Window.save_file_dialog()')
+    def set_value(self, value):
+        self._value = value
+        self.native.setText(value.isoformat(timespec="minutes"))
+        if self._dialog is not None:
+            self._dialog.updateTime(value.hour, value.minute)
+
+    def set_min_time(self, value):
+        self.interface.factory.not_implemented("TimePicker.set_min_time()")
+
+    def set_max_time(self, value):
+        self.interface.factory.not_implemented("TimePicker.set_max_time()")
+
+    def _create_dialog(self):
+        self._dialog = TimePickerDialog(
+            self._native_activity,
+            TimePickerListener(self),
+            self._value.hour,
+            self._value.minute,
+            True,
+        )
+        self._dialog.show()
```

### Comparing `toga-android-0.3.0.dev9/toga_android/factory.py` & `toga-android-0.3.1/src/toga_android/factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,64 @@
+from . import dialogs
 from .app import App, MainWindow
-# from .color import color
-# from .command import Command
-# from .font import font
+from .command import Command
+from .fonts import Font
+from .icons import Icon
+from .images import Image
+from .paths import paths
 from .widgets.box import Box
 from .widgets.button import Button
-# from .widgets.canvas import Canvas
-# from .widgets.detailedlist import DetailedList
-# from .widgets.icon import Icon
-# from .widgets.image import *
-# from .widgets.imageview import *
+from .widgets.canvas import Canvas
+from .widgets.datepicker import DatePicker
+from .widgets.detailedlist import DetailedList
+from .widgets.imageview import ImageView
 from .widgets.label import Label
-# from .widgets.multilinetextinput import *
-# from .widgets.numberinput import NumberInput
-# from .widgets.optioncontainer import *
-# from .widgets.passwordinput import *
-# from .widgets.progressbar import *
-# from .widgets.scrollcontainer import *
-# from .widgets.selection import Selection
-# from .widgets.slider import *
-# from .widgets.splitcontainer import *
-# from .widgets.switch import *
-# from .widgets.table import *
+from .widgets.multilinetextinput import MultilineTextInput
+from .widgets.numberinput import NumberInput
+from .widgets.passwordinput import PasswordInput
+from .widgets.progressbar import ProgressBar
+from .widgets.scrollcontainer import ScrollContainer
+from .widgets.selection import Selection
+from .widgets.slider import Slider
+from .widgets.switch import Switch
+from .widgets.table import Table
 from .widgets.textinput import TextInput
-# from .widgets.tree import *
-# from .widgets.webview import *
+from .widgets.timepicker import TimePicker
+from .widgets.webview import WebView
 from .window import Window
 
 
 def not_implemented(feature):
-    print('[Android] Not implemented: {}'.format(feature))
+    print(f"[Android] Not implemented: {feature}")  # pragma: nocover
 
 
 __all__ = [
-    'not_implemented',
-
-    'App', 'MainWindow',
-    # 'color',
-    # 'Command',
-    # 'font',
-    'Box',
-    'Button',
-    # 'Canvas',
-    'DetailedList',
-    # 'Icon',
-    # 'Image',
-    # 'ImageView',
-    'Label',
-    # 'MultilineTextInput',
-    # 'NumberInput',
-    # 'OptionContainer',
-    # 'PasswordInput',
-    # 'ProgressBar',
-    # 'ScrollContainer',
-    # 'Selection',
-    # 'Slider',
-    # 'SplitContainer',
-    # 'Switch',
-    # 'Table',
-    'TextInput',
-    # 'Tree',
-    # 'WebView',
-    'Window',
+    "App",
+    "Box",
+    "Button",
+    "Canvas",
+    "Command",
+    "DatePicker",
+    "Font",
+    "Icon",
+    "Image",
+    "ImageView",
+    "Label",
+    "MainWindow",
+    "MultilineTextInput",
+    "NumberInput",
+    "PasswordInput",
+    "ProgressBar",
+    "Selection",
+    "Slider",
+    "ScrollContainer",
+    "Switch",
+    "Table",
+    "TextInput",
+    "TimePicker",
+    "WebView",
+    "Window",
+    "DetailedList",
+    "not_implemented",
+    "paths",
+    "dialogs",
 ]
```

### Comparing `toga-android-0.3.0.dev9/toga_android/widgets/button.py` & `toga-android-0.3.1/src/toga_android/widgets/selection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,61 @@
 from travertino.size import at_least
 
-from .base import Widget
+from ..libs.android import R__layout
+from ..libs.android.view import Gravity, View__MeasureSpec
+from ..libs.android.widget import ArrayAdapter, OnItemSelectedListener, Spinner
+from .base import Widget, align
 
 
-class TogaButton(extends=android.widget.Button):
-    @super({context: android.content.Context})
-    def __init__(self, context, interface):
-        self._interface = interface
+class TogaOnItemSelectedListener(OnItemSelectedListener):
+    def __init__(self, impl):
+        super().__init__()
+        self._impl = impl
 
+    def onItemSelected(self, _parent, _view, _position, _id):
+        if self._impl.interface.on_select:
+            self._impl.interface.on_select(widget=self._impl.interface)
 
-class TogaButtonListener(implements=android.view.View[OnClickListener]):
-    @super({})
-    def __init__(self, interface):
-        self._interface = interface
 
-    def onClick(self, v: android.view.View) -> None:
-        self._interface.on_press(self._interface)
-
-
-class Button(Widget):
+class Selection(Widget):
     def create(self):
-        self.native = TogaButton(self.app._impl, self.interface)
-
-        self._listener = TogaButtonListener(self)
-
-        self.native.setOnClickListener(self._listener)
+        self.native = Spinner(self._native_activity, Spinner.MODE_DROPDOWN)
+        self.native.setOnItemSelectedListener(TogaOnItemSelectedListener(impl=self))
+        self.adapter = ArrayAdapter(
+            self._native_activity, R__layout.simple_spinner_item
+        )
+        self.adapter.setDropDownViewResource(R__layout.simple_spinner_dropdown_item)
+        self.native.setAdapter(self.adapter)
+        # Create a mapping from text to numeric index to support `select_item()`.
+        self._indexByItem = {}
+
+    def add_item(self, item):
+        new_index = self.adapter.getCount()
+        self.adapter.add(str(item))
+        self._indexByItem[item] = new_index
+
+    def select_item(self, item):
+        self.native.setSelection(self._indexByItem[item])
+
+    def get_selected_item(self):
+        selected = self.native.getSelectedItem()
+        if selected:
+            return str(selected)
+        else:
+            return None
 
-    def set_label(self, label):
-        self.native.setText(self.interface.label)
+    def remove_all_items(self):
+        self.adapter.clear()
 
-    def set_enabled(self, value):
-        self.interface.factory.not_implemented('Button.set_enabled()')
+    def rehint(self):
+        self.native.measure(
+            View__MeasureSpec.UNSPECIFIED, View__MeasureSpec.UNSPECIFIED
+        )
+        self.interface.intrinsic.width = at_least(self.native.getMeasuredWidth())
+        self.interface.intrinsic.height = self.native.getMeasuredHeight()
 
-    def set_background_color(self, value):
-        self.interface.factory.not_implemented('Button.set_background_color()')
+    def set_alignment(self, value):
+        self.native.setGravity(Gravity.CENTER_VERTICAL | align(value))
 
-    def set_on_press(self, handler):
-        # No special handling required
+    def set_on_select(self, handler):
+        # No special handling is required.
         pass
-
-    def rehint(self):
-        if self.native.getMeasuredWidth():
-            # print("REHINT button", self, self.native.getMeasuredWidth(), self.native.getMeasuredHeight())
-            self.interface.intrinsic.width = at_least(self.native.getMeasuredWidth() / self.app._impl.device_scale)
-            self.interface.intrinsic.height = self.native.getMeasuredHeight() / self.app._impl.device_scale
```

### Comparing `toga-android-0.3.0.dev9/README.rst` & `toga-android-0.3.1/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -5,31 +5,38 @@
 
 **Toga requires Python 3**
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_,
 
 For more details, see the `Toga project on Github`_.
 
+.. _Toga widget toolkit: http://beeware.org/toga
+.. _the core Toga library: https://pypi.python.org/pypi/toga-core
+.. _Toga project on Github: https://github.com/beeware/toga
+
 Community
 ---------
 
 Toga is part of the `BeeWare suite`_. You can talk to the community through:
 
-* `@pybeeware on Twitter`_
-
-* The `pybee/general`_ channel on Gitter.
+* `@beeware@fosstodon.org on Mastodon`_
+* `Discord`_
+* The Toga `Github Discussions forum`_
+
+We foster a welcoming and respectful community as described in our
+`BeeWare Community Code of Conduct`_.
+
+.. _BeeWare suite: http://beeware.org
+.. _@beeware@fosstodon.org on Mastodon: https://fosstodon.org/@beeware
+.. _Discord: https://beeware.org/bee/chat/
+.. _Github Discussions forum: https://github.com/beeware/toga/discussions
+.. _BeeWare Community Code of Conduct: http://beeware.org/community/behavior/
 
 Contributing
 ------------
 
 If you experience problems with this backend, `log them on GitHub`_. If you
 want to contribute code, please `fork the code`_ and `submit a pull request`_.
 
-.. _Toga widget toolkit: http://pybee.org/toga
-.. _the core Toga library: https://pypi.python.org/pypi/toga-core
-.. _Toga project on Github: https://github.com/pybee/toga
-.. _BeeWare suite: http://pybee.org
-.. _@pybeeware on Twitter: https://twitter.com/pybeeware
-.. _pybee/general: https://gitter.im/pybee/general
-.. _log them on Github: https://github.com/pybee/toga/issues
-.. _fork the code: https://github.com/pybee/toga
-.. _submit a pull request: https://github.com/pybee/toga/pulls
+.. _log them on Github: https://github.com/beeware/toga/issues
+.. _fork the code: https://github.com/beeware/toga
+.. _submit a pull request: https://github.com/beeware/toga/pulls
```

