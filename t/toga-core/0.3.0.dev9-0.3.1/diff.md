# Comparing `tmp/toga-core-0.3.0.dev9.tar.gz` & `tmp/toga-core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-core-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:18 2018, max compression
+gzip compressed data, was "toga-core-0.3.1.tar", last modified: Wed Apr 12 01:58:30 2023, max compression
```

## Comparing `toga-core-0.3.0.dev9.tar` & `toga-core-0.3.1.tar`

### file list

```diff
@@ -1,113 +1,159 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:18.000000 toga-core-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     6065 2018-07-07 05:55:18.000000 toga-core-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/tests/
--rw-r--r--   0 rkm        (501) staff       (20)     6485 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/test_command.py
--rw-r--r--   0 rkm        (501) staff       (20)      339 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/test_key.py
--rw-r--r--   0 rkm        (501) staff       (20)       66 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/tests/test_handler.py
--rw-r--r--   0 rkm        (501) staff       (20)     1224 2018-05-17 17:50:27.000000 toga-core-0.3.0.dev9/tests/test_font.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/__init__.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/tests/style/
--rw-r--r--   0 rkm        (501) staff       (20)    10105 2018-06-23 02:09:29.000000 toga-core-0.3.0.dev9/tests/style/test_pack.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/tests/style/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     2322 2018-06-10 23:51:35.000000 toga-core-0.3.0.dev9/tests/test_window.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/tests/sources/
--rw-r--r--   0 rkm        (501) staff       (20)    24543 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/tests/sources/test_tree_source.py
--rw-r--r--   0 rkm        (501) staff       (20)     1255 2017-12-22 11:14:30.000000 toga-core-0.3.0.dev9/tests/sources/test_value_source.py
--rw-r--r--   0 rkm        (501) staff       (20)    12242 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/tests/sources/test_list_source.py
--rw-r--r--   0 rkm        (501) staff       (20)     1515 2017-12-23 03:47:49.000000 toga-core-0.3.0.dev9/tests/sources/test_source.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/sources/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     3534 2018-05-14 13:05:36.000000 toga-core-0.3.0.dev9/tests/sources/test_accessors.py
--rw-r--r--   0 rkm        (501) staff       (20)     2338 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/test_app.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/tests/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)     2526 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/widgets/test_slider.py
--rw-r--r--   0 rkm        (501) staff       (20)     1491 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/widgets/test_button.py
--rw-r--r--   0 rkm        (501) staff       (20)      851 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_label.py
--rw-r--r--   0 rkm        (501) staff       (20)     1814 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_scrollcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     1653 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/widgets/test_tree.py
--rw-r--r--   0 rkm        (501) staff       (20)      604 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_icon.py
--rw-r--r--   0 rkm        (501) staff       (20)      863 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_optioncontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     2194 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/widgets/test_table.py
--rw-r--r--   0 rkm        (501) staff       (20)      659 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/widgets/test_navigationview.py
--rw-r--r--   0 rkm        (501) staff       (20)      763 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_box.py
--rw-r--r--   0 rkm        (501) staff       (20)      553 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_image.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     2003 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_selection.py
--rw-r--r--   0 rkm        (501) staff       (20)    20813 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/tests/widgets/test_canvas.py
--rw-r--r--   0 rkm        (501) staff       (20)      803 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/widgets/test_imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)     1844 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     4315 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/widgets/test_progressbar.py
--rw-r--r--   0 rkm        (501) staff       (20)     2124 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/tests/widgets/test_base.py
--rw-r--r--   0 rkm        (501) staff       (20)     1025 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/widgets/test_multilinetextinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     2083 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/widgets/test_webview.py
--rw-r--r--   0 rkm        (501) staff       (20)     2215 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/widgets/test_detailedlist.py
--rw-r--r--   0 rkm        (501) staff       (20)     2374 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/tests/widgets/test_numberinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     1051 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     2150 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/tests/widgets/test_splitcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     1722 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/tests/widgets/test_switch.py
--rw-r--r--   0 rkm        (501) staff       (20)      187 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/MANIFEST.in
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:18.000000 toga-core-0.3.0.dev9/toga_core.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     6065 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga_core.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)        1 2017-04-17 07:59:42.000000 toga-core-0.3.0.dev9/toga_core.egg-info/not-zip-safe
--rw-r--r--   0 rkm        (501) staff       (20)     2558 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga_core.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)       47 2017-03-13 00:57:40.000000 toga-core-0.3.0.dev9/toga_core.egg-info/pbr.json
--rw-r--r--   0 rkm        (501) staff       (20)       18 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga_core.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)       11 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga_core.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga_core.egg-info/dependency_links.txt
--rw-r--r--   0 rkm        (501) staff       (20)     1729 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/setup.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga/hardware/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/hardware/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)       77 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/toga/color.py
--rw-r--r--   0 rkm        (501) staff       (20)     3701 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/command.py
--rw-r--r--   0 rkm        (501) staff       (20)     9650 2018-06-10 23:51:35.000000 toga-core-0.3.0.dev9/toga/window.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga/constants/
--rw-r--r--   0 rkm        (501) staff       (20)    10332 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/constants/key.py
--rw-r--r--   0 rkm        (501) staff       (20)       34 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/toga/constants/__init__.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga/resources/
--rw-r--r--   0 rkm        (501) staff       (20)   396417 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/resources/tiberius.icns
--rw-r--r--   0 rkm        (501) staff       (20)     1970 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/resources/tiberius-32.png
--rw-r--r--   0 rkm        (501) staff       (20)     2339 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/toga/handlers.py
--rw-r--r--   0 rkm        (501) staff       (20)     1958 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     2500 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/keys.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga/style/
--rw-r--r--   0 rkm        (501) staff       (20)    20349 2018-06-24 23:35:08.000000 toga-core-0.3.0.dev9/toga/style/pack.py
--rw-r--r--   0 rkm        (501) staff       (20)       83 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/toga/style/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      978 2018-05-17 17:50:27.000000 toga-core-0.3.0.dev9/toga/style/applicator.py
--rw-r--r--   0 rkm        (501) staff       (20)      874 2018-05-17 17:50:27.000000 toga-core-0.3.0.dev9/toga/font.py
--rw-r--r--   0 rkm        (501) staff       (20)     1431 2018-01-23 22:27:00.000000 toga-core-0.3.0.dev9/toga/platform.py
--rw-r--r--   0 rkm        (501) staff       (20)     6084 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/toga/app.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:17.000000 toga-core-0.3.0.dev9/toga/sources/
--rw-r--r--   0 rkm        (501) staff       (20)     2243 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/sources/accessors.py
--rw-r--r--   0 rkm        (501) staff       (20)     4541 2018-02-21 05:36:56.000000 toga-core-0.3.0.dev9/toga/sources/tree_source.py
--rw-r--r--   0 rkm        (501) staff       (20)     3684 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/toga/sources/list_source.py
--rw-r--r--   0 rkm        (501) staff       (20)      170 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/sources/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      471 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/sources/value_source.py
--rw-r--r--   0 rkm        (501) staff       (20)     1001 2017-12-23 03:47:49.000000 toga-core-0.3.0.dev9/toga/sources/base.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:18.000000 toga-core-0.3.0.dev9/toga/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)     1820 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/widgets/icon.py
--rw-r--r--   0 rkm        (501) staff       (20)     2953 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/toga/widgets/tree.py
--rw-r--r--   0 rkm        (501) staff       (20)     1434 2018-06-10 23:51:35.000000 toga-core-0.3.0.dev9/toga/widgets/imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)      954 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/widgets/box.py
--rw-r--r--   0 rkm        (501) staff       (20)     3165 2017-12-27 05:49:07.000000 toga-core-0.3.0.dev9/toga/widgets/splitcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     4648 2018-05-17 17:50:27.000000 toga-core-0.3.0.dev9/toga/widgets/detailedlist.py
--rw-r--r--   0 rkm        (501) staff       (20)     2258 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/widgets/multilinetextinput.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     3044 2018-01-18 21:56:40.000000 toga-core-0.3.0.dev9/toga/widgets/textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     2396 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/toga/widgets/switch.py
--rw-r--r--   0 rkm        (501) staff       (20)     2753 2018-01-12 22:11:27.000000 toga-core-0.3.0.dev9/toga/widgets/scrollcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     2731 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/toga/widgets/slider.py
--rw-r--r--   0 rkm        (501) staff       (20)     2051 2018-01-12 22:11:27.000000 toga-core-0.3.0.dev9/toga/widgets/button.py
--rw-r--r--   0 rkm        (501) staff       (20)     3031 2018-05-17 17:50:27.000000 toga-core-0.3.0.dev9/toga/widgets/progressbar.py
--rw-r--r--   0 rkm        (501) staff       (20)      524 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/toga/widgets/navigationview.py
--rw-r--r--   0 rkm        (501) staff       (20)     1151 2018-01-18 21:56:40.000000 toga-core-0.3.0.dev9/toga/widgets/label.py
--rw-r--r--   0 rkm        (501) staff       (20)     5190 2018-05-27 12:31:45.000000 toga-core-0.3.0.dev9/toga/widgets/numberinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     2649 2018-05-17 17:50:27.000000 toga-core-0.3.0.dev9/toga/widgets/passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     4973 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/widgets/table.py
--rw-r--r--   0 rkm        (501) staff       (20)     2456 2018-03-19 02:46:43.000000 toga-core-0.3.0.dev9/toga/widgets/selection.py
--rw-r--r--   0 rkm        (501) staff       (20)     2535 2018-05-26 09:29:22.000000 toga-core-0.3.0.dev9/toga/widgets/webview.py
--rw-r--r--   0 rkm        (501) staff       (20)     2531 2017-12-23 03:47:56.000000 toga-core-0.3.0.dev9/toga/widgets/optioncontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      901 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/toga/widgets/image.py
--rw-r--r--   0 rkm        (501) staff       (20)     4208 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/toga/widgets/base.py
--rw-r--r--   0 rkm        (501) staff       (20)    31639 2018-07-07 05:52:00.000000 toga-core-0.3.0.dev9/toga/widgets/canvas.py
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:18.000000 toga-core-0.3.0.dev9/setup.cfg
--rw-r--r--   0 rkm        (501) staff       (20)     4203 2017-12-22 11:14:05.000000 toga-core-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.344973 toga-core-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:57:47.000000 toga-core-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:57:47.000000 toga-core-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 01:57:47.000000 toga-core-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-12 01:58:30.344973 toga-core-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-12 01:57:47.000000 toga-core-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 01:57:47.000000 toga-core-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-12 01:58:30.344973 toga-core-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 01:57:47.000000 toga-core-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.328973 toga-core-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.332973 toga-core-0.3.1/src/toga/
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22599 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.332973 toga-core-0.3.1/src/toga/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.332973 toga-core-0.3.1/src/toga/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.332973 toga-core-0.3.1/src/toga/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   396417 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/resources/toga.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   370070 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/resources/toga.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/resources/toga.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.332973 toga-core-0.3.1/src/toga/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/sources/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/sources/list_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/sources/tree_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/sources/value_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.332973 toga-core-0.3.1/src/toga/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/style/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27344 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/style/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.336973 toga-core-0.3.1/src/toga/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38952 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/datepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/timepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-04-12 01:57:47.000000 toga-core-0.3.1/src/toga/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.336973 toga-core-0.3.1/src/toga_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-12 01:58:30.000000 toga-core-0.3.1/src/toga_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-12 01:58:30.000000 toga-core-0.3.1/src/toga_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:30.000000 toga-core-0.3.1/src/toga_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:57:53.000000 toga-core-0.3.1/src/toga_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 01:58:30.000000 toga-core-0.3.1/src/toga_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 01:58:30.000000 toga-core-0.3.1/src/toga_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/command/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/command/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/command/test_commands_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/command/test_commands_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/sources/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/sources/test_list_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/sources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24013 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/sources/test_tree_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/sources/test_value_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/style/test_applicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61251 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/style/test_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_deprecated_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_font.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/testbed/installed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/installed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/installed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/installed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/testbed/installed.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/installed.dist-info/INSTALLER
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/installed.dist-info/METADATA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/testbed/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/simple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/simple/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/standalone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.340973 toga-core-0.3.1/tests/testbed/subclassed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/subclassed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/subclassed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/testbed/subclassed/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:30.344973 toga-core-0.3.1/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26990 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28790 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_datepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_timepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-12 01:57:47.000000 toga-core-0.3.1/tests/widgets/test_webview.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-core-0.3.0.dev9/tests/test_command.py` & `toga-core-0.3.1/tests/command/test_commands_group.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,183 @@
 import unittest
-from unittest.mock import Mock
+
+from tests.command.constants import PARENT_GROUP1, PARENT_GROUP2
+from tests.utils import order_test
 
 import toga
-import toga_dummy
 
 
-class TestCommand(unittest.TestCase):
+class TestCommandsGroup(unittest.TestCase):
     def test_group_init_no_order(self):
-        grp = toga.Group('label')
-        self.assertEqual(grp.label, 'label')
+        grp = toga.Group("text")
+        self.assertEqual(grp.text, "text")
         self.assertEqual(grp.order, 0)
 
     def test_group_init_with_order(self):
-        grp = toga.Group('label', 2)
-        self.assertEqual(grp.label, 'label')
+        grp = toga.Group("text", 2)
+        self.assertEqual(grp.text, "text")
         self.assertEqual(grp.order, 2)
 
-    def test_group_lt(self):
-        grp1, grp2 = toga.Group('A'), toga.Group('B')
-        self.assertTrue(toga.Group('A', 1) < toga.Group('A', 2))
-        self.assertTrue(toga.Group('A') < toga.Group('B'))
+    def test_hashable(self):
+        grp1 = toga.Group("text 1")
+        grp2 = toga.Group("text 2")
+
+        # The hash is based on the full path, not just the text.
+        # This allows texts to be non-unique, as long as they're in
+        # different groups
+        grp1_child = toga.Group("text", parent=grp1)
+        grp2_child = toga.Group("text", parent=grp2)
+
+        # Insert the groups as keys in a dict. This is
+        # only possible if Group is hashable.
+        groups = {
+            grp1: "First",
+            grp2: "Second",
+            grp1_child: "Child of 1",
+            grp2_child: "Child of 2",
+        }
+
+        self.assertEqual(groups[grp1], "First")
+        self.assertEqual(groups[grp2], "Second")
+        self.assertEqual(groups[grp1_child], "Child of 1")
+        self.assertEqual(groups[grp2_child], "Child of 2")
 
     def test_group_eq(self):
-        self.assertEqual(toga.Group('A'), toga.Group('A'))
-        self.assertEqual(toga.Group('A', 1), toga.Group('A', 1))
-        self.assertNotEqual(toga.Group('A'), toga.Group('B'))
-        self.assertNotEqual(toga.Group('A', 1), toga.Group('A', 2))
-        self.assertNotEqual(toga.Group('A', 1), toga.Group('B', 1))
-
-    def test_command_init_defaults(self):
-        cmd = toga.Command(lambda x: print('Hello World'), 'test', factory=toga_dummy.factory)
-        self.assertEqual(cmd.label, 'test')
-        self.assertEqual(cmd.shortcut, None)
-        self.assertEqual(cmd.tooltip, None)
-        self.assertEqual(cmd.icon_id, None)
-        self.assertEqual(cmd.group, toga.Group.COMMANDS)
-        self.assertEqual(cmd.section, 0)
-        self.assertEqual(cmd.order, 0)
-        self.assertTrue(cmd._enabled)
-        self.assertEqual(cmd._widgets, [])
-
-    def test_command_init_kargs(self):
-        grp = toga.Group('Test group', order=10)
-        cmd = toga.Command(lambda x: print('Hello World'),
-                           label='test',
-                           tooltip='test command',
-                           shortcut='t',
-                           icon='icons/none.png',
-                           group=grp,
-                           section=1,
-                           order=1,
-                           factory=toga_dummy.factory
-                           )
-        self.assertEqual(cmd.label, 'test')
-        self.assertEqual(cmd.shortcut, 't')
-        self.assertEqual(cmd.tooltip, 'test command')
-        self.assertEqual(cmd.icon_id, 'icons/none.png')
-        self.assertEqual(cmd.group, grp)
-        self.assertEqual(cmd.section, 1)
-        self.assertEqual(cmd.order, 1)
-        self.assertTrue(cmd._enabled)
-        self.assertEqual(cmd._widgets, [])
-        self.assertTrue(cmd.enabled)
-        cmd.enabled = False
-        self.assertFalse(cmd._enabled)
-        self.assertFalse(cmd.enabled)
-
-    def test_command_bind(self):
-        grp = toga.Group('Test group', order=10)
-        cmd = toga.Command(lambda x: print('Hello World'),
-                           label='test',
-                           tooltip='test command',
-                           shortcut='t',
-                           icon='icons/none.png',
-                           group=grp,
-                           section=1,
-                           order=1,
-                           factory=toga_dummy.factory
-                           )
-        retur_val = cmd.bind(factory=toga_dummy.factory)
-        self.assertEqual(retur_val, cmd._impl)
-
-    def test_command_enabler(self):
-        test_widget = toga.Widget(factory=toga_dummy.factory)
-        grp = toga.Group('Test group', order=10)
-        cmd = toga.Command(
-                           lambda x: print('Hello World'),
-                           label='test',
-                           tooltip='test command',
-                           shortcut='t',
-                           icon='icons/none.png',
-                           group=grp,
-                           section=1,
-                           order=1,
-                           factory=toga_dummy.factory
-                           )
-        cmd._widgets.append(test_widget)
-        cmd._widgets[0]._impl = Mock()
-        cmd.enabled = False
-        self.assertEqual(cmd._enabled,False)
-
-        for widget in cmd._widgets:
-          self.assertEqual(widget.enabled, False)        
-
-    def test_cmd_sort_key(self):
-        grp = toga.Group('Test group', order=10)
-        cmd = toga.Command(lambda x: print('Hello World'),
-                           label='test',
-                           tooltip='test command',
-                           shortcut='t',
-                           icon='icons/none.png',
-                           group=grp,
-                           section=1,
-                           order=1,
-                           factory=toga_dummy.factory
-                           )
-        self.assertEqual(toga.cmd_sort_key(cmd), (grp, 1, 1, 'test'))
-
-class TestCommandSet(unittest.TestCase):
-    changed = False
-
-    def _changed(self):
-        self.changed = True
-
-    def test_cmdset_init(self):
-        test_widget = toga.Widget(factory=toga_dummy.factory)
-        cs = toga.CommandSet(test_widget)
-        self.assertEqual(cs.widget, test_widget)
-        self.assertEqual(cs._values, set())
-        self.assertEqual(cs.on_change, None)
-
-    def test_cmdset_add(self):
-        self.changed = False
-        test_widget = toga.Widget(factory=toga_dummy.factory)
-        cs = toga.CommandSet(test_widget, on_change=self._changed)
-        grp = toga.Group('Test group', order=10)
-        cmd = toga.Command(lambda x: print('Hello World'),
-                           label='test',
-                           tooltip='test command',
-                           shortcut='t',
-                           icon='icons/none.png',
-                           group=grp,
-                           section=1,
-                           order=1,
-                           factory=toga_dummy.factory
-                           )
-        cs.add(cmd)
-        self.assertTrue(self.changed)
-
-    def test_cmdset_iter(self):
-        test_widget = toga.Widget(factory=toga_dummy.factory)
-        cs = toga.CommandSet(test_widget)
-        grp = toga.Group('Test group', order=10)
-        cmd = toga.Command(lambda x: print('Hello World'),
-                           label='test',
-                           tooltip='test command',
-                           shortcut='t',
-                           icon='icons/none.png',
-                           group=grp,
-                           section=1,
-                           order=1,
-                           factory=toga_dummy.factory
-                           )
-        cs.add(cmd)
-        self.assertEqual(list(cs), [cmd])
+        self.assertEqual(toga.Group("A"), toga.Group("A"))
+        self.assertEqual(toga.Group("A", 1), toga.Group("A", 1))
+        self.assertNotEqual(toga.Group("A"), toga.Group("B"))
+        self.assertNotEqual(toga.Group("A"), None)
+        self.assertNotEqual(toga.Group("A", 1), toga.Group("A", 2))
+        self.assertNotEqual(toga.Group("A", 1), toga.Group("B", 1))
+
+    def test_set_parent_in_constructor(self):
+        parent = toga.Group("parent")
+        child = toga.Group("child", parent=parent)
+        self.assert_parent_and_root(parent, None, parent)
+        self.assert_parent_and_root(child, parent, parent)
+
+    def test_set_parent_in_property(self):
+        parent = toga.Group("parent")
+        child = toga.Group("child")
+        child.parent = parent
+        self.assert_parent_and_root(parent, None, parent)
+        self.assert_parent_and_root(child, parent, parent)
+
+    def test_change_parent(self):
+        parent1 = toga.Group("parent1")
+        parent2 = toga.Group("parent2")
+        child = toga.Group("child", parent=parent1)
+        child.parent = parent2
+        self.assert_parent_and_root(parent1, None, parent1)
+        self.assert_parent_and_root(parent2, None, parent2)
+        self.assert_parent_and_root(child, parent2, parent2)
+
+    def test_is_parent_and_is_child_of(self):
+        top = toga.Group("C")
+        middle = toga.Group("B", parent=top)
+        bottom = toga.Group("A", parent=middle)
+        groups = [top, middle, bottom]
+        for i in range(0, 2):
+            for j in range(i + 1, 3):
+                self.assertTrue(groups[i].is_parent_of(groups[j]))
+                self.assertTrue(groups[j].is_child_of(groups[i]))
+
+    def test_is_parent_of_none(self):
+        group = toga.Group("A")
+        self.assertFalse(group.is_parent_of(None))
+
+    def test_root(self):
+        top = toga.Group("C")
+        middle = toga.Group("B", parent=top)
+        bottom = toga.Group("A", parent=middle)
+        self.assertEqual(top.root, top)
+        self.assertEqual(middle.root, top)
+        self.assertEqual(top.root, top)
+        self.assertEqual(bottom.root, top)
+
+    test_order_by_number = order_test(toga.Group("A", 1), toga.Group("A", 2))
+    test_order_ignore_text = order_test(toga.Group("B", 1), toga.Group("A", 2))
+    test_order_by_text = order_test(toga.Group("A"), toga.Group("B"))
+    test_order_by_groups = order_test(
+        PARENT_GROUP1,
+        toga.Group("C", parent=PARENT_GROUP1),
+        toga.Group("D", parent=PARENT_GROUP1),
+        toga.Group("A", parent=PARENT_GROUP1, section=2),
+        PARENT_GROUP2,
+        toga.Group("B", parent=PARENT_GROUP2),
+    )
+
+    def test_group_repr(self):
+        parent = toga.Group("P")
+        self.assertEqual(repr(toga.Group("A")), "<Group text=A order=0 parent=None>")
+        self.assertEqual(
+            repr(toga.Group("A", parent=parent)), "<Group text=A order=0 parent=P>"
+        )
+
+    def test_set_section_without_parent(self):
+        with self.assertRaises(ValueError):
+            toga.Group("A", section=2)
+
+    def test_set_parent_causes_cyclic_parenting(self):
+        parent = toga.Group("P")
+        child = toga.Group("C", parent=parent)
+        with self.assertRaises(ValueError):
+            parent.parent = child
+        self.assert_parent_and_root(parent, None, parent)
+        self.assert_parent_and_root(child, parent, parent)
+
+    def test_cannot_set_self_as_parent(self):
+        group = toga.Group("P")
+        with self.assertRaises(ValueError):
+            group.parent = group
+        self.assert_parent_and_root(group, None, group)
+
+    def test_cannot_set_child_to_be_a_parent_of_its_grandparent(self):
+        grandparent = toga.Group("G")
+        parent = toga.Group("P", parent=grandparent)
+        child = toga.Group("C", parent=parent)
+        with self.assertRaises(ValueError):
+            grandparent.parent = child
+        self.assert_parent_and_root(grandparent, None, grandparent)
+        self.assert_parent_and_root(parent, grandparent, grandparent)
+        self.assert_parent_and_root(child, parent, grandparent)
+
+    def assert_parent_and_root(self, group, parent, root):
+        self.assertEqual(group.parent, parent)
+        self.assertEqual(group.root, root)
+
+    def test_missing_argument(self):
+        "If the no text is provided for the group, an error is raised"
+        # This test is only required as part of the backwards compatibility
+        # path renaming label->text; when that shim is removed, this teset
+        # validates default Python behavior
+        with self.assertRaises(TypeError):
+            toga.Group()
+
+    ######################################################################
+    # 2022-07: Backwards compatibility
+    ######################################################################
+
+    def test_label_deprecated(self):
+        grp = toga.Group(label="text")
+        new_text = "New Text"
+        with self.assertWarns(DeprecationWarning):
+            grp.label = new_text
+        with self.assertWarns(DeprecationWarning):
+            self.assertEqual(grp.label, new_text)
+        self.assertEqual(grp.text, new_text)
+
+    def test_init_with_deprecated(self):
+        # label is a deprecated argument
+        with self.assertWarns(DeprecationWarning):
+            toga.Group(label="test")
+
+        # can't specify both label *and* text
+        with self.assertRaises(ValueError):
+            toga.Group(
+                label="test",
+                text="test",
+            )
+
+    ######################################################################
+    # End backwards compatibility.
+    ######################################################################
```

### Comparing `toga-core-0.3.0.dev9/tests/test_font.py` & `toga-core-0.3.1/tests/test_font.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 import toga
-from toga.font import Font, SANS_SERIF, ITALIC, SMALL_CAPS, BOLD
-
-import toga_dummy
+from toga.fonts import (
+    _REGISTERED_FONT_CACHE,
+    BOLD,
+    ITALIC,
+    NORMAL,
+    SANS_SERIF,
+    SMALL_CAPS,
+)
 from toga_dummy.utils import TestCase
 
 
 class FontTests(TestCase):
     def setUp(self):
         super().setUp()
 
         self.family = SANS_SERIF
         self.size = 14
         self.style = ITALIC
         self.variant = SMALL_CAPS
         self.weight = BOLD
+        self.custom_family = "customFamily"
+        self.custom_path = "resource/custom-font.otf"
 
         self.font = toga.Font(
             family=self.family,
             size=self.size,
             style=self.style,
             variant=self.variant,
-            weight=self.weight)
+            weight=self.weight,
+        )
+
+        # Bind is a no-op
+        with self.assertWarns(DeprecationWarning):
+            impl = self.font.bind()
 
