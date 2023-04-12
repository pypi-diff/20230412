# Comparing `tmp/toga-dummy-0.3.0.dev9.tar.gz` & `tmp/toga-dummy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-dummy-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:18 2018, max compression
+gzip compressed data, was "toga-dummy-0.3.1.tar", last modified: Wed Apr 12 01:58:43 2023, max compression
```

## Comparing `toga-dummy-0.3.0.dev9.tar` & `toga-dummy-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,62 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     2383 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     2383 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)     1227 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)       22 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)       11 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy.egg-info/dependency_links.txt
--rw-r--r--   0 rkm        (501) staff       (20)     1550 2018-07-07 05:52:00.000000 toga-dummy-0.3.0.dev9/setup.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy/
--rw-r--r--   0 rkm        (501) staff       (20)       31 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/color.py
--rw-r--r--   0 rkm        (501) staff       (20)      178 2018-05-26 09:29:22.000000 toga-dummy-0.3.0.dev9/toga_dummy/command.py
--rw-r--r--   0 rkm        (501) staff       (20)     1816 2018-06-10 23:51:35.000000 toga-dummy-0.3.0.dev9/toga_dummy/window.py
--rw-r--r--   0 rkm        (501) staff       (20)      375 2018-05-17 17:50:36.000000 toga-dummy-0.3.0.dev9/toga_dummy/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      256 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/font.py
--rw-r--r--   0 rkm        (501) staff       (20)    15924 2018-01-12 22:09:22.000000 toga-dummy-0.3.0.dev9/toga_dummy/test_implementation.py
--rw-r--r--   0 rkm        (501) staff       (20)     1532 2018-01-25 04:51:21.000000 toga-dummy-0.3.0.dev9/toga_dummy/factory.py
--rw-r--r--   0 rkm        (501) staff       (20)      469 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/container.py
--rw-r--r--   0 rkm        (501) staff       (20)    15739 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/utils.py
--rw-r--r--   0 rkm        (501) staff       (20)      765 2018-07-07 05:52:00.000000 toga-dummy-0.3.0.dev9/toga_dummy/app.py
--rw-r--r--   0 rkm        (501) staff       (20)      333 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/dialogs.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)      194 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/icon.py
--rw-r--r--   0 rkm        (501) staff       (20)      604 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/tree.py
--rw-r--r--   0 rkm        (501) staff       (20)      254 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)      103 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/box.py
--rw-r--r--   0 rkm        (501) staff       (20)      322 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/splitcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      885 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/detailedlist.py
--rw-r--r--   0 rkm        (501) staff       (20)      436 2018-05-26 09:29:22.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/multilinetextinput.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      719 2018-01-18 21:56:40.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)      467 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/switch.py
--rw-r--r--   0 rkm        (501) staff       (20)      376 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/scrollcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      465 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/slider.py
--rw-r--r--   0 rkm        (501) staff       (20)      341 2018-01-12 22:11:27.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/button.py
--rw-r--r--   0 rkm        (501) staff       (20)      363 2018-02-21 05:36:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/progressbar.py
--rw-r--r--   0 rkm        (501) staff       (20)      249 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/navigationview.py
--rw-r--r--   0 rkm        (501) staff       (20)      334 2018-01-18 21:56:40.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/label.py
--rw-r--r--   0 rkm        (501) staff       (20)      739 2018-01-18 21:56:40.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/numberinput.py
--rw-r--r--   0 rkm        (501) staff       (20)      134 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)      657 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/table.py
--rw-r--r--   0 rkm        (501) staff       (20)      576 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/selection.py
--rw-r--r--   0 rkm        (501) staff       (20)      558 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/webview.py
--rw-r--r--   0 rkm        (501) staff       (20)      319 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/optioncontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      274 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/image.py
--rw-r--r--   0 rkm        (501) staff       (20)     1367 2017-12-23 03:47:56.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/base.py
--rw-r--r--   0 rkm        (501) staff       (20)     2675 2018-07-07 05:52:00.000000 toga-dummy-0.3.0.dev9/toga_dummy/widgets/canvas.py
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:18.000000 toga-dummy-0.3.0.dev9/setup.cfg
--rw-r--r--   0 rkm        (501) staff       (20)     1174 2017-12-22 11:14:05.000000 toga-dummy-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:43.194497 toga-dummy-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-12 01:58:43.194497 toga-dummy-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-12 01:58:43.194497 toga-dummy-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:43.170496 toga-dummy-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:43.178496 toga-dummy-0.3.1/src/toga_dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/test_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:43.194497 toga-dummy-0.3.1/src/toga_dummy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/datepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/timepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-12 01:58:01.000000 toga-dummy-0.3.1/src/toga_dummy/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:43.182496 toga-dummy-0.3.1/src/toga_dummy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-12 01:58:43.000000 toga-dummy-0.3.1/src/toga_dummy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 01:58:43.000000 toga-dummy-0.3.1/src/toga_dummy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:43.000000 toga-dummy-0.3.1/src/toga_dummy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 01:58:43.000000 toga-dummy-0.3.1/src/toga_dummy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:28.000000 toga-dummy-0.3.1/src/toga_dummy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-12 01:58:43.000000 toga-dummy-0.3.1/src/toga_dummy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 01:58:43.000000 toga-dummy-0.3.1/src/toga_dummy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/window.py` & `toga-dummy-0.3.1/src/toga_dummy/window.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,81 @@
-from .utils import not_required_on, LoggedObject
+from .utils import LoggedObject, not_required, not_required_on
+
+
+@not_required
+class Viewport:
+    def __init__(self, window):
+        self.baseline_dpi = 96
+        self.dpi = 96
+        self.window = window
+
+    @property
+    def width(self):
+        return self.window.get_size()[0]
+
+    @property
+    def height(self):
+        return self.window.get_size()[1]
 
 
 class Window(LoggedObject):
-    def __init__(self, interface):
+    def __init__(self, interface, title, position, size):
         super().__init__()
         self.interface = interface
 
-    def create(self):
-        self.action('create Window')
+        self.set_title(title)
+        self.set_position(position)
+        self.set_size(size)
 
     def create_toolbar(self):
-        self._action('create toolbar')
+        self._action("create toolbar")
+
+    def clear_content(self):
+        self._action("clear content")
 
     def set_content(self, widget):
-        self._action('set content', widget=widget)
+        self._action("set content", widget=widget)
+        self._set_value("content", widget)
+        widget.viewport = Viewport(self)
+
+    def get_title(self):
+        return self._get_value("title")
 
     def set_title(self, title):
-        self._set_value('title', title)
+        self._set_value("title", title)
+
+    def get_position(self):
+        return self._get_value("position")
 
     def set_position(self, position):
-        self._set_value('position', position)
+        self._set_value("position", position)
+
+    def get_size(self):
+        return self._get_value("size")
 
     def set_size(self, size):
-        self._set_value('size', size)
+        self._set_value("size", size)
 
     def set_app(self, app):
-        self._set_value('app', app)
+        self._set_value("app", app)
 
     def show(self):
-        self._action('show')
+        self._action("show")
+        self._set_value("visible", True)
 
-    def set_full_screen(self, is_full_screen):
-        self._set_value('is_full_screen', is_full_screen)
-
-    @not_required_on('mobile')
-    def on_close(self):
-        self._action('handle Window on_close')
-
-    def info_dialog(self, title, message):
-        self._action('show info dialog', title=title, message=message)
+    def hide(self):
+        self._action("hide")
+        self._set_value("visible", False)
 
-    def question_dialog(self, title, message):
-        self._action('show question dialog', title=title, message=message)
+    def get_visible(self):
+        return self._get_value("visible")
 
-    def confirm_dialog(self, title, message):
-        self._action('show confirm dialog', title=title, message=message)
+    def close(self):
+        self._action("close")
 
-    def error_dialog(self, title, message):
-        self._action('show error dialog', title=title, message=message)
-
-    def stack_trace_dialog(self, title, message, content, retry=False):
-        self._action('show stack trace dialog', title=title, message=message, content=content, retry=retry)
+    @not_required_on("mobile")
+    def set_full_screen(self, is_full_screen):
+        self._set_value("is_full_screen", is_full_screen)
 
