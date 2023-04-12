# Comparing `tmp/toga-cocoa-0.3.0.dev9.tar.gz` & `tmp/toga-cocoa-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-cocoa-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:19 2018, max compression
+gzip compressed data, was "toga-cocoa-0.3.1.tar", last modified: Wed Apr 12 01:58:15 2023, max compression
```

## Comparing `toga-cocoa-0.3.0.dev9.tar` & `toga-cocoa-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,93 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     2418 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/hardware/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2018-05-26 09:29:22.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/hardware/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      272 2017-12-23 03:47:56.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/color.py
--rw-r--r--   0 rkm        (501) staff       (20)      327 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/command.py
--rw-r--r--   0 rkm        (501) staff       (20)     8676 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/window.py
--rw-r--r--   0 rkm        (501) staff       (20)      351 2018-05-17 17:50:36.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     4066 2018-05-26 09:29:22.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/keys.py
--rw-r--r--   0 rkm        (501) staff       (20)     2331 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/font.py
--rw-r--r--   0 rkm        (501) staff       (20)     1617 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/factory.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/libs/
--rw-r--r--   0 rkm        (501) staff       (20)     6474 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/libs/core_graphics.py
--rw-r--r--   0 rkm        (501) staff       (20)      124 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/libs/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1583 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/libs/foundation.py
--rw-r--r--   0 rkm        (501) staff       (20)     3293 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/libs/core_text.py
--rw-r--r--   0 rkm        (501) staff       (20)    23301 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/libs/appkit.py
--rw-r--r--   0 rkm        (501) staff       (20)      581 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/libs/webkit.py
--rw-r--r--   0 rkm        (501) staff       (20)     6322 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/app.py
--rw-r--r--   0 rkm        (501) staff       (20)     2998 2017-12-23 03:47:56.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/constraints.py
--rw-r--r--   0 rkm        (501) staff       (20)     2891 2017-12-23 03:47:56.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/dialogs.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)     1405 2018-05-26 09:29:22.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/icon.py
--rw-r--r--   0 rkm        (501) staff       (20)     7640 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/tree.py
--rw-r--r--   0 rkm        (501) staff       (20)     1047 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)      841 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/box.py
--rw-r--r--   0 rkm        (501) staff       (20)     2577 2018-01-12 22:11:27.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/splitcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     5101 2017-12-23 03:47:56.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/detailedlist.py
--rw-r--r--   0 rkm        (501) staff       (20)     1781 2018-05-26 09:29:22.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/multilinetextinput.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/internal/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/internal/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     7585 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/internal/refresh.py
--rw-r--r--   0 rkm        (501) staff       (20)     5600 2017-12-23 03:47:49.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/internal/cells.py
--rw-r--r--   0 rkm        (501) staff       (20)      192 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/internal/data.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1871 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     1467 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/switch.py
--rw-r--r--   0 rkm        (501) staff       (20)     1512 2017-12-23 03:47:56.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/scrollcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     1133 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/slider.py
--rw-r--r--   0 rkm        (501) staff       (20)     1242 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/button.py
--rw-r--r--   0 rkm        (501) staff       (20)     1039 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/progressbar.py
--rw-r--r--   0 rkm        (501) staff       (20)     1257 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/label.py
--rw-r--r--   0 rkm        (501) staff       (20)     6824 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/numberinput.py
--rw-r--r--   0 rkm        (501) staff       (20)      414 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     4692 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/table.py
--rw-r--r--   0 rkm        (501) staff       (20)     1203 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/selection.py
--rw-r--r--   0 rkm        (501) staff       (20)     2507 2017-12-23 03:47:56.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/webview.py
--rw-r--r--   0 rkm        (501) staff       (20)     1676 2017-12-23 03:47:56.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/optioncontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      683 2018-06-10 23:51:35.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/image.py
--rw-r--r--   0 rkm        (501) staff       (20)     1812 2018-06-30 03:06:45.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/base.py
--rw-r--r--   0 rkm        (501) staff       (20)     7239 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/canvas.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     2418 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)     1572 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)       42 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)       17 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/toga_cocoa.egg-info/dependency_links.txt
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/tests/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/tests/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      275 2017-12-22 11:14:30.000000 toga-cocoa-0.3.0.dev9/tests/test_implementation.py
--rw-r--r--   0 rkm        (501) staff       (20)      113 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/MANIFEST.in
--rw-r--r--   0 rkm        (501) staff       (20)     1698 2018-07-07 05:52:00.000000 toga-cocoa-0.3.0.dev9/setup.py
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:19.000000 toga-cocoa-0.3.0.dev9/setup.cfg
--rw-r--r--   0 rkm        (501) staff       (20)     1160 2017-12-22 11:14:05.000000 toga-cocoa-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.252044 toga-cocoa-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-12 01:58:15.252044 toga-cocoa-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-12 01:58:15.252044 toga-cocoa-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.224044 toga-cocoa-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.236044 toga-cocoa-0.3.1/src/toga_cocoa/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.240044 toga-cocoa-0.3.1/src/toga_cocoa/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.240044 toga-cocoa-0.3.1/src/toga_cocoa/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26512 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/libs/appkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/libs/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/libs/core_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/libs/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/libs/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.244044 toga-cocoa-0.3.1/src/toga_cocoa/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.248044 toga-cocoa-0.3.1/src/toga_cocoa/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/imageview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.248044 toga-cocoa-0.3.1/src/toga_cocoa/widgets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/internal/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/internal/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/internal/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/src/toga_cocoa/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.240044 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-12 01:58:15.000000 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-12 01:58:15.000000 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:15.000000 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 01:58:15.000000 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:57:56.000000 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 01:58:15.000000 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 01:58:15.000000 toga-cocoa-0.3.1/src/toga_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.248044 toga-cocoa-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests/test_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.248044 toga-cocoa-0.3.1/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:15.252044 toga-cocoa-0.3.1/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-12 01:57:23.000000 toga-cocoa-0.3.1/tests_backend/widgets/textinput.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/factory.py` & `toga-cocoa-0.3.1/src/toga_cocoa/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,79 @@
-from .app import App, MainWindow
-from .color import native_color
+from . import dialogs
+from .app import App, DocumentApp, MainWindow
 from .command import Command
-from .font import Font
+from .documents import Document
 
+# Resources
+from .fonts import Font
+from .icons import Icon
+from .images import Image
+from .paths import paths
+
+# Widgets
+from .widgets.activityindicator import ActivityIndicator
 from .widgets.box import Box
 from .widgets.button import Button
 from .widgets.canvas import Canvas
 from .widgets.detailedlist import DetailedList
-from .widgets.icon import Icon
-from .widgets.image import Image
+from .widgets.divider import Divider
 from .widgets.imageview import ImageView
 from .widgets.label import Label
 from .widgets.multilinetextinput import MultilineTextInput
 from .widgets.numberinput import NumberInput
 from .widgets.optioncontainer import OptionContainer
 from .widgets.passwordinput import PasswordInput
 from .widgets.progressbar import ProgressBar
 from .widgets.scrollcontainer import ScrollContainer
 from .widgets.selection import Selection
-from .widgets.slider import *
+from .widgets.slider import Slider
 from .widgets.splitcontainer import SplitContainer
 from .widgets.switch import Switch
 from .widgets.table import Table
 from .widgets.textinput import TextInput
 from .widgets.tree import Tree
 from .widgets.webview import WebView
 from .window import Window
 
 
 def not_implemented(feature):