-        # Bind the font to the dummy factory
-        self.font.bind(toga_dummy.factory)
+        self.assertIsNotNone(impl)
+
+        # Register a file-based custom font
+        toga.Font.register(self.custom_family, self.custom_path)
 
     def test_family(self):
         self.assertEqual(self.font.family, self.family)
 
     def test_size(self):
         self.assertEqual(self.font.size, self.size)
 
@@ -36,10 +50,14 @@
 
     def test_variant(self):
         self.assertEqual(self.font.variant, self.variant)
 
     def test_weight(self):
         self.assertEqual(self.font.weight, self.weight)
 
-    def test_measure(self):
-        self.font.measure('measured text', tight=True)
-        self.assertActionPerformedWith(self.font, 'measure', text='measured text', tight=True)
+    def test_register(self):
+        font_key = toga.Font.registered_font_key(
+            self.custom_family, NORMAL, NORMAL, NORMAL
+        )
+
+        self.assertIn(font_key, _REGISTERED_FONT_CACHE)
+        self.assertEqual(self.custom_path, _REGISTERED_FONT_CACHE[font_key])
```

### Comparing `toga-core-0.3.0.dev9/tests/sources/test_tree_source.py` & `toga-core-0.3.1/tests/sources/test_tree_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from toga.sources import TreeSource
 from toga.sources.tree_source import Node
 
 
 class LeafNodeTests(TestCase):
     def setUp(self):
         self.source = Mock()
-        self.example = Node(val1='value 1', val2=42)
+        self.example = Node(val1="value 1", val2=42)
         self.example._source = self.source
 
     def test_initial_state(self):
         "A node holds values as expected"
-        self.assertEqual(self.example.val1, 'value 1')
+        self.assertEqual(self.example.val1, "value 1")
         self.assertEqual(self.example.val2, 42)
         self.assertFalse(self.example.can_have_children())
         self.assertEqual(len(self.example), 0)
 
     def test_change_value(self):
         "If a node value changes, the source is notified"
-        self.example.val1 = 'new value'
+        self.example.val1 = "new value"
 
-        self.assertEqual(self.example.val1, 'new value')
-        self.source._notify.assert_called_once_with('change', item=self.example)
+        self.assertEqual(self.example.val1, "new value")
+        self.source._notify.assert_called_once_with("change", item=self.example)
 
     def test_iterate_children(self):
         "Children of a node can be iterated over -- should have no children"
         result = 0
 
         for child in self.example:
             result += child.val2
@@ -38,78 +38,85 @@
 class NodeTests(TestCase):
     def setUp(self):
         self.source = Mock()
 
         def bound_create_node(s):
             def create_node(value):
                 return Node(source=s, **value)
+
             return create_node
 
         self.source._create_node = bound_create_node(self.source)
 
-        self.parent = Node(val1='value 1', val2=42)
+        self.parent = Node(val1="value 1", val2=42)
         self.parent._source = self.source
         self.parent._children = []
-        for datum in [{'val1': 'child 1', 'val2': 11}, {'val1': 'child 2', 'val2': 22}]:
+        for datum in [{"val1": "child 1", "val2": 11}, {"val1": "child 2", "val2": 22}]:
             child = Node(**datum)
             child.source = self.source
             self.parent._children.append(child)
 
     def test_initial_state(self):
         "A node holds values as expected"
 
-        self.assertEqual(self.parent.val1, 'value 1')
+        self.assertEqual(self.parent.val1, "value 1")
         self.assertEqual(self.parent.val2, 42)
         self.assertTrue(self.parent.can_have_children())
         self.assertEqual(len(self.parent), 2)
 
     def test_change_value(self):
         "If a node value changes, the source is notified"
-        self.parent.val1 = 'new value'
+        self.parent.val1 = "new value"
 
-        self.assertEqual(self.parent.val1, 'new value')
-        self.source._notify.assert_called_once_with('change', item=self.parent)
+        self.assertEqual(self.parent.val1, "new value")
+        self.source._notify.assert_called_once_with("change", item=self.parent)
 
     def test_empty_children(self):
         "A parent with 0 children isn't the same as a parent who *can't* have children"
-        parent = Node(source=self.source, val1='value 1', val2=42)
+        parent = Node(source=self.source, val1="value 1", val2=42)
         parent._children = []
 
         self.assertTrue(parent.can_have_children())
         self.assertEqual(len(parent), 0)
 
     def test_change_child(self):
         "Changing a child notifies the source"
         # Check initial value
         self.assertEqual(len(self.parent), 2)
-        self.assertEqual(self.parent[1].val1, 'child 2')
+        self.assertEqual(self.parent[1].val1, "child 2")
         self.assertEqual(self.parent[1].val2, 22)
 
         # Change the value
-        self.parent[1] = {'val1': 'new child', 'val2': 33}
+        self.parent[1] = {"val1": "new child", "val2": 33}
 
         # Check the values after modification
         self.assertEqual(len(self.parent), 2)
-        self.assertEqual(self.parent[1].val1, 'new child')
+        self.assertEqual(self.parent[1].val1, "new child")
         self.assertEqual(self.parent[1].val2, 33)
 
     def test_insert_child(self):
         "A new child can be inserted; defers to the source"
-        self.parent.insert(1, val1='inserted 1', val2=33)
-        self.source.insert.assert_called_once_with(self.parent, 1, val1='inserted 1', val2=33)
+        self.parent.insert(1, val1="inserted 1", val2=33)
+        self.source.insert.assert_called_once_with(
+            self.parent, 1, val1="inserted 1", val2=33
+        )
 
     def test_append_child(self):
         "A new child can be appended; defers to the source"
-        self.parent.append(val1='appended 1', val2=33)
-        self.source.append.assert_called_once_with(self.parent, val1='appended 1', val2=33)
+        self.parent.append(val1="appended 1", val2=33)
+        self.source.append.assert_called_once_with(
+            self.parent, val1="appended 1", val2=33
+        )
 
     def test_prepend_child(self):
         "A new child can be prepended; defers to the source"
-        self.parent.prepend(val1='prepended 1', val2=33)
-        self.source.prepend.assert_called_once_with(self.parent, val1='prepended 1', val2=33)
+        self.parent.prepend(val1="prepended 1", val2=33)
+        self.source.prepend.assert_called_once_with(
+            self.parent, val1="prepended 1", val2=33
+        )
 
     def test_remove_child(self):
         "A child can be removed; defers to the source"
         child = self.parent[1]
         self.parent.remove(child)
         self.source.remove.assert_called_once_with(self.parent, child)
 
@@ -124,644 +131,605 @@
 
 
 class TreeSourceTests(TestCase):
     def test_init_with_list_of_tuples(self):
         "TreeSources can be instantiated from lists of tuples"
         source = TreeSource(
             data=[
-                ('first', 111),
-                ('second', 222),
-                ('third', 333),
+                ("first", 111),
+                ("second", 222),
+                ("third", 333),
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
         self.assertFalse(source[0].can_have_children())
         self.assertEqual(len(source[0]), 0)
 
-        self.assertEqual(source[1].val1, 'second')
+        self.assertEqual(source[1].val1, "second")
         self.assertEqual(source[1].val2, 222)
         self.assertFalse(source[1].can_have_children())
         self.assertEqual(len(source[1]), 0)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Set element 1
-        source[1] = ('new element', 999)
+        source[1] = ("new element", 999)
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[1].val1, 'new element')
+        self.assertEqual(source[1].val1, "new element")
         self.assertEqual(source[1].val2, 999)
         self.assertFalse(source[1].can_have_children())
         self.assertEqual(len(source[1]), 0)
 
         listener.change.assert_called_once_with(item=source[1])
 
     def test_init_with_list_of_dicts(self):
         "TreeSource nodes can be instantiated from lists of dicts"
         source = TreeSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
         self.assertFalse(source[0].can_have_children())
         self.assertEqual(len(source[0]), 0)
 
-        self.assertEqual(source[1].val1, 'second')
+        self.assertEqual(source[1].val1, "second")
         self.assertEqual(source[1].val2, 222)
         self.assertFalse(source[1].can_have_children())
         self.assertEqual(len(source[1]), 0)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Set element 1
-        source[1] = {'val1': 'new element', 'val2': 999}
+        source[1] = {"val1": "new element", "val2": 999}
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[1].val1, 'new element')
+        self.assertEqual(source[1].val1, "new element")
         self.assertEqual(source[1].val2, 999)
         self.assertFalse(source[1].can_have_children())
         self.assertEqual(len(source[1]), 0)
 
         listener.change.assert_called_once_with(item=source[1])
 
     def test_init_with_dict_of_lists(self):
         "TreeSource nodes can be instantiated from dicts of lists"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    {'val1': 'third.two', 'val2': 332}
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [
+                    ("third.one", 331),
+                    {"val1": "third.two", "val2": 332},
+                ],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
         self.assertFalse(source[0].can_have_children())
         self.assertEqual(len(source[0]), 0)
 
-        self.assertEqual(source[1].val1, 'second')
+        self.assertEqual(source[1].val1, "second")
         self.assertEqual(source[1].val2, 222)
         self.assertTrue(source[1].can_have_children())
         self.assertEqual(len(source[1]), 0)
 
-        self.assertEqual(source[2].val1, 'third')
+        self.assertEqual(source[2].val1, "third")
         self.assertEqual(source[2].val2, 333)
         self.assertTrue(source[2].can_have_children())
         self.assertEqual(len(source[2]), 2)
 
-        self.assertEqual(source[2].val1, 'third')
+        self.assertEqual(source[2].val1, "third")
         self.assertEqual(source[2].val2, 333)
         self.assertTrue(source[2].can_have_children())
         self.assertEqual(len(source[2]), 2)
 
-        self.assertEqual(source[2][0].val1, 'third.one')
+        self.assertEqual(source[2][0].val1, "third.one")
         self.assertEqual(source[2][0].val2, 331)
         self.assertFalse(source[2][0].can_have_children())
         self.assertEqual(len(source[2][0]), 0)
 
-        self.assertEqual(source[2][1].val1, 'third.two')
+        self.assertEqual(source[2][1].val1, "third.two")
         self.assertEqual(source[2][1].val2, 332)
         self.assertFalse(source[2][1].can_have_children())
         self.assertEqual(len(source[2][1]), 0)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Set element 2
-        source[2] = {'val1': 'new element', 'val2': 999}
+        source[2] = {"val1": "new element", "val2": 999}
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[2].val1, 'new element')
+        self.assertEqual(source[2].val1, "new element")
         self.assertEqual(source[2].val2, 999)
 
         listener.change.assert_called_once_with(item=source[2])
 
     def test_init_with_dict_of_dicts(self):
         "TreeSource nodes can be instantiated from dicts of dicts"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): {
-                    ('third.one', 331): None,
-                    ('third.two', 332): [
-                        ('third.two.sub', 321)
-                    ]
-                }
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): {
+                    ("third.one", 331): None,
+                    ("third.two", 332): [("third.two.sub", 321)],
+                },
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
         self.assertFalse(source[0].can_have_children())
         self.assertEqual(len(source[0]), 0)
 
-        self.assertEqual(source[1].val1, 'second')
+        self.assertEqual(source[1].val1, "second")
         self.assertEqual(source[1].val2, 222)
         self.assertTrue(source[1].can_have_children())
         self.assertEqual(len(source[1]), 0)
 
-        self.assertEqual(source[2].val1, 'third')
+        self.assertEqual(source[2].val1, "third")
         self.assertEqual(source[2].val2, 333)
         self.assertTrue(source[2].can_have_children())
         self.assertEqual(len(source[2]), 2)
 
-        self.assertEqual(source[2].val1, 'third')
+        self.assertEqual(source[2].val1, "third")
         self.assertEqual(source[2].val2, 333)
         self.assertTrue(source[2].can_have_children())
         self.assertEqual(len(source[2]), 2)
 
-        self.assertEqual(source[2][0].val1, 'third.one')
+        self.assertEqual(source[2][0].val1, "third.one")
         self.assertEqual(source[2][0].val2, 331)
         self.assertFalse(source[2][0].can_have_children())
         self.assertEqual(len(source[2][0]), 0)
 
-        self.assertEqual(source[2][1].val1, 'third.two')
+        self.assertEqual(source[2][1].val1, "third.two")
         self.assertEqual(source[2][1].val2, 332)
         self.assertTrue(source[2][1].can_have_children())
         self.assertEqual(len(source[2][1]), 1)
 
-        self.assertEqual(source[2][1][0].val1, 'third.two.sub')
+        self.assertEqual(source[2][1][0].val1, "third.two.sub")
         self.assertEqual(source[2][1][0].val2, 321)
         self.assertFalse(source[2][1][0].can_have_children())
         self.assertEqual(len(source[2][1][0]), 0)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Set element 2
-        source[2] = {'val1': 'new element', 'val2': 999}
+        source[2] = {"val1": "new element", "val2": 999}
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[2].val1, 'new element')
+        self.assertEqual(source[2].val1, "new element")
         self.assertEqual(source[2].val2, 999)
 
         listener.change.assert_called_once_with(item=source[2])
 
     def test_iter(self):
         "TreeSource roots can be iterated over"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         result = 0
         for root in source:
             result += root.val2
 
         self.assertEqual(result, 666)
 
     def test_insert_root_args(self):
         "A new root can be inserted using value args"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.insert(None, 1, 'new element', 999)
+        node = source.insert(None, 1, "new element", 999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[1], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=None, index=1, item=node)
 
     def test_insert_root_kwargs(self):
         "A new root can be inserted using kwargs"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.insert(None, 1, val1='new element', val2=999)
+        node = source.insert(None, 1, val1="new element", val2=999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[1], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=None, index=1, item=node)
 
     def test_insert_child_args(self):
         "A new child can be inserted using value args"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.insert(source[2], 1, val1='new element', val2=999)
+        node = source.insert(source[2], 1, val1="new element", val2=999)
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 3)
         self.assertEqual(source[2][1], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=source[2], index=1, item=node)
 
     def test_insert_child_kwargs(self):
         "A new child can be inserted using kwargs"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.insert(source[2], 1, val1='new element', val2=999)
+        node = source.insert(source[2], 1, val1="new element", val2=999)
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 3)
         self.assertEqual(source[2][1], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=source[2], index=1, item=node)
 
     def test_insert_first_child(self):
         "If a node previously didn't allow children, inserting changes this"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertFalse(source[0].can_have_children())
         self.assertEqual(len(source[0]), 0)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.insert(source[0], 0, val1='new element', val2=999)
+        node = source.insert(source[0], 0, val1="new element", val2=999)
 
         self.assertEqual(len(source), 3)
         self.assertTrue(source[0].can_have_children())
         self.assertEqual(len(source[0]), 1)
         self.assertEqual(source[0][0], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=source[0], index=0, item=node)
 
     def test_append_root(self):
         "A new root can be appended"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.append(None, val1='new element', val2=999)
+        node = source.append(None, val1="new element", val2=999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[3], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=None, index=3, item=node)
 
     def test_append_child(self):
         "A new child can be appended"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.append(source[2], val1='new element', val2=999)
+        node = source.append(source[2], val1="new element", val2=999)
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 3)
         self.assertEqual(source[2][2], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=source[2], index=2, item=node)
 
     def test_prepend_root(self):
         "A new root can be prepended"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.prepend(None, val1='new element', val2=999)
+        node = source.prepend(None, val1="new element", val2=999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[0], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=None, index=0, item=node)
 
     def test_prepend_child(self):
         "A new child can be prepended"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        node = source.prepend(source[2], val1='new element', val2=999)
+        node = source.prepend(source[2], val1="new element", val2=999)
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 3)
         self.assertEqual(source[2][0], node)
-        self.assertEqual(node.val1, 'new element')
+        self.assertEqual(node.val1, "new element")
         self.assertEqual(node.val2, 999)
 
         listener.insert.assert_called_once_with(parent=source[2], index=0, item=node)
 
     def test_remove_root(self):
         "A root can be removed"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Remove the root element
         node = source.remove(source[1])
 
         self.assertEqual(len(source), 2)
         self.assertEqual(len(source[1]), 2)
 
-        listener.remove.assert_called_once_with(item=node)
+        listener.remove.assert_called_once_with(item=node, index=1, parent=None)
 
     def test_remove_child(self):
         "A child can be removed"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
-        # Remove the child element
+        # Remove "third.two"
         node = source.remove(source[2][1])
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 1)
 
-        listener.remove.assert_called_once_with(item=node)
+        listener.remove.assert_called_once_with(item=node, index=1, parent=source[2])
+
+        # Remove "third.one"
+        node = source.remove(source[2][0])
+
+        self.assertEqual(len(source), 3)
+        self.assertEqual(len(source[2]), 0)
+
+        listener.remove.assert_any_call(item=node, index=0, parent=source[2])
 
     def test___setitem___for_root(self):
         "A root can be set (changed) with __setitem__"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Re-assign the first root
-        source[0] = ('first_new', -111)
+        source[0] = ("first_new", -111)
 
         self.assertEqual(len(source), 3)
-        self.assertEqual(source[0].val1, 'first_new')
+        self.assertEqual(source[0].val1, "first_new")
         self.assertEqual(source[0].val2, -111)
 
         listener.change.assert_called_once_with(item=source[0])
 
     def test___setitem___for_child(self):
         "A child can be set (changed) with __setitem__"
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
         self.assertEqual(len(source[2]), 2)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Re-assign the first root
-        source[2][0] = ('third.one_new', -331)
+        source[2][0] = ("third.one_new", -331)
 
         self.assertEqual(len(source), 3)