-    def save_file_dialog(self, title, suggested_filename, file_types):
-        self._action(
-            'show save file dialog', title=title, suggested_filename=suggested_filename, file_types=file_types
-        )
+    @not_required
+    def toga_on_close(self):
+        self._action("handle Window on_close")
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/test_implementation.py` & `toga-dummy-0.3.1/src/toga_dummy/test_implementation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,72 @@
 import ast
+import importlib
 import os
 import unittest
-from collections import namedtuple, defaultdict
+from collections import defaultdict, namedtuple
+
+try:
+    # Usually, the pattern is "import module; if it doesn't exist,
+    # import the shim". However, we need the 3.10 API for entry_points,
+    # as the 3.8 didn't support the `groups` argument to entry_points.
+    # Therefore, we try to import the compatibility shim first; and fall
+    # back to the stdlib module if the shim isn't there.
+    from importlib_metadata import entry_points
+except ImportError:
+    from importlib.metadata import entry_points
+
 from itertools import zip_longest
+from os.path import join
+from pathlib import Path
 
 import toga_dummy
 
 
 class NoDefault:
-    """ This utility class to indicate that no argument default exists.
-    The use of `None` is not possible because it itself could be a default argument value."""
+    """This utility class to indicate that no argument default exists.
+
+    The use of `None` is not possible because it itself could be a
+    default argument value.
+    """
 
     def __eq__(self, other):
         if isinstance(other, NoDefault):
             return True
         else:
             return False
 
     def __repr__(self):
-        return 'no_default'
+        return "no_default"
 
 
-FunctionArguments = namedtuple('FunctionArguments', ['args', 'vararg', 'kwarg', 'kwonlyargs'])
+FunctionArguments = namedtuple(
+    "FunctionArguments", ["args", "vararg", "kwarg", "kwonlyargs"]
+)
 
 
 class DefinitionExtractor:
-    """ The DefinitionExtractor consumes a .py file and extracts information,
-        with the help of the 'ast' module from it.
-        Non existing files result in a empty DefinitionExtractor, this means the all properties
-        return empty lists or dicts.
+    """The DefinitionExtractor consumes a .py file and extracts information,
+    with the help of the 'ast' module from it.
 
-        Args:
-            path (str): The path to the .py file.
+    Non-existing files result in an empty DefinitionExtractor, this means the
+    all properties return empty lists or dicts.
+
+    Args:
+        path (str): The path to the .py file.
     """
 
     def __init__(self, path, platform_category=None):
         self.exists = os.path.isfile(path)
         self._classes = {}
         self._methods = defaultdict(dict)
         self.platform = platform_category if platform_category else None
 
         if self.exists:
             # open the file and parse it with the ast module.
-            with open(path, 'r') as f:
+            with open(path) as f:
                 lines = f.read()
             self.tree = ast.parse(lines)
             self._extract_file()
 
     def _extract_file(self):
         self._extract_classes()
         self._extract_class_methods()
@@ -60,29 +80,41 @@
         return self._methods.keys()
 
     def _extract_classes(self):
         for node in ast.walk(self.tree):
             if isinstance(node, ast.ClassDef):
                 if self.is_required_for_platform(node):
                     self._classes[node.name] = node  # use the class name as the key
+            elif isinstance(node, ast.Assign) and node.col_offset == 0:
+                # Allow a class with no new methods to be defined by assigning
+                # from an existing class. The col_offset means we only pay
+                # attention to assignments at the top level of a module, not
+                # assignments inside method bodies.
+                for target in node.targets:
+                    if isinstance(target, ast.Name):
+                        self._classes[target.id] = node
 
     def is_required_for_platform(self, node):
-        """ Checks if the class or function is required for the given platform.
+        """Checks if the class or function is required for the given platform.
         It looks for a decorator with the name `not_required_on`.
 
         Returns:
             `True` if the class/function is required for the platform.
             `False` if the class/function is not required and can be dropped for this platform.
         """
         if node.decorator_list:  # check if a decorator list exists
             for decorator in node.decorator_list:
                 try:
-                    if decorator.func.id == 'not_required':
+                    # @not_required is a bare decorator, so the decorator node
+                    # has an `id` attribute.
+                    # @not_required_on is a decorator factory, so the decorator
+                    # node contains a function that has an id.
+                    if getattr(decorator, "id", None) == "not_required":
                         return False
-                    elif decorator.func.id == 'not_required_on':
+                    elif decorator.func.id == "not_required_on":
                         platforms_to_skip = [arg.s for arg in decorator.args]
                         if self.platform.intersection(set(platforms_to_skip)):
                             return False
                 except Exception:
                     pass
         return True
 
@@ -106,64 +138,77 @@
             elif isinstance(default, ast.Call):
                 defaults.append(default.func)
             elif isinstance(default, ast.Attribute):
                 defaults.append(default.value)
             elif isinstance(default, ast.Name):
                 defaults.append(default.id)
             else:
-                raise RuntimeWarning('ast classes of type "{}" can not be handled at the moment. '
-                                     'Please implement to make this warning disappear.'.format(default))
+                raise RuntimeWarning(
+                    'ast classes of type "{}" can not be handled at the moment. '
+                    "Please implement to make this warning disappear.".format(default)
+                )
         return defaults
 
     def _extract_class_methods(self):
-        """ Extract all the methods from the classes and save them in `self.methods`.
-        Use the combination of class and method name, like so: `<class_name>.<method_name>` as the key.
+        """Extract all the methods from the classes and save them in
+        `self.methods`.
+
+        Use the combination of class and method name, like so:
+        `<class_name>.<method_name>` as the key.
         """
         for class_name in self._classes:
             for node in ast.walk(self._classes[class_name]):
                 if isinstance(node, ast.FunctionDef):
                     if self.is_required_for_platform(node):
-                        function_id = '{}.{}'.format(class_name, node.name)
-                        self._methods[function_id]['node'] = node
-                        self._methods[function_id]['arguments'] = self._extract_function_signature(node)
+                        function_id = f"{class_name}.{node.name}"
+                        self._methods[function_id]["node"] = node
+                        self._methods[function_id][
+                            "arguments"
+                        ] = self._extract_function_signature(node)
 
     def _extract_function_signature(self, node):
         for node in ast.walk(node):
             if isinstance(node, ast.arguments):
                 # Extract positional arguments and possible default values.
                 args = [arg.arg for arg in node.args]
                 args_defaults = self._get_function_defaults(node)
                 # Extract kwonlyargs and defaults.
                 kwonlyargs = [arg.arg for arg in node.kwonlyargs]
                 kwonlyargs_defaults = self._get_function_defaults(node, kwonlyargs=True)
 
                 # Combine arguments and their corresponding default values,
                 # if no default value exists fill it with a NoDefault object.
-                args_plus_defaults = list(zip_longest(reversed(args),
-                                                      reversed(args_defaults),
-                                                      fillvalue=NoDefault()))
-                kwonlyargs_plus_defaults = list(zip_longest(reversed(kwonlyargs),
-                                                            reversed(kwonlyargs_defaults),
-                                                            fillvalue=NoDefault()))
+                args_plus_defaults = list(
+                    zip_longest(
+                        reversed(args), reversed(args_defaults), fillvalue=NoDefault()
+                    )
+                )
+                kwonlyargs_plus_defaults = list(
+                    zip_longest(
+                        reversed(kwonlyargs),
+                        reversed(kwonlyargs_defaults),
+                        fillvalue=NoDefault(),
+                    )
+                )
 
                 vararg = node.vararg.arg if node.vararg is not None else None
                 kwarg = node.kwarg.arg if node.kwarg is not None else None
 
                 return FunctionArguments(
                     args=args_plus_defaults,
                     vararg=vararg,
                     kwarg=kwarg,
-                    kwonlyargs=kwonlyargs_plus_defaults
+                    kwonlyargs=kwonlyargs_plus_defaults,
                 )
 
     def get_function_def(self, function_id):
         return self._methods[function_id]
 
     def methods_of_class(self, class_name):
-        """ Get all methods names of a class.
+        """Get all methods names of a class.
 
         Args:
             class_name(str): Name of the class to extract the methodes
 
         Returns:
             Returns a `List` of (str) with all methods names of the class.
 
@@ -172,263 +217,241 @@
         """
         methods = []
         if self.exists:
             if class_name in self._classes.keys():
                 class_node = self._classes[class_name]
                 for node in ast.walk(class_node):
                     if isinstance(node, ast.FunctionDef):
