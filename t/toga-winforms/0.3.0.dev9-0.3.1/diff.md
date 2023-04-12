# Comparing `tmp/toga-winforms-0.3.0.dev9.tar.gz` & `tmp/toga-winforms-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-winforms-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:21 2018, max compression
+gzip compressed data, was "toga-winforms-0.3.1.tar", last modified: Wed Apr 12 01:59:01 2023, max compression
```

## Comparing `toga-winforms-0.3.0.dev9.tar` & `toga-winforms-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,94 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     2403 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms/hardware/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/hardware/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      238 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/color.py
--rw-r--r--   0 rkm        (501) staff       (20)      506 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/command.py
--rw-r--r--   0 rkm        (501) staff       (20)     7145 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/toga_winforms/window.py
--rw-r--r--   0 rkm        (501) staff       (20)      351 2018-05-17 17:50:36.000000 toga-winforms-0.3.0.dev9/toga_winforms/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1412 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/factory.py
--rw-r--r--   0 rkm        (501) staff       (20)     3076 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/toga_winforms/app.py
--rw-r--r--   0 rkm        (501) staff       (20)      852 2018-01-25 04:51:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/dialogs.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)     1481 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/icon.py
--rw-r--r--   0 rkm        (501) staff       (20)     1070 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/tree.py
--rw-r--r--   0 rkm        (501) staff       (20)     1156 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)     1053 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/box.py
--rw-r--r--   0 rkm        (501) staff       (20)     1734 2018-05-17 17:50:27.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/splitcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      879 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/multilinetextinput.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1306 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     1038 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/switch.py
--rw-r--r--   0 rkm        (501) staff       (20)     1332 2018-05-17 17:50:27.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/scrollcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     1094 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/slider.py
--rw-r--r--   0 rkm        (501) staff       (20)     1316 2018-05-17 17:50:27.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/button.py
--rw-r--r--   0 rkm        (501) staff       (20)     1082 2018-05-17 17:50:27.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/progressbar.py
--rw-r--r--   0 rkm        (501) staff       (20)      715 2018-05-17 17:50:27.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/label.py
--rw-r--r--   0 rkm        (501) staff       (20)     2010 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/numberinput.py
--rw-r--r--   0 rkm        (501) staff       (20)      163 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     2060 2018-05-17 17:50:27.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/table.py
--rw-r--r--   0 rkm        (501) staff       (20)     1313 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/selection.py
--rw-r--r--   0 rkm        (501) staff       (20)     1233 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/webview.py
--rw-r--r--   0 rkm        (501) staff       (20)      889 2018-05-17 17:50:27.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/optioncontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      504 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/image.py
--rw-r--r--   0 rkm        (501) staff       (20)     2094 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/widgets/base.py
--rw-r--r--   0 rkm        (501) staff       (20)     1125 2018-05-26 09:29:22.000000 toga-winforms-0.3.0.dev9/toga_winforms/libs.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/tests/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-winforms-0.3.0.dev9/tests/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      278 2017-12-22 11:14:30.000000 toga-winforms-0.3.0.dev9/tests/test_implementation.py
--rw-r--r--   0 rkm        (501) staff       (20)     1744 2018-07-07 05:52:00.000000 toga-winforms-0.3.0.dev9/setup.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms.egg-info/
--rw-r--r--   0 rkm        (501) staff       (20)     2403 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms.egg-info/PKG-INFO
--rw-r--r--   0 rkm        (501) staff       (20)     1235 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms.egg-info/SOURCES.txt
--rw-r--r--   0 rkm        (501) staff       (20)       32 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms.egg-info/requires.txt
--rw-r--r--   0 rkm        (501) staff       (20)       20 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms.egg-info/top_level.txt
--rw-r--r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/toga_winforms.egg-info/dependency_links.txt
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:21.000000 toga-winforms-0.3.0.dev9/setup.cfg
--rw-r--r--   0 rkm        (501) staff       (20)     1132 2017-12-22 11:14:05.000000 toga-winforms-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.445381 toga-winforms-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-12 01:59:01.445381 toga-winforms-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-12 01:59:01.445381 toga-winforms-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.409381 toga-winforms-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.417381 toga-winforms-0.3.1/src/toga_winforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.421381 toga-winforms-0.3.1/src/toga_winforms/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.421381 toga-winforms-0.3.1/src/toga_winforms/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.425381 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)   306600 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.Core.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    35280 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/Microsoft.Web.WebView2.WinForms.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.425381 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/arm64/
+-rw-r--r--   0 runner    (1001) docker     (123)   127912 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/arm64/WebView2Loader.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.425381 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/x64/
+-rw-r--r--   0 runner    (1001) docker     (123)   141224 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/x64/WebView2Loader.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.425381 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)   110504 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/WebView2/x86/WebView2Loader.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/proactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/libs/winforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.437381 toga-winforms-0.3.1/src/toga_winforms/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/datepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/timepicker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/src/toga_winforms/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.421381 toga-winforms-0.3.1/src/toga_winforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-12 01:59:01.000000 toga-winforms-0.3.1/src/toga_winforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-12 01:59:01.000000 toga-winforms-0.3.1/src/toga_winforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:59:01.000000 toga-winforms-0.3.1/src/toga_winforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 01:59:01.000000 toga-winforms-0.3.1/src/toga_winforms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:45.000000 toga-winforms-0.3.1/src/toga_winforms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 01:59:01.000000 toga-winforms-0.3.1/src/toga_winforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 01:59:01.000000 toga-winforms-0.3.1/src/toga_winforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.437381 toga-winforms-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests/test_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.441381 toga-winforms-0.3.1/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:59:01.445381 toga-winforms-0.3.1/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 01:58:13.000000 toga-winforms-0.3.1/tests_backend/widgets/textinput.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/window.py` & `toga-winforms-0.3.1/src/toga_winforms/window.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,108 @@
 from toga import GROUP_BREAK, SECTION_BREAK
