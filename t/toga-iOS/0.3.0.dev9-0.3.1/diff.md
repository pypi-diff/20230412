# Comparing `tmp/toga-iOS-0.3.0.dev9.tar.gz` & `tmp/toga-iOS-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-iOS-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:19 2018, max compression
+gzip compressed data, was "toga-iOS-0.3.1.tar", last modified: Wed Apr 12 01:58:44 2023, max compression
```

## Comparing `toga-iOS-0.3.0.dev9.tar` & `toga-iOS-0.3.1.tar`

### file list

```diff
@@ -1,52 +1,75 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     2279 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     2279 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)     1125 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)       42 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)       15 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS.egg-info/dependency_links.txt
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/tests/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/tests/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      273 2017-12-22 11:14:30.000000 toga-iOS-0.3.0.dev9/tests/test_implementation.py
--rw-r--r--   0 rkm        (501) staff       (20)      111 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/MANIFEST.in
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS/hardware/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2018-05-26 09:29:22.000000 toga-iOS-0.3.0.dev9/toga_iOS/hardware/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      272 2017-12-23 03:47:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/color.py
--rw-r--r--   0 rkm        (501) staff       (20)     2900 2018-06-10 23:51:35.000000 toga-iOS-0.3.0.dev9/toga_iOS/window.py
--rw-r--r--   0 rkm        (501) staff       (20)      351 2018-05-17 17:50:36.000000 toga-iOS-0.3.0.dev9/toga_iOS/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1847 2017-12-23 03:47:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/font.py
--rw-r--r--   0 rkm        (501) staff       (20)     1531 2018-05-26 09:29:22.000000 toga-iOS-0.3.0.dev9/toga_iOS/factory.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS/libs/
--rw-r--r--   0 rkm        (501) staff       (20)      822 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/toga_iOS/libs/core_graphics.py
--rw-r--r--   0 rkm        (501) staff       (20)       76 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/toga_iOS/libs/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1458 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/toga_iOS/libs/foundation.py
--rw-r--r--   0 rkm        (501) staff       (20)    12252 2018-07-07 05:52:00.000000 toga-iOS-0.3.0.dev9/toga_iOS/libs/uikit.py
--rw-r--r--   0 rkm        (501) staff       (20)     3905 2018-07-07 05:52:00.000000 toga-iOS-0.3.0.dev9/toga_iOS/app.py
--rw-r--r--   0 rkm        (501) staff       (20)     2964 2017-12-23 03:47:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/constraints.py
--rw-r--r--   0 rkm        (501) staff       (20)     1748 2017-12-22 11:14:30.000000 toga-iOS-0.3.0.dev9/toga_iOS/dialogs.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)      232 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/icon.py
--rw-r--r--   0 rkm        (501) staff       (20)      790 2018-05-17 17:50:27.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)      791 2017-12-23 03:47:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/box.py
--rw-r--r--   0 rkm        (501) staff       (20)     4535 2018-02-21 05:36:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/detailedlist.py
--rw-r--r--   0 rkm        (501) staff       (20)     4359 2018-07-07 05:52:00.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/multilinetextinput.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1740 2018-07-07 05:52:00.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     2329 2018-05-26 09:29:22.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/switch.py
--rw-r--r--   0 rkm        (501) staff       (20)     4305 2018-05-26 09:29:22.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/scrollcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     1298 2018-05-26 09:29:22.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/slider.py
--rw-r--r--   0 rkm        (501) staff       (20)     1357 2018-05-17 17:50:23.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/button.py
--rw-r--r--   0 rkm        (501) staff       (20)     1002 2018-05-26 09:29:22.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/progressbar.py
--rw-r--r--   0 rkm        (501) staff       (20)     1841 2018-02-21 05:36:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/navigationview.py
--rw-r--r--   0 rkm        (501) staff       (20)     1293 2018-02-21 05:36:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/label.py
--rw-r--r--   0 rkm        (501) staff       (20)     3164 2018-07-07 05:52:00.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/numberinput.py
--rw-r--r--   0 rkm        (501) staff       (20)      159 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     2254 2018-03-19 02:54:39.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/selection.py
--rw-r--r--   0 rkm        (501) staff       (20)     1684 2018-02-21 05:36:56.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/webview.py
--rw-r--r--   0 rkm        (501) staff       (20)      794 2018-06-10 23:51:35.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/image.py
--rw-r--r--   0 rkm        (501) staff       (20)     2128 2018-05-26 09:29:22.000000 toga-iOS-0.3.0.dev9/toga_iOS/widgets/base.py
--rw-r--r--   0 rkm        (501) staff       (20)     1673 2018-07-07 05:52:00.000000 toga-iOS-0.3.0.dev9/setup.py
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:19.000000 toga-iOS-0.3.0.dev9/setup.cfg
--rw-r--r--   0 rkm        (501) staff       (20)     1085 2017-12-22 11:14:05.000000 toga-iOS-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.785338 toga-iOS-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-12 01:58:44.785338 toga-iOS-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-12 01:58:44.785338 toga-iOS-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.757338 toga-iOS-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.765338 toga-iOS-0.3.1/src/toga_iOS/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.769338 toga-iOS-0.3.1/src/toga_iOS/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.773338 toga-iOS-0.3.1/src/toga_iOS/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/libs/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/libs/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/libs/uikit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/libs/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.781338 toga-iOS-0.3.1/src/toga_iOS/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/src/toga_iOS/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.769338 toga-iOS-0.3.1/src/toga_iOS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-12 01:58:44.000000 toga-iOS-0.3.1/src/toga_iOS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-12 01:58:44.000000 toga-iOS-0.3.1/src/toga_iOS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:44.000000 toga-iOS-0.3.1/src/toga_iOS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 01:58:44.000000 toga-iOS-0.3.1/src/toga_iOS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:29.000000 toga-iOS-0.3.1/src/toga_iOS.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 01:58:44.000000 toga-iOS-0.3.1/src/toga_iOS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 01:58:44.000000 toga-iOS-0.3.1/src/toga_iOS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.781338 toga-iOS-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.781338 toga-iOS-0.3.1/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:44.785338 toga-iOS-0.3.1/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 01:58:03.000000 toga-iOS-0.3.1/tests_backend/widgets/textinput.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/libs/foundation.py` & `toga-iOS-0.3.1/src/toga_iOS/libs/foundation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 ##########################################################################
 # System/Library/Frameworks/Foundation.framework
 ##########################################################################
-from ctypes import *
-from ctypes import util
+from ctypes import c_bool, cdll, util
 
-from rubicon.objc import *
+from rubicon.objc import NSPoint, NSRect, ObjCClass
 
 ######################################################################
-foundation = cdll.LoadLibrary(util.find_library('Foundation'))
+foundation = cdll.LoadLibrary(util.find_library("Foundation"))
 ######################################################################
 
 foundation.NSMouseInRect.restype = c_bool
 foundation.NSMouseInRect.argtypes = [NSPoint, NSRect, c_bool]
 
+
 ######################################################################
 # NSArray.h
-NSMutableArray = ObjCClass('NSMutableArray')
+NSMutableArray = ObjCClass("NSMutableArray")
+
 
 ######################################################################
 # NSBundle.h
-NSBundle = ObjCClass('NSBundle')
+NSBundle = ObjCClass("NSBundle")
+
 
 ######################################################################
 # NSData.h
-NSData = ObjCClass('NSData')
+NSData = ObjCClass("NSData")
+
+
+######################################################################
+# NSDate.h
+NSDate = ObjCClass("NSDate")
+
 
 ######################################################################
 # NSIndexPath.h
-NSIndexPath = ObjCClass('NSIndexPath')
+NSIndexPath = ObjCClass("NSIndexPath")
+
 
 ######################################################################
-# NSNSNotification.h
-NSNotificationCenter = ObjCClass('NSNotificationCenter')
+# NSNotification.h
+NSNotificationCenter = ObjCClass("NSNotificationCenter")
+
+
+######################################################################
+# NSRunLoop.h
+NSRunLoop = ObjCClass("NSRunLoop")
+
+NSRunLoop.declare_class_property("currentRunLoop")
+
 
 ######################################################################
 # NSURL.h