-                        if self.is_required_for_platform(node):
+                        if self.is_required_for_platform(
+                            node
+                        ) and not node.name.startswith("simulate_"):
                             methods.append(node.name)
         return methods
 
 
 def get_platform_category(path_to_backend):
-    name = os.path.basename(path_to_backend)
-    if name in ['toga_cocoa', 'toga_gtk', 'toga_winforms', 'toga_win32', 'toga_uwp']:
-        return {'desktop', name.split('_')[-1]}
-    elif name in ['toga_iOS', 'toga_android']:
-        return {'mobile', name.split('_')[-1]}
-    elif name in ['toga_django', 'toga_flask', 'toga_pyramid']:
-        return {'web', name.split('_')[-1]}
-    elif name in ['toga_curses',]:
-        return {'console', name.split('_')[-1]}
-    elif name in ['toga_tvOS',]:
-        return {'settop', name.split('_')[-1]}
-    elif name in ['toga_watchOS',]:
-        return {'watch', name.split('_')[-1]}
-    else:
-        raise RuntimeError('Couldn\'t identify a supported host platform: "{}"'.format(name))
-
+    backend_name = os.path.basename(path_to_backend)
+    importlib.import_module(backend_name)
+    platform = {ep.value: ep.name for ep in entry_points(group="toga.backends")}[
+        backend_name
+    ]
+
+    return {
+        # Desktop
+        "macOS": {"desktop", backend_name.split("_")[-1]},
+        "windows": {"desktop", backend_name.split("_")[-1]},
+        "linux": {"desktop", backend_name.split("_")[-1]},
+        # Mobile
+        "iOS": {"mobile", backend_name.split("_")[-1]},
+        "android": {"mobile", backend_name.split("_")[-1]},
+    }.get(platform, {platform, backend_name.split("_")[-1]})
+
+
+def get_required_files(platform_category, path_to_backend):
+    # Find the list of files in the dummy backend
+    # that aren't *this* file, or an __init__.py.
+    files = [
+        str(p.relative_to(Path(__file__).parent))
+        for p in Path(__file__).parent.rglob("**/*.py")
+        if str(p) != __file__ and p.name != "__init__.py"
+    ]
+    if "desktop" in platform_category:
+        for f in TOGA_DESKTOP_EXCLUDED_FILES:
+            files.remove(f)
+    if "mobile" in platform_category:
+        for f in TOGA_MOBILE_EXCLUDED_FILES:
+            files.remove(f)
+    if "web" in platform_category:
+        for f in TOGA_WEB_EXCLUDED_FILES:
+            files.remove(f)
+    if "console" in platform_category:
+        for f in TOGA_CONSOLE_EXCLUDED_FILES:
+            files.remove(f)
+    if "settop" in platform_category:
+        for f in TOGA_SETTOP_EXCLUDED_FILES:
+            files.remove(f)
+    if "watch" in platform_category:
+        for f in TOGA_WATCH_EXCLUDED_FILES:
+            files.remove(f)
 
-def get_required_files(path_to_backend):
-    name = os.path.basename(path_to_backend)
-    if name in ['toga_cocoa', 'toga_gtk', 'toga_winforms', 'toga_win32', 'toga_uwp']:
-        return TOGA_BASE_FILES + TOGA_DESKTOP_FILES
-    elif name in ['toga_iOS', 'toga_android']:
-        return TOGA_BASE_FILES + TOGA_MOBILE_FILES
-    elif name in ['toga_django', 'toga_flask', 'toga_pyramid']:
-        return TOGA_BASE_FILES + TOGA_WEB_FILES
-    elif name in ['toga_curses',]:
-        return TOGA_BASE_FILES + TOGA_CONSOLE_FILES
-    elif name in ['toga_tvOS',]:
-        return TOGA_BASE_FILES + TOGA_SETTOP_FILES
-    elif name in ['toga_watchOS',]:
-        return TOGA_BASE_FILES + TOGA_WATCH_FILES
-    else:
-        raise RuntimeError('Couldn\'t identify a supported host platform: "{}"'.format(name))
+    return files
 
 
 def create_impl_tests(root):