-        self.assertEqual(source[2][0].val1, 'third.one_new')
+        self.assertEqual(source[2][0].val1, "third.one_new")
         self.assertEqual(source[2][0].val2, -331)
 
         listener.change.assert_called_once_with(item=source[2][0])
 
     def test_get_node_index(self):
         "You can get the index of any node within a tree source, relative to its parent"
 
         source = TreeSource(
             data={
-                ('first', 111): None,
-                ('second', 222): [],
-                ('third', 333): [
-                    ('third.one', 331),
-                    ('third.two', 332)
-                ]
+                ("first", 111): None,
+                ("second", 222): [],
+                ("third", 333): [("third.one", 331), ("third.two", 332)],
             },
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         for i, node in enumerate(source):
             self.assertEqual(i, source.index(node))
 
         # Test indices on deep nodes, too
         third = source[2]
         for i, node in enumerate(third):
             self.assertEqual(i, source.index(node))
 
         # look-alike nodes are not equal, so index lookup should fail
         with self.assertRaises(ValueError):
-            lookalike_node = Node(val1='second', val2=222)
+            lookalike_node = Node(val1="second", val2=222)
             source.index(lookalike_node)
 
         # Describe how edge cases are handled
 
         with self.assertRaises(AttributeError):
             source.index(None)
```

### Comparing `toga-core-0.3.0.dev9/tests/sources/test_value_source.py` & `toga-core-0.3.1/tests/sources/test_value_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 
 from toga.sources.value_source import ValueSource
 
 
 class ValueTests(TestCase):
     def setUp(self):
         self.source = Mock()
-        self.example = ValueSource('label')
+        self.example = ValueSource("label")
         self.example._source = self.source
 
     def test_initial_state(self):
         "A test value holds data as expected"
         # Value is rendered as-is
-        self.assertEqual(self.example.value, 'label')
+        self.assertEqual(self.example.value, "label")
 
         # Object string rendering is the same as 'value'
-        self.assertEqual(str(self.example), 'label')
+        self.assertEqual(str(self.example), "label")
 
     def test_set_value(self):
-        "If the value is modified, internal representation is updated, and notifications are propegated"
+        "If the value is modified, internal representation is updated, and notifications are propagated"
         self.example.value = 42
 
         self.assertEqual(self.example.value, 42)
-        self.assertEqual(str(self.example), '42')
-        self.source._notify.assert_called_once_with('change', item=self.example)
+        self.assertEqual(str(self.example), "42")
+        self.source._notify.assert_called_once_with("change", item=self.example)
 
     def test_clear_value(self):
-        "If the value is cleared, internal representation is updated, and notifications are propegated"
+        "If the value is cleared, internal representation is updated, and notifications are propagated"
         self.example.value = None
 
         self.assertIsNone(self.example.value)
-        self.assertEqual(str(self.example), '')
-        self.source._notify.assert_called_once_with('change', item=self.example)
+        self.assertEqual(str(self.example), "")
+        self.source._notify.assert_called_once_with("change", item=self.example)
```

### Comparing `toga-core-0.3.0.dev9/tests/sources/test_list_source.py` & `toga-core-0.3.1/tests/sources/test_list_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,146 +4,147 @@
 from toga.sources import ListSource
 from toga.sources.list_source import Row
 
 
 class RowTests(TestCase):
     def setUp(self):
         self.source = Mock()
-        self.example = Row(val1='value 1', val2=42)
+        self.example = Row(val1="value 1", val2=42)
         self.example._source = self.source
 
     def test_initial_state(self):
         "A row holds values as expected"
 
-        self.assertEqual(self.example.val1, 'value 1')
+        self.assertEqual(self.example.val1, "value 1")
         self.assertEqual(self.example.val2, 42)
 
     def test_change_value(self):
         "If a row value changes, the source is notified"
-        self.example.val1 = 'new value'
+        self.example.val1 = "new value"
 
-        self.assertEqual(self.example.val1, 'new value')
-        self.source._notify.assert_called_once_with('change', item=self.example)
+        self.assertEqual(self.example.val1, "new value")
+        self.source._notify.assert_called_once_with("change", item=self.example)
 
 
 class ListSourceTests(TestCase):
     def test_init_with_tuple(self):
         "A ListSource can be instantiated from tuples"
         source = ListSource(
             data=[
-                ('first', 111),
-                ('second', 222),
-                ('third', 333),
+                ("first", 111),
+                ("second", 222),
+                ("third", 333),
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
 
-        self.assertEqual(source[1].val1, 'second')
+        self.assertEqual(source[1].val1, "second")
         self.assertEqual(source[1].val2, 222)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Set element 1
-        source[1] = ('new element', 999)
+        source[1] = ("new element", 999)
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[1].val1, 'new element')
+        self.assertEqual(source[1].val1, "new element")
         self.assertEqual(source[1].val2, 999)
 
         listener.insert.assert_called_once_with(index=1, item=source[1])
 
     def test_init_with_list(self):
         "A ListSource can be instantiated from lists"
         source = ListSource(
             data=[
-                ['first', 111],
-                ['second', 222],
-                ['third', 333],
+                ["first", 111],
+                ["second", 222],
+                ["third", 333],
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
 
-        self.assertEqual(source[1].val1, 'second')
+        self.assertEqual(source[1].val1, "second")
         self.assertEqual(source[1].val2, 222)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Set element 1
-        source[1] = ['new element', 999]
+        source[1] = ["new element", 999]
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[1].val1, 'new element')
+        self.assertEqual(source[1].val1, "new element")
         self.assertEqual(source[1].val2, 999)
 
         listener.insert.assert_called_once_with(index=1, item=source[1])
 
     def test_init_with_dict(self):
         "A ListSource can be instantiated from dicts"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
 
-        self.assertEqual(source[1].val1, 'second')
+        self.assertEqual(source[1].val1, "second")
         self.assertEqual(source[1].val2, 222)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Set element 1
-        source[1] = {'val1': 'new element', 'val2': 999}
+        source[1] = {"val1": "new element", "val2": 999}
 
         self.assertEqual(len(source), 3)
 
-        self.assertEqual(source[1].val1, 'new element')
+        self.assertEqual(source[1].val1, "new element")
         self.assertEqual(source[1].val2, 999)
 
         listener.insert.assert_called_once_with(index=1, item=source[1])
 
     def test_init_with_flat_list_of_objects(self):
         "A list source can be created from a flat list of objects"
 
         class MyObject:
             def __init__(self, info):
                 self.info = info
+
             def __str__(self):
                 return "string value %s" % self.info
 
         data = [
             MyObject(True),
             MyObject(2),
             MyObject("string"),
         ]
 
         source = ListSource(
             data=data,
-            accessors=['col1'],
+            accessors=["col1"],
         )
 
         for i, row in enumerate(source):
             self.assertEqual(row.col1, data[i])
 
     def test_init_with_flat_list_of_numbers(self):
         "A list source can be created from a flat list of numbers"
@@ -152,15 +153,15 @@
             100,
             200.0,
             -3.14,
         ]
 
         source = ListSource(
             data=data,
-            accessors=['col1'],
+            accessors=["col1"],
         )
 
         for i, row in enumerate(source):
             self.assertEqual(row.col1, data[i])
 
     def test_init_with_flat_list_of_strings(self):
         "A list source can be created from a flat list of strings"
@@ -169,48 +170,48 @@
             "xxx",
             "yyy",
             "zzz",
         ]
 
         source = ListSource(
             data=data,
-            accessors=['col1'],
+            accessors=["col1"],
         )
 
         for i, row in enumerate(source):
             self.assertEqual(row.col1, data[i])
 
     def test_iter(self):
         "A list source can be iterated over"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         result = 0
         for row in source:
             result += row.val2
 
         self.assertEqual(result, 666)
 
     def test_clear(self):
         "A list source can be cleared"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
@@ -220,212 +221,212 @@
 
         listener.clear.assert_called_once_with()
 
     def test_insert_kwarg(self):
         "You can insert into a list source using kwargs"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        row = source.insert(1, val1='new element', val2=999)
+        row = source.insert(1, val1="new element", val2=999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[1], row)
-        self.assertEqual(row.val1, 'new element')
+        self.assertEqual(row.val1, "new element")
         self.assertEqual(row.val2, 999)
 
         listener.insert.assert_called_once_with(index=1, item=row)
 
     def test_insert(self):
         "You can insert into a list source using positional args"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        row = source.insert(1, 'new element', 999)
+        row = source.insert(1, "new element", 999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[1], row)
-        self.assertEqual(row.val1, 'new element')
+        self.assertEqual(row.val1, "new element")
         self.assertEqual(row.val2, 999)
 
         listener.insert.assert_called_once_with(index=1, item=row)
 
     def test_prepend_kwarg(self):
         "You can prepend to a list source using kwargs"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Insert the new element
-        row = source.prepend(val1='new element', val2=999)
+        row = source.prepend(val1="new element", val2=999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[0], row)
-        self.assertEqual(row.val1, 'new element')
+        self.assertEqual(row.val1, "new element")
         self.assertEqual(row.val2, 999)
 
         listener.insert.assert_called_once_with(index=0, item=row)
 
     def test_prepend(self):
         "You can prepend to a list source using positional args"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Prepend the new element
-        row = source.prepend('new element', 999)
+        row = source.prepend("new element", 999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[0], row)
-        self.assertEqual(row.val1, 'new element')
+        self.assertEqual(row.val1, "new element")
         self.assertEqual(row.val2, 999)
 
         listener.insert.assert_called_once_with(index=0, item=row)
 
     def test_append_kwarg(self):
         "You can append to a list source using kwargs"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Append the new element
-        row = source.append(val1='new element', val2=999)
+        row = source.append(val1="new element", val2=999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[3], row)
-        self.assertEqual(row.val1, 'new element')
+        self.assertEqual(row.val1, "new element")
         self.assertEqual(row.val2, 999)
 
         listener.insert.assert_called_once_with(index=3, item=row)
 
     def test_append(self):
         "You can append to a list source using positional args"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Append the new element
-        row = source.append('new element', 999)
+        row = source.append("new element", 999)
 
         self.assertEqual(len(source), 4)
         self.assertEqual(source[3], row)
-        self.assertEqual(row.val1, 'new element')
+        self.assertEqual(row.val1, "new element")
         self.assertEqual(row.val2, 999)
 
         listener.insert.assert_called_once_with(index=3, item=row)
 
     def test_remove(self):
         "You can remove an item from a list source"
         source = ListSource(
             data=[
-                {'val1': 'first', 'val2': 111},
-                {'val1': 'second', 'val2': 222},
-                {'val1': 'third', 'val2': 333},
+                {"val1": "first", "val2": 111},
+                {"val1": "second", "val2": 222},
+                {"val1": "third", "val2": 333},
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         self.assertEqual(len(source), 3)
 
         listener = Mock()
         source.add_listener(listener)
 
         # Remove the second element
         row = source.remove(source[1])
 
         self.assertEqual(len(source), 2)
-        self.assertEqual(source[0].val1, 'first')
+        self.assertEqual(source[0].val1, "first")
         self.assertEqual(source[0].val2, 111)
 
-        self.assertEqual(source[1].val1, 'third')
+        self.assertEqual(source[1].val1, "third")
         self.assertEqual(source[1].val2, 333)
 
-        listener.remove.assert_called_once_with(item=row)
+        listener.remove.assert_called_once_with(item=row, index=1)
 
     def test_get_row_index(self):
         "You can get the index of any row within a list source"
 
         source = ListSource(
             data=[
-                ('first', 111),
-                ('second', 222),
-                ('third', 333),
+                ("first", 111),
+                ("second", 222),
+                ("third", 333),
             ],
-            accessors=['val1', 'val2']
+            accessors=["val1", "val2"],
         )
 
         for i, row in enumerate(source):
             self.assertEqual(i, source.index(row))
 
         # look-alike rows are not equal, so index lookup should fail
         with self.assertRaises(ValueError):
-            lookalike_row = Row(val1='second', val2=222)
+            lookalike_row = Row(val1="second", val2=222)
             source.index(lookalike_row)
 
         with self.assertRaises(ValueError):
             source.index(None)
 
         with self.assertRaises(ValueError):
             source.index(Row())
```

### Comparing `toga-core-0.3.0.dev9/tests/sources/test_source.py` & `toga-core-0.3.1/tests/sources/test_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,41 +9,41 @@
         listener1 = Mock()
         source = Source()
 
         source.add_listener(listener1)
         self.assertListEqual(source.listeners, [listener1])
 
         # activate listener
-        source._notify('message1')
+        source._notify("message1")
         listener1.message1.assert_called_once_with()
 
         # activate listener with data
-        source._notify('message2', arg1=11, arg2=22)
+        source._notify("message2", arg1=11, arg2=22)
         listener1.message2.assert_called_once_with(arg1=11, arg2=22)
 
         # add more widgets to listeners
         listener2 = Mock()
         source.add_listener(listener2)
         self.assertListEqual(source.listeners, [listener1, listener2])
 
         # activate listener
-        source._notify('message3')
+        source._notify("message3")
         listener1.message3.assert_called_once_with()
         listener2.message3.assert_called_once_with()
 
         # activate listener with data
-        source._notify('message4', arg1=11, arg2=22)
+        source._notify("message4", arg1=11, arg2=22)
         listener1.message4.assert_called_once_with(arg1=11, arg2=22)
         listener2.message4.assert_called_once_with(arg1=11, arg2=22)
 
         # remove from listeners
         source.remove_listener(listener2)
         self.assertListEqual(source.listeners, [listener1])
 
     def test_missing_listener_method(self):
         listener1 = object()
         source = Source()
 
         source.add_listener(listener1)
 
         # This shouldn't raise an error
-        source._notify('message1')
+        source._notify("message1")
```

### Comparing `toga-core-0.3.0.dev9/tests/widgets/test_scrollcontainer.py` & `toga-core-0.3.1/tests/widgets/test_webview.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 import toga
-import toga_dummy
-from toga_dummy.utils import TestCase, TestStyle
+from toga_dummy.utils import TestCase
 
+from ..utils import async_test
 
-class ScrollContainerTests(TestCase):
+
+class WebViewTests(TestCase):
     def setUp(self):
         super().setUp()
 
-        self.sc = toga.ScrollContainer(style=TestStyle(), factory=toga_dummy.factory)
+        self.url = "https://beeware.org/"
 
-    def test_widget_created(self):
-        self.assertEqual(self.sc._impl.interface, self.sc)
-        self.assertActionPerformed(self.sc, 'create ScrollContainer')
+        def callback(widget):
+            pass
 
-    def test_set_content_with_widget(self):
-        self.assertEqual(self.sc.content, None, 'The default value of content should be None')
+        self.on_key_down = callback
+        self.web_view = toga.WebView(
+            url=self.url, on_key_down=self.on_key_down, user_agent="DUMMY AGENT"
+        )
+
+    def test_widget_created(self):
+        self.assertEqual(self.web_view._impl.interface, self.web_view)
+        self.assertActionPerformed(self.web_view, "create WebView")
 
-        new_content = toga.Box(style=TestStyle(), factory=toga_dummy.factory)
-        self.sc.content = new_content
-        self.assertEqual(self.sc.content, new_content)
-        self.assertEqual(self.sc._content, new_content)
-        self.assertActionPerformedWith(self.sc, 'set content', widget=new_content._impl)
-
-        self.assertActionPerformedWith(new_content, 'set bounds', x=0, y=0, width=0, height=0)
-
-    def test_set_content_with_None(self):
-        new_content = None
-        self.assertEqual(self.sc.content, new_content)
-        self.assertEqual(self.sc._content, new_content)
-        self.assertActionNotPerformed(self.sc, 'set content')
-
-    def test_vertical_property(self):
-        self.assertEqual(self.sc.vertical, True, 'The default should be True')
-
-        new_value = False
-        self.sc.vertical = new_value
-        self.assertEqual(self.sc.vertical, new_value)
-        self.assertValueSet(self.sc, 'vertical', new_value)
-
-    def test_horizontal_property(self):
-        self.assertEqual(self.sc.horizontal, True, 'The default should be True')
-
-        new_value = False
-        self.sc.horizontal = new_value
-        self.assertEqual(self.sc.horizontal, new_value)
-        self.assertValueSet(self.sc, 'horizontal', new_value)
+    def test_setting_url_invokes_impl_method(self):
+        new_url = "https://github.com/"
+        self.web_view.url = new_url
+        self.assertEqual(self.web_view.url, new_url)
+        self.assertValueSet(self.web_view, "url", new_url)
+
+    def test_set_content_invokes_impl_method(self):
+        root_url = "https://github.com/"
+        new_content = """<!DOCTYPE html>
+            <html>
+              <body>
+                <h1>My First Heading</h1>
+                <p>My first paragraph.</p>
+              </body>
+            </html>
+        """
+
+        self.web_view.set_content(root_url, new_content)
+        self.assertActionPerformedWith(
+            self.web_view, "set content", root_url=root_url, content=new_content
+        )
+
+    def test_get_dom(self):
+        dom = self.web_view.dom
+        self.assertEqual(dom, "DUMMY DOM")
+        self.assertActionPerformed(self.web_view, "get DOM")
+
+    def test_get_user_agent(self):
+        self.assertEqual(self.web_view.user_agent, "DUMMY AGENT")
+
+    def test_set_user_agent(self):
+        new_user_agent = "DUMMY AGENT 2"
+        self.web_view.user_agent = new_user_agent
+        self.assertEqual(self.web_view.user_agent, new_user_agent)
+        self.assertValueSet(self.web_view, "user_agent", new_user_agent)
+
+    @async_test
+    async def test_evaluate_javascript(self):
+        result = await self.web_view.evaluate_javascript("test(1);")
+        self.assertActionPerformed(self.web_view, "evaluate_javascript")
+        self.assertEqual(result, "JS RESULT")
+
+    def test_invoke_javascript(self):
+        self.web_view.invoke_javascript("test(1);")
+        self.assertActionPerformed(self.web_view, "invoke_javascript")
```

### Comparing `toga-core-0.3.0.dev9/tests/widgets/test_tree.py` & `toga-core-0.3.1/tests/widgets/test_tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 import toga
-import toga_dummy
+from toga.sources import TreeSource
 from toga_dummy.utils import TestCase
-from toga.sources import TreeSource, Source
+
 
 class TreeTests(TestCase):
     def setUp(self):
         super().setUp()
 
-        self.headings = ['Heading {}'.format(x) for x in range(3)]
+        self.headings = [f"Heading {x}" for x in range(3)]
 
         self.data = None
-        self.tree = toga.Tree(headings=self.headings,
-                              data=self.data,
-                              factory=toga_dummy.factory)
+        self.tree = toga.Tree(
+            headings=self.headings,
+            data=self.data,
+        )
 
     def test_widget_created(self):
         self.assertEqual(self.tree._impl.interface, self.tree)
-        self.assertActionPerformed(self.tree, 'create Tree')
+        self.assertActionPerformed(self.tree, "create Tree")
         self.assertIsInstance(self.tree.data, TreeSource)
 
         self.assertEqual(self.tree.headings, self.headings)
 
+    def test_setter_creates_tree_with_TreeSource_data(self):
+        data = {("one", 1): [("one.one", 1.1), ("one.two", 2.1)], ("two", 2): None}
+
+        accessors = [f"heading{i}" for i in range(3)]
+
+        self.tree.data = TreeSource(data=data, accessors=accessors)
+
+        self.assertIsInstance(self.tree.data, TreeSource)
+        self.assertEqual(self.tree.data[0].heading0, "one")
+        self.assertEqual(self.tree.data[0][0].heading1, 1.1)
+        self.assertEqual(self.tree.data[1].heading1, 2)
+
     def test_setter_creates_tree_with_dict_data(self):
         self.data = {
-            ('first', 111): None,
-            ('second', 222): [],
-            ('third', 333): [
-                ('third.one', 331),
-                {'heading_0': 'third.two', 'heading_1': 332}
-            ]
+            ("first", 111): None,
+            ("second", 222): [],
+            ("third", 333): [
+                ("third.one", 331),
+                {"heading_0": "third.two", "heading_1": 332},
+            ],
         }
         self.tree.data = self.data
 
         self.assertIsInstance(self.tree.data, TreeSource)
         self.assertFalse(self.tree.data[0].can_have_children())
         self.assertTrue(self.tree.data[1].can_have_children())
         self.assertEqual(self.tree.data[1].heading_1, 222)
@@ -45,7 +58,28 @@
         pass
 
     def test_data_setter_creates_tree_with_data_source(self):
         pass
 
     def test_data_setter_creates_tree_with_data_none(self):
         pass
+
+    def test_multiselect_getter(self):
+        super().setUp()
+        self.headings = [f"Heading {x}" for x in range(3)]
+
+        self.data = None
+        self.tree = toga.Tree(
+            headings=self.headings,
+            data=self.data,
+            multiple_select=True,
+        )
+
+        self.assertEqual(self.tree.multiple_select, True)
+
+        self.tree = toga.Tree(
+            headings=self.headings,
+            data=self.data,
+            multiple_select=False,
+        )
+
+        self.assertEqual(self.tree.multiple_select, False)
```

### Comparing `toga-core-0.3.0.dev9/tests/widgets/test_selection.py` & `toga-core-0.3.1/tests/widgets/test_selection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import toga
-import toga_dummy
 from toga_dummy.utils import TestCase
 
 
 class SelectionTests(TestCase):
     def setUp(self):
         super().setUp()
 
-        self.items = ['item_{}'.format(x) for x in range(0, 3)]
-        self.selection = toga.Selection(factory=toga_dummy.factory)
-        self.selection = toga.Selection(items=self.items, factory=toga_dummy.factory)
+        self.items = [f"item_{x}" for x in range(0, 3)]
+        self.selection = toga.Selection(items=self.items)
 
     def test_widget_created(self):
         self.assertEqual(self.selection._impl.interface, self.selection)
-        self.assertActionPerformed(self.selection, 'create Selection')
+        self.assertActionPerformed(self.selection, "create Selection")
 
     def test_items_were_set(self):
         self.assertEqual(self.selection.items, self.items)
-        self.assertActionPerformedWith(self.selection, 'add item', item=self.items[0])
-        self.assertActionPerformedWith(self.selection, 'add item', item=self.items[1])
-        self.assertActionPerformedWith(self.selection, 'add item', item=self.items[2])
+        self.assertActionPerformedWith(self.selection, "add item", item=self.items[0])
+        self.assertActionPerformedWith(self.selection, "add item", item=self.items[1])
+        self.assertActionPerformedWith(self.selection, "add item", item=self.items[2])
 
     def test_set_items(self):
-        new_items = ['new_item_{}'.format(x) for x in range(0, 3)]
+        new_items = [f"new_item_{x}" for x in range(0, 3)]
         self.selection.items = new_items
-        self.assertActionPerformed(self.selection, 'remove all items')
+        self.assertActionPerformed(self.selection, "remove all items")
         for item in new_items:
-            self.assertActionPerformedWith(self.selection, 'add item', item=item)
+            self.assertActionPerformedWith(self.selection, "add item", item=item)
         self.assertEqual(self.selection.items, new_items)
         self.assertEqual(self.selection._items, new_items)
 
     def test_get_selected_item_invokes_impl_method(self):
-        value = self.selection.value
-        self.assertValueGet(self.selection, 'selected_item')
+        self.selection.value
+        self.assertValueGet(self.selection, "selected_item")
 
     def test_set_selected_item_invokes_impl_methods(self):
         self.selection.value = self.items[0]
-        self.assertActionPerformedWith(self.selection, 'select item', item=self.items[0])
+        self.assertActionPerformedWith(
+            self.selection, "select item", item=self.items[0]
+        )
 
     def test_set_selected_item_is_in_items(self):
         self.selection.value = self.items[2]
 
         with self.assertRaises(ValueError):
-            self.selection.value = 'not in items'
+            self.selection.value = "not in items"
 
     def test_on_select(self):
-        on_select = self.selection.on_select
+        on_select = self.selection.on_select._raw
         self.assertEqual(on_select, None)
+
+    def test_focus(self):
+        self.selection.focus()
+        self.assertActionPerformed(self.selection, "focus")
```

### Comparing `toga-core-0.3.0.dev9/tests/widgets/test_canvas.py` & `toga-core-0.3.1/tests/widgets/test_canvas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from math import pi, cos, sin
+from math import cos, pi, sin
+from unittest import mock
 
 import toga
-import toga_dummy
-from toga.font import SANS_SERIF, SERIF
+from toga.colors import BLANCHEDALMOND, CRIMSON, REBECCAPURPLE, rgb
+from toga.fonts import SANS_SERIF, SERIF
+from toga.widgets.canvas import FillRule
 from toga_dummy.utils import TestCase
-from toga.color import REBECCAPURPLE, BLANCHEDALMOND, CRIMSON, rgb
 
 
 class CanvasTests(TestCase):
     def setUp(self):
         super().setUp()
 
         # Create a canvas with the dummy factory
-        self.testing_canvas = toga.Canvas(factory=toga_dummy.factory)
+        self.testing_canvas = toga.Canvas()
 
     def test_widget_created(self):
         self.assertEqual(self.testing_canvas._impl.interface, self.testing_canvas)
         self.assertActionPerformed(self.testing_canvas, "create Canvas")
 
     def test_basic_drawing(self):
         with self.testing_canvas.context() as basic_context:
@@ -67,14 +68,15 @@
 
     def test_fill_checks(self):
         check_size = 32
         x = 10
         y = -10
         width = 200
         height = 200
+
         with self.testing_canvas.fill(color="rgba(1, 1, 1, 1)") as fill1:
             rect = fill1.rect(x, y, width, height)
             self.assertIn(rect, fill1.drawing_objects)
         self.assertActionPerformedWith(
             self.testing_canvas, "rect", x=10, y=-10, width=200, height=200
         )
         self.assertActionPerformedWith(self.testing_canvas, "fill")
@@ -93,78 +95,116 @@
                             x=i,
                             y=j,
                             width=check_size,
                             height=check_size,
                         )
         self.assertActionPerformedWith(self.testing_canvas, "fill")
 
+        with self.testing_canvas.fill(color=None) as fill3:
+            rect = fill3.rect(x, y, width, height)
+            self.assertIn(rect, fill3.drawing_objects)
+        self.assertActionPerformedWith(
+            self.testing_canvas, "rect", x=10, y=-10, width=200, height=200
+        )
+        self.assertActionPerformedWith(self.testing_canvas, "fill")
+
+        with self.testing_canvas.fill(color=None) as fill4:
+            # Only works for check_size a power of 2
+            for j in range(x & -check_size, height, check_size):
+                for i in range(y & -check_size, width, check_size):
+                    if (i / check_size + j / check_size) % 2 == 0:
+                        rect = fill4.rect(i, j, check_size, check_size)
+                        self.testing_canvas.redraw()
+                        self.assertIn(rect, fill4.drawing_objects)
+                        self.assertActionPerformedWith(
+                            self.testing_canvas,
+                            "rect",
+                            x=i,
+                            y=j,
+                            width=check_size,
+                            height=check_size,
+                        )
+        self.assertActionPerformedWith(self.testing_canvas, "fill")
+
+    def test_fill_raises_error_on_invalid_fill_rule(self):
+        def fill_context():
+            with self.testing_canvas.fill(fill_rule="unknown"):
+                pass
+
+        self.assertRaisesRegex(
+            ValueError,
+            "^fill rule should be one of the followings: evenodd, nonzero$",
+            fill_context,
+        )
+        self.assertActionNotPerformed(self.testing_canvas, "fill")
+
     def test_draw_3circles(self):
         xc = 100
         yc = 150
         radius = 0.5 * 50 - 10
         alpha = 0.8
-        subradius = radius * (2 / 3. - 0.1)
+        subradius = radius * (2 / 3.0 - 0.1)
 
         with self.testing_canvas.fill(
             color="rgba(1, 0, 0, " + str(alpha) + ")"
         ) as fill1:
             ellipse1 = fill1.ellipse(
-                xc + radius / 3. * cos(pi * 0.5),
-                yc - radius / 3. * sin(pi * 0.5),
+                xc + radius / 3.0 * cos(pi * 0.5),
+                yc - radius / 3.0 * sin(pi * 0.5),
                 subradius,
                 subradius,
                 2.0 * pi,
             )
             self.assertIn(ellipse1, fill1.drawing_objects)
         self.assertActionPerformedWith(
             self.testing_canvas,
             "ellipse",
-            x=xc + radius / 3. * cos(pi * 0.5),
-            y=yc - radius / 3. * sin(pi * 0.5),
+            x=xc + radius / 3.0 * cos(pi * 0.5),
+            y=yc - radius / 3.0 * sin(pi * 0.5),
             radiusx=subradius,
             radiusy=subradius,
             rotation=2.0 * pi,
         )
         self.assertActionPerformedWith(self.testing_canvas, "fill")
 
         with self.testing_canvas.fill(
             color="rgba(0, 1, 0, " + str(alpha) + ")"
         ) as fill2:
             ellipse2 = fill2.ellipse(
-                xc + radius / 3. * cos(pi * (0.5 + 2 / .3)),
-                yc - radius / 3. * sin(pi * (0.5 + 2 / .3)),
+                xc + radius / 3.0 * cos(pi * (0.5 + 2 / 0.3)),
+                yc - radius / 3.0 * sin(pi * (0.5 + 2 / 0.3)),
                 subradius,
                 subradius,
             )
             self.assertIn(ellipse2, fill2.drawing_objects)
         self.assertActionPerformedWith(
             self.testing_canvas,
             "ellipse",
-            x=xc + radius / 3. * cos(pi * (0.5 + 2 / .3)),
-            y=yc - radius / 3. * sin(pi * (0.5 + 2 / .3)),
+            x=xc + radius / 3.0 * cos(pi * (0.5 + 2 / 0.3)),
+            y=yc - radius / 3.0 * sin(pi * (0.5 + 2 / 0.3)),
             radiusx=subradius,
             radiusy=subradius,
         )
         self.assertActionPerformedWith(self.testing_canvas, "fill")
 
         with self.testing_canvas.fill(
             color="rgba(0, 0, 1, " + str(alpha) + ")"
         ) as fill3:
             ellipse3 = fill3.ellipse(
-                xc + radius / 3. * cos(pi * (0.5 + 4 / .3)),
-                yc - radius / 3. * sin(pi * (0.5 + 4 / .3)),
+                xc + radius / 3.0 * cos(pi * (0.5 + 4 / 0.3)),
+                yc - radius / 3.0 * sin(pi * (0.5 + 4 / 0.3)),
                 subradius,
                 subradius,
             )
             self.assertIn(ellipse3, fill3.drawing_objects)
         self.assertActionPerformedWith(
             self.testing_canvas,
             "ellipse",
-            x=xc + radius / 3. * cos(pi * (0.5 + 4 / .3)),
-            y=yc - radius / 3. * sin(pi * (0.5 + 4 / .3)),
+            x=xc + radius / 3.0 * cos(pi * (0.5 + 4 / 0.3)),
+            y=yc - radius / 3.0 * sin(pi * (0.5 + 4 / 0.3)),
             radiusx=subradius,
             radiusy=subradius,
         )
         self.assertActionPerformedWith(self.testing_canvas, "fill")
 
     def test_draw_triangle(self):
         with self.testing_canvas.closed_path(32, 0) as closed:
@@ -184,14 +224,23 @@
         self.assertActionPerformedWith(self.testing_canvas, "new path")
 
     def test_new_path_remove(self):
         new_path = self.testing_canvas.new_path()
         self.testing_canvas.remove(new_path)
         self.assertNotIn(new_path, self.testing_canvas.drawing_objects)
 
+    def test_canvas_context_clear(self):
+        # Create canvas objects
+        new_path = self.testing_canvas.new_path()
+        rect = self.testing_canvas.rect(x=1000.2, y=2000, width=3000, height=-4000.0)
+
+        self.testing_canvas.clear()
+        self.assertNotIn(new_path, self.testing_canvas.drawing_objects)
+        self.assertNotIn(rect, self.testing_canvas.drawing_objects)
+
     def test_new_path_repr(self):
         new_path = self.testing_canvas.new_path()
         self.assertEqual(repr(new_path), "NewPath()")
 
     def test_closed_path_modify(self):
         with self.testing_canvas.closed_path(0, -5) as closed:
             closed.line_to(10, 10)
@@ -413,42 +462,54 @@
             filler.fill_rule = "evenodd"
             filler.preserve = True
             self.testing_canvas.redraw()
         self.assertActionPerformedWith(
             self.testing_canvas,
             "fill",
             color=rgb(102, 51, 153),
-            fill_rule="evenodd",
+            fill_rule=FillRule.EVENODD,
             preserve=True,
         )
 
     def test_fill_repr(self):
         with self.testing_canvas.fill(
             color=CRIMSON, fill_rule="evenodd", preserve=True
         ) as filler:
             self.assertEqual(
                 repr(filler),
-                "Fill(color=rgb(220, 20, 60), fill_rule=evenodd, preserve=True)",
+                "Fill(color=rgb(220, 20, 60), fill_rule=FillRule.EVENODD, preserve=True)",
             )
 
     def test_stroke_modify(self):
         with self.testing_canvas.stroke(
-            color=BLANCHEDALMOND, line_width=5.0
+            color=BLANCHEDALMOND, line_width=5.0, line_dash=[2, 2]
         ) as stroker:
             stroker.color = REBECCAPURPLE
             stroker.line_width = 1
+            stroker.line_dash = [1, 1]
             self.testing_canvas.redraw()
         self.assertActionPerformedWith(
-            self.testing_canvas, "stroke", color=rgb(102, 51, 153), line_width=1
+            self.testing_canvas,
+            "stroke",
+            color=rgb(102, 51, 153),
+            line_width=1,
+            line_dash=[1, 1],
         )
 
     def test_stroke_repr(self):
-        with self.testing_canvas.stroke() as stroker:
+        with self.testing_canvas.stroke() as stroker1:
+            self.assertEqual(
+                repr(stroker1),
+                "Stroke(color=rgb(0, 0, 0), line_width=2.0, line_dash=None)",
+            )
+
+        # Testing to draw a colorless stroke, i.e. with color=None
+        with self.testing_canvas.stroke(color=None) as stroker2:
             self.assertEqual(
-                repr(stroker), "Stroke(color=rgb(0, 0, 0), line_width=2.0)"
+                repr(stroker2), "Stroke(color=None, line_width=2.0, line_dash=None)"
             )
 
     def test_rotate_simple(self):
         rotate = self.testing_canvas.rotate(pi)
         self.assertIn(rotate, self.testing_canvas.drawing_objects)
         self.assertActionPerformedWith(self.testing_canvas, "rotate", radians=pi)
 
@@ -521,15 +582,15 @@
     def test_write_text_default(self):
         write_text = self.testing_canvas.write_text("test text")
         self.assertActionPerformedWith(
             self.testing_canvas, "write text", text="test text"
         )
         self.assertEqual(
             repr(write_text),
-            "WriteText(text=test text, x=0, y=0, font=<Font: 12pt system>)",
+            "WriteText(text=test text, x=0, y=0, font=<Font: system default size system>)",
         )
 
     def test_write_text_modify(self):
         write_text = self.testing_canvas.write_text("test text")
         modify_font = toga.Font(family=SERIF, size=1.2)
         write_text.text, write_text.x, write_text.y, write_text.font = (
             "hello again",
@@ -550,7 +611,150 @@
     def test_write_text_repr(self):
         font = toga.Font(family=SERIF, size=4)
         write_text = self.testing_canvas.write_text("hello", x=10, y=-4.2, font=font)
         self.assertEqual(
             repr(write_text),
             "WriteText(text=hello, x=10, y=-4.2, font=<Font: 4pt serif>)",
         )
+
+    def test_on_resize(self):
+        self.assertIsNone(self.testing_canvas.on_resize._raw)
+
+        # set a new callback
+        def callback(widget, **extra):
+            return f"called {type(widget)} with {extra}"
+
+        self.testing_canvas.on_resize = callback
+        self.assertEqual(self.testing_canvas.on_resize._raw, callback)
+        self.assertEqual(
+            self.testing_canvas.on_resize(None, a=1),
+            "called <class 'toga.widgets.canvas.Canvas'> with {'a': 1}",
+        )
+        self.assertValueSet(
+            self.testing_canvas, "on_resize", self.testing_canvas.on_resize
+        )
+
+    def test_on_press(self):
+        """Check on_press handler being invoked."""
+        self.assertIsNone(self.testing_canvas.on_press._raw)
+
+        # set a new callback
+        def callback(widget, **extra):
+            return f"called {type(widget)} with {extra}"
+
+        self.testing_canvas.on_press = callback
+        self.assertEqual(self.testing_canvas.on_press._raw, callback)
+        self.assertEqual(
+            self.testing_canvas.on_press(None, a=1),
+            "called <class 'toga.widgets.canvas.Canvas'> with {'a': 1}",
+        )
+        self.assertValueSet(
+            self.testing_canvas, "on_press", self.testing_canvas.on_press
+        )
+
+    def test_on_release(self):
+        """Check on_release handler being invoked."""
+        self.assertIsNone(self.testing_canvas.on_release._raw)
+
+        # set a new callback
+        def callback(widget, **extra):
+            return f"called {type(widget)} with {extra}"
+
+        self.testing_canvas.on_release = callback
+        self.assertEqual(self.testing_canvas.on_release._raw, callback)
+        self.assertEqual(
+            self.testing_canvas.on_release(None, a=1),
+            "called <class 'toga.widgets.canvas.Canvas'> with {'a': 1}",
+        )
+        self.assertValueSet(
+            self.testing_canvas, "on_release", self.testing_canvas.on_release
+        )
+
+    def test_on_drag(self):
+        """Check on_drag handler being invoked."""
+        self.assertIsNone(self.testing_canvas.on_drag._raw)
+
+        # set a new callback
+        def callback(widget, **extra):
+            return f"called {type(widget)} with {extra}"
+
+        self.testing_canvas.on_drag = callback
+        self.assertEqual(self.testing_canvas.on_drag._raw, callback)
+        self.assertEqual(
+            self.testing_canvas.on_drag(None, a=1),
+            "called <class 'toga.widgets.canvas.Canvas'> with {'a': 1}",
+        )
+        self.assertValueSet(self.testing_canvas, "on_drag", self.testing_canvas.on_drag)
+
+    def test_on_alt_press(self):
+        """Check on_alt_press handler being invoked."""
+        self.assertIsNone(self.testing_canvas.on_alt_press._raw)
+
+        # set a new callback
+        def callback(widget, **extra):
+            return f"called {type(widget)} with {extra}"
+
+        self.testing_canvas.on_alt_press = callback
+        self.assertEqual(self.testing_canvas.on_alt_press._raw, callback)
+        self.assertEqual(
+            self.testing_canvas.on_alt_press(None, a=1),
+            "called <class 'toga.widgets.canvas.Canvas'> with {'a': 1}",
+        )
+        self.assertValueSet(
+            self.testing_canvas, "on_alt_press", self.testing_canvas.on_alt_press
+        )
+
+    def test_on_alt_release(self):
+        """Check on_alt_release handler being invoked."""
+        self.assertIsNone(self.testing_canvas.on_alt_release._raw)
+
+        # set a new callback
+        def callback(widget, **extra):
+            return f"called {type(widget)} with {extra}"
+
+        self.testing_canvas.on_alt_release = callback
+        self.assertEqual(self.testing_canvas.on_alt_release._raw, callback)
+        self.assertEqual(
+            self.testing_canvas.on_alt_release(None, a=1),
+            "called <class 'toga.widgets.canvas.Canvas'> with {'a': 1}",
+        )
+        self.assertValueSet(
+            self.testing_canvas, "on_alt_release", self.testing_canvas.on_alt_release
+        )
+
+    def test_on_alt_drag(self):
+        """Check on_alt_dragged handler being invoked."""
+        self.assertIsNone(self.testing_canvas.on_alt_drag._raw)
+
+        # set a new callback
+        def callback(widget, **extra):
+            return f"called {type(widget)} with {extra}"
+
+        self.testing_canvas.on_alt_drag = callback
+        self.assertEqual(self.testing_canvas.on_alt_drag._raw, callback)
+        self.assertEqual(
+            self.testing_canvas.on_alt_drag(None, a=1),
+            "called <class 'toga.widgets.canvas.Canvas'> with {'a': 1}",
+        )
+        self.assertValueSet(
+            self.testing_canvas, "on_alt_drag", self.testing_canvas.on_alt_drag
+        )
+
+    def test_measure_text(self):
+        text = "This is text"
+        font = mock.Mock()
+        self.testing_canvas.measure_text(text, font=font)
+        self.assertActionPerformedWith(
+            self.testing_canvas, "measure text", text=text, font=font, tight=False
+        )
+
+    def test_measure_text_tight(self):
+        text = "This is text"
+        font = mock.Mock()
+        self.testing_canvas.measure_text(text, font=font, tight=True)
+        self.assertActionPerformedWith(
+            self.testing_canvas, "measure text", text=text, font=font, tight=True
+        )
+
+    def test_canvas_as_image(self):
+        self.testing_canvas.as_image()
+        self.assertActionPerformed(self.testing_canvas, "get image data")
```

### Comparing `toga-core-0.3.0.dev9/tests/widgets/test_base.py` & `toga-core-0.3.1/src/toga/style/applicator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,51 @@
-import toga
-from toga.style import Pack
-import toga_dummy
-from toga_dummy.utils import TestCase
-
-
-class WidgetTests(TestCase):
-    def setUp(self):
-        super().setUp()
-
-        self.id = 'widget_id'
-        self.style = Pack(padding=666)
-
-        self.widget = toga.Widget(id=self.id,
-                                  style=self.style,
-                                  factory=toga_dummy.factory)
-
-    def test_arguments_were_set_correctly(self):
-        self.assertEqual(self.widget.id, self.id)
-        self.assertEqual(self.widget.style.padding, self.style.padding)
-
-    def test_create_widget_with_no_style(self):
-        widget = toga.Widget(factory=toga_dummy.factory)
-        self.assertTrue(isinstance(widget.style, Pack))
-
-    def test_enabled_with_None(self):
-        # Using a Box for test because we need a concrete implementation to use this property.
-        box = toga.Box(factory=toga_dummy.factory)
-        box.enabled = None
-        self.assertFalse(box.enabled)
-        self.assertActionPerformedWith(box, 'set enabled', value=None)
-
-    def test_adding_child(self):
-        """
-        """
-        self.assertEqual(self.widget.children, [], 'No child was added, should return a empty list.')
-        # Create a child widget to add to the our widget.
-        child = toga.Widget(factory=toga_dummy.factory)
-
-        with self.assertRaises(ValueError, msg='Widget cannot have children.'):
-            self.widget.add(child)
-
-        # Deliberately set widget._children = [] to allow it to have children.
-        # Only for test purposes!
-        self.widget._children = []
-        self.widget.add(child)
-        self.assertEqual(self.widget.children, [child])
-
-    def test_adding_children(self):
-        self.assertEqual(self.widget.children, [], ' No children added, should return a empty list.')
-        # Create 2 children to add to widget.
-        child1 = toga.Widget(factory=toga_dummy.factory)
-        child2 = toga.Widget(factory=toga_dummy.factory)
-
-        self.widget._children = []
-        self.widget.add(child1, child2)
-        self.assertEqual(self.widget.children, [child1, child2])
+class TogaApplicator:
+    """Apply styles to a Toga widget."""
+
+    def __init__(self, widget):
+        self.widget = widget
+
+    def refresh(self):
+        # print("RE-EVALUATE LAYOUT", self.widget)
+        self.widget.refresh()
+
+    def set_bounds(self):
+        # print("  APPLY LAYOUT", self.widget, self.widget.layout)
+        self.widget._impl.set_bounds(
+            self.widget.layout.absolute_content_left,
+            self.widget.layout.absolute_content_top,
+            self.widget.layout.content_width,
+            self.widget.layout.content_height,
+        )
+        for child in self.widget.children:
+            child.applicator.set_bounds()
+
+    def set_text_alignment(self, alignment):
+        self.widget._impl.set_alignment(alignment)
+
+    def set_hidden(self, hidden):
+        self.widget._impl.set_hidden(hidden)
+        for child in self.widget.children:
+            # If the parent is hidden, then so are all children. However, if the
+            # parent is visible, then the child's explicit visibility style is
+            # taken into account. This visibility cascades into any
+            # grandchildren.
+            #
+            # parent hidden child hidden style child final hidden state
+            # ============= ================== ========================
+            # True          True               True
+            # True          False              True
+            # False         True               True
+            # False         False              False
+            child.applicator.set_hidden(hidden or child.style._hidden)
+
+    def set_font(self, font):
+        # Changing the font of a widget can make the widget change size,
+        # which in turn means we need to do a re-layout
+        self.widget._impl.set_font(font)
+        self.widget.refresh()
+
+    def set_color(self, color):
+        self.widget._impl.set_color(color)
+
+    def set_background_color(self, color):
+        self.widget._impl.set_background_color(color)
```

### Comparing `toga-core-0.3.0.dev9/tests/widgets/test_passwordinput.py` & `toga-core-0.3.1/tests/widgets/test_passwordinput.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import toga
-import toga_dummy
 from toga_dummy.utils import TestCase
 
 
 class PasswordInputTests(TestCase):
-    """
-    """
+    """"""
+
     def setUp(self):
         super().setUp()
 
-        self.value = 'Password'
-        self.placeholder = 'Placeholder'
+        self.value = "Password"
+        self.placeholder = "Placeholder"
         self.readonly = False
 
-        self.password_input = toga.PasswordInput(factory=toga_dummy.factory)
+        self.password_input = toga.PasswordInput()
 
     def test_widget_created(self):
         self.assertEqual(self.password_input._impl.interface, self.password_input)
-        self.assertActionPerformed(self.password_input, 'create PasswordInput')
+        self.assertActionPerformed(self.password_input, "create PasswordInput")
 
     def test_widget(self):
         self.assertEqual(self.password_input.readonly, False)
 
-        new_placeholder = 'new placeholder'
+        new_placeholder = "new placeholder"
         self.password_input.placeholder = new_placeholder
         self.assertEqual(self.password_input.placeholder, new_placeholder)
 
-        new_value = 'new value'
+        new_value = "new value"
         self.password_input.value = new_value
         self.assertEqual(self.password_input.value, new_value)
 
         self.password_input.clear()
-        self.assertEqual(self.password_input.value, '')
+        self.assertEqual(self.password_input.value, "")
+
+    def test_focus(self):
+        self.password_input.focus()
+        self.assertActionPerformed(self.password_input, "focus")
```

### Comparing `toga-core-0.3.0.dev9/toga/window.py` & `toga-core-0.3.1/src/toga/widgets/table.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,288 +1,253 @@
-from builtins import id as identifier
+import warnings
 
-from toga.command import CommandSet
-from toga.platform import get_platform_factory
+from toga.handlers import wrapped_handler
+from toga.sources import ListSource
+from toga.sources.accessors import build_accessors, to_accessor
 
+from .base import Widget
 
-class Window:
-    """The top level container of a application.
+
+class Table(Widget):
+    """A Table Widget allows the display of data in the form of columns and
+    rows.
 
     Args:
-        id (str): The ID of the window (optional).
-        title (str): Title for the window (optional).
-        position (``tuple`` of (int, int)): Position of the window, as x,y coordinates.
-        size (``tuple`` of (int, int)):  Size of the window, as (width, height) sizes, in pixels.
-        toolbar (``list`` of :class:`toga.Widget`): A list of widgets to add to a toolbar
-        resizeable (bool): Toggle if the window is resizable by the user, defaults to `True`.
-        closeable (bool): Toggle if the window is closable by the user, defaults to `True`.
-        minimizable (bool): Toggle if the window is minimizable by the user, defaults to `True`.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional; normally not needed)
-    """
-    _WINDOW_CLASS = 'Window'
+        headings (``list`` of ``str``): The list of headings for the table.
+        id (str): An identifier for this widget.
+        data (``list`` of ``tuple``): The data to be displayed on the table.
+        accessors: A list of methods, same length as ``headings``, that describes
+            how to extract the data value for each column from the row. (Optional)
+        style (:obj:`Style`): An optional style object.
+            If no style is provided` then a new one will be created for the widget.
+        on_select (``callable``): A function to be invoked on selecting a row of the table.
+        on_double_click (``callable``): A function to be invoked on double clicking a row of
+            the table.
+        missing_value (``str`` or ``None``): value for replacing a missing value
+            in the data source. (Default: None). When 'None', a warning message
+            will be shown.
+
+    Examples:
+        >>> headings = ['Head 1', 'Head 2', 'Head 3']
+        >>> data = []
+        >>> table = Table(headings, data=data)
+
+        Data can be in several forms.
+        A list of dictionaries, where the keys match the heading names:
+
+        >>> data = [{'head_1': 'value 1', 'head_2': 'value 2', 'head_3': 'value3'}),
+        >>>         {'head_1': 'value 1', 'head_2': 'value 2', 'head_3': 'value3'}]
 
-    def __init__(self, id=None, title=None,
-                 position=(100, 100), size=(640, 480),
-                 toolbar=None, resizeable=True,
-                 closeable=True, minimizable=True, factory=None):
-
-        self._id = id if id else identifier(self)
-        self._impl = None
-        self._app = None
-        self._content = None
-        self._position = position
-        self._size = size
-        self._is_full_screen = False
-
-        self.resizeable = resizeable
-        self.closeable = closeable
-        self.minimizable = minimizable
-
-        self.factory = get_platform_factory(factory)
-        self._impl = getattr(self.factory, self._WINDOW_CLASS)(interface=self)
-
-        self._toolbar = CommandSet(self, self._impl.create_toolbar)
-
-        self.position = position
-        self.size = size
-        self.title = title
+        A list of lists. These will be mapped to the headings in order:
 
-    @property
-    def id(self):
-        """ The DOM identifier for the window.
-        This id can be used to target CSS directives
+        >>> data = [('value 1', 'value 2', 'value3'),
+        >>>         ('value 1', 'value 2', 'value3')]
 
-        Returns:
-            The identifier as a ``str``.
-        """
-        return self._id
+        A list of values. This is only accepted if there is a single heading.
 
-    @property
-    def app(self):
-        """ Instance of the :class:`toga.App` that this window belongs to.
+        >>> data = ['item 1', 'item 2', 'item 3']
+    """
 
-        Returns:
-            The app that it belongs to :class:`toga.App`.
+    def __init__(
+        self,
+        headings,
+        id=None,
+        style=None,
+        data=None,
+        accessors=None,
+        multiple_select=False,
+        on_select=None,
+        on_double_click=None,
+        missing_value=None,
+        factory=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
 
-        Raises:
-            Exception: If the window already is associated with another app.
-        """
-        return self._app
+        self.headings = headings[:]
+        self._accessors = build_accessors(self.headings, accessors)
+        self._multiple_select = multiple_select
+        self._on_select = None
+        self._on_double_click = None
+        self._data = None
+        if missing_value is None:
+            print(
+                "WARNING: Using empty string for missing value in data. "
+                "Define a 'missing_value' on the table to silence this message"
+            )
+        self._missing_value = missing_value or ""
 
-    @app.setter
-    def app(self, app):
-        if self._app:
-            raise Exception("Window is already associated with an App")
+        self._impl = self.factory.Table(interface=self)
+        self.data = data
 
-        self._app = app
-        self._impl.set_app(app._impl)
+        self.on_select = on_select
+        self.on_double_click = on_double_click
 
     @property
-    def title(self):
-        """ Title of the window. If no title is given it defaults to "Toga".
+    def data(self):
+        """The data source of the widget. It accepts table data in the form of
+        ``list``, ``tuple``, or :obj:`ListSource`
 
         Returns:
-            The current title of the window as a ``str``.
+            Returns a (:obj:`ListSource`).
         """
-        return self._title
+        return self._data
 
-    @title.setter
-    def title(self, title):
-        if not title:
-            title = "Toga"
+    @data.setter
+    def data(self, data):
+        if data is None:
+            self._data = ListSource(accessors=self._accessors, data=[])
+        elif isinstance(data, (list, tuple)):
+            self._data = ListSource(accessors=self._accessors, data=data)
+        else:
+            self._data = data
 
-        self._title = title
-        self._impl.set_title(title)
+        self._data.add_listener(self._impl)
+        self._impl.change_source(source=self._data)
 
     @property
-    def toolbar(self):
-        """ Toolbar for the window.
-
-        Returns:
-            A ``list`` of :class:`toga.Widget`
-        """
-        return self._toolbar
+    def multiple_select(self):
+        """Does the table allow multiple rows to be selected?"""
+        return self._multiple_select
 
     @property
-    def content(self):
-        """ Content of the window.
-        On setting, the content is added to the same app as the window and to the same app.
+    def selection(self):
+        """The current selection of the table.
 
-        Returns:
-            A :class:`toga.Widget`
-        """
-        return self._content
-
-    @content.setter
-    def content(self, widget):
-        # Assign the content widget to the same app as the window.
-        widget.app = self.app
-
-        # Assign the content widget to the window.
-        widget.window = self
-
-        # Track our new content
-        self._content = widget
-
-        # Manifest the widget
-        self._impl.set_content(widget._impl)
-
-        # Update the geometry of the widget
-        widget.refresh()
+        A value of None indicates no selection.
+        If the table allows multiple selection, returns a list of
+        selected data nodes. Otherwise, returns a single data node.
 
-    @property
-    def size(self):
-        """ Size of the window, as width, height.
-
-        Returns:
-            A ``tuple`` of (``int``, ``int``) where the first value is
-            the width and the second it the height of the window.
+        The value of a column of the selection can be accessed with selection.accessor_name
+        (for single selection) and with selection[x].accessor_name (for multiple selection)
         """
-        return self._size
+        return self._impl.get_selection()
 
-    @size.setter
-    def size(self, size):
-        self._size = size
-        self._impl.set_size(size)
-        if self.content:
-            self.content.refresh()
+    def scroll_to_top(self):
+        """Scroll the view so that the top of the list (first row) is
+        visible."""
+        self.scroll_to_row(0)
 
-    @property
-    def position(self):
-        """ Position of the window, as x, y
+    def scroll_to_row(self, row):
+        """Scroll the view so that the specified row index is visible.
 
-        Returns:
-            A ``tuple`` of (``int``, ``int``) int the from (x, y).
+        Args:
+            row: The index of the row to make visible. Negative values refer
+                 to the nth last row (-1 is the last row, -2 second last,
+                 and so on)
         """
-        return self._position
+        if row >= 0:
+            self._impl.scroll_to_row(row)
+        else:
+            self._impl.scroll_to_row(len(self.data) + row)
 
-    @position.setter
-    def position(self, position):
-        self._position = position
-        self._impl.set_position(position)
-
-    def show(self):
-        """ Show window, if hidden """
-        self._impl.show()
+    def scroll_to_bottom(self):
+        """Scroll the view so that the bottom of the list (last row) is
+        visible."""
+        self.scroll_to_row(-1)
 
     @property
-    def full_screen(self):
-        return self._is_full_screen
+    def on_select(self):
+        """The callback function that is invoked when a row of the table is
+        selected. The provided callback function has to accept two arguments
+        table (:obj:`Table`) and row (``Row`` or ``None``).
 
-    @full_screen.setter
-    def full_screen(self, is_full_screen):
-        self._is_full_screen = is_full_screen
-        self._impl.set_full_screen(is_full_screen)
-
-    def on_close(self):
-        self._impl.on_close()
-
-    ############################################################
-    # Dialogs
-    ############################################################
-
-    def info_dialog(self, title, message):
-        """ Opens a info dialog with a 'OK' button to close the dialog.
-
-        Args:
-            title (str): The title of the dialog window.
-            message (str): The dialog message to display.
+        The value of a column of row can be accessed with row.accessor_name
 
         Returns:
-            Returns `None` after the user pressed the 'OK' button.
+            (``callable``) The callback function.
         """
-        return self._impl.info_dialog(title, message)
+        return self._on_select
 
-    def question_dialog(self, title, message):
-        """ Opens a dialog with a 'YES' and 'NO' button.
+    @on_select.setter
+    def on_select(self, handler):
+        """Set the function to be executed on node selection.
 
-        Args:
-            title (str): The title of the dialog window.
-            message (str): The dialog message to display.
-
-        Returns:
-            Returns `True` when the 'YES' button was pressed, `False` when the 'NO' button was pressed.
+        :param handler: callback function
+        :type handler: ``callable``
         """
-        return self._impl.question_dialog(title, message)
+        self._on_select = wrapped_handler(self, handler)
+        self._impl.set_on_select(self._on_select)
 
-    def confirm_dialog(self, title, message):
-        """ Opens a dialog with a 'Cancel' and 'OK' button.
+    @property
+    def on_double_click(self):
+        """The callback function that is invoked when a row of the table is
+        double clicked. The provided callback function has to accept two
+        arguments table (:obj:`Table`) and row (``Row`` or ``None``).
 
-        Args:
-            title (str): The title of the dialog window.
-            message (str): The dialog message to display.
+        The value of a column of row can be accessed with row.accessor_name
 
         Returns:
-            Returns `True` when the 'OK' button was pressed, `False` when the 'CANCEL' button was pressed.
+            (``callable``) The callback function.
         """
-        return self._impl.confirm_dialog(title, message)
-
-    def error_dialog(self, title, message):
-        """ Opens a error dialog with a 'OK' button to close the dialog.
+        return self._on_double_click
 
-        Args:
-            title (str): The title of the dialog window.
-            message (str): The dialog message to display.
+    @on_double_click.setter
+    def on_double_click(self, handler):
+        """Set the function to be executed on node double click.
 
-        Returns:
-            Returns `None` after the user pressed the 'OK' button.
+        :param handler: callback function
+        :type handler: ``callable``
         """
-        return self._impl.error_dialog(title, message)
-
-    def stack_trace_dialog(self, title, message, content, retry=False):
-        """ Calling this function opens a dialog that allows to display a
-        large text body in a scrollable fashion.
+        self._on_double_click = wrapped_handler(self, handler)
+        self._impl.set_on_double_click(self._on_double_click)
 
-        Args:
-            title (str): The title of the dialog window.
-            message (str): The dialog message to display.
-            content (str):
-            retry (bool):
+    def add_column(self, heading, accessor=None):
+        """Add a new column to the table.
 
-        Returns:
-            Returns `None` after the user pressed the 'OK' button.
+        :param heading: title of the column
+        :type heading: ``string``
+        :param accessor: accessor of this new column
+        :type heading: ``string``
         """
-        return self._impl.stack_trace_dialog(title, message, content, retry)
 
-    def save_file_dialog(self, title, suggested_filename, file_types=None):
-        """ This opens a native dialog where the user can select a place to save a file.
-        It is possible to suggest a filename and force the user to use a specific file extension.
-        If no path is returned (eg. dialog is canceled), a ValueError is raised.
+        if not accessor:
+            accessor = to_accessor(heading)
 
-        Args:
-            title (str): The title of the dialog window.
-            suggested_filename(str): The automatically filled in filename.
-            file_types: A list of strings with the allowed file extensions.
+        if accessor in self._accessors:
+            raise ValueError(f'Accessor "{accessor}" is already in use')
 
-        Returns:
-            The absolute path(str) to the selected location.
-        """
-        return self._impl.save_file_dialog(title, suggested_filename, file_types)
+        self.headings.append(heading)
+        self._accessors.append(accessor)
 
-    def open_file_dialog(self, title, initial_directory=None, file_types=None, multiselect=False):
-        """ This opens a native dialog where the user can select the file to open.
-        It is possible to set the initial folder and only show files with specified file extensions.
-        If no path is returned (eg. dialog is canceled), a ValueError is raised.
-        Args:
-            title (str): The title of the dialog window.
-            initial_directory(str): Initial folder displayed in the dialog.
-            file_types: A list of strings with the allowed file extensions.
-            multiselect: Value showing whether a user can select multiple files.
+        self._impl.add_column(heading, accessor)
 
-        Returns:
-            The absolute path(str) to the selected file or a list(str) if multiselect
+    def remove_column(self, column):
+        """Remove a table column.
+
+        :param column: accessor or position (>0)
+        :type column: ``string``
+        :type column: ``int``
         """
-        return self._impl.open_file_dialog(title, initial_directory, file_types, multiselect)
 
-    def select_folder_dialog(self, title, initial_directory=None):
-        """ This opens a native dialog where the user can select a folder.
-        It is possible to set the initial folder.
-        If no path is returned (eg. dialog is canceled), a ValueError is raised.
-        Args:
-            title (str): The title of the dialog window.
-            initial_directory(str): Initial folder displayed in the dialog.
+        if isinstance(column, str):
+            # Column is a string; use as-is
+            accessor = column
+        else:
+            try:
+                accessor = self._accessors[column]
+            except IndexError:
+                # Column specified as an integer, but the integer is out of range.
+                raise ValueError(f"Column {column} does not exist")
+            except TypeError:
+                # Column specified as something other than int or str
+                raise ValueError("Column must be an integer or string")
 
-        Returns:
-            The absolute path(str) to the selected file or None
-        """
-        return self._impl.select_folder_dialog(title, initial_directory)
+        try:
+            # Remove column
+            self._impl.remove_column(accessor)
+            del self.headings[self._accessors.index(accessor)]
+            self._accessors.remove(accessor)
+        except KeyError:
+            raise ValueError(f'Invalid column: "{column}"')
+
+    @property
+    def missing_value(self):
+        return self._missing_value
```

### Comparing `toga-core-0.3.0.dev9/toga/resources/tiberius.icns` & `toga-core-0.3.1/src/toga/resources/toga.icns`

 * *Files identical despite different names*

### Comparing `toga-core-0.3.0.dev9/toga/resources/tiberius-32.png` & `toga-core-0.3.1/src/toga/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga-core-0.3.0.dev9/toga/handlers.py` & `toga-core-0.3.1/src/toga/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,85 @@
 import asyncio
 import inspect
 import sys
 import traceback
 
 
-async def long_running_task(generator, cleanup):
-    """Run a generator as an asynchronous coroutine
+class NativeHandler:
+    def __init__(self, handler):
+        self.native = handler
 
-    """
+
+async def long_running_task(generator, cleanup):
+    """Run a generator as an asynchronous coroutine."""
     try:
         while True:
             delay = next(generator)
             await asyncio.sleep(delay)
     except StopIteration:
         if cleanup:
             cleanup()
     except Exception as e:
-        print('Error in long running handler:', e, file=sys.stderr)
+        print("Error in long running handler:", e, file=sys.stderr)
         traceback.print_exc()
 
 
 async def handler_with_cleanup(handler, cleanup, interface, *args, **kwargs):
     try:
-        await handler(interface, *args, **kwargs)
+        result = await handler(interface, *args, **kwargs)
         if cleanup:
-            cleanup()
+            cleanup(interface, result)
     except Exception as e:
-        print('Error in async handler:', e, file=sys.stderr)
+        print("Error in async handler:", e, file=sys.stderr)
         traceback.print_exc()
 
 
 def wrapped_handler(interface, handler, cleanup=None):
     """Wrap a handler provided by the user so it can be invoked.
 
+    If the handler is a NativeHandler, return the handler object
+        contained in the NativeHandler.
     If the handler is a bound method, or function, invoke it as it,
         and return the result.
     If the handler is a generator, invoke it asynchronously, with
         the yield values from the generator representing the duration
         to sleep between iterations.
     If the handler is a coroutine, install it on the asynchronous
         event loop.
 
-    Returns a wrapped function that will invoke the handler, using
-    the interface as context. The wrapper function is annotated with
-    the original handler function on the `_raw` attribute.
+    Returns either the native handler, or a wrapped function that will
+    invoke the handler, using the interface as context. If a non-native
+    handler, the wrapper function is annotated with the original handler
+    function on the `_raw` attribute.
     """
     if handler:
+        if isinstance(handler, NativeHandler):
+            return handler.native
+
         def _handler(widget, *args, **kwargs):
             if asyncio.iscoroutinefunction(handler):
                 asyncio.ensure_future(
                     handler_with_cleanup(handler, cleanup, interface, *args, **kwargs)
                 )
             else:
                 result = handler(interface, *args, **kwargs)
                 if inspect.isgenerator(result):
-                    asyncio.ensure_future(
-                        long_running_task(result, cleanup)
-                    )
+                    asyncio.ensure_future(long_running_task(result, cleanup))
                 else:
                     try:
                         if cleanup:
-                            cleanup()
+                            cleanup(interface, result)
                         return result
                     except Exception as e:
-                        print('Error in handler:', e, file=sys.stderr)
+                        print("Error in handler:", e, file=sys.stderr)
                         traceback.print_exc()
 
         _handler._raw = handler
 
-        return _handler
+    else:
+        # A dummy no-op handler
+        def _handler(widget, *args, **kwargs):
+            pass
+
+        _handler._raw = None
+
+    return _handler
```

### Comparing `toga-core-0.3.0.dev9/toga/app.py` & `toga-core-0.3.1/src/toga/widgets/detailedlist.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,176 @@
-import os
-import signal
-import sys
-from builtins import id as identifier
+import warnings
 
-from toga.command import CommandSet
 from toga.handlers import wrapped_handler
-from toga.platform import get_platform_factory
-from toga.widgets.icon import Icon
-from toga.window import Window
+from toga.sources import ListSource
 
+from .base import Widget
 
-class MainWindow(Window):
-    _WINDOW_CLASS = 'MainWindow'
 
-    def __init__(self, id=None, title=None, position=(100, 100), size=(640, 480), factory=None):
-        super().__init__(id=id, title=title, position=position, size=size, factory=factory)
-
-
-class App:
-    """ The App is the top level of any GUI program. It is the manager of all
-    the other bits of the GUI app: the main window and events that window
-    generates like user input.
-
-    When you create an App you need to provide it a name, an id for uniqueness
-    (by convention, the identifier is a "reversed domain name".) and an
-    optional startup function which should run once the App has initialised.
-    The startup function typically constructs some initial user interface.
-
-    Once the app is created you should invoke the main_loop() method, which
-    will hand over execution of your program to Toga to make the App interface
-    do its thing.
+class DetailedList(Widget):
+    """A widget to hold data in a list form. Rows are selectable and can be
+    deleted. An updated function can be invoked by pulling the list down.
 
     Args:
-        name (str): Is the name of the application.
-        app_id (str): The unique application identifier, the reversed domain name, e.g. 'org.pybee.me'
-        icon (str): Path to the icon for the application.
-        id (str): The DOM identifier for the app (optional)
-        startup(``callable``): The callback method before starting the app, typically to add the components.
-            Must be a ``callable`` that expects a single argument of :class:`toga.App`.
-        document_types (:obj:`list` of :obj:`str`): Document types.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
+        id (str): An identifier for this widget.
+        data (list of `dict`): List of dictionaries with required 'icon', 'title', and
+            'subtitle' keys as well as optional custom keys to store additional
+            info like 'pk' for a database primary key (think Django ORM)
+        on_delete (``Callable``): Function that is invoked on row deletion.
+        on_refresh (``Callable``): Function that is invoked on user initialized refresh.
+        on_select (``Callable``): Function that is invoked on row selection.
+        style (:obj:`Style`): An optional style object. If no style is provided then
+            a new one will be created for the widget.
 
     Examples:
-        >>> # Here is the absolute minimum App::
-        >>> app = toga.App('Empty App', 'org.pybee.empty')
-        >>> app.main_loop()
+        >>> import toga
+        >>> def selection_handler(widget, row):
+        >>>     print('Row {} of widget {} was selected.'.format(row, widget))
+        >>>
+        >>> dlist = toga.DetailedList(
+        ...     data=[
+        ...         {
+        ...             'icon': '',
+        ...             'title': 'John Doe',
+        ...             'subtitle': 'Employee of the Month',
+        ...             'pk': 100
+        ...          }
+        ...      ],
+        ...      on_select=selection_handler
+        ... )
     """
-    app = None
-
-    def __init__(self, name, app_id,
-                 id=None, icon=None, startup=None, document_types=None, on_exit=None, factory=None):
-        self.factory = get_platform_factory(factory)
-
-        # Keep an accessible copy of the app instance
-        App.app = self
-        App.app_module = self.__module__.split('.')[0]
-        App.app_dir = os.path.dirname(sys.modules[App.app_module].__file__)
 
-        self.name = name
-        self._app_id = app_id
-        self._id = id if id else identifier(self)
+    MIN_HEIGHT = 100
+    MIN_WIDTH = 100
 
-        self.commands = CommandSet(None)
+    def __init__(
+        self,
+        id=None,
+        data=None,
+        on_delete=None,
+        on_refresh=None,
+        on_select=None,
+        style=None,
+        factory=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
+
+        self._data = None
+        self._on_delete = None
+        self._on_refresh = None
+        # at least _on_select must be defined before setting data for the Gtk impl
+        self._on_select = None
+        self._impl = self.factory.DetailedList(interface=self)
+
+        self.data = data
+        self.on_delete = on_delete
+        self.on_refresh = on_refresh
+        self.on_select = on_select
+
+    @property
+    def data(self):
+        """The data source of the widget. It accepts data in the form of
+        ``list`` of ``dict`` or :class:`ListSource`
+
+        Returns:
+            Returns a (:obj:`ListSource`).
+        """
+        return self._data
+
+    @data.setter
+    def data(self, data):
+        if data is None:
+            self._data = ListSource(data=[], accessors=["icon", "title", "subtitle"])
+        elif isinstance(data, (list, tuple)):
+            self._data = ListSource(data=data, accessors=["icon", "title", "subtitle"])
+        else:
+            self._data = data
+
+        self._data.add_listener(self._impl)
+        self._impl.change_source(source=self._data)
+
+    def scroll_to_top(self):
+        """Scroll the view so that the top of the list (first row) is
+        visible."""
+        self.scroll_to_row(0)
 
-        self.document_types = document_types
-        self._documents = []
-
-        self._startup_method = startup
-
-        self.default_icon = Icon('tiberius', system=True)
-        self.icon = icon
-        self._main_window = None
-        self._on_exit = None
-
-        self._impl = self.factory.App(interface=self)
-        self.on_exit = on_exit
-
-    @property
-    def app_id(self):
-        """ The identifier for the app.
-        This is the reversed domain name, often used for targetting resources, etc.
+    def scroll_to_row(self, row):
+        """Scroll the view so that the specified row index is visible.
 
-        Returns:
-            The identifier as a ``str``.
+        Args:
+            row: The index of the row to make visible. Negative values refer
+                 to the nth last row (-1 is the last row, -2 second last,
+                 and so on)
         """
-        return self._app_id
+        if row >= 0:
+            self._impl.scroll_to_row(row)
+        else:
+            self._impl.scroll_to_row(len(self.data) + row)
 
-    @property
-    def id(self):
-        """ The DOM identifier for the app. This id can be used to target CSS directives.
-
-        Returns:
-            The identifier for the app as a ``str``.
-        """
-        return self._id
+    def scroll_to_bottom(self):
+        """Scroll the view so that the bottom of the list (last row) is
+        visible."""
+        self.scroll_to_row(-1)
 
     @property
-    def icon(self):
-        """ The Icon for the app. On setting, the icon is loaded automatically.
+    def on_delete(self):
+        """The function invoked on row deletion. The delete handler must accept
+        two arguments. The first is a ref. to the widget and the second the row
+        that is about to be deleted.
 
-        Returns:
-            The icon of the app ``toga.Icon``.
-        """
-        return self._icon
-
-    @icon.setter
-    def icon(self, name):
-        self._icon = Icon.load(name, default=self.default_icon)
-
-    @property
-    def main_window(self):
-        """The main Windows for the app.
+        Examples:
+            >>> def delete_handler(widget, row):
+            >>>     print('row ', row, 'is going to be deleted from widget', widget)
 
         Returns:
-            The main Window of the app.
+            The function that is invoked when deleting a row.
         """
-        return self._main_window
+        return self._on_delete
 
-    @main_window.setter
-    def main_window(self, window):
-        self._main_window = window
-        window.app = self
+    @on_delete.setter
+    def on_delete(self, handler: callable):
+        self._on_delete = wrapped_handler(self, handler)
+        self._impl.set_on_delete(self._on_delete)
 
     @property
-    def documents(self):
-        """ Return the list of documents associated with this app.
-
-        Returns:
-            A ``list`` of ``str``.
-        """
-        return self._documents
-
-    def add_document(self, doc):
-        """ Add a new document to this app.
-
-        Args:
-            doc (str): The document to add.
-        """
-        doc.app = self
-        self._documents.append(doc)
-
-    def open_document(self, fileURL):
-        """ Add a new document to this app.
-
-        Args:
-            fileURL (str): The URL/path to the file to add as a document.
+    def on_refresh(self):
         """
-        raise NotImplementedError('Application class must define open_document()')
-
-    def startup(self):
-        """ Create and show the main window for the application
+        Returns:
+            The function to be invoked on user initialized refresh.
         """
-        self.main_window = MainWindow(title=self.name, factory=self.factory)
-
-        if self._startup_method:
-            self.main_window.content = self._startup_method(self)
-
-        self.main_window.show()
+        return self._on_refresh
 
-    def main_loop(self):
-        """ Invoke the application to handle user input.
-        This method typically only returns once the application is exiting.
-        """
-        # Modify signal handlers to make sure Ctrl-C is caught and handled.
-        signal.signal(signal.SIGINT, signal.SIG_DFL)
+    @on_refresh.setter
+    def on_refresh(self, handler: callable):
+        self._on_refresh = wrapped_handler(self, handler, self._impl.after_on_refresh)
+        self._impl.set_on_refresh(self._on_refresh)
 
-        self._impl.main_loop()
+    @property
+    def selection(self):
+        """The current selection.
 
-    def exit(self):
-        """ Quit the application gracefully.
+        A value of None indicates no selection.
         """
-        self._impl.exit()
+        return self._impl.get_selection()
 
     @property
-    def on_exit(self):
-        """The handler to invoke before the application exits.
+    def on_select(self):
+        """The handler function must accept two arguments, widget and row.
 
         Returns:
-            The function ``callable`` that is called on application exit.
+            The function to be invoked on selecting a row.
         """
-        return self._on_exit
-
-    @on_exit.setter
-    def on_exit(self, handler):
-        """Set the handler to invoke before the app exits.
+        return self._on_select
 
-        Args:
-            handler (:obj:`callable`): The handler to invoke before the app exits.
-        """
-        self._on_exit = wrapped_handler(self, handler)
-        self._impl.set_on_exit(self._on_exit)
+    @on_select.setter
+    def on_select(self, handler: callable):
+        self._on_select = wrapped_handler(self, handler)
+        self._impl.set_on_select(self._on_select)
```

### Comparing `toga-core-0.3.0.dev9/toga/sources/accessors.py` & `toga-core-0.3.1/src/toga/sources/accessors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
+NON_ACCESSOR_CHARS = re.compile(r"[^\w ]")
+WHITESPACE = re.compile(r"\s+")
 
-NON_ACCESSOR_CHARS = re.compile('[^\w ]')
-WHITESPACE = re.compile('\s+')
 
 def to_accessor(heading):
-    """Convert a human-readable heading into a data attribute accessor
+    """Convert a human-readable heading into a data attribute accessor.
 
     This won't be infallible; for ambiguous cases, you'll need to manually
     specify the accessors.
 
     Examples:
         'Heading 1' -> 'heading_1'
         'Heading - Title' -> 'heading_title'
@@ -18,55 +18,57 @@
     Args:
         heading (``str``): The column heading.
 
     Returns:
         the accessor derived from the heading.
     """
     value = WHITESPACE.sub(
-        ' ',
-        NON_ACCESSOR_CHARS.sub('', heading.lower()),
-    ).replace(' ', '_')
+        " ",
+        NON_ACCESSOR_CHARS.sub("", heading.lower()),
+    ).replace(" ", "_")
 
     if len(value) == 0 or value[0].isdigit():
-        raise ValueError("Unable to automatically generate accessor from heading '{}'.".format(heading))
+        raise ValueError(
+            f"Unable to automatically generate accessor from heading '{heading}'."
+        )
 
     return value
 
+
 def build_accessors(headings, accessors):
-    """Convert a list of headings (with accessor overrides) to a finalised list of accessors.
+    """Convert a list of headings (with accessor overrides) to a finalised list
+    of accessors.
 
     Args:
         headings: a list of strings to be used as headings
         accessors: the accessor overrides. Can be:
          - A list, same length as headings. Each entry is
            a string providing the override name for the accessor,
            or None, indicating the default accessor should be used.
          - A dictionary from the heading names to the accessor. If
-           a heading name isn't present in the dictonary, the default
+           a heading name isn't present in the dictionary, the default
            accessor will be used
          - Otherwise, a final list of ready-to-use accessors.
 
     Returns:
-        A finalized list of accessors.
-
+        A finalised list of accessors.
     """
     if accessors:
         if isinstance(accessors, dict):
             result = [
-                accessors[h] if h in accessors else to_accessor(h)
-                for h in headings
+                accessors[h] if h in accessors else to_accessor(h) for h in headings
             ]
         else:
             if len(headings) != len(accessors):
-                raise ValueError('Number of accessors must match number of headings')
+                raise ValueError("Number of accessors must match number of headings")
 
             result = [
                 a if a is not None else to_accessor(h)
                 for h, a in zip(headings, accessors)
             ]
     else:
         result = [to_accessor(h) for h in headings]
 
     if len(result) != len(set(result)):
-        raise ValueError('Data accessors are not unique.')
+        raise ValueError("Data accessors are not unique.")
 
     return result
```

### Comparing `toga-core-0.3.0.dev9/toga/sources/tree_source.py` & `toga-core-0.3.1/src/toga/sources/tree_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __iter__(self):
         return iter(self._children or [])
 
     def __setitem__(self, index, value):
         node = self._source._create_node(value)
         self._children[index] = node
-        self._source._notify('change', item=node)
+        self._source._notify("change", item=node)
 
     def insert(self, index, *values, **named):
         self._source.insert(self, index, *values, **named)
 
     def prepend(self, *values, **named):
         self._source.prepend(self, *values, **named)
 
@@ -61,14 +61,17 @@
 
     def __len__(self):
         return len(self._roots)
 
     def __getitem__(self, index):
         return self._roots[index]
 
+    def can_have_children(self):
+        return True
+
     ######################################################################
     # Factory methods for new nodes
     ######################################################################
 
     def _create_node(self, data, children=None):
         if isinstance(data, dict):
             node = Node(**data)
@@ -89,58 +92,63 @@
     def _create_nodes(self, data):
         if isinstance(data, dict):
             return [
                 self._create_node(value, children)
                 for value, children in sorted(data.items())
             ]
         else:
-            return [
-                self._create_node(value)
-                for value in data
-            ]
+            return [self._create_node(value) for value in data]
 
     ######################################################################
     # Utility methods to make TreeSources more dict-like
     ######################################################################
 
     def __setitem__(self, index, value):
         root = self._create_node(value)
         self._roots[index] = root
-        self._notify('change', item=root)
+        self._notify("change", item=root)
 
     def __iter__(self):
         return iter(self._roots)
 
+    def clear(self):
+        self._roots = []
+        self._notify("clear")
+
     def insert(self, parent, index, *values, **named):
         node = self._create_node(dict(zip(self._accessors, values), **named))
 
         if parent is None:
             self._roots.insert(index, node)
         else:
             if parent._children is None:
                 parent._children = []
             parent._children.insert(index, node)
 
         node._parent = parent
-        self._notify('insert', parent=parent, index=index, item=node)
+        self._notify("insert", parent=parent, index=index, item=node)
         return node
 
     def prepend(self, parent, *values, **named):
         return self.insert(parent, 0, *values, **named)
 
     def append(self, parent, *values, **named):
         return self.insert(parent, len(parent or self), *values, **named)
 
     def remove(self, node):
+        i = self.index(node)
+        parent = node._parent
         if node._parent is None:
-            self._roots.remove(node)
+            del self._roots[i]
         else:
-            node._parent._children.remove(node)
+            del node._parent._children[i]
+            # node is not in parent's children so it shouldn't keep a link to parent
+            del node._parent
 
-        self._notify('remove', item=node)
+        self._notify("remove", parent=parent, index=i, item=node)
         return node
 
     def index(self, node):
         if node._parent:
             return node._parent._children.index(node)
         else:
             return self._roots.index(node)
```

### Comparing `toga-core-0.3.0.dev9/toga/sources/list_source.py` & `toga-core-0.3.1/src/toga/sources/list_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,29 +12,31 @@
     # Utility wrappers
     ######################################################################
 
     def __setattr__(self, attr, value):
         super().__setattr__(attr, value)
         if attr in self._attrs:
             if self._source is not None:
-                self._source._notify('change', item=self)
+                self._source._notify("change", item=self)
 
 
 class ListSource(Source):
-    """A data source to store a list of multiple data values, in a row-like fashion.
+    """A data source to store a list of multiple data values, in a row-like
+    fashion.
 
     Args:
         data (`list`): The data in the list. Each entry in the list should have the
-            same number of entries as there are accessors. 
+            same number of entries as there are accessors.
         accessors (`list`): A list of attribute names for accessing the value
             in each column of the row.
     """
+
     def __init__(self, data, accessors):
         super().__init__()
-        self._accessors = accessors
+        self._accessors = accessors.copy()
         self._data = []
         for value in data:
             self._data.append(self._create_row(value))
 
     ######################################################################
     # Methods required by the ListSource interface
     ######################################################################
@@ -47,60 +49,62 @@
 
     ######################################################################
     # Factory methods for new rows
     ######################################################################
 
     def _create_row(self, data):
         """Create a Row object from the given data.
+
         Args:
             data (any): The type of `data` determines how it is handled
                 ``dict``: each key corresponds to a column accessor
                 iterables, except ``str`` and ``dict``: each item corresponds to a column
                 all else: `data` will fill the first column
         """
 
         if isinstance(data, dict):
             row = Row(**data)
-        elif hasattr(data, '__iter__') and not isinstance(data, str):
+        elif hasattr(data, "__iter__") and not isinstance(data, str):
             row = Row(**dict(zip(self._accessors, data)))
         else:
             row = Row(**{self._accessors[0]: data})
         row._source = self
         return row
 
     ######################################################################
     # Utility methods to make ListSources more list-like
     ######################################################################
 
     def __setitem__(self, index, value):
         row = self._create_row(value)
         self._data[index] = row
-        self._notify('insert', index=index, item=row)
+        self._notify("insert", index=index, item=row)
 
     def __iter__(self):
         return iter(self._data)
 
     def clear(self):
         self._data = []
-        self._notify('clear')
+        self._notify("clear")
 
     def insert(self, index, *values, **named):
         # Coalesce values and data into a single data dictionary,
         # and use that to create the data row. Explicitly named data override.
         row = self._create_row(dict(zip(self._accessors, values), **named))
         self._data.insert(index, row)
-        self._notify('insert', index=index, item=row)
+        self._notify("insert", index=index, item=row)
         return row
 
     def prepend(self, *values, **named):
         return self.insert(0, *values, **named)
 
     def append(self, *values, **named):
         return self.insert(len(self), *values, **named)
 
     def remove(self, row):
-        self._data.remove(row)
-        self._notify('remove', item=row)
+        i = self._data.index(row)
+        del self._data[i]
+        self._notify("remove", index=i, item=row)
         return row
 
     def index(self, row):
         return self._data.index(row)
```

### Comparing `toga-core-0.3.0.dev9/toga/sources/base.py` & `toga-core-0.3.1/src/toga/sources/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-
-
 class Source:
     def __init__(self):
         self._listeners = []
 
     @property
     def listeners(self) -> list:
-        """ The listeners of this data source.
-        Listeners can be ``callable`` or :obj:``toga.Widget``.
+        """The listeners of this data source. Listeners can be ``callable`` or
+        :obj:``toga.Widget``.
 
         Returns:
             A list of objects that are listening for data change.
         """
         return self._listeners
 
     def add_listener(self, listener):
@@ -21,15 +19,16 @@
         """
         self._listeners.append(listener)
 
     def remove_listener(self, listener):
         self._listeners.remove(listener)
 
     def _notify(self, notification, **kwargs):
-        """Invoke a notification function on all listeners that are subscribed to this data source."""
+        """Invoke a notification function on all listeners that are subscribed
+        to this data source."""
         for listener in self._listeners:
             try:
                 method = getattr(listener, notification)
             except AttributeError:
                 method = None
 
             if method:
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/imageview.py` & `toga-core-0.3.1/src/toga/widgets/imageview.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,61 @@
-from .base import Widget
+import warnings
+
+from toga.images import Image
+from toga.widgets.base import Widget
 
 
 class ImageView(Widget):
     """
 
     Args:
-        image (:class:`toga.Image`): The image to display.
+        image (:class:`~toga.images.Image`): The image to display.
         id (str): An identifier for this widget.
         style (:obj:`Style`):
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
 
     Todo:
         * Finish implementation.
     """
 
-    def __init__(self, image=None,
-                 id=None, style=None, factory=None, ):
-        super().__init__(id=id, style=style, factory=factory)
+    def __init__(
+        self,
+        image=None,
+        id=None,
+        style=None,
+        factory=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
 
         self._impl = self.factory.ImageView(interface=self)
         self.image = image
 
     @property
     def image(self):
-        self._impl.get_image()
         return self._image
 
     @image.setter
     def image(self, image):
-        self._image = image
-        self._impl.set_image(self._image)
-        self._impl.rehint()
+        if isinstance(image, str):
+            self._image = Image(image)
+        else:
+            self._image = image
+
+        if self._image is not None:
+            self._impl.set_image(image)
+            self.refresh()
 
         # @property
         # def alignment(self):
         #     return self._alignment
 
         # @alignment.setter
         # def alignment(self, value):
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/detailedlist.py` & `toga-core-0.3.1/src/toga/widgets/timepicker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,157 @@
+import datetime
+import warnings
+
 from toga.handlers import wrapped_handler
-from toga.sources import ListSource
 
 from .base import Widget
 
 
-class DetailedList(Widget):
-    """ A widget to hold data in a list form. Rows are selectable and can be deleted.
-    A updated function can be invoked by pulling the list down.
+class TimePicker(Widget):
+    """A widget to get user selected datetime object.
 
     Args:
         id (str): An identifier for this widget.
-        data (list of `str`): List of strings which to display on the widget.
-        on_delete (``callable``): Function that is invoked on row deletion.
-        on_refresh (``callable``): Function that is invoked on user initialised refresh.
-        on_select (``callable``): Function that is invoked on row selection.
         style (:obj:`Style`): An optional style object. If no style is provided then
             a new one will be created for the widget.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
-
-    Examples:
-        >>> import toga
-        >>> def selection_handler(widget, selection):
-        >>>     print('Row {} of widget {} was selected.'.format(selection, widget))
-        >>>
-        >>> dlist = toga.DetailedList(data=['Item 0', 'Item 1', 'Item 2'], on_select=selection_handler)
+        value (str): The initial value to set the widget to. (Defaults to time of program execution)
+        min_time (str): The minimum allowable time for the widget.
+        max_time (str): The maximum allowable time for the widget.
+        on_change (``callable``): Function that is invoked on time value change.
     """
-    MIN_HEIGHT = 100
+
     MIN_WIDTH = 100
 
-    def __init__(self, id=None, data=None, on_delete=None, on_refresh=None, on_select=None, style=None, factory=None):
-        super().__init__(id=id, style=style, factory=factory)
-        self._data = None
-        self._impl = self.factory.DetailedList(interface=self)
-
-        self.data = data
-        self.on_delete = on_delete
-        self.on_refresh = on_refresh
-        self.on_select = on_select
+    def __init__(
+        self,
+        id=None,
+        style=None,
+        factory=None,  # DEPRECATED!
+        value=None,
+        min_time=None,
+        max_time=None,
+        on_change=None,
+        initial=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
+
+        self._on_change = None
+
+        # Create a platform specific implementation of a TimePicker
+        self._impl = self.factory.TimePicker(interface=self)
+
+        ##################################################################
+        # 2022-07: Backwards compatibility
+        ##################################################################
+
+        # initial replaced with value
+        if initial is not None:
+            if value is not None:
+                raise ValueError(
+                    "Cannot specify both `initial` and `value`; "
+                    "`initial` has been deprecated, use `value`"
+                )
+            else:
+                warnings.warn("`initial` has been renamed `value`", DeprecationWarning)
+            value = initial
+
+        ##################################################################
+        # End backwards compatibility.
+        ##################################################################
+
+        self.min_time = min_time
+        self.max_time = max_time
+        # Set the value after the min/max has been set
+        self.value = value
+        # Set the change handler after the initial value has been set
+        self.on_change = on_change
 
     @property
-    def data(self):
-        """ The data source of the widget. It accepts table data
-        in the form of ``list``, ``tuple``, or :obj:`ListSource`
-
-        Returns:
-            Returns a (:obj:`ListSource`).
-        """
-        return self._data
+    def value(self):
+        """The value of the currently selected time.
 
-    @data.setter
-    def data(self, data):
-        if data is None:
-            self._data = ListSource(data=[], accessors=['icon', 'label1', 'label2'])
-        elif isinstance(data, (list, tuple)):
-            self._data = ListSource(data=data, accessors=['icon', 'label1', 'label2'])
-        else:
-            self._data = data
-
-        self._data.add_listener(self._impl)
-        self._impl.change_source(source=self._data)
-
-    def scroll_to_top(self):
-        """Scroll the view so that the top of the list (first row) is visible
+        :return: Selected time as time object
         """
-        self.scroll_to_row(0)
+        return self._impl.get_value()
 
-    def scroll_to_row(self, row):
-        """Scroll the view so that the specified row index is visible.
-
-        Args:
-            row: The index of the row to make visible. Negative values refer
-                 to the nth last row (-1 is the last row, -2 second last,
-                 and so on)
-        """
-        if row >= 0:
-            self._impl.scroll_to_row(row)
+    def _convert_time(self, value):
+        if value is None:
+            return datetime.datetime.today().time().replace(microsecond=0)
+        elif isinstance(value, datetime.time):
+            return value
+        elif isinstance(value, datetime.datetime):
+            return value.time()
+        elif isinstance(value, str):
+            return datetime.time.fromisoformat(value)
         else:
-            self._impl.scroll_to_row(len(self.data) + row)
+            raise TypeError("not a valid time value")
 
-    def scroll_to_bottom(self):
-        """Scroll the view so that the bottom of the list (last row) is visible
-        """
-        self.scroll_to_row(-1)
+    @value.setter
+    def value(self, value):
+        self._impl.set_value(self._convert_time(value))
 
     @property
-    def on_delete(self):
-        """ The function invoked on row deletion. The delete handler must accept two arguments.
-        The first is a ref. to the widget and the second the row that is about to be deleted.
-
-        Examples:
-            >>> def delete_handler(widget, row):
-            >>>     print('row ', row, 'is going to be deleted from widget', widget)
-
-        Returns:
-            The function that is invoked when deleting a row.
-        """
-        return self._on_delete
-
-    @on_delete.setter
-    def on_delete(self, handler: callable):
-        self._on_delete = wrapped_handler(self, handler)
-        self._impl.set_on_delete(self._on_delete)
+    def min_time(self):
+        """The minimum allowable time for the widget. The widget will not allow
+        the user to enter at time less than the min time. If initial time set
+        is less than the minimum time, the minimum time will be used as the
+        initial value.
+
+        :return: The minimum time specified. Returns None if min_time not specified
+        """
+        return self._min_time
+
+    @min_time.setter
+    def min_time(self, value):
+        if value is None:
+            self._min_time = None
+        else:
+            self._min_time = self._convert_time(value)
+        self._impl.set_min_time(self._min_time)
 
     @property
-    def on_refresh(self):
-        """
-        Returns:
-            The function to be invoked on user initialised refresh.
-        """
-        return self._on_refresh
+    def max_time(self):
+        """The maximum allowable time for the widget. The widget will not allow
+        the user to enter at time greater than the max time. If initial time
+        set is greater than the maximum time, the maximum time will be used as
+        the initial value.
+
+        :return: The maximum time specified. Returns None if max_time not specified
+        """
+        return self._max_time
+
+    @max_time.setter
+    def max_time(self, value):
+        if value is None:
+            self._max_time = None
+        else:
+            self._max_time = self._convert_time(value)
 
-    @on_refresh.setter
-    def on_refresh(self, handler: callable):
-        self._on_refresh = wrapped_handler(self, handler, self._impl.after_on_refresh)
-        self._impl.set_on_refresh(self._on_refresh)
+        self._impl.set_max_time(self._max_time)
 
     @property
-    def on_select(self):
-        """ The handler function must accept two arguments, widget and row.
+    def on_change(self):
+        """The handler to invoke when the value changes.
 
         Returns:
-            The function to be invoked on selecting a row.
+            The function ``callable`` that is called on a content change.
         """
-        return self._on_select
+        return self._on_change
 
-    @on_select.setter
-    def on_select(self, handler: callable):
-        self._on_select = wrapped_handler(self, handler)
-        self._impl.set_on_select(self._on_select)
+    @on_change.setter
+    def on_change(self, handler):
+        """Set the handler to invoke when the date is changed.
 
+        Args:
+            handler (:obj:`callable`): The handler to invoke when the date is changed.
+        """
+        self._on_change = wrapped_handler(self, handler)
+        self._impl.set_on_change(self._on_change)
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/textinput.py` & `toga-core-0.3.1/src/toga/widgets/switch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,104 +1,92 @@
 from toga.handlers import wrapped_handler
 
 from .base import Widget
 
 
-class TextInput(Widget):
-    """ A widget get user input.
-
-    Args:
-        id (str): An identifier for this widget.
-        style (:obj:`Style`): An optional style object. If no style is provided then
-            a new one will be created for the widget.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
-        initial (str): The initial text for the input.
-        placeholder (str): If no input is present this text is shown.
-        readonly (bool):  Whether a user can write into the text input, defaults to `False`.
-    """
-    MIN_WIDTH = 100
-
+class Switch(Widget):
     def __init__(
-            self, id=None, style=None, factory=None,
-            initial=None, placeholder=None, readonly=False, on_change=None):
-        super().__init__(id=id, style=style, factory=factory)
-
-        # Create a platform specific implementation of a TextInput
-        self._impl = self.factory.TextInput(interface=self)
-
-        self.value = initial
-        self.placeholder = placeholder
-        self.readonly = readonly
-        self.on_change = on_change
-
-    @property
-    def readonly(self):
-        """ Whether a user can write into the text input
-
-        Returns:
-            ``True`` if only read is possible.
-            ``False`` if read and write is possible.
+        self,
+        text,
+        id=None,
+        style=None,
+        on_change=None,
+        value=False,
+        enabled=True,
+    ):
+        """Create a new Switch widget.
+
+        Inherits from :class:`~toga.widgets.base.Widget`.
+
+        :param text: The text to display beside the switch.
+        :param id: The ID for the widget.
+        :param style: A style object. If no style is provided, a default style
+            will be applied to the widget.
+        :param on_change: A handler that will be invoked when the switch changes
+            value.
+        :param enabled: Is the switch enabled (i.e., can it be pressed?).
+            Optional; by default, switches are created in an enabled state.
         """
-        return self._readonly
+        super().__init__(id=id, style=style)
 
-    @readonly.setter
-    def readonly(self, value):
-        self._readonly = value
-        self._impl.set_readonly(value)
+        self._impl = self.factory.Switch(interface=self)
 
-    @property
-    def placeholder(self):
-        """ The placeholder text.
+        self.text = text
 
-        Returns:
-            The placeholder text as a ``str``.
-        """
-        return self._placeholder
+        # Set a dummy handler before installing the actual on_change, because we do not want
+        # on_change triggered by the initial value being set
+        self.on_change = None
+        self.value = value
 
-    @placeholder.setter
-    def placeholder(self, value):
-        if value is None:
-            self._placeholder = ''
-        else:
-            self._placeholder = str(value)
-        self._impl.set_placeholder(value)
+        self.on_change = on_change
+
+        self.enabled = enabled
 
     @property
-    def value(self):
-        """ The value of the text input field
+    def text(self):
+        """The text label for the Switch.
+
+        ``None``, and the Unicode codepoint U+200B (ZERO WIDTH SPACE), will be
+        interpreted and returned as an empty string. Any other object will be
+        converted to a string using ``str()``.
 
-        Returns:
-            The current text of the widget as a ``str``.
+        Only one line of text can be displayed. Any content after the first
+        newline will be ignored.
         """
-        return self._impl.get_value()
+        return self._impl.get_text()
 
-    @value.setter
-    def value(self, value):
-        if value is None:
-            v = ''
+    @text.setter
+    def text(self, value):
+        if value is None or value == "\u200B":
+            value = ""
         else:
-            v = str(value)
-        self._impl.set_value(v)
+            # Switch text can't include line breaks. Strip any content
+            # after a line break (if provided)
+            value = str(value).split("\n")[0]
 
-    def clear(self):
-        """ Clears the text of the widget """
-        self.value = ''
+        self._impl.set_text(value)
+        self.refresh()
 
     @property
     def on_change(self):
-        """The handler to invoke when the value changes
-
-        Returns:
-            The function ``callable`` that is called on a content change.
-        """
+        """The handler to invoke when the value of the switch changes."""
         return self._on_change
 
     @on_change.setter
     def on_change(self, handler):
-        """Set the handler to invoke when the value is changeed.
+        self._on_change = wrapped_handler(self, handler)
+
+    @property
+    def value(self):
+        """The current state of the switch, as a Boolean.
 
-        Args:
-            handler (:obj:`callable`): The handler to invoke when the value is changeed.
+        Any non-Boolean value will be converted to a Boolean.
         """
-        self._on_change = wrapped_handler(self, handler)
-        self._impl.set_on_change(self._on_change)
+        return self._impl.get_value()
+
+    @value.setter
+    def value(self, value):
+        self._impl.set_value(bool(value))
+
+    def toggle(self):
+        """Reverse the current value of the switch."""
+        self.value = not self.value
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/slider.py` & `toga-core-0.3.1/src/toga/widgets/selection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,100 @@
+import warnings
+
 from toga.handlers import wrapped_handler
 
 from .base import Widget
 
 
-class Slider(Widget):
-    """ Slider widget, displays a range of values
+class Selection(Widget):
+    """The Selection widget lets you pick from a defined selection of options.
 
     Args:
-        id: An identifier for this widget.
-        style (:obj:`Style`):
-        default (float): Default value of the slider
-        range (``tuple``): Min and max values of the slider in this form (min, max).
-        on_slide (``callable``): The function that is executed on_slide.
-        enabled (bool): Whether user interaction is possible or not.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
+        id (str): An identifier for this widget.
+        style ( :obj:`Style`): An optional style object.
+            If no style is provided then a new one will be created for the widget.
+        items (``list`` of ``str``): The items for the selection.
     """
-    MIN_WIDTH = 100
 
-    def __init__(self, id=None, style=None, default=None, range=None, on_slide=None, enabled=True, factory=None):
-        super().__init__(id=id, style=style, factory=factory)
-        self._on_slide = None # needed for _impl initialization
-        self._impl = self.factory.Slider(interface=self)
-
-        self.range = range
-        self.value = default
-        self.on_slide = on_slide
+    def __init__(
+        self,
+        id=None,
+        style=None,
+        items=None,
+        on_select=None,
+        enabled=True,
+        factory=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
+
+        self._on_select = None  # needed for _impl initialization
+        self._impl = self.factory.Selection(interface=self)
+
+        if items is None:
+            self._items = []
+        else:
+            self._items = items
+            for item in self._items:
+                self._impl.add_item(item)
+
+        self.on_select = on_select
         self.enabled = enabled
 
     @property
-    def value(self):
-        """ Current slider value.
+    def items(self):
+        """The list of items.
 
         Returns:
-            The current slider value as a ``float``.
-
-        Raises:
-            ValueError: If the new value is not in the range of min and max.
+             The ``list`` of ``str`` of all selectable items.
         """
-        self._value = self._impl.get_value()
-        return self._value
+        return self._items
 
-    @value.setter
-    def value(self, value):
-        _min, _max = self.range
-        if value is None:
-            self._value = 0.5
-        elif _min <= value <= _max:
-            self._value = value
-        else:
-            raise ValueError('Slider value ({}) is not in range ({}-{})'.format(value, _min, _max))
-        self._impl.set_value(self._value)
+    @items.setter
+    def items(self, items):
+        self._impl.remove_all_items()
+        self._items = items
+
+        for i in items:
+            self._impl.add_item(i)
 
     @property
-    def range(self):
-        """ Range composed of min and max slider value.
+    def value(self):
+        """The value of the currently selected item.
 
         Returns:
-            Returns the range in a ``tuple`` like this (min, max)
+            The selected item as a ``str``.
         """
-        return self._range
+        return self._impl.get_selected_item()
 
-    @range.setter
-    def range(self, range):
-        default_range = (0.0, 1.0)
-        _min, _max = default_range if range is None else range
-        if _min > _max or _min == _max:
-            raise ValueError('Range min value has to be smaller than max value.')
-        self._range = (_min, _max)
-        self._impl.set_range((_min, _max))
+    @value.setter
+    def value(self, value):
+        if value not in self._items:
+            raise ValueError("Not an item in the list.")
+
+        self._impl.select_item(value)
 
     @property
-    def on_slide(self):
-        """ The function for when the slider is slided
+    def on_select(self):
+        """The callable function for when a node on the Tree is selected.
 
-        Returns:
-            The ``callable`` that is executed on slide.
+        :rtype: ``callable``
         """
-        return self._on_slide
+        return self._on_select
 
-    @on_slide.setter
-    def on_slide(self, handler):
-        self._on_slide = wrapped_handler(self, handler)
-        self._impl.set_on_slide(self._on_slide)
+    @on_select.setter
+    def on_select(self, handler):
+        """Set the function to be executed on node selection.
+
+        :param handler:     callback function
+        :type handler:      ``callable``
+        """
+        self._on_select = wrapped_handler(self, handler)
+        self._impl.set_on_select(self._on_select)
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/navigationview.py` & `toga-core-0.3.1/src/toga/widgets/navigationview.py`

 * *Files identical despite different names*

### Comparing `toga-core-0.3.0.dev9/toga/widgets/label.py` & `toga-core-0.3.1/src/toga/widgets/label.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 from .base import Widget
 
 
 class Label(Widget):
-    """A text label.
-
-    Args:
-        text (str): Text of the label.
-        id (str): An identifier for this widget.
-        style (:obj:`Style`): An optional style object. If no style is provided then
-            a new one will be created for the widget.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional; normally not needed)
-    """
-
-    def __init__(self, text, id=None, style=None, factory=None):
-        super().__init__(id=id, style=style, factory=factory)
+    def __init__(
+        self,
+        text,
+        id=None,
+        style=None,
+    ):
+        """Create a new text label.
+
+        Inherits from :class:`~toga.widgets.base.Widget`.
+
+        :param text: Text of the label.
+        :param id: The ID for the widget.
+        :param style: A style object. If no style is provided, a default style
+            will be applied to the widget.
+        """
+        super().__init__(id=id, style=style)
 
         # Create a platform specific implementation of a Label
         self._impl = self.factory.Label(interface=self)
 
         self.text = text
 
+    def focus(self):
+        "No-op; Label cannot accept input focus"
+        pass
+
     @property
     def text(self):
         """The text displayed by the label.
 
-        Returns:
-            The text displayed by the label.
+        ``None``, and the Unicode codepoint U+200B (ZERO WIDTH SPACE), will be
+        interpreted and returned as an empty string. Any other object will be
+        converted to a string using ``str()``.
+
         """
-        return self._text
+        return self._impl.get_text()
 
     @text.setter
     def text(self, value):
-        if value is None:
-            self._text = ''
+        if value is None or value == "\u200B":
+            text = ""
         else:
-            self._text = str(value)
-        self._impl.set_text(value)
-        self._impl.rehint()
+            text = str(value)
+
+        self._impl.set_text(text)
+        self.refresh()
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/numberinput.py` & `toga-core-0.3.1/src/toga/widgets/numberinput.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,110 @@
+import warnings
 from decimal import Decimal, InvalidOperation
 
 from toga.handlers import wrapped_handler
 
 from .base import Widget
 
 
 class NumberInput(Widget):
-    """ A `NumberInput` widget specifies a fixed range of possible numbers.
-    The user has two buttons to increment/decrement the value by a step size.
-    Step, min and max can be integers, floats, or Decimals; They can also be specified
-    as strings, which will be converted to Decimals internally. The value of the
-    widget will be evaluated as a Decimal.
+    """A `NumberInput` widget specifies a fixed range of possible numbers. The
+    user has two buttons to increment/decrement the value by a step size. Step,
+    min and max can be integers, floats, or Decimals; They can also be
+    specified as strings, which will be converted to Decimals internally. The
+    value of the widget will be evaluated as a Decimal.
 
     Args:
         id (str): An identifier for this widget.
         style (:obj:`Style`):  an optional style object.
             If no style is provided then a new one will be created for the widget.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
 
         step (number): Step size of the adjustment buttons.
         min_value (number): The minimum bound for the widget's value.
         max_value (number): The maximum bound for the widget's value.
+        value (number): Initial value for the widget
         readonly (bool):  Whether a user can write/change the number input, defaults to `False`.
         on_change (``callable``): The handler to invoke when the value changes.
         **ex:
     """
-    MIN_WIDTH = 100
 
-    def __init__(self, id=None, style=None, factory=None, step=1,
-                 min_value=None, max_value=None, readonly=False, on_change=None):
-        super().__init__(id=id, style=style, factory=factory)
+    def __init__(
+        self,
+        id=None,
+        style=None,
+        factory=None,  # DEPRECATED!
+        step=1,
+        min_value=None,
+        max_value=None,
+        value=None,
+        readonly=False,
+        on_change=None,
+        default=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
+
         self._value = None
         self._on_change = None
         self._impl = self.factory.NumberInput(interface=self)
 
+        ##################################################################
+        # 2022-07: Backwards compatibility
+        ##################################################################
+
+        # default replaced with value
+        if default is not None:
+            if value is not None:
+                raise ValueError(
+                    "Cannot specify both `default` and `value`; "
+                    "`default` has been deprecated, use `value`"
+                )
+            else:
+                warnings.warn("`default` has been renamed `value`", DeprecationWarning)
+            value = default
+
+        ##################################################################
+        # End backwards compatibility.
+        ##################################################################
+
         self.readonly = readonly
         self.step = step
         self.min_value = min_value
         self.max_value = max_value
         self.on_change = on_change
 
+        if value is not None:
+            self.value = value
+
     @property
     def readonly(self):
-        """ Whether a user can write/change the number input
+        """Whether a user can write/change the number input.
 
         Returns:
             ``True`` if only read is possible.
             ``False`` if read and write is possible.
         """
         return self._readonly
 
     @readonly.setter
     def readonly(self, value):
         self._readonly = value
         self._impl.set_readonly(value)
 
     @property
     def step(self):
-        """The step value for the widget
+        """The step value for the widget.
 
         Returns:
             The current step value for the widget.
         """
         return self._step
 
     @step.setter
@@ -111,15 +153,15 @@
             raise ValueError("max_value must be a number")
         except TypeError:
             self._max_value = None
         self._impl.set_max_value(self._max_value)
 
     @property
     def value(self):
-        """Current value contained by the widget
+        """Current value contained by the widget.
 
         Returns:
             The current value(int) of the widget. Returns None
             if the field has no value set.
         """
         return self._value
 
@@ -137,23 +179,23 @@
         except TypeError:
             self._value = None
 
         self._impl.set_value(value)
 
     @property
     def on_change(self):
-        """The handler to invoke when the value changes
+        """The handler to invoke when the value changes.
 
         Returns:
             The function ``callable`` that is called on a content change.
         """
         return self._on_change
 
     @on_change.setter
     def on_change(self, handler):
-        """Set the handler to invoke when the value is changeed.
+        """Set the handler to invoke when the value is changed.
 
         Args:
-            handler (:obj:`callable`): The handler to invoke when the value is changeed.
+            handler (:obj:`callable`): The handler to invoke when the value is changed.
         """
         self._on_change = wrapped_handler(self, handler)
         self._impl.set_on_change(self._on_change)
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/passwordinput.py` & `toga-core-0.3.1/src/toga/widgets/button.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,73 @@
-from .base import Widget
-
+from toga.handlers import wrapped_handler
 
-class PasswordInput(Widget):
-    """ This widgets behaves like a TextInput but does not reveal what text is entered.
+from .base import Widget
 
-    Args:
-        id (str): An identifier for this widget.
-        style (:obj:`Style`): An optional style object. If no style is provided then
-            a new one will be created for the widget.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
-        initial (str): The initial text that is displayed before the user inputs anything.
-        placeholder (str): The text that is displayed if no input text is present.
-        readonly (bool): Whether a user can write into the text input, defaults to `False`.
-    """
-    MIN_WIDTH = 100
-
-    def __init__(self, id=None, style=None, factory=None,
-                initial=None, placeholder=None, readonly=False):
-        super().__init__(id=id, style=style, factory=factory)
-
-        # Create a platform specific implementation of a PasswordInput
-        self._impl = self.factory.PasswordInput(interface=self)
-
-        self.value = initial
-        self.placeholder = placeholder
-        self.readonly = readonly
 
-    @property
-    def readonly(self):
-        """ Whether a user can write into the password input
-
-        Returns:
-            ``True`` if the user can only read,
-            ``False`` if the user can read and write into the input.
+class Button(Widget):
+    def __init__(
+        self,
+        text,
+        id=None,
+        style=None,
+        on_press=None,
+        enabled=True,
+    ):
+        """Create a new button widget.
+
+        Inherits from :class:`~toga.widgets.base.Widget`.
+
+        :param text: The text to display on the button.
+        :param id: The ID for the widget.
+        :param style: A style object. If no style is provided, a default style
+            will be applied to the widget.
+        :param on_press: A handler that will be invoked when the button is
+            pressed.
+        :param enabled: Is the button enabled (i.e., can it be pressed?).
+            Optional; by default, buttons are created in an enabled state.
         """
-        return self._readonly
+        super().__init__(id=id, style=style)
 
-    @readonly.setter
-    def readonly(self, value):
-        self._readonly = value
-        self._impl.set_readonly(value)
+        # Create a platform specific implementation of a Button
+        self._impl = self.factory.Button(interface=self)
 
-    @property
-    def placeholder(self):
-        """ The placeholder text is the displayed before the user input something.
+        # Set a dummy handler before installing the actual on_press, because we do not want
+        # on_press triggered by the initial value being set
+        self.on_press = None
+        self.text = text
 
-        Returns:
-            The placeholder text (str) of the widget.
-        """
-        return self._placeholder
-
-    @placeholder.setter
-    def placeholder(self, value):
-        if value is None:
-            self._placeholder = ''
-        else:
-            self._placeholder = str(value)
-        self._impl.set_placeholder(self._placeholder)
-        self._impl.rehint()
+        self.on_press = on_press
+        self.enabled = enabled
 
     @property
-    def value(self):
-        """ The value of the text input field.
+    def text(self):
+        """The text displayed on the button.
+
+        ``None``, and the Unicode codepoint U+200B (ZERO WIDTH SPACE), will be
+        interpreted and returned as an empty string. Any other object will be
+        converted to a string using ``str()``.
 
-        Returns:
-            The text as a ``str`` of the password input widget.
+        Only one line of text can be displayed. Any content after the first
+        newline will be ignored.
         """
-        return self._impl.get_value()
+        return self._impl.get_text()
 
-    @value.setter
-    def value(self, value):
-        if value is None:
-            v = ''
+    @text.setter
+    def text(self, value):
+        if value is None or value == "\u200B":
+            value = ""
         else:
-            v = str(value)
-        self._impl.set_value(v)
-        self._impl.rehint()
+            # Button text can't include line breaks. Strip any content
+            # after a line break (if provided)
+            value = str(value).split("\n")[0]
 
-    def clear(self):
-        """ Clears the input field of the widget.
-        """
-        self.value = ''
+        self._impl.set_text(value)
+        self.refresh()
+
+    @property
+    def on_press(self):
+        """The handler to invoke when the button is pressed."""
+        return self._on_press
+
+    @on_press.setter
+    def on_press(self, handler):
+        self._on_press = wrapped_handler(self, handler)
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/table.py` & `toga-core-0.3.1/src/toga/widgets/tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,102 @@
+import warnings
+
 from toga.handlers import wrapped_handler
-from toga.sources import ListSource
+from toga.sources import TreeSource
 from toga.sources.accessors import build_accessors
 
 from .base import Widget
 
 
-class Table(Widget):
-    """ A Table Widget allows the display of data in the from of columns and rows.
-
-    Args:
-        headings (``list`` of ``str``): The list of headings for the table.
-        id (str): An identifier for this widget.
-        data (``list`` of ``tuple``): The data to be displayed on the table.
-        accessors: A list of methods, same length as ``headings``, that describes
-            how to extract the data value for each column from the row. (Optional)
-        style (:obj:`Style`): An optional style object.
-            If no style is provided` then a new one will be created for the widget.
-        on_select (``callable``): A function to be invoked on selecting a row of the table.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional & normally not needed)
-
-    Examples:
-        >>> headings = ['Head 1', 'Head 2', 'Head 3']
-        >>> data = []
-        >>> table = Table(headings, data=data)
-
-        # Data can be in several forms.
-        # A list of dictionaries, where the keys match the heading names:
-        >>> data = [{'head_1': 'value 1', 'head_2': 'value 2', 'head_3': 'value3'}),
-        >>>         {'head_1': 'value 1', 'head_2': 'value 2', 'head_3': 'value3'}]
-
-        # A list of lists. These will be mapped to the headings in order:
-        >>> data = [('value 1', 'value 2', 'value3'),
-        >>>         ('value 1', 'value 2', 'value3')]
+class Tree(Widget):
+    """Tree Widget.
 
-        # A list of values. This is only accepted if there is a single heading.
-        >>> data = ['item 1', 'item 2', 'item 3']
+    :param headings: The list of headings for the interface.
+    :param id:  An identifier for this widget.
+    :param style: An optional style object. If no style is provided then a new
+        one will be created for the widget.
+    :param data: The data to display in the widget. Can be an instance of
+        :class:`~toga.sources.TreeSource`, a list, dict or tuple with data to
+        display in the tree widget, or a class instance which implements the
+        interface of :class:`~toga.sources.TreeSource`. Entries can be:
+
+          - any Python object ``value`` with a string representation. This
+            string will be shown in the widget. If ``value`` has an attribute
+            ``icon``, instance of (:class:`~toga.icons.Icon`), the icon will be
+            shown in front of the text.
+
+          - a tuple ``(icon, value)`` where again the string representation of
+            ``value`` will be used as text.
+
+    :param accessors: Optional; a list of attributes to access the value in the
+        columns. If not given, the headings will be taken.
+    :param multiple_select: Boolean; if ``True``, allows for the selection of
+        multiple rows. Defaults to ``False``.
+    :param on_select: A handler to be invoked when the user selects one or
+        multiple rows.
+    :param on_double_click: A handler to be invoked when the user double clicks a row.
     """
+
     MIN_WIDTH = 100
     MIN_HEIGHT = 100
 
-    def __init__(self, headings, id=None, style=None, data=None, accessors=None,
-                 multiple_select=False, on_select=None, factory=None):
-        super().__init__(id=id, style=style, factory=factory)
+    def __init__(
+        self,
+        headings,
+        id=None,
+        style=None,
+        data=None,
+        accessors=None,
+        multiple_select=False,
+        on_select=None,
+        on_double_click=None,
+        factory=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
+
         self.headings = headings
         self._accessors = build_accessors(headings, accessors)
         self._multiple_select = multiple_select
-        self._on_select = None
-        self._selection = None
         self._data = None
+        self._on_select = None
+        self._on_double_click = None
 
-        self._impl = self.factory.Table(interface=self)
+        self._impl = self.factory.Tree(interface=self)
         self.data = data
 
         self.on_select = on_select
+        self.on_double_click = on_double_click
 
     @property
     def data(self):
-        """ The data source of the widget. It accepts table data
-        in the form of ``list``, ``tuple``, or :obj:`ListSource`
-
-        Returns:
-            Returns a (:obj:`ListSource`).
+        """
+        :returns: The data source of the tree
         """
         return self._data
 
     @data.setter
     def data(self, data):
+        """Set the data source of the data.
+
+        :param data: Data source
+        :type  data: ``dict`` or ``class``
+        """
         if data is None:
-            self._data = ListSource(accessors=self._accessors, data=[])
-        elif isinstance(data, (list, tuple)):
-            self._data = ListSource(accessors=self._accessors, data=data)
+            self._data = TreeSource(accessors=self._accessors, data=[])
+        elif isinstance(data, (list, tuple, dict)):
+            self._data = TreeSource(accessors=self._accessors, data=data)
         else:
             self._data = data
 
         self._data.add_listener(self._impl)
         self._impl.change_source(source=self._data)
 
     @property
@@ -82,57 +104,52 @@
         """Does the table allow multiple rows to be selected?"""
         return self._multiple_select
 
     @property
     def selection(self):
         """The current selection of the table.
 
-        A value of None indicates no selection.
-        If the table allows multiple selection, returns a list of
-        selected data nodes. Otherwise, returns a single data node.
+        A value of None indicates no selection. If the tree allows
+        multiple selection, returns a list of selected data nodes.
+        Otherwise, returns a single data node.
         """
-        return self._selection
-
-    def scroll_to_top(self):
-        """Scroll the view so that the top of the list (first row) is visible
-        """
-        self.scroll_to_row(0)
-
-    def scroll_to_row(self, row):
-        """Scroll the view so that the specified row index is visible.
-
-        Args:
-            row: The index of the row to make visible. Negative values refer
-                 to the nth last row (-1 is the last row, -2 second last,
-                 and so on)
-        """
-        if row >= 0:
-            self._impl.scroll_to_row(row)
-        else:
-            self._impl.scroll_to_row(len(self.data) + row)
-
-    def scroll_to_bottom(self):
-        """Scroll the view so that the bottom of the list (last row) is visible
-        """
-        self.scroll_to_row(-1)
+        return self._impl.get_selection()
 
     @property
     def on_select(self):
-        """ The callback function that is invoked when a row of the table is selected.
-        The provided callback function has to accept two arguments table (``:obj:Table`)
-        and row (``int`` or ``None``).
+        """The callable function for when a node on the Tree is selected. The
+        provided callback function has to accept two arguments tree
+        (:obj:`Tree`) and node (``Node`` or ``None``).
 
-        Returns:
-            (``callable``) The callback function.
+        :rtype: ``callable``
         """
         return self._on_select
 
     @on_select.setter
     def on_select(self, handler):
-        """
-        Set the function to be executed on node selection
+        """Set the function to be executed on node select.
 
         :param handler:     callback function
         :type handler:      ``callable``
         """
         self._on_select = wrapped_handler(self, handler)
         self._impl.set_on_select(self._on_select)
+
+    @property
+    def on_double_click(self):
+        """The callable function for when a node on the Tree is selected. The
+        provided callback function has to accept two arguments tree
+        (:obj:`Tree`) and node (``Node`` or ``None``).
+
+        :rtype: ``callable``
+        """
+        return self._on_double_click
+
+    @on_double_click.setter
+    def on_double_click(self, handler):
+        """Set the function to be executed on node double click.
+
+        :param handler:     callback function
+        :type handler:      ``callable``
+        """
+        self._on_double_click = wrapped_handler(self, handler)
+        self._impl.set_on_double_click(self._on_double_click)
```

### Comparing `toga-core-0.3.0.dev9/toga/widgets/canvas.py` & `toga-core-0.3.1/src/toga/widgets/canvas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,287 +1,280 @@
+import warnings
 from contextlib import contextmanager
+from enum import Enum
 from math import pi
 
+from toga.colors import BLACK, color as parse_color
+from toga.fonts import SYSTEM, Font
+from toga.handlers import wrapped_handler
+
+from .. import Image
 from .base import Widget
-from ..color import BLACK
-from ..color import color as parse_color
-from ..font import Font, SYSTEM
 
 
-class Context:
-    """The user-created :class:`Context <Context>` drawing object to populate a
-    drawing with visual context.
+class FillRule(Enum):
+    EVENODD = 0
+    NONZERO = 1
+
 
-    The top left corner of the canvas must be painted at the origin of the
-    context and is sized using the rehint() method.
+class Context:
+    """The user-created :class:`Context` drawing object to populate a drawing
+    with visual context.
 
+    The top left corner of the canvas must be painted at the origin of
+    the context and is sized using the rehint() method.
     """
 
     def __init__(self, *args, **kwargs):  # kwargs used to support multiple inheritance
         super().__init__(*args, **kwargs)
         self._canvas = None
         self.drawing_objects = []
 
     def __repr__(self):
-        return "{}()".format(self.__class__.__name__)
+        return f"{self.__class__.__name__}()"
 
     def _draw(self, impl, *args, **kwargs):
         """Draw all drawing objects that are on the context or canvas.
 
-
-        This method is used by the implementation to tell the interface canvas
-        to draw all objects on it, and used by a context to draw all the
-        objects that are on the context.
-
+        This method is used by the implementation to tell the interface
+        canvas to draw all objects on it, and used by a context to draw
+        all the objects that are on the context.
         """
         for obj in self.drawing_objects:
             obj._draw(impl, *args, **kwargs)
 
     ###########################################################################
     # Methods to keep track of the canvas, automatically redraw it
     ###########################################################################
 
     @property
     def canvas(self):
         """The canvas property of the current context.
 
         Returns:
             The canvas node. Returns self if this node *is* the canvas node.
-
         """
         return self._canvas if self._canvas else self
 
     @canvas.setter
     def canvas(self, value):
         """Set the canvas of the context.
 
         Args:
             value: The canvas to set.
-
         """
         self._canvas = value
 
     def add_draw_obj(self, draw_obj):
-        """A drawing object to add to the drawing object stack on a context
+        """A drawing object to add to the drawing object stack on a context.
 
         Args:
             draw_obj: (:obj:`Drawing Object`): The drawing object to add
-
         """
         self.drawing_objects.append(draw_obj)
 
         # Only redraw if drawing to canvas directly
         if self.canvas is self:
             self.redraw()
 
         return draw_obj
 
     def redraw(self):
-        """Force a redraw of the Canvas
-
-        The Canvas will be automatically redrawn after adding or remove a
-        drawing object. If you modify a drawing object, this method is used to
-        force a redraw.
+        """Force a redraw of the Canvas.
 
+        The Canvas will be automatically redrawn after adding or remove
+        a drawing object. If you modify a drawing object, this method is
+        used to force a redraw.
         """
         self.canvas._impl.redraw()
 
     ###########################################################################
     # Operations on drawing objects
     ###########################################################################
 
     def remove(self, drawing_object):
-        """Remove a drawing object
+        """Remove a drawing object.
 
         Args:
             drawing_object (:obj:'Drawing Object'): The drawing object to remove
-
         """
         self.drawing_objects.remove(drawing_object)
         self.redraw()
 
+    def clear(self):
+        """Remove all drawing objects."""
+        self.drawing_objects.clear()
+        self.redraw()
+
     ###########################################################################
     # Contexts to draw with
     ###########################################################################
 
     @contextmanager
     def context(self):
-        """Constructs and returns a :class:`Context <Context>`.
+        """Constructs and returns a :class:`Context`.
 
         Makes use of an existing context. The top left corner of the canvas must
         be painted at the origin of the context and is sized using the rehint()
         method.
 
         Yields:
-            :class:`Context <Context>` object.
-
+            :class:`Context` object.
         """
         context = Context()
         self.add_draw_obj(context)
         context.canvas = self.canvas
         yield context
         self.redraw()
 
     @contextmanager
-    def fill(self, color=BLACK, fill_rule="nonzero", preserve=False):
-        """Constructs and yields a :class:`Fill <Fill>`.
+    def fill(self, color=BLACK, fill_rule=FillRule.NONZERO, preserve=False):
+        """Constructs and yields a :class:`Fill`.
 
         A drawing operator that fills the current path according to the current
         fill rule, (each sub-path is implicitly closed before being filled).
 
         Args:
-            fill_rule (str, optional): 'nonzero' is the non-zero winding rule and
+            fill_rule (str, Optional): 'nonzero' is the non-zero winding rule and
                                        'evenodd' is the even-odd winding rule.
-            preserve (bool, optional): Preserves the path within the Context.
-            color (str, optional): color value in any valid color format,
+            preserve (bool, Optional): Preserves the path within the Context.
+            color (str, Optional): color value in any valid color format,
                 default to black.
 
         Yields:
-            :class:`Fill <Fill>` object.
-
+            :class:`Fill` object.
         """
-        if fill_rule is "evenodd":
-            fill = Fill(color, fill_rule, preserve)
-        else:
-            fill = Fill(color, "nonzero", preserve)
+        fill = Fill(color, fill_rule, preserve)
         fill.canvas = self.canvas
         yield self.add_draw_obj(fill)
         self.redraw()
 
     @contextmanager
-    def stroke(self, color=BLACK, line_width=2.0):
-        """Constructs and yields a :class:`Stroke <Stroke>`.
+    def stroke(self, color=BLACK, line_width=2.0, line_dash=None):
+        """Constructs and yields a :class:`Stroke`.
 
         Args:
-            color (str, optional): color value in any valid color format,
+            color (str, Optional): color value in any valid color format,
                 default to black.
-            line_width (float, optional): stroke line width, default is 2.0.
+            line_width (float, Optional): stroke line width, default is 2.0.
+            line_dash (array of floats, Optional): stroke line dash pattern, default is None.
 
         Yields:
-            :class:`Stroke <Stroke>` object.
-
+            :class:`Stroke` object.
         """
-        stroke = Stroke(color, line_width)
+        stroke = Stroke(color, line_width, line_dash)
         stroke.canvas = self.canvas
         yield self.add_draw_obj(stroke)
         self.redraw()
 
     @contextmanager
     def closed_path(self, x, y):
         """Calls move_to(x,y) and then constructs and yields a
-        :class:`ClosedPath <ClosedPath>`.
+        :class:`ClosedPath`.
 
         Args:
             x (float): The x axis of the beginning point.
             y (float): The y axis of the beginning point.
 
         Yields:
-            :class:`ClosedPath <ClosedPath>` object.
+            :class:`ClosedPath` object.
 
         """
         closed_path = ClosedPath(x, y)
         closed_path.canvas = self.canvas
         yield self.add_draw_obj(closed_path)
         self.redraw()
 
     ###########################################################################
     # Paths to draw with
     ###########################################################################
 
     def new_path(self):
-        """Constructs and returns a :class:`NewPath <NewPath>`.
+        """Constructs and returns a :class:`NewPath`.
 
         Returns:
-            :class: `NewPath <NewPath>` object.
-
+            :class: `NewPath` object.
         """
         new_path = NewPath()
         return self.add_draw_obj(new_path)
 
     def move_to(self, x, y):
-        """Constructs and returns a :class:`MoveTo <MoveTo>`.
+        """Constructs and returns a :class:`MoveTo`.
 
         Args:
             x (float): The x axis of the point.
             y (float): The y axis of the point.
 
         Returns:
-            :class:`MoveTo <MoveTo>` object.
-
+            :class:`MoveTo` object.
         """
         move_to = MoveTo(x, y)
         return self.add_draw_obj(move_to)
 
     def line_to(self, x, y):
-        """Constructs and returns a :class:`LineTo <LineTo>`.
+        """Constructs and returns a :class:`LineTo`.
 
         Args:
             x (float): The x axis of the coordinate for the end of the line.
             y (float): The y axis of the coordinate for the end of the line.
 
         Returns:
-            :class:`LineTo <LineTo>` object.
-
+            :class:`LineTo` object.
         """
         line_to = LineTo(x, y)
         return self.add_draw_obj(line_to)
 
     def bezier_curve_to(self, cp1x, cp1y, cp2x, cp2y, x, y):
-        """Constructs and returns a :class:`BezierCurveTo <BezierCurveTo>`.
+        """Constructs and returns a :class:`BezierCurveTo`.
 
         Args:
             cp1x (float): x coordinate for the first control point.
             cp1y (float): y coordinate for first control point.
             cp2x (float): x coordinate for the second control point.
             cp2y (float): y coordinate for the second control point.
             x (float): x coordinate for the end point.
             y (float): y coordinate for the end point.
 
         Returns:
-            :class:`BezierCurveTo <BezierCurveTo>` object.
-
+            :class:`BezierCurveTo` object.
         """
         bezier_curve_to = BezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)
         return self.add_draw_obj(bezier_curve_to)
 
     def quadratic_curve_to(self, cpx, cpy, x, y):
-        """Constructs and returns a :class:`QuadraticCurveTo <QuadraticCurveTo>`.
+        """Constructs and returns a :class:`QuadraticCurveTo`.
 
         Args:
             cpx (float): The x axis of the coordinate for the control point.
             cpy (float): The y axis of the coordinate for the control point.
             x (float): The x axis of the coordinate for the end point.
             y (float): The y axis of the coordinate for the end point.
 
         Returns:
-            :class:`QuadraticCurveTo <QuadraticCurveTo>` object.
-
+            :class:`QuadraticCurveTo` object.
         """
         quadratic_curve_to = QuadraticCurveTo(cpx, cpy, x, y)
         return self.add_draw_obj(quadratic_curve_to)
 
     def arc(self, x, y, radius, startangle=0.0, endangle=2 * pi, anticlockwise=False):
-        """Constructs and returns a :class:`Arc <Arc>`.
+        """Constructs and returns a :class:`Arc`.
 
-        Args:
-            x (float): The x coordinate of the arc's center.
-            y (float): The y coordinate of the arc's center.
-            radius (float): The arc's radius.
-            startangle (float, optional): The angle (in radians) at which the
+        :param x: The x coordinate of the arc's center.
+        :param y: The y coordinate of the arc's center.
+        :param radius: The arc's radius.
+        :param startangle: The angle (in radians) at which the
                 arc starts, measured clockwise from the positive x axis,
                 default 0.0.
-            endangle (float, optional): The angle (in radians) at which the arc ends,
+        :param endangle: The angle (in radians) at which the arc ends,
                 measured clockwise from the positive x axis, default 2*pi.
-            anticlockwise (bool, optional): If true, causes the arc to be drawn
+        :param anticlockwise: If true, causes the arc to be drawn
                 counter-clockwise between the two angles instead of clockwise,
                 default false.
 
-        Returns:
-            :class:`Arc <Arc>` object.
-
+        :returns: :class:`Arc` object.
         """
         arc = Arc(x, y, radius, startangle, endangle, anticlockwise)
         return self.add_draw_obj(arc)
 
     def ellipse(
         self,
         x,
@@ -289,352 +282,557 @@
         radiusx,
         radiusy,
         rotation=0.0,
         startangle=0.0,
         endangle=2 * pi,
         anticlockwise=False,
     ):
-        """Constructs and returns a :class:`Ellipse <Ellipse>`.
+        """Constructs and returns a :class:`Ellipse`.
 
-        Args:
-            x (float): The x axis of the coordinate for the ellipse's center.
-            y (float): The y axis of the coordinate for the ellipse's center.
-            radiusx (float): The ellipse's major-axis radius.
-            radiusy (float): The ellipse's minor-axis radius.
-            rotation (float, optional): The rotation for this ellipse, expressed in radians, default 0.0.
-            startangle (float, optional): The starting point in radians, measured from the x
-                axis, from which it will be drawn, default 0.0.
-            endangle (float, optional): The end ellipse's angle in radians to which it will
-                be drawn, default 2*pi.
-            anticlockwise (bool, optional): If true, draws the ellipse
-                anticlockwise (counter-clockwise) instead of clockwise, default false.
+        :param x: The x axis of the coordinate for the ellipse's center.
+        :param y: The y axis of the coordinate for the ellipse's center.
+        :param radiusx: The ellipse's major-axis radius.
+        :param radiusy: The ellipse's minor-axis radius.
+        :param rotation: The rotation for this ellipse, expressed in radians,
+            default 0.0.
+        :param startangle: The starting point in radians, measured from the x
+            axis, from which it will be drawn, default 0.0.
+        :param endangle: The end ellipse's angle in radians to which it will e
+            drawn, default 2*pi.
+        :param anticlockwise: If true, draws the ellipse anticlockwise
+            (counter-clockwise) instead of clockwise, default false.
 
         Returns:
-            :class:`Ellipse <Ellipse>` object.
-
+            :class:`Ellipse` object.
         """
         ellipse = Ellipse(
             x, y, radiusx, radiusy, rotation, startangle, endangle, anticlockwise
         )
         self.add_draw_obj(ellipse)
         return ellipse
 
     def rect(self, x, y, width, height):
-        """Constructs and returns a :class:`Rect <Rect>`.
+        """Constructs and returns a :class:`Rect`.
 
         Args:
             x (float): x coordinate for the rectangle starting point.
             y (float): y coordinate for the rectangle starting point.
             width (float): The rectangle's width.
             height (float): The rectangle's width.
 
         Returns:
-            :class:`Rect <Rect>` object.
-
+            :class:`Rect` object.
         """
         rect = Rect(x, y, width, height)
         return self.add_draw_obj(rect)
 
     ###########################################################################
     # Text drawing
     ###########################################################################
 
     def write_text(self, text, x=0, y=0, font=None):
-        """Constructs and returns a :class:`WriteText <WriteText>`.
+        """Constructs and returns a :class:`WriteText`.
 
         Writes a given text at the given (x,y) position. If no font is provided,
         then it will use the font assigned to the Canvas Widget, if it exists,
         or use the default font if there is no font assigned.
 
         Args:
-            text (string): The text to fill.
-            x (float, optional): The x coordinate of the text. Default to 0.
-            y (float, optional): The y coordinate of the text. Default to 0.
-            font (:class:`toga.Font`, optional): The font to write with.
+            text (str): The text to fill.
+            x (float, Optional): The x coordinate of the text. Default to 0.
+            y (float, Optional): The y coordinate of the text. Default to 0.
+            font (:class:`~toga.fonts.Font`, Optional): The font to write with.
 
         Returns:
-            :class:`WriteText <WriteText>` object.
-
+            :class:`WriteText` object.
         """
         if font is None:
             font = Font(family=SYSTEM, size=self._canvas.style.font_size)
         write_text = WriteText(text, x, y, font)
         return self.add_draw_obj(write_text)
 
 
 class Fill(Context):
-    """A user-created :class:`Fill <Fill>` drawing object for a fill context.
+    """A user-created :class:`Fill` drawing object for a fill context.
 
     A drawing object that fills the current path according to the current
     fill rule, (each sub-path is implicitly closed before being filled).
 
     Args:
-        color (str, optional): Color value in any valid color format,
+        color (str, Optional): Color value in any valid color format,
             default to black.
-        fill_rule (str, optional): 'nonzero' if the non-zero winding rule and
+        fill_rule (str, Optional): 'nonzero' if the non-zero winding rule and
                                    'evenodd' if the even-odd winding rule.
-        preserve (bool, optional): Preserves the path within the Context.
-
+        preserve (bool, Optional): Preserves the path within the Context.
     """
 
-    def __init__(self, color=BLACK, fill_rule="nonzero", preserve=False):
+    def __init__(self, color=BLACK, fill_rule=FillRule.NONZERO, preserve=False):
         super().__init__()
         self.color = color
         self.fill_rule = fill_rule
         self.preserve = preserve
 
     def __repr__(self):
         return "{}(color={}, fill_rule={}, preserve={})".format(
             self.__class__.__name__, self.color, self.fill_rule, self.preserve
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Used by parent to draw all objects that are part of the context.
-
-        """
+        """Used by parent to draw all objects that are part of the context."""
         impl.new_path(*args, **kwargs)
         for obj in self.drawing_objects:
             kwargs["fill_color"] = self.color
             obj._draw(impl, *args, **kwargs)
         impl.fill(self.color, self.fill_rule, self.preserve, *args, **kwargs)
 
     @property
+    def fill_rule(self):
+        return self._fill_rule
+
+    @fill_rule.setter
+    def fill_rule(self, fill_rule):
+        if isinstance(fill_rule, str):
+            try:
+                fill_rule = FillRule[fill_rule.upper()]
+            except KeyError:
+                raise ValueError(
+                    "fill rule should be one of the followings: {}".format(
+                        ", ".join([value.name.lower() for value in FillRule])
+                    )
+                )
+        self._fill_rule = fill_rule
+
+    @property
     def color(self):
         return self._color
 
     @color.setter
     def color(self, value):
         if value is None:
             self._color = None
         else:
             self._color = parse_color(value)
 
 
 class Stroke(Context):
-    """A user-created :class:`Stroke <Stroke>` drawing object for a stroke context.
+    """A user-created :class:`Stroke` drawing object for a stroke context.
 
     A drawing operator that strokes the current path according to the
     current line style settings.
 
     Args:
-        color (str, optional): Color value in any valid color format,
+        color (str, Optional): Color value in any valid color format,
             default to black.
-        line_width (float, optional): Stroke line width, default is 2.0.
-
+        line_width (float, Optional): Stroke line width, default is 2.0.
+        line_dash (array of floats, Optional): Stroke line dash pattern, default is None.
     """
 
-    def __init__(self, color=BLACK, line_width=2.0):
+    def __init__(self, color=BLACK, line_width=2.0, line_dash=None):
         super().__init__()
         self._color = None
         self.color = color
         self.line_width = line_width
+        self.line_dash = line_dash
 
     def __repr__(self):
-        return "{}(color={}, line_width={})".format(
-            self.__class__.__name__, self.color, self.line_width
+        return "{}(color={}, line_width={}, line_dash={})".format(
+            self.__class__.__name__, self.color, self.line_width, self.line_dash
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Used by parent to draw all objects that are part of the context.
-
-        """
+        """Used by parent to draw all objects that are part of the context."""
         for obj in self.drawing_objects:
             kwargs["stroke_color"] = self.color
             kwargs["text_line_width"] = self.line_width
+            kwargs["text_line_dash"] = self.line_dash
             obj._draw(impl, *args, **kwargs)
-        impl.stroke(self.color, self.line_width, *args, **kwargs)
+        impl.stroke(self.color, self.line_width, self.line_dash, *args, **kwargs)
 
     @property
     def color(self):
         return self._color
 
     @color.setter
     def color(self, value):
         if value is None:
             self._color = None
         else:
             self._color = parse_color(value)
 
 
 class ClosedPath(Context):
-    """A user-created :class:`ClosedPath <ClosedPath>` drawing object for a
-    closed path context.
+    """A user-created :class:`ClosedPath` drawing object for a closed path
+    context.
 
     Creates a new path and then closes it.
 
     Args:
         x (float): The x axis of the beginning point.
         y (float): The y axis of the beginning point.
-
     """
 
     def __init__(self, x, y):
         super().__init__()
         self.x = x
         self.y = y
 
     def __repr__(self):
-        return "{}(x={}, y={})".format(self.__class__.__name__, self.x, self.y)
+        return f"{self.__class__.__name__}(x={self.x}, y={self.y})"
 
     def _draw(self, impl, *args, **kwargs):
-        """Used by parent to draw all objects that are part of the context.
-
-        """
+        """Used by parent to draw all objects that are part of the context."""
         impl.move_to(self.x, self.y, *args, **kwargs)
         for obj in self.drawing_objects:
             obj._draw(impl, *args, **kwargs)
         impl.closed_path(self.x, self.y, *args, **kwargs)
 
 
 class Canvas(Context, Widget):
     """Create new canvas.
 
     Args:
         id (str):  An identifier for this widget.
         style (:obj:`Style`): An optional style object. If no
             style is provided then a new one will be created for the widget.
-        factory (:obj:`module`): A python module that is capable to return a
-            implementation of this class with the same name. (optional &
-            normally not needed)
+        on_resize (:obj:`Callable`): Handler to invoke when the canvas is resized.
+        on_press (:obj:`Callable`): Handler to invoke when the primary
+            (usually the left) button is pressed.
+        on_release (:obj:`Callable`): Handler to invoke when the primary
+            (usually the left) button is released.
+        on_drag (:obj:`Callable`): Handler to invoke when cursor is dragged with
+            the primary (usually the left) button pressed.
+        on_alt_press (:obj:`Callable`): Handler to invoke when the alternate
+            (usually the right) button pressed.
+        on_alt_release (:obj:`Callable`): Handler to invoke when the alternate
+            (usually the right) button released
+        on_alt_drag (:obj:`Callable`): Handler to invoke when the cursor is
+            dragged with the alternate (usually the right) button pressed.
     """
 
-    def __init__(self, id=None, style=None, factory=None):
-        super().__init__(id=id, style=style, factory=factory)
+    def __init__(
+        self,
+        id=None,
+        style=None,
+        on_resize=None,
+        on_press=None,
+        on_release=None,
+        on_drag=None,
+        on_alt_press=None,
+        on_alt_release=None,
+        on_alt_drag=None,
+        factory=None,  # DEPRECATED!
+    ):
+        super().__init__(id=id, style=style)
+        ######################################################################
+        # 2022-09: Backwards compatibility
+        ######################################################################
+        # factory no longer used
+        if factory:
+            warnings.warn("The factory argument is no longer used.", DeprecationWarning)
+        ######################################################################
+        # End backwards compatibility.
+        ######################################################################
+
         self._canvas = self
 
         # Create a platform specific implementation of Canvas
         self._impl = self.factory.Canvas(interface=self)
 
+        # Set all the properties
+        self.on_resize = on_resize
+        self.on_press = on_press
+        self.on_release = on_release
+        self.on_drag = on_drag
+        self.on_alt_press = on_alt_press
+        self.on_alt_release = on_alt_release
+        self.on_alt_drag = on_alt_drag
+
+    @property
+    def on_resize(self):
+        """The handler to invoke when the canvas is resized.
+
+        Returns:
+            The handler that is invoked on canvas resize.
+        """
+        return self._on_resize
+
+    @on_resize.setter
+    def on_resize(self, handler):
+        """Set the handler to invoke when the canvas is resized.
+
+        Args:
+            handler (:obj:`Callable`): The handler to invoke when the canvas is resized.
+        """
+        self._on_resize = wrapped_handler(self, handler)
+        self._impl.set_on_resize(self._on_resize)
+
+    @property
+    def on_press(self):
+        """Return the handler invoked when the primary (usually the left) mouse
+        button is pressed.
+
+        Returns:
+            The handler that is invoked when the primary mouse button is pressed.
+        """
+        return self._on_press
+
+    @on_press.setter
+    def on_press(self, handler):
+        """Set the handler to invoke when the primary (usually the left) mouse
+        button is pressed.
+
+        Args:
+            handler (:obj:`Callable`): The handler to invoke when the
+            primary mouse button is pressed.
+        """
+        self._on_press = wrapped_handler(self, handler)
+        self._impl.set_on_press(self._on_press)
+
+    @property
+    def on_release(self):
+        """Return the handler invoked when the primary (usually the left) mouse
+        button is released.
+
+        Returns:
+            The handler that is invoked when the primary mouse button is released.
+        """
+        return self._on_release
+
+    @on_release.setter
+    def on_release(self, handler):
+        """Set the handler to invoke when the primary (usually the left) mouse
+        button is released.
+
+        Args:
+            handler (:obj:`Callable`): The handler to invoke when the
+            primary mouse button is released.
+        """
+        self._on_release = wrapped_handler(self, handler)
+        self._impl.set_on_release(self._on_release)
+
+    @property
+    def on_drag(self):
+        """Return the handler invoked when the mouse is dragged with the
+        primary (usually the left) mouse button is pressed.
+
+        Returns:
+            The handler that is invoked when the mouse is dragged with
+            the primary button pressed.
+        """
+        return self._on_drag
+
+    @on_drag.setter
+    def on_drag(self, handler):
+        """Set the handler to invoke when the mouse button is dragged with the
+        primary (usually the left) button pressed.
+
+        Args:
+            handler (:obj:`Callable`): The handler to invoke when the
+            mouse is dragged with the primary button pressed.
+        """
+        self._on_drag = wrapped_handler(self, handler)
+        self._impl.set_on_drag(self._on_drag)
+
+    @property
+    def on_alt_press(self):
+        """Return the handler to invoke when the alternate (usually the right)
+        mouse button is pressed.
+
+        Returns:
+            The handler that is invoked when the alternate mouse button is pressed.
+        """
+        return self._on_alt_press
+
+    @on_alt_press.setter
+    def on_alt_press(self, handler):
+        """Set the handler to invoke when the alternate (usually the right)
+        mouse button is pressed.
+
+        Args:
+            handler (:obj:`Callable`): The handler to invoke when the
+            alternate mouse button is pressed.
+        """
+        self._on_alt_press = wrapped_handler(self, handler)
+        self._impl.set_on_alt_press(self._on_alt_press)
+
+    @property
+    def on_alt_release(self):
+        """Return the handler to invoke when the alternate (usually the right)
+        mouse button is released.
+
+        Returns:
+            The handler that is invoked when the alternate mouse button is released.
+        """
+        return self._on_alt_release
+
+    @on_alt_release.setter
+    def on_alt_release(self, handler):
+        """Set the handler to invoke when the alternate (usually the right)
+        mouse button is released.
+
+        Args:
+            handler (:obj:`Callable`): The handler to invoke when the
+            alternate mouse button is released.
+        """
+        self._on_alt_release = wrapped_handler(self, handler)
+        self._impl.set_on_alt_release(self._on_alt_release)
+
+    @property
+    def on_alt_drag(self):
+        """Return the handler to invoke when the mouse is dragged while the
+        alternate (usually the right) mouse button is pressed.
+
+        Returns:
+            The handler that is invoked when the mouse is dragged with
+            the alternate mouse button pressed.
+        """
+        return self._on_alt_drag
+
+    @on_alt_drag.setter
+    def on_alt_drag(self, handler):
+        """Set the handler to invoke when the mouse is dragged with the
+        alternate (usually the right) button pressed.
+
+        Args:
+            handler (:obj:`Callable`): The handler to invoke when the
+            mouse is dragged with the alternate button pressed.
+        """
+        self._on_alt_drag = wrapped_handler(self, handler)
+        self._impl.set_on_alt_drag(self._on_alt_drag)
+
     ###########################################################################
     # Transformations of a canvas
     ###########################################################################
 
     def rotate(self, radians):
-        """Constructs and returns a :class:`Rotate <Rotate>`.
+        """Constructs and returns a :class:`Rotate`.
 
         Args:
             radians (float): The angle to rotate clockwise in radians.
 
         Returns:
-            :class:`Rotate <Rotate>` object.
-
+            :class:`Rotate` object.
         """
         rotate = Rotate(radians)
         return self.add_draw_obj(rotate)
 
     def scale(self, sx, sy):
-        """Constructs and returns a :class:`Scale <Scale>`.
+        """Constructs and returns a :class:`Scale`.
 
         Args:
             sx (float): scale factor for the X dimension.
             sy (float): scale factor for the Y dimension.
 
         Returns:
-            :class:`Scale <Scale>` object.
-
+            :class:`Scale` object.
         """
         scale = Scale(sx, sy)
         return self.add_draw_obj(scale)
 
     def translate(self, tx, ty):
-        """Constructs and returns a :class:`Translate <Translate>`.
+        """Constructs and returns a :class:`Translate`.
 
         Args:
             tx (float): X value of coordinate.
             ty (float): Y value of coordinate.
 
         Returns:
-            :class:`Translate <Translate>` object.
-
+            :class:`Translate` object.
         """
         translate = Translate(tx, ty)
         return self.add_draw_obj(translate)
 
     def reset_transform(self):
-        """Constructs and returns a :class:`ResetTransform <ResetTransform>`.
+        """Constructs and returns a :class:`ResetTransform`.
 
         Returns:
-            :class:`ResetTransform <ResetTransform>` object.
-
+            :class:`ResetTransform` object.
         """
         reset_transform = ResetTransform()
         return self.add_draw_obj(reset_transform)
 
+    ###########################################################################
+    # Text measurement
+    ###########################################################################
+
+    def measure_text(self, text, font, tight=False):
+        return self._impl.measure_text(text, font, tight=tight)
+
+    ###########################################################################
+    # As image
+    ###########################################################################
+
+    def as_image(self):
+        return Image(data=self._impl.get_image_data())
+
 
 class MoveTo:
-    """A user-created :class:`MoveTo <MoveTo>` drawing object which moves the
-    start of the next operation to a point.
+    """A user-created :class:`MoveTo` drawing object which moves the start of
+    the next operation to a point.
 
     Moves the starting point of a new sub-path to the (x, y) coordinates.
 
 
     Args:
         x (float): The x axis of the point.
         y (float): The y axis of the point.
-
     """
 
     def __init__(self, x, y):
         self.x = x
         self.y = y
 
     def __repr__(self):
-        return "{}(x={}, y={})".format(self.__class__.__name__, self.x, self.y)
+        return f"{self.__class__.__name__}(x={self.x}, y={self.y})"
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.move_to(self.x, self.y, *args, **kwargs)
 
 
 class LineTo:
-    """A user-created :class:`LineTo <LineTo>` drawing object which draws a line
-    to a point.
+    """A user-created :class:`LineTo` drawing object which draws a line to a
+    point.
 
     Connects the last point in the sub-path to the (x, y) coordinates
     with a straight line (but does not actually draw it).
 
     Args:
         x (float): The x axis of the coordinate for the end of the line.
         y (float): The y axis of the coordinate for the end of the line.
-
     """
 
     def __init__(self, x, y):
         self.x = x
         self.y = y
 
     def __repr__(self):
-        return "{}(x={}, y={})".format(self.__class__.__name__, self.x, self.y)
+        return f"{self.__class__.__name__}(x={self.x}, y={self.y})"
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.line_to(self.x, self.y, *args, **kwargs)
 
 
 class BezierCurveTo:
-    """A user-created :class:`BezierCurveTo <BezierCurveTo>` drawing
-    object which adds a Bézier curve.
+    """A user-created :class:`BezierCurveTo` drawing object which adds a Bézier
+    curve.
 
     It requires three points. The first two points are control points
     and the third one is the end point. The starting point is the last
     point in the current path, which can be changed using move_to() before
     creating the Bézier curve.
 
     Args:
         cp1x (float): x coordinate for the first control point.
         cp1y (float): y coordinate for first control point.
         cp2x (float): x coordinate for the second control point.
         cp2y (float): y coordinate for the second control point.
         x (float): x coordinate for the end point.
         y (float): y coordinate for the end point.
-
     """
 
     def __init__(self, cp1x, cp1y, cp2x, cp2y, x, y):
         self.cp1x = cp1x
         self.cp1y = cp1y
         self.cp2x = cp2x
         self.cp2y = cp2y
@@ -649,77 +847,70 @@
             self.cp2x,
             self.cp2y,
             self.x,
             self.y,
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.bezier_curve_to(
             self.cp1x, self.cp1y, self.cp2x, self.cp2y, self.x, self.y, *args, **kwargs
         )
 
 
 class QuadraticCurveTo:
-    """A user-created :class:`QuadraticCurveTo <QuadraticCurveTo>` drawing
-    object which adds a quadratic curve.
+    """A user-created :class:`QuadraticCurveTo` drawing object which adds a
+    quadratic curve.
 
     It requires two points. The first point is a control point and the
     second one is the end point. The starting point is the last point in the
-    current path, which can be changed using moveTo() before creating the
+    current path, which can be changed using ``moveTo()`` before creating the
     quadratic Bézier curve.
 
-    Args:
-        cpx (float): The x axis of the coordinate for the control point.
-        cpy (float): The y axis of the coordinate for the control point.
-        x (float): The x axis of the coordinate for the end point.
-        y (float): he y axis of the coordinate for the end point.
-
+    :param cpx: The x axis of the coordinate for the control point.
+    :param cpy: The y axis of the coordinate for the control point.
+    :param x: The x axis of the coordinate for the end point.
+    :param y: he y axis of the coordinate for the end point.
     """
 
     def __init__(self, cpx, cpy, x, y):
         self.cpx = cpx
         self.cpy = cpy
         self.x = x
         self.y = y
 
     def __repr__(self):
         return "{}(cpx={}, cpy={}, x={}, y={})".format(
             self.__class__.__name__, self.cpx, self.cpy, self.x, self.y
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.quadratic_curve_to(self.cpx, self.cpy, self.x, self.y, *args, **kwargs)
 
 
 class Ellipse:
-    """A user-created :class:`Ellipse <Ellipse>` drawing object which adds an ellipse.
-
-    The ellipse is centered at (x, y) position with the radii radiusx and radiusy
-    starting at startAngle and ending at endAngle going in the given
-    direction by anticlockwise (defaulting to clockwise).
-
-    Args:
-        x (float): The x axis of the coordinate for the ellipse's center.
-        y (float): The y axis of the coordinate for the ellipse's center.
-        radiusx (float): The ellipse's major-axis radius.
-        radiusy (float): The ellipse's minor-axis radius.
-        rotation (float, optional): The rotation for this ellipse, expressed in radians, default 0.0.
-        startangle (float, optional): The starting point in radians, measured from the x
-            axis, from which it will be drawn, default 0.0.
-        endangle (float, optional): The end ellipse's angle in radians to which it will
-            be drawn, default 2*pi.
-        anticlockwise (bool, optional): If true, draws the ellipse anticlockwise
-            (counter-clockwise) instead of clockwise, default false.
+    """A user-created :class:`Ellipse` drawing object which adds an ellipse.
 
+    The ellipse is centered at ``(x, y)`` position with the radii ``radiusx``
+    and ``radiusy`` starting at ``startangle`` and ending at ``endangle`` going
+    in the given direction by anticlockwise (defaulting to clockwise).
+
+    :param x: The x axis of the coordinate for the ellipse's center.
+    :param y: The y axis of the coordinate for the ellipse's center.
+    :param radiusx: The ellipse's major-axis radius.
+    :param radiusy: The ellipse's minor-axis radius.
+    :param rotation: The rotation for this ellipse, expressed in radians, default
+        0.0.
+    :param startangle: The starting point in radians, measured from the x axis,
+        from which it will be drawn, default 0.0.
+    :param endangle: The end ellipse's angle in radians to which it will be
+        drawn, default 2*pi.
+    :param anticlockwise: If true, draws the ellipse anticlockwise
+        (counter-clockwise) instead of clockwise, default false.
     """
 
     def __init__(
         self,
         x,
         y,
         radiusx,
@@ -735,64 +926,61 @@
         self.radiusy = radiusy
         self.rotation = rotation
         self.startangle = startangle
         self.endangle = endangle
         self.anticlockwise = anticlockwise
 
     def __repr__(self):
-        return "{}(x={}, y={}, radiusx={}, radiusy={}, rotation={}, startangle={}, endangle={}, anticlockwise={})".format(
-            self.__class__.__name__,
-            self.x,
-            self.y,
-            self.radiusx,
-            self.radiusy,
-            self.rotation,
-            self.startangle,
-            self.endangle,
-            self.anticlockwise,
+        return (
+            "{}(x={}, y={}, radiusx={}, radiusy={}, "
+            "rotation={}, startangle={}, endangle={}, anticlockwise={})".format(
+                self.__class__.__name__,
+                self.x,
+                self.y,
+                self.radiusx,
+                self.radiusy,
+                self.rotation,
+                self.startangle,
+                self.endangle,
+                self.anticlockwise,
+            )
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.ellipse(
             self.x,
             self.y,
             self.radiusx,
             self.radiusy,
             self.rotation,
             self.startangle,
             self.endangle,
             self.anticlockwise,
             *args,
-            **kwargs
+            **kwargs,
         )
 
 
 class Arc:
-    """A user-created :class:`Arc <Arc>` drawing object which adds an arc.
-
-    The arc is centered at (x, y) position with radius r starting at startangle
-    and ending at endangle going in the given direction by anticlockwise
-    (defaulting to clockwise).
-
-    Args:
-        x (float): The x coordinate of the arc's center.
-        y (float): The y coordinate of the arc's center.
-        radius (float): The arc's radius.
-        startangle (float, optional): The angle (in radians) at which the
-            arc starts, measured clockwise from the positive x axis,
-            default 0.0.
-        endangle (float, optional): The angle (in radians) at which the arc ends,
-            measured clockwise from the positive x axis, default 2*pi.
-        anticlockwise (bool, optional): If true, causes the arc to be drawn
-            counter-clockwise between the two angles instead of clockwise,
-            default false.
+    """A user-created :class:`Arc` drawing object which adds an arc.
 
+    The arc is centered at ``(x, y)`` position with radius ``r`` starting at
+    ``startangle`` and ending at ``endangle`` going in the given direction by
+    anticlockwise (defaulting to clockwise).
+
+    :param x: The x coordinate of the arc's center.
+    :param y: The y coordinate of the arc's center.
+    :param radius: The arc's radius.
+    :param startangle: The angle (in radians) at which the arc starts, measured
+        clockwise from the positive x axis, default 0.0.
+    :param endangle: The angle (in radians) at which the arc ends, measured
+        clockwise from the positive x axis, default 2*pi.
+    :param anticlockwise: If true, causes the arc to be drawn counter-clockwise
+        between the two angles instead of clockwise, default false.
     """
 
     def __init__(
         self, x, y, radius, startangle=0.0, endangle=2 * pi, anticlockwise=False
     ):
         self.x = x
         self.y = y
@@ -809,197 +997,172 @@
             self.radius,
             self.startangle,
             self.endangle,
             self.anticlockwise,
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.arc(
             self.x,
             self.y,
             self.radius,
             self.startangle,
             self.endangle,
             self.anticlockwise,
             *args,
-            **kwargs
+            **kwargs,
         )
 
 
 class Rect:
-    """A user-created :class:`Rect <Rect>` drawing object which adds a rectangle.
+    """A user-created :class:`Rect` drawing object which adds a rectangle.
 
     The rectangle is at position (x, y) with a size that is determined by
     width and height. Those four points are connected by straight lines and
     the sub-path is marked as closed, so that you can fill or stroke this
     rectangle.
 
     Args:
         x (float): x coordinate for the rectangle starting point.
         y (float): y coordinate for the rectangle starting point.
         width (float): The rectangle's width.
         height (float): The rectangle's width.
-
     """
 
     def __init__(self, x, y, width, height):
         self.x = x
         self.y = y
         self.width = width
         self.height = height
 
     def __repr__(self):
         return "{}(x={}, y={}, width={}, height={})".format(
             self.__class__.__name__, self.x, self.y, self.width, self.height
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.rect(self.x, self.y, self.width, self.height, *args, **kwargs)
 
 
 class Rotate:
-    """A user-created :class:`Rotate <Rotate>` to add canvas rotation.
+    """A user-created :class:`Rotate` to add canvas rotation.
 
     Modifies the canvas by rotating the canvas by angle radians. The rotation
     center point is always the canvas origin which is in the upper left of the
     canvas. To change the center point, move the canvas by using the
     translate() method.
 
     Args:
         radians (float): The angle to rotate clockwise in radians.
-
     """
 
     def __init__(self, radians):
         self.radians = radians
 
     def __repr__(self):
-        return "{}(radians={})".format(self.__class__.__name__, self.radians)
+        return f"{self.__class__.__name__}(radians={self.radians})"
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.rotate(self.radians, *args, **kwargs)
 
 
 class Scale:
-    """A user-created :class:`Scale <Scale>` to add canvas scaling.
+    """A user-created :class:`Scale` to add canvas scaling.
 
     Modifies the canvas by scaling the X and Y canvas axes by sx and sy.
 
     Args:
         sx (float): scale factor for the X dimension.
         sy (float): scale factor for the Y dimension.
-
     """
 
     def __init__(self, sx, sy):
         self.sx = sx
         self.sy = sy
 
     def __repr__(self):
-        return "{}(sx={}, sy={})".format(self.__class__.__name__, self.sx, self.sy)
+        return f"{self.__class__.__name__}(sx={self.sx}, sy={self.sy})"
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.scale(self.sx, self.sy, *args, **kwargs)
 
 
 class Translate:
-    """A user-created :class:`Translate <Translate>` to translate the canvas.
+    """A user-created :class:`Translate` to translate the canvas.
 
     Modifies the canvas by translating the canvas origin by (tx, ty).
 
     Args:
         tx (float): X value of coordinate.
         ty (float): Y value of coordinate.
-
     """
 
     def __init__(self, tx, ty):
         self.tx = tx
         self.ty = ty
 
     def __repr__(self):
-        return "{}(tx={}, ty={})".format(self.__class__.__name__, self.tx, self.ty)
+        return f"{self.__class__.__name__}(tx={self.tx}, ty={self.ty})"
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.translate(self.tx, self.ty, *args, **kwargs)
 
 
 class ResetTransform:
-    """A user-created :class:`ResetTransform <ResetTransform>` to reset the
-    canvas.
+    """A user-created :class:`ResetTransform` to reset the canvas.
 
     Resets the canvas by setting it equal to the canvas with no
     transformations.
-
     """
 
     def __repr__(self):
-        return "{}()".format(self.__class__.__name__)
+        return f"{self.__class__.__name__}()"
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.reset_transform(*args, **kwargs)
 
 
 class WriteText:
-    """A user-created :class:`WriteText <WriteText>` to add text.
+    """A user-created :class:`WriteText` to add text.
 
     Writes a given text at the given (x,y) position. If no font is provided,
     then it will use the font assigned to the Canvas Widget, if it exists,
     or use the default font if there is no font assigned.
 
     Args:
-        text (string): The text to fill.
-        x (float, optional): The x coordinate of the text. Default to 0.
-        y (float, optional): The y coordinate of the text. Default to 0.
-        font (:class:`toga.Font`, optional): The font to write with.
-
+        text (str): The text to fill.
+        x (float, Optional): The x coordinate of the text. Default to 0.
+        y (float, Optional): The y coordinate of the text. Default to 0.
+        font (:class:`toga.fonts.Font`, Optional): The font to write with.
     """
 
     def __init__(self, text, x, y, font):
         self.text = text
         self.x = x
         self.y = y
         self.font = font
 
     def __repr__(self):
         return "{}(text={}, x={}, y={}, font={})".format(
             self.__class__.__name__, self.text, self.x, self.y, self.font
         )
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.write_text(self.text, self.x, self.y, self.font, *args, **kwargs)
 
 
 class NewPath:
-    """A user-created :class:`NewPath <NewPath>` to add a new path.
-
-    """
+    """A user-created :class:`NewPath` to add a new path."""
 
     def __repr__(self):
-        return "{}()".format(self.__class__.__name__)
+        return f"{self.__class__.__name__}()"
 
     def _draw(self, impl, *args, **kwargs):
-        """Draw the drawing object using the implementation.
-
-        """
+        """Draw the drawing object using the implementation."""
         impl.new_path(*args, **kwargs)
```

### Comparing `toga-core-0.3.0.dev9/README.rst` & `toga-core-0.3.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 This will pop up a GUI window with some sample widgets.
 
 Prerequisites
 ~~~~~~~~~~~~~
 
 Toga has some minimum requirements:
 
-* If you're on OS X, you need to be on 10.7 (Lion) or newer.
+* If you're on OS X, you need to be on 10.10 (Yosemite) or newer.
 
 * If you're on Linux, you need to have GTK+ 3.4 or later. This is the version
   that ships starting with Ubuntu 12.04 and Fedora 17.
 
 * If you want to use the WebView widget, you'll also need to have WebKit, plus
   the GI bindings to WebKit installed.
 
@@ -74,50 +74,49 @@
         $ ln -si /usr/lib64/python3.5/site-packages/gi/
 
 Documentation
 -------------
 
 Documentation for Toga can be found on `Read The Docs`_.
 
+.. _Read The Docs: https://toga.readthedocs.io
+
 Related projects
 ----------------
 
 This package is a top level package. It depends on the use of platform-specific
 backends to provide real functionality:
 
-* `toga-cocoa`_: for OS/X
-* `toga-gtk`_: GTK+ backend for Linux desktops
-* `toga-iOS`_: for iOS devices (iPhone, iPad, iPod)
-* `toga-android`_: for Android devices (limited support)
-* `toga-win32`_: for old Windows desktops (limited support)
-* `toga-winforms`_: for recent Window devices (limited support)
-* `toga-uwp`_: for Windows 10 and Windows Mobile devices (limited support)
+* ``toga-cocoa``: for macOS
+* ``toga-gtk``: GTK+ backend for Linux desktops
+* ``toga-iOS``: for iOS devices (iPhone, iPad, iPod)
+* ``toga-android``: for Android devices (limited support)
+* ``toga-winforms``: for recent Window devices (limited support)
+* ``toga-django``: for web deployment (limited support)
 
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
 
 If you experience problems with Toga, `log them on GitHub`_. If you
 want to contribute code, please `fork the code`_ and `submit a pull request`_.
 
-.. _BeeWare suite: http://pybee.org
-.. _Read The Docs: https://toga.readthedocs.io
-.. _toga-cocoa: https://pypi.python.org/pypi/toga-cocoa
-.. _toga-gtk: https://pypi.python.org/pypi/toga-gtk
-.. _toga-win32: https://pypi.python.org/pypi/toga-win32
-.. _toga-iOS: https://pypi.python.org/pypi/toga-iOS
-.. _toga-android: https://pypi.python.org/pypi/toga-android
-.. _toga-winforms: https://pypi.python.org/pypi/toga-winforms
-.. _toga-uwp: https://pypi.python.org/pypi/toga-uwp
-.. _@pybeeware on Twitter: https://twitter.com/pybeeware
-.. _pybee/general: https://gitter.im/pybee/general
-.. _log them on Github: https://github.com/pybee/toga/issues
-.. _fork the code: https://github.com/pybee/toga
-.. _submit a pull request: https://github.com/pybee/toga/pulls
+.. _log them on Github: https://github.com/beeware/toga/issues
+.. _fork the code: https://github.com/beeware/toga
+.. _submit a pull request: https://github.com/beeware/toga/pulls
```