-NSURL = ObjCClass('NSURL')
+NSURL = ObjCClass("NSURL")
+
 
 ######################################################################
 # NSURLRequest.h
-NSURLRequest = ObjCClass('NSURLRequest')
+NSURLRequest = ObjCClass("NSURLRequest")
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/libs/uikit.py` & `toga-iOS-0.3.1/src/toga_iOS/libs/uikit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 ##########################################################################
 # System/Library/Frameworks/UIKit.framework
 ##########################################################################
-from ctypes import *
-from ctypes import util
+from ctypes import POINTER, Structure, c_char_p, c_int, c_void_p, cdll, util
 from enum import Enum
 
-from rubicon.objc import *
-from toga.constants import *
+from rubicon.objc import CGFloat, ObjCClass, objc_const
+
+from toga.constants import CENTER, JUSTIFY, LEFT, RIGHT
+from toga_iOS.libs.core_graphics import CGContextRef
 
 ######################################################################
-uikit = cdll.LoadLibrary(util.find_library('UIKit'))
+uikit = cdll.LoadLibrary(util.find_library("UIKit"))
 ######################################################################
 
 uikit.UIApplicationMain.restype = c_int
 uikit.UIApplicationMain.argtypes = [c_int, POINTER(c_char_p), c_void_p, c_void_p]
 
 ######################################################################
+# NSAttributedString.h
+NSAttributedString = ObjCClass("NSAttributedString")
+
+NSFontAttributeName = objc_const(uikit, "NSFontAttributeName")
+NSForegroundColorAttributeName = objc_const(uikit, "NSForegroundColorAttributeName")
+NSStrokeColorAttributeName = objc_const(uikit, "NSStrokeColorAttributeName")
+NSStrokeWidthAttributeName = objc_const(uikit, "NSStrokeWidthAttributeName")
+
+######################################################################
 # NSLayoutConstraint.h
-NSLayoutConstraint = ObjCClass('NSLayoutConstraint')
+NSLayoutConstraint = ObjCClass("NSLayoutConstraint")
 
 NSLayoutRelationLessThanOrEqual = -1
 NSLayoutRelationEqual = 0
 NSLayoutRelationGreaterThanOrEqual = 1
 
 NSLayoutAttributeLeft = 1
 NSLayoutAttributeRight = 2
@@ -33,56 +43,59 @@
 NSLayoutAttributeHeight = 8
 NSLayoutAttributeCenterX = 9
 NSLayoutAttributeCenterY = 10
 NSLayoutAttributeBaseline = 11
 
 NSLayoutAttributeNotAnAttribute = 0
 
-NSLayoutFormatAlignAllLeft = (1 << NSLayoutAttributeLeft)
-NSLayoutFormatAlignAllRight = (1 << NSLayoutAttributeRight)
-NSLayoutFormatAlignAllTop = (1 << NSLayoutAttributeTop)
-NSLayoutFormatAlignAllBottom = (1 << NSLayoutAttributeBottom)
-NSLayoutFormatAlignAllLeading = (1 << NSLayoutAttributeLeading)
-NSLayoutFormatAlignAllTrailing = (1 << NSLayoutAttributeTrailing)
-NSLayoutFormatAlignAllCenterX = (1 << NSLayoutAttributeCenterX)
-NSLayoutFormatAlignAllCenterY = (1 << NSLayoutAttributeCenterY)
-NSLayoutFormatAlignAllBaseline = (1 << NSLayoutAttributeBaseline)
+NSLayoutFormatAlignAllLeft = 1 << NSLayoutAttributeLeft
+NSLayoutFormatAlignAllRight = 1 << NSLayoutAttributeRight
+NSLayoutFormatAlignAllTop = 1 << NSLayoutAttributeTop
+NSLayoutFormatAlignAllBottom = 1 << NSLayoutAttributeBottom
+NSLayoutFormatAlignAllLeading = 1 << NSLayoutAttributeLeading
+NSLayoutFormatAlignAllTrailing = 1 << NSLayoutAttributeTrailing
+NSLayoutFormatAlignAllCenterX = 1 << NSLayoutAttributeCenterX
+NSLayoutFormatAlignAllCenterY = 1 << NSLayoutAttributeCenterY
+NSLayoutFormatAlignAllBaseline = 1 << NSLayoutAttributeBaseline
 
 NSLayoutFormatAlignmentMask = 0xFFFF
 
 NSLayoutFormatDirectionLeadingToTrailing = 0 << 16
 NSLayoutFormatDirectionLeftToRight = 1 << 16
 NSLayoutFormatDirectionRightToLeft = 2 << 16
 
 NSLayoutFormatDirectionMask = 0x3 << 16
 
-NSLayoutConstraintOrientationHorizontal = 0,
+NSLayoutConstraintOrientationHorizontal = (0,)
 NSLayoutConstraintOrientationVertical = 1
 
-class NSEdgetInsets(Structure):
+
+class NSEdgeInsets(Structure):
     _fields_ = [
         ("top", CGFloat),
         ("left", CGFloat),
         ("bottom", CGFloat),
         ("right", CGFloat),
     ]
 
+
 def NSEdgeInsetsMake(top, left, bottom, right):
     return NSEdgeInsets(top, left, bottom, right)
 
 
 class NSLayoutPriority(Enum):
     Required = 1000
     DefaultHigh = 750
     DragThatCanResizeWindow = 510
     WindowSizeStayPut = 500
     DragThatCannotResizeWindow = 490
     DefaultLow = 250
     FittingSizeCompression = 50
 
+
 ######################################################################
 # NSParagraphStyle.h
 NSLineBreakByWordWrapping = 0
 NSLineBreakByCharWrapping = 1
 NSLineBreakByClipping = 2
 NSLineBreakByTruncatingHead = 3
 NSLineBreakByTruncatingTail = 4
@@ -92,90 +105,116 @@
 # NSText.h (The order is different on macOS and iOS)
 NSLeftTextAlignment = 0
 NSCenterTextAlignment = 1
 NSRightTextAlignment = 2
 NSJustifiedTextAlignment = 3
 NSNaturalTextAlignment = 4
 
+
 def NSTextAlignment(alignment):
     return {
         LEFT: NSLeftTextAlignment,
         RIGHT: NSRightTextAlignment,
         CENTER: NSCenterTextAlignment,
         JUSTIFY: NSJustifiedTextAlignment,
     }[alignment]
 
+
+######################################################################
+# UIAlertController.h
+UIAlertController = ObjCClass("UIAlertController")
+UIAlertAction = ObjCClass("UIAlertAction")
+
+
+class UIAlertControllerStyle(Enum):
+    ActionSheet = 0
+    Alert = 1
+
+
+class UIAlertActionStyle(Enum):
+    Default = 0
+    Cancel = 1
+    Destructive = 2
+
+
 ######################################################################
 # UIApplication.h
-UIApplication = ObjCClass('UIApplication')
+UIApplication = ObjCClass("UIApplication")
+
 
 class UIInterfaceOrientation(Enum):
     Unknown = 0
     Portrait = 1
     PortraitUpsideDown = 2
     LandscapeLeft = 3
     LandscapeRight = 4
 
+
 ######################################################################
 # UIBarButtonItem.h
-UIBarButtonItem = ObjCClass('UIBarButtonItem')
+UIBarButtonItem = ObjCClass("UIBarButtonItem")
+
+
+class UIBarButtonSystemItem(Enum):
+    Done = 0
+    Cancel = 1
+    Edit = 2
+    Save = 3
+    Add = 4
+    FlexibleSpace = 5
+    FixedSpace = 6
+    Compose = 7
+    Reply = 8
+    Action = 9
+    Organize = 10
+    Bookmarks = 11
+    Search = 12
+    Refresh = 13
+    Stop = 14
+    Camera = 15
+    Trash = 16
+    Play = 17
+    Pause = 18
+    Rewind = 19
+    FastForward = 20
+    Undo = 21
+    Redo = 22
+    PageCurl = 23
 