-    """ Calling this function with a the path to a Toga backend will return
-    the implementation tests for this backend.
+    """Calling this function with the path to a Toga backend will return the
+    implementation tests for this backend.
 
     Args:
         root (str): The absolute path to a toga backend.
 
     Returns:
         A dictionary of test classes.
     """
     platform_category = get_platform_category(root)
-    dummy_files = collect_dummy_files(get_required_files(root))
+    dummy_files = collect_dummy_files(get_required_files(platform_category, root))
     tests = {}
     for name, dummy_path in dummy_files:
-        if 'widgets' in dummy_path:
-            path = os.path.join(root, 'widgets/{}.py'.format(name))
+        if "widgets" in dummy_path:
+            path = os.path.join(root, f"widgets/{name}.py")
         else:
-            path = os.path.join(root, '{}.py'.format(name))
+            path = os.path.join(root, f"{name}.py")
 
         tests.update(make_toga_impl_check_class(path, dummy_path, platform_category))
     return tests
 
 
-TestFile = namedtuple('TestFile', ['name', 'path'])
+TestFile = namedtuple("TestFile", ["name", "path"])
 
 
 def collect_dummy_files(required_files):
     dummy_files = []
     toga_dummy_base = os.path.dirname(toga_dummy.__file__)
 
     for root, dirs, filenames in os.walk(toga_dummy_base):
         for filename in filenames:
             # exclude non .py filenames or start with '__'
-            if filename.startswith('__') or not filename.endswith('.py'):
+            if filename.startswith("__") or not filename.endswith(".py"):
                 continue
 
-            full_filename = os.path.join(root, filename)[len(toga_dummy_base) + 1:]
+            full_filename = os.path.join(root, filename)[len(toga_dummy_base) + 1 :]
             if full_filename in required_files:
                 f = TestFile(filename[:-3], os.path.join(root, filename))
                 dummy_files.append(f)
 
     return dummy_files
 
 
 def make_test_function(element, element_list, error_msg=None):
     def fn(self):
-        self.assertIn(element, element_list, msg=error_msg)
+        self.assertIn(element, element_list, msg=error_msg if error_msg else fn.__doc__)
 
     return fn
 
 
 def make_test_class(path, cls, expected, actual, skip):
-    class_name = '{}ImplTest'.format(cls)
+    class_name = f"{cls}ImplTest"
     test_class = type(class_name, (unittest.TestCase,), {})
 
     if skip:
         test_class = unittest.skip(skip)(test_class)
 
     fn = make_test_function(cls, actual.class_names)
-    fn.__doc__ = "The class {} is defined in {}".format(cls, path)
+    fn.__doc__ = (
+        "Expect class {} to be defined in {}, to be consistent with dummy implementation"
+    ).format(cls, path)
     test_class.test_class_exists = fn
 
     for method in expected.methods_of_class(cls):
         # create a test that checks if the method exists in the class.
         fn = make_test_function(method, actual.methods_of_class(cls))
-        fn.__doc__ = 'The method {}.{}(...) exists'.format(cls, method)
-        setattr(test_class, 'test_{}_exists'.format(method), fn)
+        fn.__doc__ = f"The method {cls}.{method}(...) exists"
+        setattr(test_class, f"test_{method}_exists", fn)
 
         # create tests that check for the right method arguments.
-        method_id = '{}.{}'.format(cls, method)
-        method_def = expected.get_function_def(method_id)['arguments']
+        method_id = f"{cls}.{method}"
+        method_def = expected.get_function_def(method_id)["arguments"]
         try:
-            actual_method_def = actual.get_function_def(method_id)['arguments']
+            actual_method_def = actual.get_function_def(method_id)["arguments"]
         except KeyError:
             actual_method_def = None
 
         if actual_method_def:
             # Create test whether the method takes the right arguments
             # and if the arguments have the right name.
 
             # ARGS
             for arg in method_def.args:
                 fn = make_test_function(arg, actual_method_def.args)
-                fn.__doc__= "The argument {}.{}(..., {}={}, ...) exists".format(cls, method, *arg)
+                fn.__doc__ = "The argument {}.{}(..., {}={}, ...) exists".format(
+                    cls, method, *arg
+                )
                 setattr(
-                    test_class,
-                    'test_{}_arg_{}_default_{}'.format(method, *arg),
-                    fn
+                    test_class, "test_{}_arg_{}_default_{}".format(method, *arg), fn
                 )
 
             # *varargs
             if method_def.vararg:
                 vararg = method_def.vararg
-                actual_vararg = actual_method_def.vararg if actual_method_def.vararg else []
-                fn = make_test_function(vararg, actual_vararg)
-                fn.__doc__ = "The vararg {}.{}(..., *{}, ...) exists".format(cls, method, vararg)
-                setattr(
-                    test_class,
-                    'test_{}_vararg_{}'.format(method, vararg),
-                    fn
+                actual_vararg = (
+                    actual_method_def.vararg if actual_method_def.vararg else []
                 )
+                fn = make_test_function(vararg, actual_vararg)
+                fn.__doc__ = f"The vararg {cls}.{method}(..., *{vararg}, ...) exists"
+                setattr(test_class, f"test_{method}_vararg_{vararg}", fn)
 
             # **kwarg
             if method_def.kwarg:
                 kwarg = method_def.kwarg
-                actual_kwarg = actual_method_def.kwarg if actual_method_def.kwarg else []
-                fn = make_test_function(kwarg, actual_kwarg,
-                                        error_msg='The method does not take kwargs or the '
-                                                  'variable is not named "{}".'.format(kwarg))
-                fn.__doc__ = "The kw argument {}.{}(..., **{}, ...) exists".format(cls, method, kwarg)
-                setattr(
-                    test_class,
-                    'test_{}_kw_{}'.format(method, kwarg),
-                    fn
+                actual_kwarg = (
+                    actual_method_def.kwarg if actual_method_def.kwarg else []
+                )
+                fn = make_test_function(
+                    kwarg,
+                    actual_kwarg,
+                    error_msg="The method does not take kwargs or the "
+                    'variable is not named "{}".'.format(kwarg),
+                )
+                fn.__doc__ = (
+                    f"The kw argument {cls}.{method}(..., **{kwarg}, ...) exists"
                 )
+                setattr(test_class, f"test_{method}_kw_{kwarg}", fn)
 
             # kwonlyargs
             if method_def.kwonlyargs:
                 for kwonlyarg in method_def.kwonlyargs:
                     fn = make_test_function(kwonlyarg, actual_method_def.kwonlyargs)
-                    fn.__doc__ = "The kwonly argument {}.{}(..., {}={}, ...) exists".format(cls, method, *kwonlyarg)
+                    fn.__doc__ = (
+                        "The kwonly argument {}.{}(..., {}={}, ...) exists".format(
+                            cls, method, *kwonlyarg
+                        )
+                    )
                     setattr(
                         test_class,
-                        'test_{}_kwonly_{}_default_{}'.format(method, *kwonlyarg),
-                        fn
+                        "test_{}_kwonly_{}_default_{}".format(method, *kwonlyarg),
+                        fn,
                     )
 
     return class_name, test_class
 
 
 def make_toga_impl_check_class(path, dummy_path, platform):
     prefix = os.path.commonprefix([path, dummy_path])
     expected = DefinitionExtractor(dummy_path, platform)
     if os.path.isfile(path):
         skip = None
         actual = DefinitionExtractor(path)
     else:
-        skip = 'Implementation file {} does not exist'.format(path[len(prefix):])
+        skip = f"Implementation file {path[len(prefix):]} does not exist"
         actual = DefinitionExtractor(path)
 
     test_classes = {}
 
     for cls in expected.class_names:
-        class_name, test_class = make_test_class(path[len(prefix):], cls, expected, actual, skip)
+        class_name, test_class = make_test_class(
+            path[len(prefix) :], cls, expected, actual, skip
+        )
         test_classes[class_name] = test_class
 
     return test_classes
 
 
-# A list of files that must be present in every
-# valid Toga backend implementation.
-TOGA_BASE_FILES = [
-    'app.py',
-    'command.py',
-    'container.py',
-    'dialogs.py',
-    'factory.py',
-    'font.py',
-    'window.py',
-
-    # Widgets
-    'widgets/base.py',
-    'widgets/box.py',
-    'widgets/button.py',
-    'widgets/icon.py',
-    'widgets/image.py',
-    'widgets/imageview.py',
-    'widgets/label.py',
-    'widgets/multilinetextinput.py',
-    'widgets/numberinput.py',
-    'widgets/optioncontainer.py',
-    'widgets/passwordinput.py',
-    'widgets/progressbar.py',
-    'widgets/scrollcontainer.py',
-    'widgets/selection.py',
-    'widgets/slider.py',
-    'widgets/switch.py',
-    'widgets/table.py',
-    'widgets/textinput.py',
-    'widgets/tree.py',
-    'widgets/webview.py'
+# Files that do not need to be present in mobile implementations of Toga.
+TOGA_MOBILE_EXCLUDED_FILES = [
+    join("widgets", "splitcontainer.py"),
 ]
 
-# Files that must only be present
-# in mobile implementations of Toga.
-TOGA_MOBILE_FILES = [
-    'widgets/navigationview.py',
-    'widgets/detailedlist.py',
-]
+# Files that do not need to be present in desktop implementations of Toga.
+TOGA_DESKTOP_EXCLUDED_FILES = []
 
-# Files that must only be present
-# in desktop implementations of Toga.
-TOGA_DESKTOP_FILES = [
-    'widgets/splitcontainer.py',
+# Files do not need to be present in web implementations of Toga.
+TOGA_WEB_EXCLUDED_FILES = [
+    join("widgets", "splitcontainer.py"),
 ]
 
-# Files that must only be present
-# in web implementations of Toga.
-TOGA_WEB_FILES = [
-]
+# Files that do not need to be present in console implementations of Toga.
+TOGA_CONSOLE_EXCLUDED_FILES = []
 
-# Files that must only be present
-# in console implementations of Toga.
-TOGA_CONSOLE_FILES = [
-]
+# Files that do not need to be present in set-top box implementations of Toga.
+TOGA_SETTOP_EXCLUDED_FILES = []
 
-# Files that must only be present
-# in set-top box implementations of Toga.
-TOGA_SETTOP_FILES = [
-]
-
-# Files that must only be present
-# in watch implementations of Toga.
-TOGA_WATCH_FILES = [
-]
+# Files that do not need to be present in watch implementations of Toga.
+TOGA_WATCH_EXCLUDED_FILES = []
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/utils.py` & `toga-dummy-0.3.1/src/toga_dummy/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,65 @@
+import sys
 import unittest
+from unittest.mock import Mock
 
+import pytest
 from travertino.declaration import BaseStyle
 from travertino.layout import BaseBox
 from travertino.size import BaseIntrinsicSize
 
 
 def not_required(method_or_class):
-    """ This decorator function is used to mark methods or classes
-    that they are not required for interface compliance.
+    """This decorator function is used to mark methods or classes that they are
+    not required for interface compliance.
 
-    Args:
-        method_or_class: The method or class to decorate
-
-    Returns:
-        The method or class being decorated
+    :param method_or_class: The method or class to decorate
+    :returns: The method or class being decorated
     """
     return method_or_class
 
 
 def not_required_on(*args):
-    """ This decorator function is used to mark methods or classes
-    that they are not required on certain platforms.
-    This is only used by the implementation checks creation mechanism.
-
-    Args:
-        *args (str): Takes arguments in form of strings.
-            Possible *args are 'mobile', 'desktop',
-            as well as all platform names ('iOS', 'gtk', 'android' ...).
+    """This decorator function is used to mark methods or classes that they are
+    not required on certain platforms. This is only used by the implementation
+    checks creation mechanism.
 
     Examples:
         >>> # Marks the function as only required on platforms that are not "mobile".
         >>> @not_required_on('mobile')
         >>> def open_window():
         >>>     self.window.open()
 
         >>> # Function is not required on "mobile" and "gtk" backends.
         >>> @not_required_on('mobile', 'gtk')
         >>> def open_window():
         >>>     self.window.open()
 