-from travertino.layout import Viewport
 
-from .libs import WinForms, Size, add_handler
+from .libs import Point, Size, WinForms
 
 
 class WinFormsViewport:
     def __init__(self, native, frame):
         self.native = native
         self.frame = frame
-        self.dpi = 96  # FIXME This is almost certainly wrong...
+        self.baseline_dpi = 96
 
     @property
     def width(self):
+        # Treat `native=None` as a 0x0 viewport
+        if self.native is None:
+            return 0
         return self.native.ClientSize.Width
 
     @property
     def height(self):
+        # Treat `native=None` as a 0x0 viewport
+        if self.native is None:
+            return 0
         # Subtract any vertical shift of the frame. This is to allow
         # for toolbars, or any other viewport-level decoration.
         return self.native.ClientSize.Height - self.frame.vertical_shift
 
+    @property
+    def dpi(self):
+        if self.native is None:
+            return self.baseline_dpi
+        return self.native.CreateGraphics().DpiX
+
 
 class Window:
-    def __init__(self, interface):
+    def __init__(self, interface, title, position, size):
         self.interface = interface
         self.interface._impl = self
-        self.create()
 
-    def create(self):
-        self.native = WinForms.Form(self)
-        self.native.ClientSize = Size(self.interface._size[0], self.interface._size[1])
+        # Winforms close handling is caught on the FormClosing handler. To allow
+        # for async close handling, we need to be able to abort this close
+        # event, and then manually cause the close as part of the async result
+        # handling. However, this then causes an is_closing event, which we need
+        # to ignore. The `_is_closing` flag lets us easily identify if the
+        # window is in the process of closing.
+        self._is_closing = False
+
+        self.native = WinForms.Form()
         self.native.interface = self.interface
-        self.native.Resize += self.winforms_Resize
+        self.native.FormClosing += self.winforms_FormClosing
+
+        self.native.MinimizeBox = self.native.interface.minimizable
+
+        self.set_title(title)
+        self.set_size(size)
+        self.set_position(position)
+
         self.toolbar_native = None
         self.toolbar_items = None
+        if self.native.interface.resizeable:
+            self.native.Resize += self.winforms_resize
+        else:
+            self.native.FormBorderStyle = self.native.FormBorderStyle.FixedSingle
+            self.native.MaximizeBox = False
 
     def create_toolbar(self):
         self.toolbar_native = WinForms.ToolStrip()
         for cmd in self.interface.toolbar:
             if cmd == GROUP_BREAK:
                 item = WinForms.ToolStripSeparator()
             elif cmd == SECTION_BREAK:
                 item = WinForms.ToolStripSeparator()
             else:
-                cmd.bind(self.interface.factory)
                 if cmd.icon is not None:
-                    native_icon = cmd.icon.bind(self.interface.factory).native
-                    item = WinForms.ToolStripMenuItem(cmd.label, native_icon.ToBitmap())
+                    native_icon = cmd.icon._impl.native
+                    item = WinForms.ToolStripMenuItem(cmd.text, native_icon.ToBitmap())
                 else:
-                    item = WinForms.ToolStripMenuItem(cmd.label)
-
-                item.Click += add_handler(cmd)
+                    item = WinForms.ToolStripMenuItem(cmd.text)
+                item.Click += cmd._impl.as_handler()
+                cmd._impl.native.append(item)
             self.toolbar_native.Items.Add(item)
 
+    def get_position(self):
+        return self.native.Location.X, self.native.Location.Y
+
     def set_position(self, position):
-        pass
+        self.native.Location = Point(*position)
+
+    def get_size(self):
+        return self.native.ClientSize.Width, self.native.ClientSize.Height
 
     def set_size(self, size):
-        self.native.ClientSize = Size(self.interface._size[0], self.interface._size[1])
+        self.native.ClientSize = Size(*size)
 
     def set_app(self, app):
-        pass
+        if app is None:
+            return
+        icon_impl = app.interface.icon._impl
+        if icon_impl is None:
+            return
+        self.native.Icon = icon_impl.native
 
     @property
     def vertical_shift(self):
         # vertical shift is the toolbar height or 0
         result = 0
         try:
             result += self.native.interface._impl.toolbar_native.Height
@@ -72,120 +110,106 @@
             pass
         try:
             result += self.native.interface._impl.native.MainMenuStrip.Height
         except AttributeError:
             pass
         return result
 
+    def clear_content(self):
+        if self.interface.content:
+            for child in self.interface.content.children:
+                child._impl.container = None
+
     def set_content(self, widget):