-UIBarButtonSystemItemDone = 0
-UIBarButtonSystemItemCancel = 1
-UIBarButtonSystemItemEdit = 2
-UIBarButtonSystemItemSave = 3
-UIBarButtonSystemItemAdd = 4
-UIBarButtonSystemItemFlexibleSpace = 5
-UIBarButtonSystemItemFixedSpace = 6
-UIBarButtonSystemItemCompose = 7
-UIBarButtonSystemItemReply = 8
-UIBarButtonSystemItemAction = 9
-UIBarButtonSystemItemOrganize = 10
-UIBarButtonSystemItemBookmarks = 11
-UIBarButtonSystemItemSearch = 12
-UIBarButtonSystemItemRefresh = 13
-UIBarButtonSystemItemStop = 14
-UIBarButtonSystemItemCamera = 15
-UIBarButtonSystemItemTrash = 16
-UIBarButtonSystemItemPlay = 17
-UIBarButtonSystemItemPause = 18
-UIBarButtonSystemItemRewind = 19
-UIBarButtonSystemItemFastForward = 20
-UIBarButtonSystemItemUndo = 21
-UIBarButtonSystemItemRedo = 22
-UIBarButtonSystemItemPageCurl = 23
 
 ######################################################################
 # UIButton.h
-UIButton = ObjCClass('UIButton')
+UIButton = ObjCClass("UIButton")
+
+
 ######################################################################
 # UIColor.h
-UIColor = ObjCClass('UIColor')
+UIColor = ObjCClass("UIColor")
 
 # System colors
-UIColor.declare_class_property('darkTextColor')
-UIColor.declare_class_property('lightTextColor')
-UIColor.declare_class_property('groupTableViewBackgroundColor')
+UIColor.declare_class_property("darkTextColor")
+UIColor.declare_class_property("lightTextColor")
+UIColor.declare_class_property("groupTableViewBackgroundColor")
 
 # Predefined colors
-UIColor.declare_class_property('blackColor')
-UIColor.declare_class_property('blueColor')
-UIColor.declare_class_property('brownColor')
-UIColor.declare_class_property('clearColor')
-UIColor.declare_class_property('cyanColor')
-UIColor.declare_class_property('darkGrayColor')
-UIColor.declare_class_property('grayColor')
-UIColor.declare_class_property('greenColor')
-UIColor.declare_class_property('lightGrayColor')
-UIColor.declare_class_property('magentaColor')
-UIColor.declare_class_property('orangeColor')
-UIColor.declare_class_property('purpleColor')
-UIColor.declare_class_property('redColor')
-UIColor.declare_class_property('whiteColor')
-UIColor.declare_class_property('yellowColor')
+UIColor.declare_class_property("blackColor")
+UIColor.declare_class_property("blueColor")
+UIColor.declare_class_property("brownColor")
+UIColor.declare_class_property("clearColor")
+UIColor.declare_class_property("cyanColor")
+UIColor.declare_class_property("darkGrayColor")
+UIColor.declare_class_property("grayColor")
+UIColor.declare_class_property("greenColor")
+UIColor.declare_class_property("lightGrayColor")
+UIColor.declare_class_property("magentaColor")
+UIColor.declare_class_property("orangeColor")
+UIColor.declare_class_property("purpleColor")
+UIColor.declare_class_property("redColor")
+UIColor.declare_class_property("whiteColor")
+UIColor.declare_class_property("yellowColor")
 
 ######################################################################
 # UIControl.h
 
 # UIControlEvents
 UIControlEventTouchDown = 1 << 0
 UIControlEventTouchDownRepeat = 1 << 1
@@ -218,77 +257,97 @@
 UIControlStateDisabled = 1 << 1
 UIControlStateSelected = 1 << 2
 UIControlStateApplication = 0x00FF0000
 UIControlStateReserved = 0xFF000000
 
 ######################################################################
 # UIFont.h
-UIFont = ObjCClass('UIFont')
+UIFont = ObjCClass("UIFont")
+UIFontDescriptorTraitItalic = 1 << 0
+UIFontDescriptorTraitBold = 1 << 1
+
+######################################################################
+# UIGraphics.h
+uikit.UIGraphicsGetCurrentContext.restype = CGContextRef
 
 ######################################################################
 # UIImage.h
-UIImage = ObjCClass('UIImage')
+UIImage = ObjCClass("UIImage")
 
 ######################################################################
 # UIImageView.h
-UIImageView = ObjCClass('UIImageView')
+UIImageView = ObjCClass("UIImageView")
 
 ######################################################################
 # UILabel.h
-UILabel = ObjCClass('UILabel')
+UILabel = ObjCClass("UILabel")
 
 ######################################################################
 # UINavigationController.h
-UINavigationController = ObjCClass('UINavigationController')
+UINavigationController = ObjCClass("UINavigationController")
 
 ######################################################################
 # UIPickerView.h
-UIPickerView = ObjCClass('UIPickerView')
+UIPickerView = ObjCClass("UIPickerView")
 
 ######################################################################
 # UIProgressView.h
-UIProgressView = ObjCClass('UIProgressView')
+UIProgressView = ObjCClass("UIProgressView")
+
 
 class UIProgressViewStyle(Enum):
     Default = 0
     Bar = 1
 
+
 ######################################################################
 # UIRefreshControl.h
-UIRefreshControl = ObjCClass('UIRefreshControl')
+UIRefreshControl = ObjCClass("UIRefreshControl")
 
 ######################################################################
 # UIResponder.h
-UIResponder = ObjCClass('UIResponder')
+UIResponder = ObjCClass("UIResponder")
 
 ######################################################################
 # UIScreen.h
-UIScreen = ObjCClass('UIScreen')
-UIScreen.declare_class_property('mainScreen')
+UIScreen = ObjCClass("UIScreen")
+UIScreen.declare_class_property("mainScreen")
 
 #####################################################################
 # UIScrollView.h
-UIScrollView = ObjCClass('UIScrollView')
+UIScrollView = ObjCClass("UIScrollView")
 
 ######################################################################
 # UISlider.h
-UISlider = ObjCClass('UISlider')
+UISlider = ObjCClass("UISlider")
 
 ######################################################################
 # UIStackView.h
-UIStackView = ObjCClass('UIStackView')
+UIStackView = ObjCClass("UIStackView")
+
+
+class UIStackViewAlignment(Enum):
+    Fill = 0
+    Leading = 1
+    Top = 1
+    FirstBaseline = 2
+    Center = 3
+    Trailing = 4
+    Bottom = 4
+    LastBaseline = 5
+
 
 ######################################################################
 # UISwitch.h
-UISwitch = ObjCClass('UISwitch')
+UISwitch = ObjCClass("UISwitch")
 
 ######################################################################
 # UITableView.h
-UITableView = ObjCClass('UITableView')
-UITableViewController = ObjCClass('UITableViewController')
+UITableView = ObjCClass("UITableView")
+UITableViewController = ObjCClass("UITableViewController")
 
 UITableViewScrollPositionNone = 0
 UITableViewScrollPositionTop = 1
 UITableViewScrollPositionMiddle = 2
 UITableViewScrollPositionBottom = 3
 
 UITableViewRowAnimationFade = 0
@@ -298,15 +357,15 @@
 UITableViewRowAnimationBottom = 4
 UITableViewRowAnimationNone = 5
 UITableViewRowAnimationMiddle = 6
 UITableViewRowAnimationAutomatic = 100
 
 ######################################################################
 # UITableViewCell.h
-UITableViewCell = ObjCClass('UITableViewCell')
+UITableViewCell = ObjCClass("UITableViewCell")
 
 UITableViewCellStyleDefault = 0
 UITableViewCellStyleValue1 = 1
 UITableViewCellStyleValue2 = 2
 UITableViewCellStyleSubtitle = 3
 
 UITableViewCellEditingStyleNone = 0
@@ -314,51 +373,57 @@
 UITableViewCellEditingStyleInsert = 2
 
 UITableViewCellSeparatorStyleNone = 0
 UITableViewCellSeparatorStyleSingleLine = 1
 
 ######################################################################
 # UITextField.h
-UITextField = ObjCClass('UITextField')
+UITextField = ObjCClass("UITextField")
+
 
 class UITextBorderStyle(Enum):
     NoBorder = 0
     Line = 1
     Bezel = 2
     RoundedRect = 3
 