-    Returns:
-        The method or class being decorated
+    :param args: The platform(s) on which the method or class isn't required.
+        Can accept a specific backend (e.g., `gtk`, `iOS`), or a class of platform
+        (e.g., `mobile`, `desktop`).
+    :returns: The method or class being decorated
     """
+
     def _dec(method_or_class):
         return method_or_class
 
     return _dec
 
 
-
 ###########################################################################
 # The event types that can be logged
 ###########################################################################
 
 
 class EventLog:
     # Event types that can be logged
-    SET_VALUE = object()
-    GET_VALUE = object()
-    ACTION = object()
+    SET_VALUE = "set attribute"
+    GET_VALUE = "get attribute"
+    ACTION = "action"
 
     _log = []
     _next_sequence = 0
 
     @classmethod
     def reset(cls):
         cls._log.clear()
@@ -73,377 +70,470 @@
         cls._next_sequence += 1
         return cls._next_sequence
 
     @classmethod
     def log(cls, logtype, instance, **context):
         """Add an entry to the event log.
 
-        Args:
-            logtype: The type of object being logged (SET_VALUE, etc)
-            instance: The instance that generated loggable activity
-            context: A dictionary of data related to the event. The contents
-                of the dictionary will depend on the event that occurred.
-
-        Returns:
-            The sequence value of the log entry
+        :param logtype: The type of object being logged (SET_VALUE, etc.)
+        :param instance: The instance that generated loggable activity
+        :param context: A dictionary of data related to the event. The contents
+            of the dictionary will depend on the event that occurred.
+        :returns: The sequence value of the log entry
         """
         entry = LogEntry(logtype, instance, **context)
         cls._log.append(entry)
         return entry.sequence
 
+    @classmethod
+    def values(cls, instance, attr):
+        """Return all values that an attribute on an instance has had.
+
+        :param instance: The widget instance
+        :param attr: The attribute name to inspect
+        :return: A list of all values that have been assigned to the attribute.
+            Raises AttributeError if the attribute has not been set on the instance.
+        """
+        attrs = set()
+        values = []
+        for entry in cls._log:
+            if entry.logtype == cls.SET_VALUE and entry.instance == instance._impl:
+                if entry.context["attr"] == attr:
+                    values.append(entry.context["value"])
+                else:
+                    attrs.add(entry.context["attr"])
+
+        if values:
+            return values
+
+        if attrs:
+            known_attributes = ", ".join(f"{a!r}" for a in sorted(attrs))
+            raise AttributeError(
+                f"{instance} did not have the attribute {attr!r} set; "
+                f"known attributes were {known_attributes}."
+            )
+        else:
+            raise AttributeError(f"No attributes were set on {instance} ")
+
+    @classmethod
+    def value(cls, instance, attr):
+        """Return the current value of an attribute on an instance.
+
+        :param instance: The widget instance
+        :param attr: The attribute name to inspect
+        :return: The current value of the attribute on the instance. Raises
+            AttributeError if the attribute has not been set on the instance.
+        """
+        attrs = set()
+        for entry in cls._log[-1::-1]:
+            if entry.logtype == cls.SET_VALUE and entry.instance == instance._impl:
+                if entry.context["attr"] == attr:
+                    return entry.context["value"]
+                else:
+                    attrs.add(entry.context["attr"])
+
+        if attrs:
+            known_attributes = ", ".join(f"{a!r}" for a in sorted(attrs))
+            raise AttributeError(
+                f"{instance} did not have the attribute {attr!r} set; "
+                f"known attributes were {known_attributes}."
+            )
+        else:
+            raise AttributeError(f"No attributes were set on {instance} ")
+
+    @classmethod
+    def retrieved(cls, instance, attr):
+        """Determine if an attempt has been made to retrieve the value of an
+        attribute.
+
+        This only includes "normal" attribute access; retrievals made for test
+        purposes are *not* included.
+
+        :param instance: The widget instance
+        :param attr: The attribute name to inspect
+        :return: True if the attribute has been retrieved. Raises AttributeError
+            if no attempt to retrieve the attribute has been made.
+        """
+        attrs = set()
+        for entry in cls._log:
+            if entry.logtype == cls.GET_VALUE and entry.instance == instance._impl:
+                if entry.context["attr"] == attr:
+                    return True
+                else:
+                    attrs.add(entry.context["attr"])
+
+        if attrs:
+            known_attributes = ", ".join(f"{a!r}" for a in sorted(attrs))
+            raise AttributeError(
+                f"{instance} did not retrieve the attribute {attr!r}; "
+                f"known attribute retrievals are {known_attributes}."
+            )
+        else:
+            raise AttributeError(f"No attributes were retrieved on {instance} ")
+
+    @classmethod
+    def performed_actions(cls, instance, action=None):
+        """Return the details of all actions performed on an instance.
+
+        :param instance: The widget instance
+        :param action: (Optional) If provided, the list of actions will be
+            filtered to *only* include the named action.
+        :return: A list of individual actions that have been performed. Each
+            entry is a dictionary consisting of the attributes used to invoke
+            the action.
+        """
+        actions = set()
+        details = []
+        for entry in cls._log:
+            if entry.logtype == cls.ACTION and entry.instance == instance._impl:
+                if action is None or entry.context["action"] == action:
+                    details.append(entry.context)
+                else:
+                    actions.add(entry.context["action"])
+
+        if details:
+            return details
+
+        if actions:
+            known_actions = ", ".join(f"{a!r}" for a in sorted(actions))
+            raise AttributeError(
+                f"{instance} did not perform the action {action!r}; "
+                f"known actions were {known_actions}."
+            )
+        else:
+            raise AttributeError(f"No actions were performed on {instance}")
+
 
 class LogEntry:
     """An entry in the event log.
 
-    Args:
-        logtype: The type of object being logged (SET_VALUE, etc)
-        instance: The instance that generated loggable activity
-        context: A dictionary of data related to the event. The contents
-            of the dictionary will depend on the event that occurred.
+    :param logtype: The type of object being logged (SET_VALUE, etc.)
+    :param instance: The instance that generated loggable activity
+    :param context: A dictionary of data related to the event. The contents of
+        the dictionary will depend on the event that occurred.
     """
+
     def __init__(self, logtype, instance, **context):
         self.sequence = EventLog.next_sequence_value()
         self.logtype = logtype
         self.instance = instance
         self.context = context
 
+    def __repr__(self):
+        return f"<LogEntry: {self.logtype} on {self.instance}"
+
+
+# A constant that can be used to differentiate between a value not being
+# provided, and a value assuming a default value of None.
+NOT_PROVIDED = object()
+
 
 class LoggedObject:
-    """A base class for objects on the dummy backend whose activity will be logged.
+    """A base class for objects on the dummy backend whose activity will be
+    logged.
 
     Objects specified in the dummy backend should extend this class, and
     log any activity they perform using the methods on this object.
     """
-    def __init__(self):
-        self._actions = {}
-        self._sets = {}
-        self._gets = set()
 
     def _set_value(self, attr, value):
         """Set a value on the dummy object.
 
-        Logs the new value for the attribute, and tracks it in the ``_sets``
-        list for the widget.
+        Logs the new value for the attribute, and tracks it in the event log
 
-        Args:
-            attr: The name of the attribute to set
-            value: The new value for the attribute
+        :param attr: The name of the attribute to set
+        :param value: The new value for the attribute
         """
         EventLog.log(EventLog.SET_VALUE, instance=self, attr=attr, value=value)
-        self._sets.setdefault(attr, []).append(value)
 
-    def _get_value(self, attr, default=None):
+    def _get_value(self, attr, default=NOT_PROVIDED):
         """Get a value on the dummy object.
 
-        Logs the request for the attribute, and returns the value as stored on
-        a local attribute.
+        Logs the request for the attribute, and returns the most recent value
+        set for the attribute.
 
-        Args:
-            attr: The name of the attribute to get
-            default: The default value for the attribute if it hasn't already been set.
-
-        Returns:
-            The value of the attribute, or ``default`` if the value has not been set.
+        :param attr: The name of the attribute to get
+        :param default: The default value for the attribute if it hasn't already
+            been set.
+        :returns: The value of the attribute, or ``default`` if the value has
+            not been set.
         """
         EventLog.log(EventLog.GET_VALUE, instance=self, attr=attr)
-        self._gets.add(attr)
-        return self._sets.get(attr, [default])[-1]
+        try:
+            return EventLog.value(instance=self.interface, attr=attr)
+        except AttributeError:
+            if default is NOT_PROVIDED:
+                raise
+            return default
 
     def _action(self, action, **data):
-        """Record that an action was performed on the object
+        """Record that an action was performed on the object.
 