-    print('[Cocoa] Not implemented: {}'.format(feature))
+    print(f"[Cocoa] Not implemented: {feature}")  # pragma: nocover
 
 
 __all__ = [
-    'not_implemented',
-
-    'App', 'MainWindow',
-    'native_color',
-    'Command',
-    'Font',
-
-    'Box',
-    'Button',
-    'Canvas',
-    'DetailedList',
-    'Icon',
-    'Image',
-    'ImageView',
-    'Label',
-    'MultilineTextInput',
-    'NumberInput',
-    'OptionContainer',
-    'PasswordInput',
-    'ProgressBar',
-    'ScrollContainer',
-    'Selection',
-    'Slider',
-    'SplitContainer',
-    'Switch',
-    'Table',
-    'TextInput',
-    'Tree',
-    'WebView',
-    'Window',
+    "not_implemented",
+    "App",
+    "DocumentApp",
+    "MainWindow",
+    "Command",
+    "Document",
+    # Resources
+    "Font",
+    "Icon",
+    "Image",
+    "paths",
+    "dialogs",
+    # Widgets
+    "ActivityIndicator",
+    "Box",
+    "Button",
+    "Canvas",
+    "DetailedList",
+    "Divider",
+    "ImageView",
+    "Label",
+    "MultilineTextInput",
+    "NumberInput",
+    "OptionContainer",
+    "PasswordInput",
+    "ProgressBar",
+    "ScrollContainer",
+    "Selection",
+    "Slider",
+    "SplitContainer",
+    "Switch",
+    "Table",
+    "TextInput",
+    "Tree",
+    "WebView",
+    "Window",
 ]
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/libs/core_graphics.py` & `toga-cocoa-0.3.1/src/toga_cocoa/libs/core_graphics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 ##########################################################################
 # System/Library/Frameworks/CoreGraphics.framework
 ##########################################################################
-from ctypes import *
-from ctypes import util
+from ctypes import (
+    POINTER,
+    Structure,
+    c_int,
+    c_int32,
+    c_size_t,
+    c_uint32,
+    c_void_p,
+    c_wchar_p,
+)
 
+from rubicon.objc import CGFloat, CGRect
+from rubicon.objc.runtime import load_library
 from rubicon.objc.types import register_preferred_encoding
-from rubicon.objc import *
-
 
 ######################################################################
-core_graphics = cdll.LoadLibrary(util.find_library('CoreGraphics'))
+core_graphics = load_library("CoreGraphics")
 ######################################################################
 
 ######################################################################
 # CGAffineTransform.h
 
 
 class CGAffineTransform(Structure):
@@ -32,15 +40,15 @@
 core_graphics.CGAffineTransformInvert.argtypes = [CGAffineTransform]
 core_graphics.CGAffineTransformMakeScale.restype = CGAffineTransform
 core_graphics.CGAffineTransformMakeScale.argtypes = [CGFloat, CGFloat]
 
 ######################################################################
 # CGContext.h
 CGContextRef = c_void_p
-register_preferred_encoding(b'^{__CGContext=}', CGContextRef)
+register_preferred_encoding(b"^{__CGContext=}", CGContextRef)
 
 CGPathDrawingMode = c_int32
 kCGPathFill = 0
 kCGPathEOFill = 1
 kCGPathStroke = 2
 kCGPathFillStroke = 3
 kCGPathEOFillStroke = 4
@@ -56,21 +64,43 @@
 kCGTextClip = 7
 
 CGTextEncoding = c_int32
 kCGEncodingFontSpecific = 0
 kCGEncodingMacRoman = 1
 
 core_graphics.CGContextAddArc.restype = c_void_p
-core_graphics.CGContextAddArc.argtypes = [CGContextRef, CGFloat, CGFloat, CGFloat, CGFloat, CGFloat, c_int]
+core_graphics.CGContextAddArc.argtypes = [
+    CGContextRef,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    c_int,
+]
 core_graphics.CGContextAddCurveToPoint.restype = c_void_p
-core_graphics.CGContextAddCurveToPoint.argtypes = [CGContextRef, CGFloat, CGFloat, CGFloat, CGFloat, CGFloat, CGFloat]
+core_graphics.CGContextAddCurveToPoint.argtypes = [
+    CGContextRef,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+]
 core_graphics.CGContextAddLineToPoint.restype = c_void_p
 core_graphics.CGContextAddLineToPoint.argtypes = [CGContextRef, CGFloat, CGFloat]
 core_graphics.CGContextAddQuadCurveToPoint.restype = c_void_p
-core_graphics.CGContextAddQuadCurveToPoint.argtypes = [CGContextRef, CGFloat, CGFloat, CGFloat, CGFloat]
+core_graphics.CGContextAddQuadCurveToPoint.argtypes = [
+    CGContextRef,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+]
 core_graphics.CGContextAddRect.restype = c_void_p
 core_graphics.CGContextAddRect.argtypes = [CGContextRef, CGRect]
 core_graphics.CGContextBeginPath.restype = c_void_p
 core_graphics.CGContextBeginPath.argtypes = [c_void_p]
 core_graphics.CGContextConcatCTM.restype = c_void_p
 core_graphics.CGContextConcatCTM.argtypes = [CGContextRef, CGAffineTransform]
 core_graphics.CGContextClosePath.restype = c_void_p
@@ -86,79 +116,102 @@
 core_graphics.CGContextRotateCTM.restype = c_void_p
 core_graphics.CGContextRotateCTM.argtypes = [CGContextRef, CGFloat]
 core_graphics.CGContextSaveGState.restype = c_void_p
 core_graphics.CGContextSaveGState.argtypes = [c_void_p]
 core_graphics.CGContextScaleCTM.restype = c_void_p
 core_graphics.CGContextScaleCTM.argtypes = [CGContextRef, CGFloat, CGFloat]
 core_graphics.CGContextSelectFont.restype = c_void_p
-core_graphics.CGContextSelectFont.argtypes = [CGContextRef, c_wchar_p, CGFloat, CGTextEncoding]
+core_graphics.CGContextSelectFont.argtypes = [
+    CGContextRef,
+    c_wchar_p,
+    CGFloat,
+    CGTextEncoding,
+]
 core_graphics.CGContextSetLineWidth.restype = c_void_p
 core_graphics.CGContextSetLineWidth.argtypes = [CGContextRef, CGFloat]
+core_graphics.CGContextSetLineDash.restype = c_void_p
+core_graphics.CGContextSetLineDash.argtypes = [
+    CGContextRef,
+    CGFloat,
+    POINTER(CGFloat),
+    c_size_t,
+]
 core_graphics.CGContextSetRGBFillColor.restype = c_void_p
-core_graphics.CGContextSetRGBFillColor.argtypes = [CGContextRef, CGFloat, CGFloat, CGFloat, CGFloat]
+core_graphics.CGContextSetRGBFillColor.argtypes = [
+    CGContextRef,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+]
 core_graphics.CGContextSetRGBStrokeColor.restype = c_void_p
-core_graphics.CGContextSetRGBStrokeColor.argtypes = [CGContextRef, CGFloat, CGFloat, CGFloat, CGFloat]
+core_graphics.CGContextSetRGBStrokeColor.argtypes = [
+    CGContextRef,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+    CGFloat,
+]
 core_graphics.CGContextSetTextDrawingMode.restype = c_void_p
 core_graphics.CGContextSetTextDrawingMode.argtypes = [CGContextRef, CGTextDrawingMode]
 core_graphics.CGContextSetTextMatrix.restype = c_void_p
 core_graphics.CGContextSetTextMatrix.argtypes = [CGContextRef, CGAffineTransform]
 core_graphics.CGContextSetTextPosition.restype = c_void_p
 core_graphics.CGContextSetTextPosition.argtypes = [CGContextRef, CGFloat, CGFloat]
 core_graphics.CGContextShowTextAtPoint.restype = c_void_p
-core_graphics.CGContextShowTextAtPoint.argtypes = [CGContextRef, CGFloat, CGFloat, c_wchar_p, c_size_t]
+core_graphics.CGContextShowTextAtPoint.argtypes = [
+    CGContextRef,
+    CGFloat,
+    CGFloat,
+    c_wchar_p,
+    c_size_t,
+]
 core_graphics.CGContextTranslateCTM.restype = c_void_p
 core_graphics.CGContextTranslateCTM.argtypes = [CGContextRef, CGFloat, CGFloat]
 
 ######################################################################
 # CGEvent.h
 
 
 class CGEventRef(c_void_p):
     pass
 
 
-register_preferred_encoding(b'^{__CGEvent=}', CGEventRef)
+register_preferred_encoding(b"^{__CGEvent=}", CGEventRef)
 
 CGEventSourceRef = c_void_p
-register_preferred_encoding(b'^{__CGEventSource=}', CGEventSourceRef)
+register_preferred_encoding(b"^{__CGEventSource=}", CGEventSourceRef)
 
 CGScrollEventUnit = c_uint32
 