+
 ######################################################################
 # UITextInputTraits.h
 
+
 class UIKeyboardType(Enum):
     Default = 0
     ASCIICapable = 1
     NumbersAndPunctuation = 2
     URL = 3
     NumberPad = 4
     PhonePad = 5
     NamePhonePad = 6
     EmailAddress = 7
     DecimalPad = 8
     Twitter = 9
     WebSearch = 10
     ASCIICapableNumberPad = 11
 
+
 ######################################################################
 # UITextView.h
-UITextView = ObjCClass('UITextView')
+UITextView = ObjCClass("UITextView")
 
 ######################################################################
 # UIView.h
-UIView = ObjCClass('UIView')
+UIView = ObjCClass("UIView")
+
 
 class UILayoutConstraintAxis(Enum):
     Horizontal = 0
     Vertical = 1
 
+
 class UIViewContentMode(Enum):
     ScaleToFill = 0
     ScaleAspectFit = 1
     ScaleAspectFill = 2
     Redraw = 3
     Center = 4
     Top = 5
@@ -366,28 +431,29 @@
     Left = 7
     Right = 8
     TopLeft = 9
     TopRight = 10
     BottomLeft = 11
     BottomRight = 12
 
-######################################################################
-# UIViewController.h
-UIViewController = ObjCClass('UIViewController')
 
 ######################################################################
-# UIWebView.h
-UIWebView = ObjCClass('UIWebView')
+# UIViewController.h
+UIViewController = ObjCClass("UIViewController")
 
 ######################################################################
 # UIWindow.h
-UIWindow = ObjCClass('UIWindow')
-
-UIKeyboardWillShowNotification = objc_const(uikit, 'UIKeyboardWillShowNotification')
-UIKeyboardDidShowNotification = objc_const(uikit, 'UIKeyboardDidShowNotification')
-UIKeyboardWillHideNotification = objc_const(uikit, 'UIKeyboardWillHideNotification')
-UIKeyboardDidHideNotification = objc_const(uikit, 'UIKeyboardDidHideNotification')
-
-UIKeyboardFrameEndUserInfoKey = objc_const(uikit, 'UIKeyboardFrameEndUserInfoKey')
+UIWindow = ObjCClass("UIWindow")
 
-UIKeyboardWillChangeFrameNotification = objc_const(uikit, 'UIKeyboardWillChangeFrameNotification')
-UIKeyboardDidChangeFrameNotification = objc_const(uikit, 'UIKeyboardDidChangeFrameNotification')
+UIKeyboardWillShowNotification = objc_const(uikit, "UIKeyboardWillShowNotification")
+UIKeyboardDidShowNotification = objc_const(uikit, "UIKeyboardDidShowNotification")
+UIKeyboardWillHideNotification = objc_const(uikit, "UIKeyboardWillHideNotification")
+UIKeyboardDidHideNotification = objc_const(uikit, "UIKeyboardDidHideNotification")
+
+UIKeyboardFrameEndUserInfoKey = objc_const(uikit, "UIKeyboardFrameEndUserInfoKey")
+
+UIKeyboardWillChangeFrameNotification = objc_const(
+    uikit, "UIKeyboardWillChangeFrameNotification"
+)
+UIKeyboardDidChangeFrameNotification = objc_const(
+    uikit, "UIKeyboardDidChangeFrameNotification"
+)
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/app.py` & `toga-iOS-0.3.1/src/toga_iOS/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 import asyncio
 
-from rubicon.objc import objc_method
+from rubicon.objc import SEL, objc_method
 from rubicon.objc.eventloop import EventLoopPolicy, iOSLifecycle
 
-from .libs import (NSNotificationCenter,
-    SEL,
+from toga_iOS.libs import (
+    NSNotificationCenter,
     UIKeyboardFrameEndUserInfoKey,
     UIKeyboardWillHideNotification,
     UIKeyboardWillShowNotification,
-    UIResponder
+    UIResponder,
 )
-
-from .window import Window
+from toga_iOS.window import Window
 
 
 class MainWindow(Window):
-    def __init__(self, interface):
-        super().__init__(interface)
-
-    # def startup(self):
-    #     super().startup()
-    #     self.native.setBackgroundColor_(UIColor.whiteColor())
+    pass
 
 
 class PythonAppDelegate(UIResponder):
     @objc_method
     def applicationDidBecomeActive_(self, application) -> None:
         print("App became active.")
 
@@ -37,53 +31,60 @@
         print("App entered background.")
 
     @objc_method
     def applicationWillEnterForeground_(self, application) -> None:
         print("App about to enter foreground.")
 
     @objc_method
-    def application_didFinishLaunchingWithOptions_(self, application, launchOptions) -> bool:
+    def application_didFinishLaunchingWithOptions_(
+        self, application, launchOptions
+    ) -> bool:
         print("App finished launching.")
         App.app.create()
 
         NSNotificationCenter.defaultCenter.addObserver(
             self,
-            selector=SEL('keyboardWillShow:'),
+            selector=SEL("keyboardWillShow:"),
             name=UIKeyboardWillShowNotification,
-            object=None
+            object=None,
         )
         NSNotificationCenter.defaultCenter.addObserver(
             self,
-            selector=SEL('keyboardWillHide:'),
+            selector=SEL("keyboardWillHide:"),
             name=UIKeyboardWillHideNotification,
-            object=None
+            object=None,
         )
         # Set the initial keyboard size.
         App.app.interface.main_window.content._impl.viewport.kb_height = 0.0
 
         return True
 
     @objc_method
     def applicationWillTerminate_(self, application) -> None:
         print("App about to Terminate.")
 
     @objc_method
-    def application_didChangeStatusBarOrientation_(self, application, oldStatusBarOrientation: int) -> None:
-        """ This callback is invoked when rotating the device from landscape to portrait and vice versa. """
+    def application_didChangeStatusBarOrientation_(
+        self, application, oldStatusBarOrientation: int
+    ) -> None:
+        """This callback is invoked when rotating the device from landscape to
+        portrait and vice versa."""
         App.app.interface.main_window.content.refresh()
 
     @objc_method
     def keyboardWillShow_(self, notification) -> None:
         # Keyboard is about to be displayed.
         # This will fire multiple times - once to display the keyboard,
         # and again to display the autocomplete bar.
         kb_height = App.app.interface.main_window._impl.controller.view.convertRect(
-                notification.userInfo.objectForKey(UIKeyboardFrameEndUserInfoKey).CGRectValue,
-                fromView=None
-            ).size.height
+            notification.userInfo.objectForKey(
+                UIKeyboardFrameEndUserInfoKey
+            ).CGRectValue,
+            fromView=None,
+        ).size.height
         App.app.interface.main_window.content._impl.viewport.kb_height = kb_height
 
         App.app.interface.main_window.content.refresh()
 
     @objc_method
     def keyboardWillHide_(self, notification) -> None:
         # Reset the layout to the size of the screen.
@@ -94,28 +95,32 @@
 class App:
     def __init__(self, interface):
         self.interface = interface
         self.interface._impl = self
         App.app = self  # Add a reference for the PythonAppDelegate class to use.
 
         asyncio.set_event_loop_policy(EventLoopPolicy())
-        self.loop = asyncio.get_event_loop()
+        self.loop = asyncio.new_event_loop()
 
     def create(self):
-        """ Calls the startup method on the interface """
+        """Calls the startup method on the interface."""
         self.interface.startup()
 
     def open_document(self, fileURL):
-        """ Add a new document to this app."""
+        """Add a new document to this app."""
         pass
 
     def main_loop(self):
-        # Main loop is a no-op on iOS; the app loop is integrated with the
-        # main iOS event loop.
-
-        self.loop.run_forever(lifecycle=iOSLifecycle())
+        # Main loop is non-blocking on iOS. The app loop is integrated with the
+        # main iOS event loop, so this call will return; however, it will leave
+        # the app in a state such that asyncio events will be scheduled on the
+        # iOS event loop.
+        self.loop.run_forever_cooperatively(lifecycle=iOSLifecycle())
 
-    def exit(self):
+    def set_main_window(self, window):
         pass
 