-        Args:
-            action: The action that was performed
-            data: Any data associated with the action.
+        :param action: The action that was performed
+        :param data: Any data associated with the action.
         """
-        sequence = EventLog.log(EventLog.ACTION, instance=self, action=action, **data)
-        self._actions.setdefault(action, {})[sequence] = data
-
-
-_MODULES = {}
-
-
-def log_action(module, action, **data):
-    """Record that an action function was invoked
-
-    Args:
-        action: The action that was performed
-        data: Any data associated with the action.
-    """
-    _MODULES.setdefault(module, LoggedObject())._action(action, **data)
+        EventLog.log(EventLog.ACTION, instance=self, action=action, **data)
 
 
 class TestStyle(BaseStyle):
+    __test__ = False
+
     class IntrinsicSize(BaseIntrinsicSize):
         pass
 
     class Box(BaseBox):
         pass
 
     def layout(self, root, viewport):
         pass
 
 
-class TestCase(unittest.TestCase):
-    def setUp(self):
-        EventLog.reset()
+###########################################################################
+# Pytest widget assertion helpers
+###############################################################################
 
-    def assertFunctionNotPerformed(self, _module, action):
-        """Assert that the action function from module was *not* performed.
 
-        Args:
-            _module: The module with the action that should not have been performed.
-            action: The name of the action to check
+def attribute_value(_widget, _attr):
+    """Retrieve the current value of a widget property.
 
-        """
-        try:
-            self.assertNotIn(
-                action,
-                _MODULES[_module]._actions,
-                'Action {} unexpectedly performed by {}.'.format(action, _module)
-            )
-        except AttributeError:
-            self.fail('Module {} is not a logged object'.format(_module))
+    :param _widget: The interface of the widget to check
+    :param _attr: The attribute to retrieve.
+    :returns: The current value of the attribute
+    """
+    try:
+        return EventLog.value(_widget, _attr)
+    except AttributeError as e:
+        pytest.fail(str(e))
 
-    def assertFunctionPerformed(self, _module, action):
-        """Assert that the action function from module was performed.
 
-        Args:
-            _module: The module with the action that should have been performed.
-            action: The name of the action to check
+def attribute_values(_widget, _attr):
+    """Retrieve the list of values that the property has been set to.
+
+    :param _widget: The interface of the widget to check
+    :param _attr: The attribute to retrieve.
+    :returns: The list of values to which the attribute has been set.
+    """
+    try:
+        return EventLog.values(_widget, _attr)
+    except AttributeError as e:
+        pytest.fail(str(e))
 
-        """
-        try:
-            self.assertIn(
-                action,
-                _MODULES[_module]._actions,
-                'Action {} from {} not performed. Actions were: {}'.format(
-                    action,
-                    _module,
-                    sorted(_MODULES[_module]._actions.keys())
-                )
-            )
-        except AttributeError:
-            self.fail('Module {} is not a logged object'.format(_module))
 
-    def assertFunctionPerformedWith(self, _module, action, **test_data):
-        """Confirm that the action function form module was performed with specific test data
+def assert_attribute_retrieved(_widget, _attr):
+    """Assert that the widget implementation attempted to retrieve an attribute.
+
+    :param _widget: The interface of the widget to check
+    :param _attr: The attribute to check.
+    :returns: True if the attribute was retrieved
+    """
+    try:
+        EventLog.retrieved(_widget, _attr)
+    except AttributeError as e:
+        pytest.fail(str(e))
 
-        Args:
-            _module: The module with the action function that should have been performed.
-            action: The name of the action to check.
-            **test_data: The arguments that should have been passed to the action.
 
-        Returns:
-            If a matching action was performed, the full data of
-            the performed action if. False otherwise.
-        """
-        try:
+def assert_attribute_not_retrieved(_widget, _attr):
+    """Assert that the widget implementation did not attempt to retrieve an attribute.
+
+    :param _widget: The interface of the widget to check
+    :param _attr: The attribute to check.
+    :returns: True if the attribute was *not* retrieved
+    """
+    try:
+        EventLog.retrieved(_widget, _attr)
+        pytest.fail(f"Widget {_widget} unexpectedly retrieved the attribute {_attr!r}.")
+    except AttributeError:
+        pass
+
+
+def assert_attribute_not_set(_widget, _attr):
+    """Assert that the widget implementation did not attempt to set an attribute.
+
+    :param _widget: The interface of the widget to check
+    :param _attr: The attribute to check.
+    :returns: True if the attribute was not set
+    """
+    try:
+        EventLog.values(_widget, _attr)
+        pytest.fail(f"Widget {_widget} unexpectedly set the attribute {_attr!r}.")
+    except AttributeError:
+        pass
+
+
+def assert_action_not_performed(_widget, _action):
+    """Assert that the named action was *not* performed by a widget.
+
+    :param _widget: The interface of the widget to check
+    :param _action: The action to check.
+    :returns: True if the action was not performed
+    """
+    try:
+        EventLog.performed_actions(_widget, _action)
+        pytest.fail(f"Action {_action!r} unexpectedly performed by {_widget}.")
+    except AttributeError:
+        pass
+
+
+def assert_action_performed(_widget, _action):
+    """Assert that the named action was performed by a widget.
+
+    :param _widget: The interface of the widget to check
+    :param _action: The action to check.
+    :returns: True if the action was performed
+    """
+    try:
+        EventLog.performed_actions(_widget, _action)
+    except AttributeError as e:
+        pytest.fail(str(e))
+
+
+def assert_action_performed_with(_widget, _action, **test_data):
+    """Assert if an action was performed with specific test data.
+
+    :param _widget: The interface of the widget to check
+    :param _action: The action to check.
+    :param test_data: The arguments that should have been passed to the action.
+    :returns: True if the action was performed
+    """
+    try:
+        # Iterate over every action that was performed on
+        # this object.
+        actions_performed = EventLog.performed_actions(_widget, _action)
+        for data in actions_performed:
             found = True
-            # Iterate over every action that was performed on
-            # this object.
-            for sequence, data in _MODULES[_module]._actions[action].items():
-                # Iterate over every key and value in the test
-                # data. If the value in the recorded action
-                # doesn't match the requested value, then this isn't
-                # a match.
-                for key, value in test_data.items():
+            # Iterate over every key and value in the test
+            # data. If the value in the recorded action
+            # doesn't match the requested value, then this isn't
+            # a match.
+            for key, value in test_data.items():
+                try:
                     try:
+                        # Look for a `_raw` attribute, as that will be the
+                        # directly comparable object
+                        raw = data[key]._raw
+                        # If the _raw attribute is a mock, it doesn't actually exist
+                        if isinstance(data[key]._raw, Mock):
+                            raise AttributeError()
+
+                        if raw != value:
+                            found = False
+                    except AttributeError:
+                        # No raw attribute; use the provided value as-is
                         if data[key] != value:
                             found = False
-                    except KeyError:
-                        found = False
+                except KeyError:
+                    found = False
 
-                # Default behavior is to be found; so if we're
-                # still in a "found" state, this action is a match
-                # for the test data. Otherwise, reset, and try again
-                # with the next recorded action.
-                if found:
-                    return data
-                else:
-                    found = True
+            # Default behavior is to be found; so if we're
+            # still in a "found" state, this action is a match
+            # for the test data. Otherwise, reset, and try again
+            # with the next recorded action.
+            if found:
+                return
+
+        # None of the recorded actions match the test data.
+        pytest.fail(
+            f"Widget {_widget} did not perform action {_action!r} "
+            f"with data {test_data!r}; "
+            f"actions performed were {actions_performed!r}"
+        )
+    except AttributeError as e:
+        # None of the recorded actions match the test data.
+        pytest.fail(str(e))
 
-            # None of the recorded actions match the test data.
-            self.fail('Action {} not performed by {} with {}. Actions were: {}'.format(
-                    action,
-                    _module,
-                    test_data,
-                    sorted(_MODULES[_module]._actions[action].items())
-                ))
-        except KeyError:
-            # The action wasn't performed
-            self.fail('Action {} not performed by {}. Actions were: {}'.format(
-                    action,
-                    _module,
-                    sorted(_MODULES[_module]._actions.keys())
-                ))
-        except AttributeError:
-            self.fail('Widget {} is not a logged object'.format(_module))
 
-#####
+###########################################################################
+# Unittest widget assertions
+#
+# These have been (re)written in terms of Pytest assertions; this base
+# class is deprecated and should not be used for new tests.
+############################################################################
+class TestCase(unittest.TestCase):
+    def setUp(self):
+        EventLog.reset()
+
+        # We use the existence of a __main__ module as a proxy for being in test
+        # conditions. This isn't *great*, but the __main__ module isn't meaningful
+        # during tests, and removing it allows us to avoid having explicit "if
+        # under test conditions" checks in paths.py.
+        if "__main__" in sys.modules:
+            del sys.modules["__main__"]
 
-    def assertValueSet(self, _widget, attr, value):
-        """Assert that the widget implmentation has set an attribute to a value.
+    def reset_event_log(self):
+        EventLog.reset()
+
+    def pytest_assert(self, assertion, *args, **kwargs):
+        try:
+            return assertion(*args, **kwargs)
+        except AssertionError as e:
+            self.fail(str(e))
+
+    #####
+
+    def assertValueSet(self, _widget, _attr, value):
+        """Assert that the widget implementation has set an attribute to a
+        value.
 
         Args:
             _widget: The interface of the widget to check
-            attr: The attribute that should have been set
+            _attr: The attribute that should have been set
             value: The value that the attribute have been set to.
         """