-        if self.toolbar_native:
+        has_content = False
+        for control in self.native.Controls:
+            # The main menu and toolbar are normal in-window controls;
+            # however, they shouldn't be removed if window content is
+            # removed.
+            if control != self.native.MainMenuStrip and control != self.toolbar_native:
+                has_content = True
+                self.native.Controls.Remove(control)
+
+        # The first time content is set for the window, we also need
+        # to add the toolbar as part of the main window content.
+        # We use "did we haev to remove any content" as a marker for
+        # whether this is the first time we're setting content.
+        if not has_content:
             self.native.Controls.Add(self.toolbar_native)
-            # Create the lookup table of menu items,
-            # then force the creation of the menus.
+
+        # Add the actual window content.
         self.native.Controls.Add(widget.native)
 
         # Set the widget's viewport to be based on the window's content.
-        widget.viewport = WinFormsViewport(self.native, self)
+        widget.viewport = WinFormsViewport(native=self.native, frame=self)
         widget.frame = self
 
         # Add all children to the content widget.
         for child in widget.interface.children:
             child._impl.container = widget
 
+    def get_title(self):
+        return self.native.Text
+
     def set_title(self, title):
         self.native.Text = title
 
     def show(self):
         # The first render of the content will establish the
         # minimum possible content size; use that to enforce
         # a minimum window size.
         TITLEBAR_HEIGHT = WinForms.SystemInformation.CaptionHeight
         # Now that the content is visible, we can do our initial hinting,
         # and use that as the basis for setting the minimum window size.
         self.interface.content._impl.rehint()
-        self.interface.content.style.layout(self.interface.content, Viewport(0, 0))
+        self.interface.content.style.layout(
+            self.interface.content,
+            WinFormsViewport(native=None, frame=None),
+        )
         self.native.MinimumSize = Size(
             int(self.interface.content.layout.width),
-            int(self.interface.content.layout.height) + TITLEBAR_HEIGHT
+            int(self.interface.content.layout.height) + TITLEBAR_HEIGHT,
         )
         self.interface.content.refresh()
-        if self.interface is self.interface.app._main_window:
-            self.native.FormClosing += self.winforms_FormClosing
 
         if self.interface is not self.interface.app._main_window:
-            self.native.Show()
+            self.native.Icon = self.interface.app.icon._impl.native
+        self.native.Show()
+
+    def hide(self):
+        self.native.Hide()
+
+    def get_visible(self):
+        return self.native.Visible
+
+    def winforms_FormClosing(self, sender, event):
+        # If the app is exiting, or a manual close has been requested,
+        # don't get confirmation; just close.
+        if not self.interface.app._impl._is_exiting and not self._is_closing:
+            if not self.interface.closeable:
+                # Closeability is implemented by shortcutting the close handler.
+                event.Cancel = True
+            elif self.interface.on_close:
+                # If there is an on_close event handler, process it;
+                # but then cancel the close event. If the result of
+                # on_close handling indicates the window should close,
+                # then it will be manually triggered as part of that
+                # result handling.
+                self.interface.on_close(self)
+                event.Cancel = True
 
-            
-    def winforms_FormClosing(self, event, handler):
-        if self.interface.app.on_exit:
-            self.interface.app.on_exit(self.interface.app)
-          
     def set_full_screen(self, is_full_screen):
-        self.interface.factory.not_implemented('Window.set_full_screen()')
-        
-    def on_close(self):
-        pass
+        if is_full_screen:
+            self.native.FormBorderStyle = WinForms.FormBorderStyle(0)
+            self.native.WindowState = WinForms.FormWindowState.Maximized
+        else:
+            self.native.FormBorderStyle = WinForms.FormBorderStyle(1)
+            self.native.WindowState = WinForms.FormWindowState.Normal
 
     def close(self):
+        self._is_closing = True
         self.native.Close()
 
-    def winforms_Resize(self, sender, args):
+    def winforms_resize(self, sender, args):
         if self.interface.content:
             # Re-layout the content
             self.interface.content.refresh()
-
-    def info_dialog(self, title, message):
-        return WinForms.MessageBox.Show(message, title, WinForms.MessageBoxButtons.OK)
-
-    def question_dialog(self, title, message):
-        result = WinForms.MessageBox.Show(message, title, WinForms.MessageBoxButtons.YesNo)
-        return result
-
-    def confirm_dialog(self, title, message):
-        result = WinForms.MessageBox.Show(message, title, WinForms.MessageBoxButtons.OKCancel)
-        # this returns 1 (DialogResult.OK enum) for OK and 2 for Cancel
-        return True if result == WinForms.DialogResult.OK else False
-
-    def error_dialog(self, title, message):
-        return WinForms.MessageBox.Show(message, title, WinForms.MessageBoxButtons.OK,
-                                        WinForms.MessageBoxIcon.Error)
-
-    def stack_trace_dialog(self, title, message, content, retry=False):
-        pass
-
-    def save_file_dialog(self, title, suggested_filename, file_types):
-        dialog = WinForms.SaveFileDialog()
-        dialog.Title = title
-        if suggested_filename is not None:
-            dialog.FileName = suggested_filename
-        if dialog.ShowDialog() == WinForms.DialogResult.OK:
-            return dialog.FileName
-        else:
-            raise ValueError("No filename provided in the save file dialog")
-
-    def open_file_dialog(self, title, initial_directory, file_types, multiselect):
-        dialog = WinForms.OpenFileDialog()
-        dialog.Title = title
-        if initial_directory is not None:
-            dialog.InitialDirectory = initial_directory
-        if file_types is not None:
-            # FIXME This is the example of Filter string: Text files (*.txt)|*.txt|All files (*.*)|*.*
-
-            dialog.Filter = ';'.join(["*." + ext for ext in file_types]) + \
-                            "|All files (*.*)|*.*"
-        if multiselect:
-            dialog.Multiselect = True
-        if dialog.ShowDialog() == WinForms.DialogResult.OK:
-            return dialog.FileName
-        else:
-            raise ValueError("No filename provided in the open file dialog")
-
-    def select_folder_dialog(self, title, initial_directory):
-        dialog = WinForms.FolderBrowserDialog()
-        dialog.Title = title
-        if initial_directory is not None:
-            dialog.InitialDirectory = initial_directory
-
-        if dialog.ShowDialog() == WinForms.DialogResult.OK:
-            return dialog.SelectedPath
-        else:
-            raise ValueError("No folder provided in the select folder dialog")
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/factory.py` & `toga-winforms-0.3.1/src/toga_winforms/factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,74 @@
+from . import dialogs
 from .app import App, MainWindow
 from .command import Command