-    def set_on_exit(self, value):
+    def show_about_dialog(self):
+        self.interface.factory.not_implemented("App.show_about_dialog()")
+
+    def exit(self):
         pass
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/constraints.py` & `toga-iOS-0.3.1/src/toga_iOS/constraints.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,110 @@
-from .libs import (
-    NSLayoutAttributeTop, NSLayoutAttributeLeft,
-    NSLayoutAttributeRight, NSLayoutAttributeBottom,
-    NSLayoutRelationEqual, NSLayoutConstraint
+from toga_iOS.libs import (
+    NSLayoutAttributeBottom,
+    NSLayoutAttributeLeft,
+    NSLayoutAttributeRight,
+    NSLayoutAttributeTop,
+    NSLayoutConstraint,
+    NSLayoutRelationEqual,
 )
 
 
 class Constraints:
     def __init__(self, widget):
         """
+        A wrapper object storing the constraints required to position a widget
+        at a precise location in its container.
 
-        Args:
-            widget (:class: toga-iOS.Widget): The widget that should be constrained.
+        :param widget: The Widget implementation to be constrained.
         """
-        self._widget = widget
+        self.widget = widget
         self._container = None
 
         self.width_constraint = None
         self.height_constraint = None
 
         self.left_constraint = None
         self.top_constraint = None
 
-    @property
-    def widget(self):
-        return self._widget
+    # Deletion isn't an event we can programatically invoke; deletion
+    # of constraints can take several iterations before it occurs.
+    def __del__(self):  # pragma: nocover
+        self._remove_constraints()
 
-    @widget.setter
-    def widget(self, value):
-        self._widget = value
+    def _remove_constraints(self):
+        if self.container:
+            # print(f"Remove constraints for {self.widget} in {self.container}")
+            self.container.native.removeConstraint(self.width_constraint)
+            self.container.native.removeConstraint(self.height_constraint)
+            self.container.native.removeConstraint(self.left_constraint)
+            self.container.native.removeConstraint(self.top_constraint)
+
+            self.width_constraint.release()
+            self.height_constraint.release()
+            self.left_constraint.release()
+            self.top_constraint.release()
 
     @property
     def container(self):
         return self._container
 
     @container.setter
     def container(self, value):
+        # This will *always* remove and then add constraints. It relies on the base widget to
+        # *not* invoke this setter unless the container is actually changing.
+
+        self._remove_constraints()
         self._container = value
-        # print("Add constraints for", self.widget, 'in', self.container, self.widget.interface.layout)
-        self.left_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.widget.native, NSLayoutAttributeLeft,
-            NSLayoutRelationEqual,
-            self.container.native, NSLayoutAttributeLeft,
-            1.0, 10  # Use a dummy, non-zero value for now
-        )
-        self.container.native.addConstraint_(self.left_constraint)
-
-        self.top_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.widget.native, NSLayoutAttributeTop,
-            NSLayoutRelationEqual,
-            self.container.native, NSLayoutAttributeTop,
-            1.0, 5  # Use a dummy, non-zero value for now
-        )
-        self.container.native.addConstraint_(self.top_constraint)
-
-        self.width_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.widget.native, NSLayoutAttributeRight,
-            NSLayoutRelationEqual,
-            self.widget.native, NSLayoutAttributeLeft,
-            1.0, 50  # Use a dummy, non-zero value for now
-        )
-        self.container.native.addConstraint_(self.width_constraint)
-
-        self.height_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.widget.native, NSLayoutAttributeBottom,
-            NSLayoutRelationEqual,
-            self.widget.native, NSLayoutAttributeTop,
-            1.0, 30  # Use a dummy, non-zero value for now
-        )
-        self.container.native.addConstraint_(self.height_constraint)
+        if value is not None:
+            # print(f"Add constraints for {self.widget} in {self.container} {self.widget.interface.layout}")
+            self.left_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+                self.widget.native,
+                NSLayoutAttributeLeft,
+                NSLayoutRelationEqual,
+                self.container.native,
+                NSLayoutAttributeLeft,
+                1.0,
+                10,  # Use a dummy, non-zero value for now
+            ).retain()
+            self.container.native.addConstraint(self.left_constraint)
+
+            self.top_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+                self.widget.native,
+                NSLayoutAttributeTop,
+                NSLayoutRelationEqual,
+                self.container.native,
+                NSLayoutAttributeTop,
+                1.0,
+                5,  # Use a dummy, non-zero value for now
+            ).retain()
+            self.container.native.addConstraint(self.top_constraint)
+
+            self.width_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+                self.widget.native,
+                NSLayoutAttributeRight,
+                NSLayoutRelationEqual,
+                self.widget.native,
+                NSLayoutAttributeLeft,
+                1.0,
+                50,  # Use a dummy, non-zero value for now
+            ).retain()
+            self.container.native.addConstraint(self.width_constraint)
+
+            self.height_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+                self.widget.native,
+                NSLayoutAttributeBottom,
+                NSLayoutRelationEqual,
+                self.widget.native,
+                NSLayoutAttributeTop,
+                1.0,
+                30,  # Use a dummy, non-zero value for now
+            ).retain()
+            self.container.native.addConstraint(self.height_constraint)
 
     def update(self, x, y, width, height):
-        # print("UPDATE", self.widget, 'in', self.container, 'to', x, y, width, height)
         if self.container:
+            # print(f"UPDATE CONSTRAINTS {self.widget} in {self.container} {width}x{height}@{x},{y}")
             self.left_constraint.constant = x
             self.top_constraint.constant = y
 
             self.width_constraint.constant = width
             self.height_constraint.constant = height
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/widgets/detailedlist.py` & `toga-iOS-0.3.1/src/toga_iOS/widgets/detailedlist.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,158 @@
-from rubicon.objc import objc_method
+from rubicon.objc import SEL, objc_method, objc_property
+from travertino.size import at_least
+
 from toga_iOS.libs import (
+    NSIndexPath,
     UIControlEventValueChanged,
     UIRefreshControl,
     UITableViewCell,
     UITableViewCellEditingStyleDelete,
     UITableViewCellEditingStyleInsert,
     UITableViewCellEditingStyleNone,
     UITableViewCellSeparatorStyleNone,
     UITableViewCellStyleSubtitle,
     UITableViewController,
     UITableViewRowAnimationLeft,
-    UITableViewScrollPositionNone
+    UITableViewScrollPositionNone,
 )
-
-from .base import Widget
+from toga_iOS.widgets.base import Widget
 
 
 class TogaTableViewController(UITableViewController):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def numberOfSectionsInTableView_(self) -> int:
         return 1
 
     @objc_method
     def tableView_numberOfRowsInSection_(self, tableView, section: int) -> int:
         return len(self.interface.data)
 
     @objc_method
     def tableView_cellForRowAtIndexPath_(self, tableView, indexPath):
         cell = tableView.dequeueReusableCellWithIdentifier_("row")
         if cell is None:
-            cell = UITableViewCell.alloc().initWithStyle_reuseIdentifier_(UITableViewCellStyleSubtitle, "row")
+            cell = UITableViewCell.alloc().initWithStyle_reuseIdentifier_(
+                UITableViewCellStyleSubtitle, "row"
+            )
         value = self.interface.data[indexPath.item]
 
-        cell.textLabel.text = str(getattr(value, 'title', ''))
-        cell.detailTextLabel.text = str(getattr(value, 'subtitle', ''))
+        cell.textLabel.text = str(getattr(value, "title", ""))
+        cell.detailTextLabel.text = str(getattr(value, "subtitle", ""))
 
         # If the value has an icon attribute, get the _impl.
-        # Icons are deferred resources, so we bind to factory.
         try:
-            cell.imageView.image = value.icon.bind(self.interface.factory).native
+            cell.imageView.image = value.icon._impl.native
         except AttributeError:
             pass
 
         return cell
 
     @objc_method
-    def tableView_commitEditingStyle_forRowAtIndexPath_(self, tableView, editingStyle: int, indexPath):
+    def tableView_commitEditingStyle_forRowAtIndexPath_(
+        self, tableView, editingStyle: int, indexPath
+    ):
         if editingStyle == UITableViewCellEditingStyleDelete:
-            item = self.interface.data.row(indexPath.row)
+            item = self.interface.data[indexPath.row]
             if editingStyle == UITableViewCellEditingStyleDelete:
                 if self.interface.on_delete:
-                    self.interface.on_delete(self.interface, row=indexPath.row)
+                    self.interface.on_delete(self.interface, row=item)
 
                 tableView.beginUpdates()
-                self.interface.data.remove(item, refresh=False)
-                tableView.deleteRowsAtIndexPaths_withRowAnimation_([indexPath], UITableViewRowAnimationLeft)
+                self.interface.data.remove(item)
+                tableView.deleteRowsAtIndexPaths_withRowAnimation_(
+                    [indexPath], UITableViewRowAnimationLeft
+                )
                 tableView.endUpdates()
             elif editingStyle == UITableViewCellEditingStyleInsert:
                 pass
             elif editingStyle == UITableViewCellEditingStyleNone:
                 pass
 
     @objc_method
     def refresh(self):
         self.interface.on_refresh(self.interface)
 
     @objc_method
     def tableView_willSelectRowAtIndexPath_(self, tableView, indexPath):
+        index = indexPath.row
+        if index == -1:
+            selection = None
+        else:
+            selection = self.interface.data[index]
+
         if self.interface.on_select:
-            self.interface.on_select(self.interface, row=indexPath.row)
+            self.interface.on_select(self.interface, row=selection)
 
     # @objc_method
     # def tableView_heightForRowAtIndexPath_(self, tableView, indexPath) -> float:
     #     return 48.0
 
 
 class DetailedList(Widget):
     def create(self):
         self.controller = TogaTableViewController.alloc().init()
         self.controller.interface = self.interface
+        self.controller.impl = self
         self.native = self.controller.tableView
 
         self.native.separatorStyle = UITableViewCellSeparatorStyleNone
 
         # Add the layout constraints
         self.add_constraints()
 
     def set_on_refresh(self, handler: callable or None) -> None:
         if callable(handler):
             self.controller.refreshControl = UIRefreshControl.alloc().init()
             self.controller.refreshControl.addTarget(
                 self.controller,
-                action=SEL('refresh'),
-                forControlEvents=UIControlEventValueChanged
+                action=SEL("refresh"),
+                forControlEvents=UIControlEventValueChanged,
             )
         else:
             if self.controller.refreshControl:
                 self.controller.refreshControl.removeFromSuperview()
             self.controller.refreshControl = None
 
-    def after_on_refresh(self):
-        self.refreshControl.endRefreshing()
-        self.tableView.reloadData()
+    def after_on_refresh(self, widget, result):
+        self.controller.refreshControl.endRefreshing()
+        self.controller.tableView.reloadData()
 
     def change_source(self, source):
         self.native.reloadData()
 
     def insert(self, index, item):
         self.native.reloadData()
 
     def change(self, item):
         self.native.reloadData()
 
-    def remove(self, item):
+    def remove(self, item, index):
         self.native.reloadData()
 
     def clear(self):
         self.native.reloadData()
 
+    def get_selection(self):
+        return None
+
     def set_on_select(self, handler):
         # No special handling required
         pass
 
     def set_on_delete(self, handler):
         # No special handling required
         pass
 
     def scroll_to_row(self, row):
         self.native.scrollToRowAtIndexPath(
             NSIndexPath.indexPathForRow(row, inSection=0),
             atScrollPosition=UITableViewScrollPositionNone,
-            animated=False
+            animated=False,
         )
+
+    def rehint(self):
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = at_least(self.interface._MIN_HEIGHT)
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/widgets/multilinetextinput.py` & `toga-iOS-0.3.1/src/toga_iOS/widgets/multilinetextinput.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from rubicon.objc import (
-    CGPoint,
-    NSObject,
-    objc_method
-)
+from rubicon.objc import CGPoint, objc_method, objc_property
 from travertino.size import at_least
+
 from toga_iOS.libs import (
     NSLayoutAttributeBottom,
     NSLayoutAttributeLeading,
     NSLayoutAttributeTop,
     NSLayoutAttributeTrailing,
     NSLayoutConstraint,
     NSLayoutRelationEqual,
     UILabel,
     UITextView,
 )
+from toga_iOS.widgets.base import Widget
 
-from .base import Widget
 
 class TogaMultilineTextView(UITextView):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def pointInside_withEvent_(self, point: CGPoint, event) -> bool:
         # To keep consistency with non-mobile platforms, we'll resign the
         # responder status when you tap somewhere else outside this view
         # (except the keyboard)
-        within_x = point.x > 0 and point.x < self.frame.size.width
-        within_y = point.y > 0 and point.y < self.frame.size.height
+        within_x = 0 < point.x < self.frame.size.width
+        within_y = 0 < point.y < self.frame.size.height
         in_view = within_x and within_y
         if not in_view:
             self.resignFirstResponder()
         return in_view
 
     @objc_method
     def textViewShouldEndEditing_(self, text_view):
@@ -38,17 +38,20 @@
     def textViewDidBeginEditing_(self, text_view):
         self.placeholder_label.setHidden_(True)
 
     @objc_method
     def textViewDidEndEditing_(self, text_view):
         self.placeholder_label.setHidden_(len(text_view.text) > 0)
 
+
 class MultilineTextInput(Widget):
     def create(self):
         self.native = TogaMultilineTextView.alloc().init()
+        self.native.interface = self.interface
+        self.native.impl = self
         self.native.delegate = self.native
 
         # Placeholder isn't natively supported, so we create our
         # own
         self.placeholder_label = UILabel.alloc().init()
         self.placeholder_label.translatesAutoresizingMaskIntoConstraints = False
         self.placeholder_label.font = self.native.font
@@ -59,71 +62,78 @@
         # Delegate needs to update the placeholder depending on
         # input, so we give it just that to avoid a retain cycle
         self.native.placeholder_label = self.placeholder_label
 
         self.add_constraints()
 
     def constrain_placeholder_label(self):
-        leading_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        leading_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             self.placeholder_label,
             NSLayoutAttributeLeading,
             NSLayoutRelationEqual,
             self.native,
             NSLayoutAttributeLeading,
             1.0,
-            4.0
+            4.0,
         )
-        trailing_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        trailing_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             self.placeholder_label,
             NSLayoutAttributeTrailing,
             NSLayoutRelationEqual,
             self.native,
             NSLayoutAttributeTrailing,
             1.0,
-            0
+            0,
         )
-        top_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        top_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             self.placeholder_label,
             NSLayoutAttributeTop,
             NSLayoutRelationEqual,
             self.native,
             NSLayoutAttributeTop,
             1.0,
-            8.0
+            8.0,
         )
-        bottom_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        bottom_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             self.placeholder_label,
             NSLayoutAttributeBottom,
             NSLayoutRelationEqual,
             self.native,
             NSLayoutAttributeBottom,
             1.0,
-            0
+            0,
+        )
+        self.native.addConstraints_(
+            [leading_constraint, trailing_constraint, top_constraint, bottom_constraint]
         )
-        self.native.addConstraints_([
-            leading_constraint,
-            trailing_constraint,
-            top_constraint,
-            bottom_constraint
-        ])
 
     def set_placeholder(self, value):
         self.placeholder_label.text = value
 
     def set_readonly(self, value):
-        self.native.editable = not self.interface._readonly
+        self.native.editable = value
 
     def set_value(self, value):
-        self.native.text = self.interface._value
+        self.native.text = value
         self.placeholder_label.setHidden_(len(self.native.text) > 0)
 
     def get_value(self):
         return self.native.text
 
     def rehint(self):
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
-        self.interface.intrinsic.height = at_least(self.interface.MIN_HEIGHT)
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = at_least(self.interface._MIN_HEIGHT)
+
+    def set_font(self, font):
+        if font:
+            native_font = font._impl.native
+            self.native.font = native_font
+            self.placeholder_label.font = native_font
+
+    def set_on_change(self, handler):
+        self.interface.factory.not_implemented("MultilineTextInput.set_on_change()")
+
+    def scroll_to_bottom(self):
+        self.interface.factory.not_implemented("MultilineTextInput.scroll_to_bottom()")
 