-        try:
-            self.assertEqual(
-                _widget._impl._sets[attr][-1],
-                value,
-                'Widget {} has not had attribute {!r} set to {!r}; got {!r}.'.format(
-                    _widget,
-                    attr,
-                    value,
-                    _widget._impl._sets[attr][-1]
-                )
-            )
-        except KeyError:
-            self.fail('Widget {} did not have the attribute {!r} set; set attributes were {}.'.format(
-                _widget,
-                attr,
-                ', '.join('{!r}'.format(a) for a in sorted(_widget._impl._sets.keys()))
-            ))
-        except AttributeError:
-            self.fail('Widget {} is not a logged object'.format(_widget))
+        self.assertEqual(self.pytest_assert(attribute_value, _widget, _attr), value)
 
-    def assertValuesSet(self, _widget, attr, values):
-        """Assert that the widget implmentation has been set to multiple values.
+    def assertValuesSet(self, _widget, _attr, values):
+        """Assert that the widget implementation has been set to multiple
+        values.
 
         Args:
             _widget: The interface of the widget to check
-            attr: The attribute that should have been set
-            value: The values that the attribute have been set to.
+            _attr: The attribute that should have been set
+            values: The values that the attribute have been set to.
         """
-        try:
-            self.assertEqual(
-                _widget._impl._sets[attr],
-                values,
-                'Widget {} has not had attribute {!r} set to the values {}; got {}.'.format(
-                    _widget,
-                    attr,
-                    ', '.join('{!r}'.format(v) for v in values),
-                    ', '.join('{!r}'.format(v) for v in _widget._impl._sets[attr])
-                )
-            )
-        except KeyError:
-            self.fail('Widget {} did not have the attribute {!r} set; set attributes were {}.'.format(
-                _widget,
-                attr,
-                ','.join('{!r}'.format(a) for a in sorted(_widget._impl._sets.keys()))
-            ))
-        except AttributeError:
-            self.fail('Widget {} is not a logged object'.format(_widget))
+        self.assertEqual(self.pytest_assert(attribute_values, _widget, _attr), values)
 
-    def assertValueGet(self, _widget, attr):
-        """Assert that the widget implementation attempted to retrieve an attribute
+    def assertValueGet(self, _widget, _attr):
+        """Assert that the widget implementation attempted to retrieve an
+        attribute.
 
         Args:
             _widget: The interface of the widget to check
-            attr: The attribute that should have been retrieved
+            _attr: The attribute that should have been retrieved
         """
-        try:
-            self.assertIn(
-                attr,
-                _widget._impl._gets,
-                'Widget {} did not retrieve the attribute {!r}; retrieved attributes were {}.'.format(
-                    _widget,
-                    attr,
-                    ','.join('{!r}'.format(a) for a in sorted(_widget._impl._gets))
-            ))
-        except AttributeError:
-            self.fail('Widget {} is not a logged object'.format(_widget))
+        self.pytest_assert(assert_attribute_retrieved, _widget, _attr)
 
-    def assertActionNotPerformed(self, _widget, action):
+    def assertValueNotGet(self, _widget, _attr):
+        self.pytest_assert(assert_attribute_not_retrieved, _widget, _attr)
+
+    def assertValueNotSet(self, _widget, _attr):
+        self.pytest_assert(assert_attribute_not_set, _widget, _attr)
+
+    def assertActionNotPerformed(self, _widget, _action):
         """Assert that the named action was *not* performed by a widget.
 
         Args:
             _widget: The interface of the widget that should not have performed the action.
-            action: The name of the action to check
-
+            _action: The name of the action to check
         """
-        try:
-            self.assertNotIn(
-                action,
-                _widget._impl._actions,
-                'Action {} unexpectedly performed by {}.'.format(action, _widget)
-            )
-        except AttributeError:
-            self.fail('Widget {} is not a logged object'.format(_widget))
+        self.pytest_assert(assert_action_not_performed, _widget, _action)
 
-    def assertActionPerformed(self, _widget, action):
+    def assertActionPerformed(self, _widget, _action):
         """Assert that the named action performed by a widget.
-
         Args:
             _widget: The interface of the widget that should have performed the action.
-            action: The name of the action to check
-
+            _action: The name of the action to check
         """
-        try:
-            self.assertIn(
-                action,
-                _widget._impl._actions,
-                'Action {} not performed by {}. Actions were: {}'.format(
-                    action,
-                    _widget,
-                    sorted(_widget._impl._actions.keys())
-                )
-            )
-        except AttributeError:
-            self.fail('Widget {} is not a logged object'.format(_widget))
+        self.pytest_assert(assert_action_performed, _widget, _action)
 
-    def assertActionPerformedWith(self, _widget, action, **test_data):
-        """Was the action performed with specific test data
+    def assertActionPerformedWith(self, _widget, _action, **test_data):
+        """Was the action performed with specific test data.
 
         Args:
             _widget: The interface of the widget that should have performed the action.