-core_graphics.CGEventCreateScrollWheelEvent.argtypes = [CGEventSourceRef, CGScrollEventUnit, c_uint32, c_int32, c_int32]
+core_graphics.CGEventCreateScrollWheelEvent.argtypes = [
+    CGEventSourceRef,
+    CGScrollEventUnit,
+    c_uint32,
+    c_int32,
+    c_int32,
+]
 core_graphics.CGEventCreateScrollWheelEvent.restype = CGEventRef
 
 ######################################################################
 # CGEventTypes.h
 kCGScrollEventUnitPixel = 0
 kCGScrollEventUnitLine = 1
 
 ######################################################################
-# CGGeometry.h
-
-
-class CGRectMake(Structure):
-    _fields_ = [
-        ("origin", CGPoint),
-        ("size", CGSize),
-    ]
-
-
-######################################################################
 # CGImage.h
 kCGImageAlphaNone = 0
 kCGImageAlphaPremultipliedLast = 1
 kCGImageAlphaPremultipliedFirst = 2
 kCGImageAlphaLast = 3
 kCGImageAlphaFirst = 4
 kCGImageAlphaNoneSkipLast = 5
 kCGImageAlphaNoneSkipFirst = 6
 kCGImageAlphaOnly = 7
 
-kCGImageAlphaPremultipliedLast = 1
-
 kCGBitmapAlphaInfoMask = 0x1F
 kCGBitmapFloatComponents = 1 << 8
 
 kCGBitmapByteOrderMask = 0x7000
 kCGBitmapByteOrderDefault = 0 << 12
 kCGBitmapByteOrder16Little = 1 << 12
 kCGBitmapByteOrder32Little = 2 << 12
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/libs/core_text.py` & `toga-cocoa-0.3.1/src/toga_cocoa/libs/core_text.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 ##########################################################################
 # System/Library/Frameworks/CoreText.framework
 ##########################################################################
-from ctypes import *
-from ctypes import util
+from ctypes import POINTER, c_bool, c_double, c_uint32, c_void_p, cdll, util
 
-from rubicon.objc import *
+from rubicon.objc import CFIndex, CGFloat, CGGlyph, CGRect, CGSize, UniChar
 
 ######################################################################
-core_text = cdll.LoadLibrary(util.find_library('CoreText'))
+core_text = cdll.LoadLibrary(util.find_library("CoreText"))
 ######################################################################
 
 ######################################################################
 # CTFontDescriptor.h
 
 CTFontOrientation = c_uint32
 
@@ -19,33 +18,55 @@
 # CTFontTraits.h
 
 CTFontSymbolicTraits = c_uint32
 
 ######################################################################
 # CTFont.h
 core_text.CTFontGetBoundingRectsForGlyphs.restype = CGRect
-core_text.CTFontGetBoundingRectsForGlyphs.argtypes = [c_void_p, CTFontOrientation, POINTER(CGGlyph), POINTER(CGRect), CFIndex]
+core_text.CTFontGetBoundingRectsForGlyphs.argtypes = [
+    c_void_p,
+    CTFontOrientation,
+    POINTER(CGGlyph),
+    POINTER(CGRect),
+    CFIndex,
+]
 
 core_text.CTFontGetAdvancesForGlyphs.restype = c_double
-core_text.CTFontGetAdvancesForGlyphs.argtypes = [c_void_p, CTFontOrientation, POINTER(CGGlyph), POINTER(CGSize), CFIndex]
+core_text.CTFontGetAdvancesForGlyphs.argtypes = [
+    c_void_p,
+    CTFontOrientation,
+    POINTER(CGGlyph),
+    POINTER(CGSize),
+    CFIndex,
+]
 
 core_text.CTFontGetAscent.restype = CGFloat
 core_text.CTFontGetAscent.argtypes = [c_void_p]
 
 core_text.CTFontGetDescent.restype = CGFloat
 core_text.CTFontGetDescent.argtypes = [c_void_p]
 
 core_text.CTFontGetSymbolicTraits.restype = CTFontSymbolicTraits
 core_text.CTFontGetSymbolicTraits.argtypes = [c_void_p]
 
 core_text.CTFontGetGlyphsForCharacters.restype = c_bool
-core_text.CTFontGetGlyphsForCharacters.argtypes = [c_void_p, POINTER(UniChar), POINTER(CGGlyph), CFIndex]
+core_text.CTFontGetGlyphsForCharacters.argtypes = [
+    c_void_p,
+    POINTER(UniChar),
+    POINTER(CGGlyph),
+    CFIndex,
+]
 
 core_text.CTFontCreateWithGraphicsFont.restype = c_void_p
-core_text.CTFontCreateWithGraphicsFont.argtypes = [c_void_p, CGFloat, c_void_p, c_void_p]
+core_text.CTFontCreateWithGraphicsFont.argtypes = [
+    c_void_p,
+    CGFloat,
+    c_void_p,
+    c_void_p,
+]
 
 core_text.CTFontCopyFamilyName.restype = c_void_p
 core_text.CTFontCopyFamilyName.argtypes = [c_void_p]
 
 core_text.CTFontCopyFullName.restype = c_void_p
 core_text.CTFontCopyFullName.argtypes = [c_void_p]
 
@@ -54,32 +75,32 @@
 
 core_text.CTFontDescriptorCreateWithAttributes.restype = c_void_p
 core_text.CTFontDescriptorCreateWithAttributes.argtypes = [c_void_p]
 
 ######################################################################
 # CTFontDescriptor.h
 
-kCTFontFamilyNameAttribute = c_void_p.in_dll(core_text, 'kCTFontFamilyNameAttribute')
-kCTFontTraitsAttribute = c_void_p.in_dll(core_text, 'kCTFontTraitsAttribute')
+kCTFontFamilyNameAttribute = c_void_p.in_dll(core_text, "kCTFontFamilyNameAttribute")
+kCTFontTraitsAttribute = c_void_p.in_dll(core_text, "kCTFontTraitsAttribute")
 
 ######################################################################
 # CTFontTraits.h
 
-kCTFontSymbolicTrait = c_void_p.in_dll(core_text, 'kCTFontSymbolicTrait')
-kCTFontWeightTrait = c_void_p.in_dll(core_text, 'kCTFontWeightTrait')
+kCTFontSymbolicTrait = c_void_p.in_dll(core_text, "kCTFontSymbolicTrait")
+kCTFontWeightTrait = c_void_p.in_dll(core_text, "kCTFontWeightTrait")
 
-kCTFontItalicTrait = (1 << 0)
-kCTFontBoldTrait = (1 << 1)
+kCTFontItalicTrait = 1 << 0
+kCTFontBoldTrait = 1 << 1
 
 ######################################################################
 # CTLine.h
 
 core_text.CTLineCreateWithAttributedString.restype = c_void_p
 core_text.CTLineCreateWithAttributedString.argtypes = [c_void_p]
 
 core_text.CTLineDraw.restype = None
 core_text.CTLineDraw.argtypes = [c_void_p, c_void_p]
 
 ######################################################################
 # CTStringAttributes.h
 
-kCTFontAttributeName = c_void_p.in_dll(core_text, 'kCTFontAttributeName')
+kCTFontAttributeName = c_void_p.in_dll(core_text, "kCTFontAttributeName")
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/libs/webkit.py` & `toga-cocoa-0.3.1/src/toga_cocoa/libs/webkit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 ##########################################################################
 # System/Library/Frameworks/WebKit.framework
 ##########################################################################
-from ctypes import *
-from ctypes import util
 
-from rubicon.objc import *
+from rubicon.objc import ObjCClass
+from rubicon.objc.runtime import load_library
 
 ######################################################################
-webkit = cdll.LoadLibrary(util.find_library('WebKit'))
+webkit = load_library("WebKit")
 ######################################################################
 
 ######################################################################
 # WebView.h