-    def set_font(self, value):
-        if value:
-            self.native.font = value._impl.native
-            self.placeholder_label.font = value._impl.native
+    def scroll_to_top(self):
+        self.interface.factory.not_implemented("MultilineTextInput.scroll_to_top()")
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/widgets/switch.py` & `toga-iOS-0.3.1/src/toga_iOS/widgets/switch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,87 @@
-from rubicon.objc import objc_method, CGSize, SEL
-from toga_iOS.libs import(
+from rubicon.objc import SEL, CGSize, objc_method, objc_property
+from travertino.size import at_least
+
+from toga_iOS.colors import native_color
+from toga_iOS.libs import (
     UIControlEventValueChanged,
     UILabel,
     UILayoutConstraintAxis,
     UIStackView,
+    UIStackViewAlignment,
     UISwitch,
 )
-from travertino.size import at_least
-
-from .base import Widget
+from toga_iOS.widgets.base import Widget
 
 
 class TogaSwitch(UISwitch):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def onPress_(self, obj) -> None:
-        if self.interface.on_toggle:
-            self.interface.on_toggle(self.interface)
+        self.interface.on_change(None)
 
 
 class Switch(Widget):
+    SPACING = 10
+
     def create(self):
         self.native = UIStackView.alloc().init()
         self.native.interface = self.interface
+        self.native.impl = self
         self.native.axis = UILayoutConstraintAxis.Horizontal
+        self.native.alignment = UIStackViewAlignment.Center
+        self.native.spacing = self.SPACING
 
         self.native_label = UILabel.alloc().init()
 
         self.native_switch = TogaSwitch.alloc().init()
         self.native_switch.interface = self.interface
-        self.native_switch.addTarget_action_forControlEvents_(self.native_switch, SEL('onPress:'),
-                                                              UIControlEventValueChanged)
+        self.native_switch.addTarget(
+            self.native_switch,
+            action=SEL("onPress:"),
+            forControlEvents=UIControlEventValueChanged,
+        )
+
         # Add switch and label to UIStackView
-        self.native.addArrangedSubview_(self.native_label)
-        self.native.addArrangedSubview_(self.native_switch)
-        
+        self.native.addArrangedSubview(self.native_label)
+        self.native.addArrangedSubview(self.native_switch)
+
         # Add the layout constraints
         self.add_constraints()
 
-    def set_label(self, label):
-        self.native_label.text = str(label)
-        self.rehint()
+    def get_text(self):
+        return str(self.native_label.text)
 
-    def set_is_on(self, value):
-        self.native_switch.setOn_animated_(value, True)
+    def set_text(self, text):
+        self.native_label.text = text
 
-    def get_is_on(self):
+    def get_value(self):
         return self.native_switch.isOn()
 
-    def set_on_toggle(self, handler):
-        # No special handling required
-        pass
+    def set_value(self, value):
+        old_value = self.native_switch.isOn()
+        self.native_switch.setOn(value, animated=True)
+        if value != old_value:
+            self.interface.on_change(None)
 
     def get_enabled(self):
-        value = self.native_switch.isEnabled()
-        if value == 1:
-            return True
-        elif value == 0:
-            return False
-        else:
-            raise RuntimeError('Undefined value for enabled: {} in {}'.format(value, __class__))
+        return self.native_switch.isEnabled()
 
     def set_enabled(self, value):
-        if value:
-            self.native_label.enabled = True
-            self.native_switch.enabled = True
-        else:
-            self.native_label.enabled = False
-            self.native_switch.enabled = False
+        self.native_label.enabled = value
+        self.native_switch.enabled = value
+
+    def set_font(self, font):
+        self.native_label.font = font._impl.native
+
+    def set_color(self, value):
+        self.native_label.textColor = native_color(value)
 
     def rehint(self):
-        fitting_size = self.native.systemLayoutSizeFittingSize_(CGSize(0, 0))
-        self.interface.intrinsic.width = at_least(fitting_size.width)
-        self.interface.intrinsic.height = fitting_size.height
+        label_size = self.native_label.systemLayoutSizeFittingSize(CGSize(0, 0))
+        switch_size = self.native_switch.systemLayoutSizeFittingSize(CGSize(0, 0))
+        self.interface.intrinsic.width = at_least(
+            label_size.width + self.SPACING + switch_size.width
+        )
+        self.interface.intrinsic.height = max(label_size.height, switch_size.height)
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/widgets/scrollcontainer.py` & `toga-iOS-0.3.1/src/toga_iOS/widgets/scrollcontainer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,116 @@
 from rubicon.objc import CGSizeMake
+from travertino.size import at_least
+
 from toga_iOS.libs import (
     NSLayoutAttributeBottom,
     NSLayoutAttributeLeading,
     NSLayoutAttributeTop,
     NSLayoutAttributeTrailing,
     NSLayoutConstraint,
     NSLayoutRelationEqual,
-    UIScrollView
-)
-from toga_iOS.window import (
-    iOSViewport,
-    UIColor
+    UIColor,
+    UIScrollView,
 )
-from travertino.size import at_least
-from .base import Widget
+from toga_iOS.widgets.base import Widget
+from toga_iOS.window import iOSViewport
 
 
 class ScrollContainer(Widget):
     def update_content_size(self):
         # We need a layout pass to figure out how big the scrollable area should be
         scrollable_content = self.interface.content._impl
         scrollable_content.interface.refresh()
-        
+
         content_width = 0
         padding_horizontal = 0
         content_height = 0
         padding_vertical = 0
-        
+
         if self.interface.horizontal:
             content_width = scrollable_content.interface.layout.width
-            padding_horizontal = scrollable_content.interface.style.padding_left + scrollable_content.interface.style.padding_right
+            padding_horizontal = (
+                scrollable_content.interface.style.padding_left
+                + scrollable_content.interface.style.padding_right
+            )
         else:
             content_width = self.native.frame.size.width
-        
+
         if self.interface.vertical:
             content_height = scrollable_content.interface.layout.height
-            padding_vertical = scrollable_content.interface.style.padding_top + scrollable_content.interface.style.padding_bottom
-            # pad the scrollview for the statusbar offset
-            padding_vertical = padding_vertical + scrollable_content.viewport.statusbar_height
+            padding_vertical = (
+                scrollable_content.interface.style.padding_top
+                + scrollable_content.interface.style.padding_bottom
+            )
         else:
             content_height = self.native.frame.size.height
 
-        self.native.setContentSize_(CGSizeMake(content_width + padding_horizontal,
-                                               content_height + padding_vertical))
+        self.native.setContentSize_(
+            CGSizeMake(
+                content_width + padding_horizontal,
+                content_height + padding_vertical,
+            )
+        )
 
     def constrain_to_scrollview(self, widget):
         # The scrollview should know the content size as long as the
         # view contained has an intrinsic size and the constraints are
         # not ambiguous in any axis.
         view = widget.native
-        leading_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        leading_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             view,
             NSLayoutAttributeLeading,
             NSLayoutRelationEqual,
             self.native,
             NSLayoutAttributeLeading,
             1.0,
-            0
+            0,
         )
-        trailing_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        trailing_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             self.native,
             NSLayoutAttributeTrailing,
             NSLayoutRelationEqual,
             view,
             NSLayoutAttributeTrailing,
             1.0,
-            0
+            0,
         )
-        top_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        top_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             view,
             NSLayoutAttributeTop,
             NSLayoutRelationEqual,
             self.native,
             NSLayoutAttributeTop,
             1.0,
-            0
+            0,
         )
-        bottom_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
+        bottom_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
             self.native,
             NSLayoutAttributeBottom,
             NSLayoutRelationEqual,
             view,
             NSLayoutAttributeBottom,
             1.0,
-            0
+            0,
+        )
+        self.native.addConstraints_(
+            [leading_constraint, trailing_constraint, top_constraint, bottom_constraint]
         )
-        self.native.addConstraints_([
-            leading_constraint,
-            trailing_constraint,
-            top_constraint,
-            bottom_constraint
-        ])
 
     def create(self):
         self.native = UIScrollView.alloc().init()
         self.native.translatesAutoresizingMaskIntoConstraints = False
         self.native.backgroundColor = UIColor.whiteColor
         self.add_constraints()
 
     def set_content(self, widget):