-            action: The name of the action to check.
+            _action: The name of the action to check.
             **test_data: The arguments that should have been passed to the action.
 
         Returns:
             If a matching action was performed, the full data of
             the performed action if. False otherwise.
         """
-        try:
-            found = True
-            # Iterate over every action that was performed on
-            # this object.
-            for sequence, data in _widget._impl._actions[action].items():
-                # Iterate over every key and value in the test
-                # data. If the value in the recorded action
-                # doesn't match the requested value, then this isn't
-                # a match.
-                for key, value in test_data.items():
-                    try:
-                        if data[key] != value:
-                            found = False
-                    except KeyError:
-                        found = False
-
-                # Default behavior is to be found; so if we're
-                # still in a "found" state, this action is a match
-                # for the test data. Otherwise, reset, and try again
-                # with the next recorded action.
-                if found:
-                    return data
-                else:
-                    found = True
-
-            # None of the recorded actions match the test data.
-            self.fail('Action {} not performed by {} with {}. Actions were: {}'.format(
-                    action,
-                    _widget,
-                    test_data,
-                    sorted(_widget._impl._actions[action].items())
-                ))
-        except KeyError:
-            # The action wasn't performed
-            self.fail('Action {} not performed by {}. Actions were: {}'.format(
-                    action,
-                    _widget,
-                    sorted(_widget._impl._actions.keys())
-                ))
-        except AttributeError:
-            self.fail('Widget {} is not a logged object'.format(_widget))
+        self.pytest_assert(assert_action_performed_with, _widget, _action, **test_data)
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/app.py` & `toga-dummy-0.3.1/src/toga_dummy/widgets/multilinetextinput.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,27 @@
-from .utils import not_required_on, LoggedObject
-from .window import Window
+from .base import Widget
 
 
-class MainWindow(Window):
-    @not_required_on('mobile')
-    def on_close(self):
-        self.action('handle MainWindow on_close')
-
+class MultilineTextInput(Widget):
+    def create(self):
+        self._action("create MultilineTextInput")
 
-class App(LoggedObject):
-    def __init__(self, interface):
-        super().__init__()
-        self.interface = interface
+    def set_value(self, value):
+        self._set_value("value", value)
 
-    def create(self):
-        self._action('create')
+    def get_value(self):
+        return self._get_value("value")
 
-    def open_document(self, fileURL):
-        self._action('open document', fileURL=fileURL)
+    def set_placeholder(self, value):
+        self._set_value("placeholder", value)
 
-    @not_required_on('mobile')
-    def create_menus(self):
-        self._action('create menus')
+    def set_readonly(self, value):
+        self._set_value("readonly", value)
 
-    def main_loop(self):
-        self._action('main loop')
+    def set_on_change(self, handler):
+        self._set_value("on_change", handler)
 
-    def exit(self):
-        self._action('exit')
+    def scroll_to_bottom(self):
+        self._action("scroll to bottom")
 
-    def set_on_exit(self, value):
-        self._set_value('on_exit', value)
+    def scroll_to_top(self):
+        self._action("scroll to top")
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/widgets/tree.py` & `toga-dummy-0.3.1/src/toga_dummy/widgets/tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from .base import Widget
 
 
 class Tree(Widget):
     def create(self):
-        self._action('create Tree')
+        self._action("create Tree")
 
     def change_source(self, source):
-        self._action('change source', source=source)
+        self._action("change source", source=source)
 
     def insert(self, parent, index, item):
-        self._action('insert node', parent=parent, index=index, item=item)
+        self._action("insert node", parent=parent, index=index, item=item)
 
     def change(self, item):
-        self._action('change node', item=item)
+        self._action("change node", item=item)
 
-    def remove(self, item):
-        self._action('remove node', item=item)
+    def remove(self, parent, item, index):
+        self._action("remove node", parent=parent, index=index, item=item)
 
     def clear(self):
-        self._action('clear')
+        self._action("clear")
+
+    def get_selection(self):
+        self._action("get selection")
+        return None
 
     def set_on_select(self, handler):
-        self._set_value('on_select', handler)
+        self._set_value("on_select", handler)
+
+    def set_on_double_click(self, handler):
+        self._set_value("on_double_click", handler)
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/widgets/detailedlist.py` & `toga-dummy-0.3.1/src/toga_dummy/widgets/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from .base import Widget
 
 
-class DetailedList(Widget):
+class Table(Widget):
     def create(self):
-        self._action('create DetailedList')
+        self._action("create Table")
 
     def change_source(self, source):
-        self._action('change source', source=source)
+        self._action("change source", source=source)
 
-    def insert(self, item):
-        self._action('insert', item=item)
+    def insert(self, index, item):
+        self._action("insert row", index=index, item=item)
 
     def change(self, item):
-        self._action('change', item=item)
+        self._action("change row", item=item)
 
-    def remove(self, item):
-        self._action('remove', item=item)
+    def remove(self, index, item):
+        self._action("remove row", item=item, index=index)
 
     def clear(self):
-        self._action('clear')
+        self._action("clear")
 
-    def set_on_refresh(self, handler):
-        self._set_value('on_refresh', handler)
-
-    def after_on_refresh(self):
-        self._action('after on refresh')
-
-    def set_on_delete(self, handler):
-        self._set_value('on_delete', handler)
+    def get_selection(self):
+        self._action("get selection")
+        return None
 
     def set_on_select(self, handler):
-        self._set_value('on_select', handler)
+        self._set_value("on_select", handler)
+
+    def set_on_double_click(self, handler):
+        self._set_value("on_double_click", handler)
 
     def scroll_to_row(self, row):
-        self._set_value('scroll to', row)
+        self._set_value("scroll to", row)
+
+    def add_column(self, heading, accessor):
+        self._action("add column", heading=heading, accessor=accessor)
+
+    def remove_column(self, accessor):
+        self._action("remove column", accessor=accessor)
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/widgets/textinput.py` & `toga-dummy-0.3.1/src/toga_dummy/widgets/datepicker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 from .base import Widget
 
 
-class TextInput(Widget):
+class DatePicker(Widget):
     def create(self):
-        self._action('create TextInput')
-
-    def set_readonly(self, value):
-        self._set_value('readonly', value)
-
-    def set_placeholder(self, value):
-        self._set_value('placeholder', value)
+        self._action("create DatePicker")
 
     def get_value(self):
-        return self._get_value('value')
+        return self._get_value("value")
 
     def set_value(self, value):
-        self._set_value('value', value)
-
-    def set_font(self, value):
-        self._set_value('font', value)
+        return self._set_value("value", value)
 
-    def set_alignment(self, value):
-        self._set_value('alignment', value)
+    def set_min_date(self, value):
+        return self._set_value("min date", value)
 
-    def rehint(self):
-        self._action('rehint TextInput')
+    def set_max_date(self, value):
+        return self._set_value("max date", value)
 
     def set_on_change(self, handler):
-        self._set_value('on_change', handler)
+        self._set_value("on_change", handler)
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/widgets/numberinput.py` & `toga-dummy-0.3.1/src/toga_dummy/widgets/numberinput.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from .base import Widget
 
 
 class NumberInput(Widget):
     def create(self):
-        self._action('create NumberInput')
+        self._action("create NumberInput")
 
     def set_readonly(self, value):
-        self._set_value('readonly', value)
+        self._set_value("readonly", value)
 
     def set_step(self, step):
-        self._set_value('step', step)
+        self._set_value("step", step)
 
     def set_min_value(self, value):
-        self._set_value('min value', value)
+        self._set_value("min value", value)
 
     def set_max_value(self, value):
-        self._set_value('max value', value)
+        self._set_value("max value", value)
 
     def set_value(self, value):
-        self._set_value('value', value)
-
-    def set_font(self, value):
-        self._set_value('font', value)
+        self._set_value("value", value)
 
     def set_alignment(self, value):
-        self._set_value('alignment', value)
+        self._set_value("alignment", value)
 
     def set_on_change(self, handler):
-        self._set_value('on_change', handler)
+        self._set_value("on_change", handler)
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/widgets/selection.py` & `toga-dummy-0.3.1/src/toga_dummy/widgets/selection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from .base import Widget
 
 
 class Selection(Widget):
     def create(self):
-        self._action('create Selection')
+        self._action("create Selection")
+        self._items = []
 
     def remove_all_items(self):
-        self._action('remove all items')
+        self._action("remove all items")
+        self._items = []
 
     def add_item(self, item):
-        self._action('add item', item=item)
+        self._action("add item", item=item)
+        self._items.append(item)
 
     def select_item(self, item):
-        self._action('select item', item=item)
+        self._action("select item", item=item)
+        self._set_value("selected_item", item)
 
     def get_selected_item(self):
-        return self._get_value('selected_item')
+        try:
+            return self._get_value("selected_item")
+        except AttributeError:
+            return self._items[0]
 
     def set_on_select(self, handler):
-        self._set_value('on_select', handler)
-
-    def rehint(self):
-        self._action('rehint Selection')
+        self._set_value("on_select", handler)
```

### Comparing `toga-dummy-0.3.0.dev9/toga_dummy/widgets/webview.py` & `toga-dummy-0.3.1/src/toga_dummy/widgets/slider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import toga
+
+from ..utils import not_required
 from .base import Widget
 
 
-class WebView(Widget):
+@not_required  # Testbed coverage is complete for this widget.
+class Slider(Widget, toga.widgets.slider.SliderImpl):
     def create(self):
-        self._action('create WebView')
+        self._action("create Slider")
+
+    def get_value(self):
+        return self._get_value("value", 0)
 
-    def get_dom(self):
-        self._action('get DOM')
-        return 'DUMMY DOM'
+    def set_value(self, value):
+        self._set_value("value", value)
 
-    def set_content(self, root_url, content):
-        self._action('set content', root_url=root_url, content=content)
+    def get_range(self):
+        return self._get_value("range")
 
-    def set_user_agent(self, value):
-        self._set_value('user_agent', value)
+    def set_range(self, range):
+        self._set_value("range", range)
 
-    def set_url(self, value):
-        self._set_value('url', value)
+    def get_tick_count(self):
+        return self._get_value("tick_count", None)
 
-    def evaluate(self, javascript):
-        self._action('evaluate', javascript=javascript)
+    def set_tick_count(self, tick_count):
+        self._set_value("tick_count", tick_count)
```

### Comparing `toga-dummy-0.3.0.dev9/README.rst` & `toga-dummy-0.3.1/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -6,31 +6,38 @@
 
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