-# from .font import font
+from .fonts import Font
+from .icons import Icon
+from .images import Image
+from .paths import paths
 from .widgets.box import Box
 from .widgets.button import Button
-# from .widgets.canvas import Canvas
-# from .widgets.detailedlist import DetailedList
-from .widgets.icon import Icon
-from .widgets.image import *
-from .widgets.imageview import *
-from .widgets.label import *
-from .widgets.multilinetextinput import *
+from .widgets.canvas import Canvas
+from .widgets.datepicker import DatePicker
+from .widgets.detailedlist import DetailedList
+from .widgets.divider import Divider
+from .widgets.imageview import ImageView
+from .widgets.label import Label
+from .widgets.multilinetextinput import MultilineTextInput
 from .widgets.numberinput import NumberInput
-from .widgets.optioncontainer import *
-from .widgets.passwordinput import *
-from .widgets.progressbar import *
-from .widgets.scrollcontainer import *
+from .widgets.optioncontainer import OptionContainer
+from .widgets.passwordinput import PasswordInput
+from .widgets.progressbar import ProgressBar
+from .widgets.scrollcontainer import ScrollContainer
 from .widgets.selection import Selection
-from .widgets.slider import *
-from .widgets.splitcontainer import *
-from .widgets.switch import *
-from .widgets.table import *
-from .widgets.webview import *
+from .widgets.slider import Slider
+from .widgets.splitcontainer import SplitContainer
+from .widgets.switch import Switch
+from .widgets.table import Table
+from .widgets.textinput import TextInput
+from .widgets.timepicker import TimePicker
+from .widgets.tree import Tree
+from .widgets.webview import WebView
 from .window import Window
 
 
 def not_implemented(feature):