-        if self.interface.content != None:
+        if self.interface.content is not None:
             self.interface.content._impl.native.removeFromSuperview()
         self.native.addSubview(widget.native)
-        widget.viewport = iOSViewport(self.native)
+        widget.viewport = iOSViewport(widget)
 
         for child in widget.interface.children:
             child._impl.container = widget
 
         self.constrain_to_scrollview(widget)
 
     def set_vertical(self, value):
@@ -114,8 +118,37 @@
             self.update_content_size()
 
     def set_horizontal(self, value):
         if self.interface.content:
             self.update_content_size()
 
     def rehint(self):
-        self.update_content_size()
+        if self.interface.content:
+            self.update_content_size()
+
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = at_least(self.interface._MIN_HEIGHT)
+
+    def set_on_scroll(self, on_scroll):
+        self.interface.factory.not_implemented("ScrollContainer.set_on_scroll()")
+
+    def get_vertical_position(self):
+        self.interface.factory.not_implemented(
+            "ScrollContainer.get_vertical_position()"
+        )
+        return 0
+
+    def set_vertical_position(self, vertical_position):
+        self.interface.factory.not_implemented(
+            "ScrollContainer.set_vertical_position()"
+        )
+
+    def get_horizontal_position(self):
+        self.interface.factory.not_implemented(
+            "ScrollContainer.get_horizontal_position()"
+        )
+        return 0
+
+    def set_horizontal_position(self, horizontal_position):
+        self.interface.factory.not_implemented(
+            "ScrollContainer.set_horizontal_position()"
+        )
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/widgets/numberinput.py` & `toga-iOS-0.3.1/src/toga_iOS/widgets/textinput.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,83 @@
-from ctypes import c_int
-from decimal import Decimal
-
-from rubicon.objc import objc_method, CGSize, NSObject, SEL, NSRange, send_message
+from rubicon.objc import SEL, CGSize, objc_method, objc_property
 from travertino.size import at_least
 
-from toga_iOS.libs import(
+from toga_iOS.libs import (
     NSTextAlignment,
     UIControlEventEditingChanged,
-    UIKeyboardType,
     UITextBorderStyle,
-    UITextField
+    UITextField,
 )
+from toga_iOS.widgets.base import Widget
 
-from .base import Widget
 
+class TogaTextField(UITextField):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
 
-class TogaNumericTextField(UITextField):
     @objc_method
     def textFieldDidChange_(self, notification) -> None:
-        if self.text:
-            self.interface._value = Decimal(str(self.text)).quantize(self.interface.step)
-        else:
-            self.interface._value = None
         if self.interface.on_change:
             self.interface.on_change(self.interface)
 
-    @objc_method
-    def textField_shouldChangeCharactersInRange_replacementString_(self, textField, textRange: NSRange, chars) -> bool:
-        # chars will be zero length in the case of a deletion
-        # otherwise, accept any number, or '.' (as long as this is the first one)
-        if (len(chars) == 0
-                    or chars.isdigit()
-                    or (chars == '.' and '.' not in self.text)
-                ):
-            return True
-        return False
-
 
-class NumberInput(Widget):
+class TextInput(Widget):
     def create(self):
-        self.native = TogaNumericTextField.alloc().init()
+        self.native = TogaTextField.new()
         self.native.interface = self.interface
-        self.native.delegate = self.native
+        self.native.impl = self
+
         self.native.borderStyle = UITextBorderStyle.RoundedRect
-        # FIXME: See Rubicon #96
-        # self.native.keyboardType = UIKeyboardType.DecimalPad
-        send_message(
-            self.native,
-            'setKeyboardType:',
-            UIKeyboardType.DecimalPad.value,
-            restype=None,
-            argtypes=[c_int]
-        )
 
-        # Make the text field respond to any content change.
         self.native.addTarget(
             self.native,
-            action=SEL('textFieldDidChange:'),
-            forControlEvents=UIControlEventEditingChanged
+            action=SEL("textFieldDidChange:"),
+            forControlEvents=UIControlEventEditingChanged,
         )
 
         # Add the layout constraints
         self.add_constraints()
 
     def set_readonly(self, value):
         self.native.enabled = not value
 
     def set_placeholder(self, value):
         self.native.placeholder = value
 
-    def set_step(self, step):
-        # No implementation required.
-        # Step functionality doesn't make sense on iOS
-        pass
-
-    def set_min_value(self, value):
-        # No special handling required
-        pass
-
-    def set_max_value(self, value):
-        # No special handling required
-        pass
+    def get_value(self):
+        return str(self.native.text)
 
     def set_value(self, value):
         self.native.text = value
 
     def set_alignment(self, value):
         if value:
             self.native.textAlignment = NSTextAlignment(value)
 
-    def set_font(self, value):
-        if value:
-            self.native.font = value._impl.native
+    def set_font(self, font):
+        if font:
+            self.native.font = font._impl.native
 
     def rehint(self):
         # Height of a text input is known.
         fitting_size = self.native.systemLayoutSizeFittingSize(CGSize(0, 0))
         self.interface.intrinsic.width = at_least(fitting_size.width)
         self.interface.intrinsic.height = fitting_size.height
 
     def set_on_change(self, handler):
         # No special handling required
         pass
+
+    def set_on_gain_focus(self, handler):
+        self.interface.factory.not_implemented("TextInput.set_on_gain_focus()")
+
+    def set_on_lose_focus(self, handler):
+        self.interface.factory.not_implemented("TextInput.set_on_lose_focus()")
+
+    def set_error(self, error_message):
+        self.interface.factory.not_implemented("TextInput.set_error()")
+
+    def clear_error(self):
+        self.interface.factory.not_implemented("TextInput.clear_error()")
+
+    def is_valid(self):
+        self.interface.factory.not_implemented("TextInput.is_valid()")
```

### Comparing `toga-iOS-0.3.0.dev9/toga_iOS/widgets/selection.py` & `toga-iOS-0.3.1/src/toga_iOS/widgets/selection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-from rubicon.objc import objc_method, CGSize
+from rubicon.objc import CGSize, objc_method, objc_property
 from travertino.size import at_least
 
 from toga_iOS.libs import UIColor, UIPickerView, UITextBorderStyle, UITextField
-
-from .base import Widget
+from toga_iOS.widgets.base import Widget
 
 
 class TogaPickerView(UIPickerView):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def numberOfComponentsInPickerView_(self, pickerView) -> int:
         return 1
 
     @objc_method
     def pickerView_numberOfRowsInComponent_(self, pickerView, component: int) -> int:
         return len(self.interface.items)
 
     @objc_method
-    def pickerView_titleForRow_forComponent_(self, pickerView, row: int, component: int):
+    def pickerView_titleForRow_forComponent_(
+        self, pickerView, row: int, component: int
+    ):
         return str(self.interface.items[row])
 
     @objc_method
-    def pickerView_didSelectRow_inComponent_(self, pickerView, row: int, component: int):
+    def pickerView_didSelectRow_inComponent_(
+        self, pickerView, row: int, component: int
+    ):
         self.native.text = self.interface.items[row]
         if self.interface.on_select:
             self.interface.on_select(self.interface)
 
 
 class Selection(Widget):
     def create(self):
         self.native = UITextField.alloc().init()
         self.native.interface = self.interface
+        self.native.impl = self
         self.native.tintColor = UIColor.clearColor
         self.native.borderStyle = UITextBorderStyle.RoundedRect
 
         self.picker = TogaPickerView.alloc().init()
         self.picker.interface = self.interface
         self.picker.native = self.native
         self.picker.delegate = self.picker
@@ -55,15 +62,15 @@
         pass
 
     def add_item(self, item):
         if not self.native.text:
             self.native.text = item
 
     def select_item(self, item):
-        self.interface.factory.not_implemented('Selection.select_item()')
+        self.interface.factory.not_implemented("Selection.select_item()")
 
     def get_selected_item(self):
         return self.interface.items[self.picker.selectedRowInComponent(0)]
 
     def set_on_select(self, handler):
         # No special handling required
         pass
```