-WebView = ObjCClass('WebView')
+WebView = ObjCClass("WebView")
+
+######################################################################
+# WKWebView.h
+WKWebView = ObjCClass("WKWebView")
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/constraints.py` & `toga-cocoa-0.3.1/src/toga_cocoa/constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,110 @@
 from .libs import (
-    NSLayoutAttributeTop, NSLayoutAttributeLeft,
-    NSLayoutAttributeRight, NSLayoutAttributeBottom,
-    NSLayoutRelationEqual, NSLayoutConstraint
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
-            widget (:class: toga-cocoa.Widget): The widget that should be constrained.
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
-        self.container.native.addConstraint(self.left_constraint)
-
-        self.top_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.widget.native, NSLayoutAttributeTop,
-            NSLayoutRelationEqual,
-            self.container.native, NSLayoutAttributeTop,
-            1.0, 5  # Use a dummy, non-zero value for now
-        )
-        self.container.native.addConstraint(self.top_constraint)
-
-        self.width_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.widget.native, NSLayoutAttributeRight,
-            NSLayoutRelationEqual,
-            self.widget.native, NSLayoutAttributeLeft,
-            1.0, 50  # Use a dummy, non-zero value for now
-        )
-        self.container.native.addConstraint(self.width_constraint)
-
-        self.height_constraint = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.widget.native, NSLayoutAttributeBottom,
-            NSLayoutRelationEqual,
-            self.widget.native, NSLayoutAttributeTop,
-            1.0, 30  # Use a dummy, non-zero value for now
-        )
-        self.container.native.addConstraint(self.height_constraint)
+        if value is not None:
+            # print(f"Add constraints for {self.widget} in {self.container} {self.widget.interface.layout})
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
-            # print("IN CONTAINER")
+            # print(f"UPDATE CONSTRAINTS {self.widget} in {self.container} {width}x{height}@{x},{y}")
             self.left_constraint.constant = x
             self.top_constraint.constant = y
 
             self.width_constraint.constant = width
             self.height_constraint.constant = height
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/imageview.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/imageview.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from toga_cocoa.libs import *
+from toga_cocoa.libs import (
+    NSImage,
+    NSImageAlignment,
+    NSImageFrameNone,
+    NSImageScaleProportionallyUpOrDown,
+    NSImageView,
+    NSSize,
+)
 
 from .base import Widget
 
 
 class ImageView(Widget):
-
     def create(self):
         self.native = NSImageView.alloc().init()
-        self.native.interface = self.interface
 
         # self._impl.imageFrameStyle = NSImageFrameGrayBezel
         self.native.imageFrameStyle = NSImageFrameNone
-        self.native.imageAlignment = NSImageAlignCenter
+        self.native.imageAlignment = NSImageAlignment.Center.value
         self.native.imageScaling = NSImageScaleProportionallyUpOrDown
 
         # Add the layout constraints
         self.add_constraints()
 
-    def get_image(self):
-        return self.native.image
-
     def set_image(self, image):
         if image:
-            self.native.image = image._impl.native
+            self.native.image = self.interface._image._impl.native
         else:
             width = 0
             height = 0
             if self.interface.style.width:
                 width = self.interface.style.width
             if self.interface.style.height:
                 height = self.interface.style.height
 
             self.native.image = NSImage.alloc().initWithSize(NSSize(width, height))
 
     def rehint(self):
         pass
-
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/splitcontainer.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/splitcontainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,73 @@
-from toga_cocoa.libs import *
+from travertino.size import at_least
+
+from toga_cocoa.libs import NSObject, NSSize, NSSplitView, objc_method
 from toga_cocoa.window import CocoaViewport
 
+from ..libs import objc_property
 from .base import Widget
 
 
 class TogaSplitViewDelegate(NSObject):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def splitView_resizeSubviewsWithOldSize_(self, view, size: NSSize) -> None:
-        if size.width and size.height:
-            count = len(self.interface.content)
+        # Turn all the weights into a fraction of 1.0
+        total = sum(self.interface._weight)
+        self.interface._weight = [weight / total for weight in self.interface._weight]
 
-            # Turn all the weights into a fraction of 1.0
-            total = sum(self.interface._weight)
-            self.interface._weight = [
-                weight / total
-                for weight in self.interface._weight
-            ]
+        # Mark the subviews as needing adjustment
+        view.adjustSubviews()
 
-            # Set the splitter positions based on the new weight fractions.
+        # Set the splitter positions based on the new weight fractions.
+        cumulative = 0.0
+        if self.interface.direction == self.interface.VERTICAL:
             for i, weight in enumerate(self.interface._weight[:-1]):
-                view.setPosition(size.width * self.interface._weight[i], ofDividerAtIndex=i)
-        view.adjustSubviews()
+                cumulative += weight
+                view.setPosition(view.frame.size.width * cumulative, ofDividerAtIndex=i)
+        else:
+            for i, weight in enumerate(self.interface._weight[:-1]):
+                cumulative += weight
+                view.setPosition(
+                    view.frame.size.height * cumulative, ofDividerAtIndex=i
+                )
 
     @objc_method
     def splitViewDidResizeSubviews_(self, notification) -> None:
         # If the window is actually visible, and the split has moved,
         # a resize of all the content panels is required. The refresh
         # needs to be directed at the root container holding the widget,
         # as the splitview may not be the root container.
         if self.interface.window and self.interface.window._impl.native.isVisible:
             self.interface.refresh()
-            self._impl.on_resize()
+            self.impl.on_resize()
 
 
 class SplitContainer(Widget):