-    print('[Winforms] Not implemented: {}'.format(feature))
+    print(f"[Winforms] Not implemented: {feature}")  # pragma: nocover
 
 
 __all__ = [
-    'not_implemented',
-
-    'App', 'MainWindow',
-    # 'color',
-    'Command',
-    # 'font',
-    'Box',
-    'Button',
-    # 'Canvas',
-    # 'DetailedList',
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
-    # 'Tree',
-    'WebView',
-    'Window',
+    "not_implemented",
+    "App",
+    "MainWindow",
+    "Command",
+    # Resources
+    "Font",
+    "Icon",
+    "Image",
+    "paths",
+    "dialogs",
+    # Widgets
+    "Box",
+    "Button",
+    "Canvas",
+    "Divider",
+    "DetailedList",
+    "ImageView",
+    "DatePicker",
+    "TimePicker",
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

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/tree.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 
 
 class Tree(Widget):
     def create(self):
         self.native = WinForms.TreeView()
 
     def row_data(self, item):
-        self.interface.factory.not_implemented('Tree.row_data()')
+        self.interface.factory.not_implemented("Tree.row_data()")
 
     def on_select(self, selection):
-        self.interface.factory.not_implemented('Tree.on_select()')
+        self.interface.factory.not_implemented("Tree.on_select()")
 
     def change_source(self, source):
-        self.interface.factory.not_implemented('Tree.change_source()')
+        self.interface.factory.not_implemented("Tree.change_source()")
 
-    def insert(self, parent, index, item, **kwargs):
-        self.interface.factory.not_implemented('Tree.insert()')
+    def insert(self, parent, index, item):
+        self.interface.factory.not_implemented("Tree.insert()")
 
     def change(self, item):
-        self.interface.factory.not_implemented('Tree.change()')
+        self.interface.factory.not_implemented("Tree.change()")
 
-    def remove(self, item):
-        self.interface.factory.not_implemented('Tree.remove()')
+    def remove(self, parent, index, item):
+        self.interface.factory.not_implemented("Tree.remove()")
 
     def clear(self):
-        self.interface.factory.not_implemented('Tree.clear()')
+        self.interface.factory.not_implemented("Tree.clear()")
+
+    def get_selection(self):
+        self.interface.factory.not_implemented("Tree.get_selection()")
 
     def set_on_select(self, handler):
-        self.interface.factory.not_implemented('Tree.set_on_select()')
+        self.interface.factory.not_implemented("Tree.set_on_select()")
+
+    def set_on_double_click(self, handler):
+        self.interface.factory.not_implemented("Table.set_on_double_click()")
 
     def scroll_to_node(self, node):
-        self.interface.factory.not_implemented('Tree.scroll_to_node()')
+        self.interface.factory.not_implemented("Tree.scroll_to_node()")
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/imageview.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/imageview.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from toga_winforms.libs import WinForms, Color, Size
+from toga_winforms.libs import Color, Size, WinForms
 
 from .base import Widget
 
 
 class ImageView(Widget):
-
     def create(self):
         self.native = WinForms.PictureBox()
         self.native.interface = self.interface
-        self.native.SizeMode = WinForms.PictureBoxSizeMode.StretchImage
-
-    def get_image(self):
-        return self.native.Image
+        self.native.SizeMode = WinForms.PictureBoxSizeMode.Zoom
 
     def set_image(self, image):
-        if image and image.path is not None:
+        # If an image already exists, ensure it is destroyed
+        if self.native.Image is not None:
+            self.native.Image.Dispose()
+        if image:
             # Workaround for loading image from url
-            if isinstance(image._impl.native, str):
-                self.native.Load(image._impl.native)
+            if self.interface._image._impl.url:
+                self.native.Load(self.interface._image._impl.url)
             else:
-                self.native.Image = image._impl.native
+                self.native.Image = self.interface._image._impl.native
         else:
             width = 0
             height = 0
             if self.interface.style.width:
                 width = self.interface.style.width
             if self.interface.style.height:
                 height = self.interface.style.height
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/splitcontainer.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/optioncontainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,72 @@
-from toga_winforms.libs import WinForms, Size, Point
+from toga_winforms.libs import WinForms
 from toga_winforms.window import WinFormsViewport
 
 from .base import Widget
 
 
-class SplitContainer(Widget):
+class OptionContainer(Widget):
     def create(self):
-        self.native = WinForms.SplitContainer()
-        self.native.interface = self.interface
-        self.native.Resize += self.on_resize
-        self.native.SplitterMoved += self.on_resize
-        self.ratio = None
+        self.native = WinForms.TabControl()
+        self.native.Selected += self.winforms_selected
 
-    def add_content(self, position, widget):
+    def add_content(self, index, text, widget):
+        widget.viewport = WinFormsViewport(self.native, self)
         widget.frame = self
-
         # Add all children to the content widget.
         for child in widget.interface.children:
             child._impl.container = widget
 
-        if position >= 2:
-            raise ValueError('SplitContainer content must be a 2-tuple')
+        item = WinForms.TabPage()
+        item.Text = text
 
-        if position == 0:
-            self.native.Panel1.Controls.Add(widget.native)
-            widget.viewport = WinFormsViewport(self.native.Panel1, self)
-
-        elif position == 1:
-            self.native.Panel2.Controls.Add(widget.native)
-            widget.viewport = WinFormsViewport(self.native.Panel2, self)
-
-    def set_app(self, app):
-        if self.interface.content:
-            for content in self.interface.content:
-                content.app = self.interface.app
-
-    def set_window(self, window):
-        if self.interface.content:
-            for content in self.interface.content:
-                content.window = self.interface.window
-
-    def set_direction(self, value):
-        self.native.Orientation = WinForms.Orientation.Vertical if value \
-            else WinForms.Orientation.Horizontal
-
-    def on_resize(self, sender, args):
-        if self.interface.content:
-            # Re-layout the content
-            for content in self.interface.content:
-                content.refresh()
+        # Enable AutoSize on the container to fill
+        # the available space in the OptionContainer.
+        widget.AutoSize = True
+
+        item.Controls.Add(widget.native)
+        if index < self.native.TabPages.Count:
+            self.native.TabPages.Insert(index, item)
+        else:
+            self.native.TabPages.Add(item)
+
+    def remove_content(self, index):
+        tab_page = self.native.TabPages[index]
+        self.native.TabPages.Remove(self.native.TabPages[index])
+        tab_page.Dispose()
+
+    def set_on_select(self, handler):
+        pass
+
+    def set_option_enabled(self, index, enabled):
+        """Winforms documentation states that Enabled is not meaningful for
+        this control.
+
+        Disabling option only disables the content of the tab, not the
+        tab itself.
+        """
+        self.native.TabPages[index].Enabled = enabled
+
+    def is_option_enabled(self, index):
+        return self.native.TabPages[index].Enabled
+
+    def set_option_text(self, index, value):
+        self.native.TabPages[index].Text = value
+
+    def get_option_text(self, index):
+        return self.native.TabPages[index].Text
+
+    def get_current_tab_index(self):
+        return self.native.SelectedIndex
+
+    def set_current_tab_index(self, current_tab_index):
+        self.native.SelectedIndex = current_tab_index
+
+    def winforms_selected(self, sender, event):
+        if self.interface.on_select:
+            self.interface.on_select(
+                self.interface, option=self.interface.content[self.native.SelectedIndex]
+            )
+
+    def set_font(self, font):
+        if font:
+            self.native.Font = font._impl.native
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/multilinetextinput.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/divider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from toga_winforms.libs import WinForms
 from travertino.size import at_least
 
+from toga_winforms.libs import WinForms
+
 from .base import Widget
 
 
-class MultilineTextInput(Widget):
+class Divider(Widget):
     def create(self):
-        # because https://stackoverflow.com/a/612234
-        self.native = WinForms.RichTextBox()
-        self.native.Multiline = True
-
-    def set_readonly(self, value):
-        self.native.ReadOnly = self.interface.readonly
-
-    def set_placeholder(self, value):
-        # self.native.cell.placeholderString = self._placeholder
-        self.interface.factory.not_implemented('MultilineTextInput.set_placeholder()')
-
-    def set_value(self, value):
-        self.native.Text = value
-
-    def get_value(self):
-        return self.native.Text
+        self.native = WinForms.Label()
+        self.native.BorderStyle = WinForms.BorderStyle.Fixed3D
+        self.native.AutoSize = False
+
+        self._direction = self.interface.HORIZONTAL
+
+    def get_direction(self):
+        return self._direction
+
+    def set_direction(self, value):
+        self._direction = value
+        if value == self.interface.HORIZONTAL:
+            self.native.Height = 2
+            self.native.Width = 0
+        else:
+            self.native.Height = 0
+            self.native.Width = 2
 
     def rehint(self):
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
-        self.interface.intrinsic.height = at_least(self.interface.MIN_HEIGHT)
+        if self.get_direction() == self.interface.HORIZONTAL:
+            self.interface.intrinsic.width = at_least(self.native.Width)
+            self.interface.intrinsic.height = self.native.Height
+        else:
+            self.interface.intrinsic.width = self.native.Width
+            self.interface.intrinsic.height = at_least(self.native.Height)
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/textinput.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/numberinput.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-from toga_winforms.libs import WinForms, HorizontalTextAlignment
+import sys
+
 from travertino.size import at_least
 
+from toga_winforms.libs import Convert, HorizontalTextAlignment, WinForms
+
 from .base import Widget
 
 
-class TextInput(Widget):
+class NumberInput(Widget):
     def create(self):
-        self.native = WinForms.TextBox()
-        self.native.Multiline = False
+        self.native = WinForms.NumericUpDown()
+        self.native.Value = Convert.ToDecimal(0.0)
+        self.native.ValueChanged += self.winforms_value_changed
+
+    def winforms_value_changed(self, sender, event):
+        if self.container:
+            self.interface.value = Convert.ToString(sender.Value)
+            if self.interface.on_change:
+                self.interface.on_change(self.interface)
 
     def set_readonly(self, value):
-        self.native.ReadOnly = value
+        self.native.ReadOnly = self.interface.readonly
 
-    def set_placeholder(self, value):
-        self.native.Text = self.interface.placeholder
-
-    def get_value(self):
-        return self.native.Text
+    def set_step(self, step):
+        self.native.Increment = Convert.ToDecimal(float(self.interface.step))
+        self.native.DecimalPlaces = abs(self.interface.step.as_tuple().exponent)
+
+    def set_min_value(self, value):
+        if self.interface.min_value is None:
+            self.native.Minimum = Convert.ToDecimal(-sys.maxsize - 1)
+        else:
+            self.native.Minimum = Convert.ToDecimal(float(self.interface.min_value))
+
+    def set_max_value(self, value):
+        if self.interface.max_value is None:
+            self.native.Maximum = Convert.ToDecimal(sys.maxsize)
+        else:
+            self.native.Maximum = Convert.ToDecimal(float(self.interface.max_value))
 
     def set_value(self, value):
-        self.native.Text = value
+        if value is None or value == "":
+            self.native.Value = Convert.ToDecimal(0.0)
+        else:
+            self.native.Value = Convert.ToDecimal(float(self.interface.value))
 
     def set_alignment(self, value):
         self.native.TextAlign = HorizontalTextAlignment(value)
 
-    def set_font(self, value):
-        self.interface.factory.not_implemented('TextInput.set_font()')
+    def set_font(self, font):
+        if font:
+            self.native.Font = font._impl.native
 
     def rehint(self):
-        # Height of a text input is known and fixed.
-        # Width must be > 100
-        # print("REHINT TextInput", self, self.native.PreferredSize)
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
         self.interface.intrinsic.height = self.native.PreferredSize.Height
 
     def set_on_change(self, handler):
-        self.native.TextChanged += self.on_text_change
-
-    def on_text_change(self, sender, event):
-        if self.interface._on_change:
-            self.interface.on_change(self.interface)
+        pass
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/switch.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/selection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-from toga_winforms.libs import WinForms
 from travertino.size import at_least
 
+from toga_winforms.libs import WinForms
+
 from .base import Widget
 
 
-class TogaSwitch(WinForms.CheckBox):
+class TogaComboBox(WinForms.ComboBox):
     def __init__(self, interface):
         super().__init__()
         self.interface = interface
-        self.CheckedChanged += self.on_toggle
+        self.DropDownStyle = WinForms.ComboBoxStyle.DropDownList
+        self.SelectedIndexChanged += self.winforms_selected_index_changed
 
-    def on_toggle(self, sender, event):
-        if self.interface.on_toggle:
-            self.interface.on_toggle(self.interface)
+    def winforms_selected_index_changed(self, sender, event):
+        if self.interface.on_select:
+            self.interface.on_select(self.interface)
 
 
-class Switch(Widget):
+class Selection(Widget):
     def create(self):
-        self.native = TogaSwitch(self.interface)
+        self.native = TogaComboBox(self.interface)
+
+    def remove_all_items(self):
+        self.native.Items.Clear()
+
+    def add_item(self, item):
+        self.native.Items.Add(item)
 
-    def set_label(self, label):
-        self.native.Text = label
+        # WinfForm.ComboBox does not select the first item, so it's done here.
+        if not self.get_selected_item():
+            self.native.SelectedIndex = 0
 
-    def set_is_on(self, value):
-        if value is True:
-            self.native.Checked = True
-        elif value is False:
-            self.native.Checked = False
+    def select_item(self, item):
+        self.native.SelectedItem = item
 
-    def get_is_on(self):
-        return self.native.Checked
+    def get_selected_item(self):
+        return self.native.SelectedItem
 
-    def set_on_toggle(self, handler):
+    def set_on_select(self, handler):
         pass
 
     def rehint(self):
         self.interface.intrinsic.width = at_least(self.native.PreferredSize.Width)
         self.interface.intrinsic.height = self.native.PreferredSize.Height
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/label.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/label.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from travertino.size import at_least
 
-from toga_winforms.libs import WinForms, TextAlignment
+from toga_winforms.libs import TextAlignment, WinForms
 
 from .base import Widget
 
 
 class Label(Widget):
     def create(self):
         self.native = WinForms.Label()
+        self.native.AutoSizeMode = WinForms.AutoSizeMode.GrowAndShrink
 
     def set_alignment(self, value):
         self.native.TextAlign = TextAlignment(value)
 
+    def get_text(self):
+        return self.native.Text
+
     def set_text(self, value):
-        self.native.Text = self.interface._text
+        self.native.Text = value
+
+    def set_font(self, font):
+        self.native.Font = font._impl.native
 
     def rehint(self):
         # Width & height of a label is known and fixed.
         # self.native.Size = Size(0, 0)
         # print("REHINT label", self, self.native.PreferredSize)
         self.interface.intrinsic.width = at_least(self.native.PreferredSize.Width)
         self.interface.intrinsic.height = self.native.PreferredSize.Height
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/numberinput.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/multilinetextinput.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,88 @@
-import sys
-from toga_winforms.libs import LEFT, RIGHT, CENTER
-from toga_winforms.libs import WinForms, Convert, HorizontalTextAlignment
 from travertino.size import at_least
 
+from toga_winforms.colors import native_color
+from toga_winforms.libs import SystemColors, WinForms
+
 from .base import Widget
 
 
-class NumberInput(Widget):
+class MultilineTextInput(Widget):
     def create(self):
-        self.native = WinForms.NumericUpDown()
-        self.native.Value = Convert.ToDecimal(0.0)
+        # because https://stackoverflow.com/a/612234
+        self.native = WinForms.RichTextBox()
+        self.native.Multiline = True
+        self.native.TextChanged += self.winforms_text_changed
+        self.native.Enter += self.winforms_enter
+        self.native.Leave += self.winforms_leave
+        self._placeholder = None
+        self._color = SystemColors.WindowText
+
+    def winforms_enter(self, sender, event):
+        if self._placeholder != "" and self.native.Text == self._placeholder:
+            self.native.Text = ""
+            self._update_text_color()
+
+    def winforms_leave(self, sender, event):
+        self._update_text()
+
+    def set_font(self, font):
+        if font:
+            self.native.Font = font._impl.native
 
     def set_readonly(self, value):
         self.native.ReadOnly = self.interface.readonly
 
-    def set_step(self, step):
-        self.native.Increment = Convert.ToDecimal(float(self.interface.step))
-        self.native.DecimalPlaces = abs(self.interface.step.as_tuple().exponent)
-
-    def set_min_value(self, value):
-        if self.interface.min_value is None:
-            self.native.Minimum = Convert.ToDecimal(-sys.maxsize - 1)
-        else:
-            self.native.Minimum = Convert.ToDecimal(self.interface.min_value)
-
-    def set_max_value(self, value):
-        if self.interface.max_value is None:
-            self.native.Maximum = Convert.ToDecimal(sys.maxsize)
-        else:
-            self.native.Maximum = Convert.ToDecimal(self.interface.max_value)
+    def set_placeholder(self, value):
+        self._placeholder = value
+        self._update_text()
 
     def set_value(self, value):
-        if value is None or value is '':
-            self.native.Value = Convert.ToDecimal(0.0)
-        else:
-            self.native.Value = Convert.ToDecimal(float(self.interface.value))
-
-    def set_alignment(self, value):
-        self.native.TextAlign = HorizontalTextAlignment(value)
+        self.native.Text = value
+        self._update_text()
 
-    def set_font(self, value):
-        self.interface.factory.not_implemented('NumberInput.set_font()')
+    def get_value(self):
+        if self._placeholder != "" and self.native.Text == self._placeholder:
+            return ""
+        else:
+            return self.native.Text
 
     def rehint(self):
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
-        self.interface.intrinsic.height = self.native.PreferredSize.Height
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = at_least(self.interface._MIN_HEIGHT)
 
     def set_on_change(self, handler):
-        self.native.ValueChanged += self.on_number_change
+        pass
 
-    def on_number_change(self, sender, event):
-        self.interface.value = Convert.ToString(sender.Value)
+    def winforms_text_changed(self, sender, event):
         if self.interface.on_change:
             self.interface.on_change(self.interface)
+
+    def _update_text(self):
+        if self._placeholder != "" and self.native.Text == "":
+            self.native.Text = self._placeholder
+            self._update_placeholder_color()
+        else:
+            self._update_text_color()
+
+    def _update_text_color(self):
+        self.native.ForeColor = self._color
+
+    def _update_placeholder_color(self):
+        self.native.ForeColor = SystemColors.GrayText
+
+    def set_color(self, color):
+        if color:
+            self._color = native_color(color)
+            self._update_text_color()
+
+    def set_background_color(self, value):
+        if value:
+            self.native.BackColor = native_color(value)
+
+    def scroll_to_bottom(self):
+        self.native.SelectionStart = len(self.native.Text)
+        self.native.ScrollToCaret()
+
+    def scroll_to_top(self):
+        self.native.SelectionStart = 0
+        self.native.ScrollToCaret()
```

### Comparing `toga-winforms-0.3.0.dev9/toga_winforms/widgets/table.py` & `toga-winforms-0.3.1/src/toga_winforms/widgets/scrollcontainer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,87 @@
-from travertino.size import at_least
-
 from toga_winforms.libs import WinForms
+from toga_winforms.window import WinFormsViewport
 
 from .base import Widget
 
 
-class Table(Widget):
+class ScrollContainer(Widget):
     def create(self):
-        self._container = self
-        self.native = WinForms.ListView()
-        self.native.View = WinForms.View.Details
-
-        dataColumn = []
-        for heading in self.interface.headings:
-            col = WinForms.ColumnHeader()
-            col.Text = heading
-            dataColumn.append(col)
-
-        self.native.FullRowSelect = True
-        self.native.Multiselect = self.interface.multiple_select
-        self.native.Columns.AddRange(dataColumn)
-
-    def change_source(self, source):
-        for index, row in enumerate(self.interface.data):
-            row._impl = WinForms.ListViewItem([
-                getattr(row, attr) for attr in self.interface._accessors
-            ])
-            self.native.Items.Insert(index, row._impl)
-
-    def update_data(self):
-        self.native.Items.Clear()
-        for index, row in enumerate(self.interface.data):
-            row._impl = WinForms.ListViewItem([
-                getattr(row, attr) for attr in self.interface._accessors
-            ])
-            self.native.Items.Insert(index, row._impl)
-
-    def insert(self, index, item):
-        item._impl = WinForms.ListViewItem([
-            getattr(item, attr) for attr in self.interface._accessors
-        ])
-        self.native.Items.Insert(index, item._impl)
-
-    def change(self, item):
-        self.interface.factory.not_implemented('Table.change()')
-
-    def remove(self, item):
-        self.update_data()
-
-    def clear(self):
-        self.native.Items.Clear()
-
-    def set_on_select(self, handler):
-        self.interface.factory.not_implemented('Table.set_on_select()')
-
-    def scroll_to_row(self, row):
-        self.native.EnsureVisible(row)
-        self.interface.factory.not_implemented('Table.scroll_to_row()')
-
-    def rehint(self):
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
-        self.interface.intrinsic.height = at_least(self.interface.MIN_HEIGHT)
+        self.native = WinForms.Panel()
+        self.native.interface = self.interface
+        self.native.AutoScroll = True
+        self.native.Scroll += self.winforms_scroll
+        self.native.MouseWheel += self.winforms_scroll
+
+    def winforms_scroll(self, sender, event):
+        if self.interface.on_scroll is not None:
+            self.interface.on_scroll(self.interface)
+
+    def set_content(self, widget):
+        self.inner_container = widget
+
+        widget.viewport = WinFormsViewport(self.native, self)
+        widget.frame = self
+
+        for child in widget.interface.children:
+            child._impl.container = widget
+
+        self.native.Controls.Add(self.inner_container.native)
+
+    def set_horizontal(self, value):
+        self.native.AutoScroll = False
+        self.native.HorizontalScroll.Enabled = value
+        self.native.HorizontalScroll.Visible = value
+        self.native.AutoScroll = True
+
+    def set_vertical(self, value):
+        self.native.AutoScroll = False
+        self.native.VerticalScroll.Enabled = value
+        self.native.VerticalScroll.Visible = value
+        self.native.AutoScroll = True
+
+    def set_window(self, window):
+        if self.interface.content:
+            self.interface.content.window = window
+
+    def set_on_scroll(self, on_scroll):
+        # Do nothing
+        pass
+
+    def get_vertical_position(self):
+        return self.native.VerticalScroll.Value
+
+    def set_vertical_position(self, vertical_position):
+        if vertical_position < 0 or vertical_position > self.maximum_vertical_position:
+            raise ValueError(
+                "Vertical position should be between 0 and {}, got {}".format(
+                    self.maximum_vertical_position, vertical_position
+                )
+            )
+        self.native.VerticalScroll.Value = vertical_position
+        if self.interface.on_scroll is not None:
+            self.interface.on_scroll(self.interface)
+
+    def get_horizontal_position(self):
+        return self.native.HorizontalScroll.Value
+
+    def set_horizontal_position(self, horizontal_position):
+        if (
+            horizontal_position < 0
+            or horizontal_position > self.maximum_horizontal_position
+        ):
+            raise ValueError(
+                "Horizontal position should be between 0 and {}, got {}".format(
+                    self.maximum_horizontal_position, horizontal_position
+                )
+            )
+        self.native.HorizontalScroll.Value = horizontal_position
+        if self.interface.on_scroll is not None:
+            self.interface.on_scroll(self.interface)
+
+    @property
+    def maximum_vertical_position(self):
+        return self.native.VerticalScroll.Maximum
+
+    @property
+    def maximum_horizontal_position(self):
+        return self.native.HorizontalScroll.Maximum
```