-    """ Cocoa SplitContainer implementation
+    """Cocoa SplitContainer implementation.
 
     Todo:
         * update the minimum width of the whole SplitContainer based on the content of its sub layouts.
     """
+
     def create(self):
         self.native = NSSplitView.alloc().init()
 
         self.delegate = TogaSplitViewDelegate.alloc().init()
         self.delegate.interface = self.interface
-        self.delegate._impl = self
+        self.delegate.impl = self
         self.native.delegate = self.delegate
 
         # Add the layout constraints
         self.add_constraints()
 
-    def add_content(self, position, widget):
+    def add_content(self, position, widget, flex):
+        # TODO: add flex option to the implementation
         widget.viewport = CocoaViewport(widget.native)
 
         for child in widget.interface.children:
             child._impl.container = widget
 
         # Turn the autoresizing mask on the widget into constraints.
         # This makes the widget fill the available space inside the
@@ -64,7 +77,11 @@
         self.native.addSubview(widget.native)
 
     def set_direction(self, value):
         self.native.vertical = value
 
     def on_resize(self):
         pass
+
+    def rehint(self):
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = at_least(self.interface._MIN_HEIGHT)
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/detailedlist.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/detailedlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,49 @@
-from rubicon.objc import *
 from travertino.size import at_least
 
-from toga_cocoa.libs import *
+from toga_cocoa.libs import (
+    SEL,
+    NSBezelBorder,
+    NSMenu,
+    NSTableColumn,
+    NSTableView,
+    NSTableViewColumnAutoresizingStyle,
+    objc_method,
+    objc_property,
+)
+from toga_cocoa.widgets.base import Widget
+from toga_cocoa.widgets.internal.cells import TogaDetailedCell
+from toga_cocoa.widgets.internal.data import TogaData
+from toga_cocoa.widgets.internal.refresh import RefreshableScrollView
 
-from .base import Widget
-from .internal.cells import TogaDetailedCell
-from .internal.data import TogaData
-from .internal.refresh import RefreshableScrollView
 
-
-def attr_impl(value, attr, factory):
+def attr_impl(value, attr):
     # If the data value has an _impl attribute, invoke it.
     # This will manifest any impl-specific attributes.
     impl = getattr(value, attr, None)
     try:
-        return impl.bind(factory)
+        return impl._impl
     except AttributeError:
         return impl
 
 
 class TogaList(NSTableView):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def menuForEvent_(self, event):
         if self.interface.on_delete:
             mousePoint = self.convertPoint(event.locationInWindow, fromView=None)
             row = self.rowAtPoint(mousePoint)
 
             popup = NSMenu.alloc().initWithTitle("popup")
-            delete_item = popup.addItemWithTitle("Delete", action=SEL('actionDeleteRow:'), keyEquivalent="")
+            delete_item = popup.addItemWithTitle(
+                "Delete", action=SEL("actionDeleteRow:"), keyEquivalent=""
+            )
             delete_item.tag = row
             # action_item = popup.addItemWithTitle("???", action=SEL('actionRow:'), keyEquivalent="")
             # action_item.tag = row
 
             return popup
 
     @objc_method
@@ -47,20 +59,18 @@
     @objc_method
     def tableView_objectValueForTableColumn_row_(self, table, column, row: int):
         value = self.interface.data[row]
         try:
             data = value._impl
         except AttributeError:
             data = TogaData.alloc().init()
+            data.retain()
             value._impl = data
 
-        data.attrs = {
-            attr: attr_impl(value, attr, self.interface.factory)
-            for attr in value._attrs
-        }
+        data.attrs = {attr: attr_impl(value, attr) for attr in value._attrs}
 
         return data
 
     # TableDelegate methods
     @objc_method
     def tableView_heightOfRow_(self, table, row: int) -> float:
         return 48.0
@@ -69,45 +79,51 @@
     def selectionShouldChangeInTableView_(self, table) -> bool:
         # Explicitly allow selection on the table.
         # TODO: return False to disable selection.
         return True
 
     @objc_method
     def tableViewSelectionDidChange_(self, notification) -> None:
-        self.interface.selection = notification.object.selectedRow
-        self.interface.selected = self.interface.data[notification.object.selectedRow]
+        index = notification.object.selectedRow
+        if index == -1:
+            selection = None
+        else:
+            selection = self.interface.data[index]
+
         if self.interface.on_select:
-            row = notification.object.selectedRow if notification.object.selectedRow != -1 else None
-            self.interface.on_select(self.interface, row=row)
+            self.interface.on_select(self.interface, row=selection)
 
 
 class DetailedList(Widget):
     def create(self):
         # Create a List, and put it in a scroll view.
         # The scroll view is the _impl, because it's the outer container.
         self.native = RefreshableScrollView.alloc().init()
         self.native.interface = self.interface
+        self.native.impl = self
         self.native.hasVerticalScroller = True
         self.native.hasHorizontalScroller = False
         self.native.autohidesScrollers = False
         self.native.borderType = NSBezelBorder
 
         # Create the List widget
         self.detailedlist = TogaList.alloc().init()
         self.detailedlist.interface = self.interface
-        self.detailedlist._impl = self
-        self.detailedlist.columnAutoresizingStyle = NSTableViewUniformColumnAutoresizingStyle
+        self.detailedlist.impl = self
+        self.detailedlist.columnAutoresizingStyle = (
+            NSTableViewColumnAutoresizingStyle.Uniform
+        )
 
         # TODO: Optionally enable multiple selection
         self.detailedlist.allowsMultipleSelection = False
 
         self.native.detailedlist = self.detailedlist
 
         # Create the column for the detailed list
-        column = NSTableColumn.alloc().initWithIdentifier('data')
+        column = NSTableColumn.alloc().initWithIdentifier("data")
         self.detailedlist.addTableColumn(column)
         self.columns = [column]
 
         cell = TogaDetailedCell.alloc().init()
         column.dataCell = cell
 
         # Hide the column header.
@@ -127,31 +143,44 @@
 
     def insert(self, index, item):
         self.detailedlist.reloadData()
 
     def change(self, item):
         self.detailedlist.reloadData()
 
-    def remove(self, item):
+    def remove(self, index, item):
         self.detailedlist.reloadData()
 
+        # After deletion, the selection changes, but Cocoa doesn't send
+        # a tableViewSelectionDidChange: message.
+        selection = self.get_selection()
+        if selection and self.interface.on_select:
+            self.interface.on_select(self.interface, row=selection)
+
     def clear(self):
         self.detailedlist.reloadData()
 
     def set_on_refresh(self, handler):
         pass
 
-    def after_on_refresh(self):
+    def after_on_refresh(self, widget, result):
         self.native.finishedLoading()
 
+    def get_selection(self):
+        index = self.detailedlist.selectedRow
+        if index != -1:
+            return self.interface.data[index]
+        else:
+            return None
+
     def set_on_select(self, handler):
         pass
 
     def set_on_delete(self, handler):
         pass
 
     def scroll_to_row(self, row):
         self.detailedlist.scrollRowToVisible(row)
 
     def rehint(self):
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
-        self.interface.intrinsic.height = at_least(self.interface.MIN_HEIGHT)
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = at_least(self.interface._MIN_HEIGHT)
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/multilinetextinput.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/progressbar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 from travertino.size import at_least
 
-from toga_cocoa.libs import *
+from toga_cocoa.libs import NSProgressIndicator, NSProgressIndicatorBarStyle
 
 from .base import Widget
 
+# Implementation notes
+# ====================
+#
+# * Cocoa doesn't have a way to determine if the animation is running. We track
+#   running status independently for interface compliance.
 
-class TogaTextView(NSTextView):
-    @objc_method
-    def touchBar(self):
-        # Disable the touchbar.
-        return None
 
-
-class MultilineTextInput(Widget):
+class ProgressBar(Widget):
     def create(self):
-        # Create a multiline view, and put it in a scroll view.
-        # The scroll view is the native, because it's the outer container.
-        self.native = NSScrollView.alloc().init()
-        self.native.hasVerticalScroller = True
-        self.native.hasHorizontalScroller = False
-        self.native.autohidesScrollers = False
-        self.native.borderType = NSBezelBorder
-
-        # Disable all autolayout functionality on the outer widget
-        self.native.translatesAutoresizingMaskIntoConstraints = False
-
-        # Create the actual text widget
-        self.text = TogaTextView.alloc().init()
-        self.text.editable = True
-        self.text.selectable = True
-        self.text.verticallyResizable = True
-        self.text.horizontallyResizable = False
-
-        self.text.autoresizingMask = NSViewWidthSizable
-
-        # Put the text view in the scroll window.
-        self.native.documentView = self.text
+        self.native = NSProgressIndicator.new()
+        self.native.style = NSProgressIndicatorBarStyle
+        self.native.displayedWhenStopped = True
+        self.native.usesThreadedAnimation = False
 
         # Add the layout constraints
         self.add_constraints()
 
-    def set_placeholder(self, value):
-        self.text.placeholderString = self.interface._value
+        self._is_running = False
 
-    def set_readonly(self, value):
-        self.text.editable = not self.interface._readonly
+    def is_running(self):
+        return self._is_running
 
     def get_value(self):
-        return self.text.string
+        if self.native.isIndeterminate():
+            return None
+        return float(self.native.doubleValue)
 
     def set_value(self, value):
-        self.text.string = self.interface._value
+        self.native.doubleValue = value
+
+    def start(self):
+        self.native.startAnimation(self.native)
+        self._is_running = True
+
+    def stop(self):
+        self.native.stopAnimation(self.native)
+        self._is_running = False
+
+    def get_max(self):
+        if self.native.isIndeterminate():
+            return None
+        return float(self.native.maxValue)
+
+    def set_max(self, value):
+        if value is None:
+            self.native.doubleValue = 0.0
+            self.native.indeterminate = True
+            if self.is_running():
+                self.start()
+            else:
+                self.stop()
+        else:
+            self.native.indeterminate = False
+            self.native.maxValue = value
 
     def rehint(self):
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
-        self.interface.intrinsic.height = at_least(self.interface.MIN_HEIGHT)
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = self.native.intrinsicContentSize().height
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/internal/refresh.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/internal/refresh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,107 @@
-from rubicon.objc import *
-
-from toga_cocoa.libs import *
+from toga_cocoa.libs import (
+    SEL,
+    NSClipView,
+    NSEvent,
+    NSEventPhaseEnded,
+    NSLayoutAttributeCenterX,
+    NSLayoutAttributeCenterY,
+    NSLayoutAttributeHeight,
+    NSLayoutAttributeNotAnAttribute,
+    NSLayoutAttributeTop,
+    NSLayoutAttributeWidth,
+    NSLayoutConstraint,
+    NSLayoutRelationEqual,
+    NSMakePoint,
+    NSMakeRect,
+    NSNotificationCenter,
+    NSPoint,
+    NSProgressIndicator,
+    NSProgressIndicatorSpinningStyle,
+    NSRect,
+    NSScrollElasticityAllowed,
+    NSScrollView,
+    NSView,
+    NSViewBoundsDidChangeNotification,
+    ObjCInstance,
+    c_void_p,
+    core_graphics,
+    kCGScrollEventUnitLine,
+    objc_method,
+    objc_property,
+    send_super,
+)
 
 HEADER_HEIGHT = 45.0
 
 
 class RefreshableClipView(NSClipView):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def constrainScrollPoint_(self, proposedNewOrigin: NSPoint) -> NSPoint:
         constrained = send_super(
-            __class__, self, 'constrainScrollPoint:', proposedNewOrigin,
-            restype=NSPoint, argtypes=[NSPoint]
+            __class__,
+            self,
+            "constrainScrollPoint:",
+            proposedNewOrigin,
+            restype=NSPoint,
+            argtypes=[NSPoint],
         )
 
         if self.superview and self.superview.refreshTriggered:
             return NSMakePoint(
                 constrained.x,
-                max(proposedNewOrigin.y, -self.superview.refreshView.frame.size.height)
+                max(proposedNewOrigin.y, -self.superview.refreshView.frame.size.height),
             )
 
         return constrained
 
     @objc_method
-    def isFlipped(self):
-        return True
-
-    @objc_method
     def documentRect(self) -> NSRect:
-        rect = send_super(__class__, self, 'documentRect', restype=NSRect, argtypes=[])
+        rect = send_super(__class__, self, "documentRect", restype=NSRect, argtypes=[])
 
         if self.superview and self.superview.refreshTriggered:
             return NSMakeRect(
-                rect.origin.x, rect.origin.y - self.superview.refreshView.frame.size.height,
-                rect.size.width, rect.size.height + self.superview.refreshView.frame.size.height
+                rect.origin.x,
+                rect.origin.y - self.superview.refreshView.frame.size.height,
+                rect.size.width,
+                rect.size.height + self.superview.refreshView.frame.size.height,
             )
         return rect
 
 
 class RefreshableScrollView(NSScrollView):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     # Create Header View
     @objc_method
     def viewDidMoveToWindow(self) -> None:
         self.refreshTriggered = False
         self.isRefreshing = False
         self.refreshView = None
         self.refreshIndicator = None
         self.createRefreshView()
 
     @objc_method
     def createContentView(self):
-        superClipView = ObjCInstance(send_super(__class__, self, 'contentView'))
+        superClipView = ObjCInstance(send_super(__class__, self, "contentView"))
         if not isinstance(superClipView, RefreshableClipView):
             # create new clipview
             documentView = superClipView.documentView
             clipView = RefreshableClipView.alloc().initWithFrame(superClipView.frame)
 
             clipView.documentView = documentView
             clipView.copiesOnScroll = False
             clipView.drawsBackground = False
 
             self.setContentView(clipView)
-            superClipView = ObjCInstance(send_super(__class__, self, 'contentView'))
+            superClipView = ObjCInstance(send_super(__class__, self, "contentView"))
 
         return superClipView
 
     @objc_method
     def createRefreshView(self) -> None:
         # delete old stuff if any
         if self.refreshView:
@@ -78,124 +115,144 @@
         self.createContentView()
 
         self.contentView.postsFrameChangedNotifications = True
         self.contentView.postsBoundsChangedNotifications = True
 
         NSNotificationCenter.defaultCenter.addObserver(
             self,
-            selector=SEL('viewBoundsChanged:'),
+            selector=SEL("viewBoundsChanged:"),
             name=NSViewBoundsDidChangeNotification,
             object=self.contentView,
         )
 
         # Create view to hold the refresh widgets refreshview
         contentRect = self.contentView.documentView.frame
         self.refreshView = NSView.alloc().init()
         self.refreshView.translatesAutoresizingMaskIntoConstraints = False
 
         # Create spinner
         self.refreshIndicator = NSProgressIndicator.alloc().init()
-        self.refreshIndicator.style = NSProgressIndicatorSpinningStyle;
+        self.refreshIndicator.style = NSProgressIndicatorSpinningStyle
         self.refreshIndicator.translatesAutoresizingMaskIntoConstraints = False
         self.refreshIndicator.displayedWhenStopped = True
         self.refreshIndicator.usesThreadedAnimation = True
         self.refreshIndicator.indeterminate = True
         self.refreshIndicator.bezeled = False
         self.refreshIndicator.sizeToFit()
 
         # Center the spinner in the header
         self.refreshIndicator.setFrame(
             NSMakeRect(
-                self.refreshView.bounds.size.width / 2 - self.refreshIndicator.frame.size.width / 2,
-                self.refreshView.bounds.size.height / 2 - self.refreshIndicator.frame.size.height / 2,
+                self.refreshView.bounds.size.width / 2
+                - self.refreshIndicator.frame.size.width / 2,
+                self.refreshView.bounds.size.height / 2
+                - self.refreshIndicator.frame.size.height / 2,
                 self.refreshIndicator.frame.size.width,
-                self.refreshIndicator.frame.size.height
+                self.refreshIndicator.frame.size.height,
             )
         )
 
         # Put everything in place
         self.refreshView.addSubview(self.refreshIndicator)
         # self.refreshView.addSubview(self.refreshArrow)
         self.contentView.addSubview(self.refreshView)
 
         # set layout constraints
-        indicatorHCenter = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.refreshIndicator, NSLayoutAttributeCenterX,
+        indicatorHCenter = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+            self.refreshIndicator,
+            NSLayoutAttributeCenterX,
             NSLayoutRelationEqual,
-            self.refreshView, NSLayoutAttributeCenterX,
-            1.0, 0,
+            self.refreshView,
+            NSLayoutAttributeCenterX,
+            1.0,
+            0,
         )
         self.refreshView.addConstraint(indicatorHCenter)
 
-        indicatorVCenter = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.refreshIndicator, NSLayoutAttributeCenterY,
+        indicatorVCenter = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+            self.refreshIndicator,
+            NSLayoutAttributeCenterY,
             NSLayoutRelationEqual,
-            self.refreshView, NSLayoutAttributeCenterY,
-            1.0, 0,
+            self.refreshView,
+            NSLayoutAttributeCenterY,
+            1.0,
+            0,
         )
         self.refreshView.addConstraint(indicatorVCenter)
 
-        refreshWidth = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.refreshView, NSLayoutAttributeWidth,
+        refreshWidth = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+            self.refreshView,
+            NSLayoutAttributeWidth,
             NSLayoutRelationEqual,
-            self.contentView, NSLayoutAttributeWidth,
-            1.0, 0,
+            self.contentView,
+            NSLayoutAttributeWidth,
+            1.0,
+            0,
         )
         self.contentView.addConstraint(refreshWidth)
 
-        refreshHeight = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.refreshView, NSLayoutAttributeHeight,
+        refreshHeight = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+            self.refreshView,
+            NSLayoutAttributeHeight,
             NSLayoutRelationEqual,
-            None, NSLayoutAttributeNotAnAttribute,
-            1.0, HEADER_HEIGHT,
+            None,
+            NSLayoutAttributeNotAnAttribute,
+            1.0,
+            HEADER_HEIGHT,
         )
         self.contentView.addConstraint(refreshHeight)
 
-        refreshHeight = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-            self.refreshView, NSLayoutAttributeTop,
+        refreshHeight = NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(  # noqa: E501
+            self.refreshView,
+            NSLayoutAttributeTop,
             NSLayoutRelationEqual,
-            self.contentView, NSLayoutAttributeTop,
-            1.0, -HEADER_HEIGHT,
+            self.contentView,
+            NSLayoutAttributeTop,
+            1.0,
+            -HEADER_HEIGHT,
         )
         self.contentView.addConstraint(refreshHeight)
 
         # Scroll to top
-        self.contentView.scrollToPoint(NSMakePoint(contentRect.origin.x, 0));
+        self.contentView.scrollToPoint(NSMakePoint(contentRect.origin.x, 0))
         self.reflectScrolledClipView(self.contentView)
 
     # Detecting scroll
     @objc_method
     def scrollWheel_(self, event) -> None:
         if event.phase == NSEventPhaseEnded:
             if self.refreshTriggered and not self.isRefreshing:
                 self.reload()
 
-        send_super(__class__, self, 'scrollWheel:', event)
+        send_super(__class__, self, "scrollWheel:", event, argtypes=[c_void_p])
 
     @objc_method
     def viewBoundsChanged_(self, note) -> None:
         if self.isRefreshing:
             return
 
         if self.contentView.bounds.origin.y <= -self.refreshView.frame.size.height:
             self.refreshTriggered = True
 
     # Reload
     @objc_method
     def reload(self) -> None:
-        """Start a reload, starting the reload spinner"""
+        """Start a reload, starting the reload spinner."""
         self.isRefreshing = True
         self.refreshIndicator.startAnimation(self)
         self.interface.on_refresh(self.interface)
 
     @objc_method
     def finishedLoading(self):
-        """Invoke to mark the end of a reload, stopping and hiding the reload spinner"""
+        """Invoke to mark the end of a reload, stopping and hiding the reload
+        spinner."""
         self.isRefreshing = False
         self.refreshTriggered = False
         self.refreshIndicator.stopAnimation(self)
         self.detailedlist.reloadData()
 
         # Force a scroll event to make the scroll hide the reload
-        cgEvent = core_graphics.CGEventCreateScrollWheelEvent(None, kCGScrollEventUnitLine, 2, 1, 0)
+        cgEvent = core_graphics.CGEventCreateScrollWheelEvent(
+            None, kCGScrollEventUnitLine, 2, 1, 0
+        )
         scrollEvent = NSEvent.eventWithCGEvent(cgEvent)
         self.scrollWheel(scrollEvent)
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/switch.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/label.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,42 @@
-from rubicon.objc import objc_method, SEL
 from travertino.size import at_least
 
-from toga_cocoa.libs import *
+from toga_cocoa.colors import native_color
+from toga_cocoa.libs import NSTextAlignment, NSTextField
 
 from .base import Widget
 
 
-class TogaSwitch(NSButton):
-    @objc_method
-    def onPress_(self, obj) -> None:
-        if self.interface.on_toggle:
-            self.interface.on_toggle(self.interface)
-
-
-class Switch(Widget):
+class Label(Widget):
     def create(self):
-        self.native = TogaSwitch.alloc().init()
-        self.native.interface = self.interface
+        self.native = NSTextField.alloc().init()
 
-        self.native.bezelStyle = NSRoundedBezelStyle
-        self.native.setButtonType(NSSwitchButton)
-        self.native.target = self.native
-        self.native.action = SEL('onPress:')
+        self.native.drawsBackground = False
+        self.native.editable = False
+        self.native.bezeled = False
 
         # Add the layout constraints
         self.add_constraints()
 
-    def set_label(self, label):
-        self.native.title = label
+    def set_alignment(self, value):
+        self.native.alignment = NSTextAlignment(value)
+
+    def set_color(self, value):
+        self.native.textColor = native_color(value)
 
-    def set_is_on(self, value):
-        if value is True:
-            self.native.state = NSOnState
-        elif value is False:
-            self.native.state = NSOffState
-
-    def get_is_on(self):
-        is_on = self.native.state
-        if is_on == 1:
-            return True
-        elif is_on == 0:
-            return False
-        else:
-            raise Exception('Undefined value for is_on of {}'.format(__class__))
+    def set_font(self, font):
+        self.native.font = font._impl.native
+
+    def get_text(self):
+        return str(self.native.stringValue)
+
+    def set_text(self, value):
+        self.native.stringValue = value
 
     def rehint(self):
+        # Width & height of a label is known and fixed.
         content_size = self.native.intrinsicContentSize()
+        # print("REHINT label", self, content_size.width, content_size.height)
+        # 2020-05-11 The +1 is a hack; the label "X Translate:" gets truncated
+        # without the extra pixel.
+        self.interface.intrinsic.width = at_least(content_size.width + 1)
         self.interface.intrinsic.height = content_size.height
-        self.interface.intrinsic.width = at_least(content_size.width)
-
-    def set_on_toggle(self, handler):
-        pass
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/button.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/selection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,49 @@
-from rubicon.objc import objc_method, SEL
 from travertino.size import at_least
 
-from toga_cocoa.libs import *
-from toga_cocoa.color import native_color
+from toga_cocoa.libs import SEL, NSPopUpButton, objc_method, objc_property
 
 from .base import Widget
 
 
-class TogaButton(NSButton):
+class TogaPopupButton(NSPopUpButton):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
-    def onPress_(self, obj) -> None:
-        if self.interface.on_press:
-            self.interface.on_press(self.interface)
+    def onSelect_(self, obj) -> None:
+        if self.interface.on_select:
+            self.interface.on_select(self.interface)
 
 
-class Button(Widget):
+class Selection(Widget):
     def create(self):
-        self.native = TogaButton.alloc().init()
+        self.native = TogaPopupButton.alloc().init()
         self.native.interface = self.interface
+        self.native.impl = self
 
-        self.native.bezelStyle = NSRoundedBezelStyle
-        self.native.buttonType = NSMomentaryPushInButton
         self.native.target = self.native
-        self.native.action = SEL('onPress:')
+        self.native.action = SEL("onSelect:")
 
-        # Add the layout constraints
         self.add_constraints()
 
-    def set_font(self, value):
-        if value:
-            self.native.font = value._impl.native
-
-    def set_label(self, label):
-        self.native.title = self.interface.label
-
-    def set_on_press(self, handler):
-        # No special handling required
-        pass
-
     def rehint(self):
         content_size = self.native.intrinsicContentSize()
-        self.interface.intrinsic.width = at_least(content_size.width)
         self.interface.intrinsic.height = content_size.height
+        self.interface.intrinsic.width = at_least(
+            max(self.interface._MIN_WIDTH, content_size.width)
+        )
+
+    def remove_all_items(self):
+        self.native.removeAllItems()
+
+    def add_item(self, item):
+        self.native.addItemWithTitle(item)
+
+    def select_item(self, item):
+        self.native.selectItemWithTitle(item)
+
+    def get_selected_item(self):
+        return str(self.native.titleOfSelectedItem)
+
+    def set_on_select(self, handler):
+        pass
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/label.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/switch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,61 @@
 from travertino.size import at_least
 
-from toga_cocoa.color import native_color
-from toga_cocoa.libs import NSTextField, NSTextAlignment
+from toga_cocoa.libs import (
+    SEL,
+    NSBezelStyle,
+    NSButton,
+    NSOffState,
+    NSOnState,
+    NSSwitchButton,
+    objc_method,
+    objc_property,
+)
 
 from .base import Widget
 
 
-class Label(Widget):
+class TogaSwitch(NSButton):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
+    @objc_method
+    def onPress_(self, obj) -> None:
+        self.interface.on_change(None)
+
+
+class Switch(Widget):
     def create(self):
-        self.native = NSTextField.alloc().init()
-        self.native.impl = self
+        self.native = TogaSwitch.alloc().init()
         self.native.interface = self.interface
+        self.native.impl = self
 
-        self.native.drawsBackground = False
-        self.native.editable = False
-        self.native.bezeled = False
+        self.native.bezelStyle = NSBezelStyle.Rounded
+        self.native.setButtonType(NSSwitchButton)
+        self.native.target = self.native
+        self.native.action = SEL("onPress:")
 
         # Add the layout constraints
         self.add_constraints()
 
-    def set_alignment(self, value):
-        self.native.alignment = NSTextAlignment(value)
+    def get_text(self):
+        return str(self.native.title)
+
+    def set_text(self, text):
+        self.native.title = text
 
-    def set_color(self, value):
-        if value:
-            self.native.textColor = native_color(value)
-
-    def set_font(self, value):
-        if value:
-            self.native.font = value._impl.native
+    def set_font(self, font):
+        self.native.font = font._impl.native
 
-    def set_text(self, value):
-        self.native.stringValue = self.interface._text
+    def get_value(self):
+        return self.native.state == NSOnState
+
+    def set_value(self, value):
+        old_value = self.native.state == NSOnState
+        self.native.state = NSOnState if value else NSOffState
+        if self.interface.on_change and value != old_value:
+            self.interface.on_change(self.interface)
 
     def rehint(self):
-        # Width & height of a label is known and fixed.
         content_size = self.native.intrinsicContentSize()
-        # print("REHINT label", self, content_size.width, content_size.height)
         self.interface.intrinsic.width = at_least(content_size.width)
         self.interface.intrinsic.height = content_size.height
```

### Comparing `toga-cocoa-0.3.0.dev9/toga_cocoa/widgets/numberinput.py` & `toga-cocoa-0.3.1/src/toga_cocoa/widgets/numberinput.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,169 @@
 import sys
-from decimal import Decimal
+from decimal import Decimal, InvalidOperation
 
-from rubicon.objc import objc_method, SEL
 from travertino.size import at_least
 
-import toga
+from toga_cocoa.colors import native_color
 from toga_cocoa.libs import (
-    NSTextAlignment, NSTextFieldSquareBezel, NSTextField, NSStepper,
-    NSLayoutAttributeTop, NSLayoutAttributeBottom,
-    NSLayoutAttributeLeft, NSLayoutAttributeRight,
-    NSLayoutAttributeCenterY, NSLayoutRelationEqual, NSLayoutConstraint
+    SEL,
+    NSLayoutAttributeBottom,
+    NSLayoutAttributeCenterY,
+    NSLayoutAttributeLeft,
+    NSLayoutAttributeRight,
+    NSLayoutAttributeTop,
+    NSLayoutConstraint,
+    NSLayoutRelationEqual,
+    NSStepper,
+    NSTextAlignment,
+    NSTextField,
+    NSTextFieldSquareBezel,
+    objc_method,
+    objc_property,
 )
 
 from .base import Widget
 from .box import TogaView
 
 
 class TogaStepper(NSStepper):
+    interface = objc_property(object, weak=True)
+    impl = objc_property(object, weak=True)
+
     @objc_method
     def onChange_(self, stepper) -> None:
         self.interface.value = Decimal(stepper.floatValue).quantize(self.interface.step)
         if self.interface.on_change:
             self.interface.on_change(self.interface)
 
     @objc_method
     def controlTextDidChange_(self, notification) -> None:
         try:
-            value = Decimal(self._impl.input.stringValue)
+            value = str(self.impl.input.stringValue)
+            # Try to convert to a decimal. If the value isn't a number,
+            # this will raise InvalidOperation
+            Decimal(value)
             # We set the input widget's value to the literal text input
             # This preserves the display of "123.", which Decimal will
             # convert to "123"
-            self.interface.value = self._impl.input.stringValue
+            self.interface.value = value
             if self.interface.on_change:
                 self.interface.on_change(self.interface)
-        except ValueError:
+        except InvalidOperation:
             # If the string value isn't valid, reset the widget
             # to the widget's stored value. This will update the
             # display, removing any invalid values from view.
-            self._impl.set_value(self.interface.value)
+            self.impl.set_value(self.interface.value)
 
 
 class NumberInput(Widget):
     def create(self):
         self.native = TogaView.alloc().init()
 
         self.input = NSTextField.new()
-        self.input.interface = self.interface
         self.input.bezeled = True
         self.input.bezelStyle = NSTextFieldSquareBezel
         self.input.translatesAutoresizingMaskIntoConstraints = False
 
         self.stepper = TogaStepper.alloc().init()
         self.stepper.interface = self.interface
-        self.stepper._impl = self
+        self.stepper.impl = self
         self.stepper.translatesAutoresizingMaskIntoConstraints = False
 
         self.stepper.target = self.stepper
-        self.stepper.action = SEL('onChange:')
+        self.stepper.action = SEL("onChange:")
 
         self.stepper.controller = self.input
         self.input.delegate = self.stepper
 
         # Add the input and stepper to the constraining box.
         self.native.addSubview(self.input)
         self.native.addSubview(self.stepper)
 
         # Add constraints to lay out the input and stepper.
         # Stepper is always top right corner.
         self.native.addConstraint(
             NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-                self.native, NSLayoutAttributeTop,
+                self.native,
+                NSLayoutAttributeTop,
                 NSLayoutRelationEqual,
-                self.stepper, NSLayoutAttributeTop,
-                1.0, 0
+                self.stepper,
+                NSLayoutAttributeTop,
+                1.0,
+                0,
             )
         )
         self.native.addConstraint(
             NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-                self.native, NSLayoutAttributeRight,
+                self.native,
+                NSLayoutAttributeRight,
                 NSLayoutRelationEqual,
-                self.stepper, NSLayoutAttributeRight,
-                1.0, 0
+                self.stepper,
+                NSLayoutAttributeRight,
+                1.0,
+                0,
             )
         )
 
         # Stepper height matches container box height
         self.native.addConstraint(
             NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-                self.native, NSLayoutAttributeBottom,
+                self.native,
+                NSLayoutAttributeBottom,
                 NSLayoutRelationEqual,
-                self.stepper, NSLayoutAttributeBottom,
-                1.0, 0
+                self.stepper,
+                NSLayoutAttributeBottom,
+                1.0,
+                0,
             )
         )
 
         # Input is always left, centred vertically on the stepper
         self.native.addConstraint(
             NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-                self.stepper, NSLayoutAttributeCenterY,
+                self.stepper,
+                NSLayoutAttributeCenterY,
                 NSLayoutRelationEqual,
-                self.input, NSLayoutAttributeCenterY,
-                1.0, 0
+                self.input,
+                NSLayoutAttributeCenterY,
+                1.0,
+                0,
             )
         )
         self.native.addConstraint(
             NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-                self.native, NSLayoutAttributeLeft,
+                self.native,
+                NSLayoutAttributeLeft,
                 NSLayoutRelationEqual,
-                self.input, NSLayoutAttributeLeft,
-                1.0, 0
+                self.input,
+                NSLayoutAttributeLeft,
+                1.0,
+                0,
             )
         )
 
         # Stepper and input meet in the middle with a small gap
         self.native.addConstraint(
             NSLayoutConstraint.constraintWithItem_attribute_relatedBy_toItem_attribute_multiplier_constant_(
-                self.stepper, NSLayoutAttributeLeft,
+                self.stepper,
+                NSLayoutAttributeLeft,
                 NSLayoutRelationEqual,
-                self.input, NSLayoutAttributeRight,
-                1.0, 2
+                self.input,
+                NSLayoutAttributeRight,
+                1.0,
+                2,
             )
         )
 
         # Add the layout constraints for the main box
         self.add_constraints()
 
+    def set_color(self, color):
+        self.input.textColor = native_color(color)
+
     def set_readonly(self, value):
         # Even if it's not editable, it's still selectable.
         self.input.editable = not value
         self.input.selectable = True
 
     def set_placeholder(self, value):
         self.input.cell.placeholderString = value
@@ -147,37 +182,41 @@
             self.stepper.maxValue = sys.maxsize
         else:
             self.stepper.maxValue = value
 
     def set_alignment(self, value):
         self.input.alignment = NSTextAlignment(value)
 
-    def set_font(self, value):
-        if value:
-            self.input.font = value._impl.native
+    def set_font(self, font):
+        if font:
+            self.input.font = font._impl.native
 
     def set_value(self, value):
         if self.interface.value is None:
             self.stepper.floatValue = 0
-            self.input.stringValue = ''
+            self.input.stringValue = ""
         else:
             self.stepper.floatValue = float(self.interface.value)
             # We use the *literal* input value here, not the value
             # stored in the interface, because we want to display
             # what the user has actually input, not the interpreted
             # Decimal value. Any invalid input value should result
             # in the interface to a value of None, so this branch
             # should only execute if we know the raw value can be
             # converted to a Decimal.
             self.input.stringValue = value
 
+    def set_enabled(self, value):
+        self.input.enabled = value
+        self.stepper.enabled = value
+
     def rehint(self):
         # Height of a text input is known and fixed.
         stepper_size = self.input.intrinsicContentSize()
         input_size = self.input.intrinsicContentSize()
 
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
         self.interface.intrinsic.height = max(input_size.height, stepper_size.height)
 
     def set_on_change(self, handler):
         # No special handling required
         pass
```

### Comparing `toga-cocoa-0.3.0.dev9/README.rst` & `toga-cocoa-0.3.1/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -5,36 +5,43 @@
 
 **Toga requires Python 3**
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For more details, see the `Toga project on Github`_.
 
+.. _Toga widget toolkit: http://beeware.org/toga
+.. _the core Toga library: https://pypi.python.org/pypi/toga-core
+.. _Toga project on Github: https://github.com/beeware/toga
+
 Prerequisites
 ~~~~~~~~~~~~~
 
-This backend requires OS X 10.7 (Lion).
+This backend requires OS X 10.10 (Yosemite).
 
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

