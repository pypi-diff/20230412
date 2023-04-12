# Comparing `tmp/toga-gtk-0.3.0.dev9.tar.gz` & `tmp/toga-gtk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toga-gtk-0.3.0.dev9.tar", last modified: Sat Jul  7 05:55:20 2018, max compression
+gzip compressed data, was "toga-gtk-0.3.1.tar", last modified: Wed Apr 12 01:58:52 2023, max compression
```

## Comparing `toga-gtk-0.3.0.dev9.tar` & `toga-gtk-0.3.1.tar`

### file list

```diff
@@ -1,60 +1,106 @@
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/
--rw-r--r--   0 rkm        (501) staff       (20)     3179 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/PKG-INFO
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk/
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk/hardware/
--rw-r--r--   0 rkm        (501) staff       (20)        0 2018-05-26 09:29:22.000000 toga-gtk-0.3.0.dev9/toga_gtk/hardware/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      182 2017-12-23 03:47:56.000000 toga-gtk-0.3.0.dev9/toga_gtk/color.py
--rw-r--r--   0 rkm        (501) staff       (20)      498 2017-12-22 11:14:30.000000 toga-gtk-0.3.0.dev9/toga_gtk/command.py
--rw-r--r--   0 rkm        (501) staff       (20)     5758 2018-06-10 23:51:35.000000 toga-gtk-0.3.0.dev9/toga_gtk/window.py
--rw-r--r--   0 rkm        (501) staff       (20)      351 2018-05-17 17:50:36.000000 toga-gtk-0.3.0.dev9/toga_gtk/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     2327 2018-07-07 05:52:00.000000 toga-gtk-0.3.0.dev9/toga_gtk/font.py
--rw-r--r--   0 rkm        (501) staff       (20)     1616 2018-06-10 23:51:35.000000 toga-gtk-0.3.0.dev9/toga_gtk/factory.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk/libs/
--rw-r--r--   0 rkm        (501) staff       (20)       21 2017-12-22 11:14:05.000000 toga-gtk-0.3.0.dev9/toga_gtk/libs/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      340 2017-12-23 03:47:56.000000 toga-gtk-0.3.0.dev9/toga_gtk/libs/utils.py
--rw-r--r--   0 rkm        (501) staff       (20)     5126 2018-07-07 05:52:00.000000 toga-gtk-0.3.0.dev9/toga_gtk/app.py
--rw-r--r--   0 rkm        (501) staff       (20)     3893 2018-06-10 23:51:35.000000 toga-gtk-0.3.0.dev9/toga_gtk/dialogs.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)     1310 2018-05-26 09:29:22.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/icon.py
--rw-r--r--   0 rkm        (501) staff       (20)     2819 2018-01-18 21:56:40.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/tree.py
--rw-r--r--   0 rkm        (501) staff       (20)     2367 2018-07-07 05:52:00.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)     2714 2018-01-12 22:11:27.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/box.py
--rw-r--r--   0 rkm        (501) staff       (20)     1380 2018-01-25 04:51:21.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/splitcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     1431 2018-05-26 09:29:22.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/detailedlist.py
--rw-r--r--   0 rkm        (501) staff       (20)     2243 2017-12-29 03:46:07.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/multilinetextinput.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1340 2018-02-21 05:36:56.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/textinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     1485 2018-02-21 05:36:56.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/switch.py
--rw-r--r--   0 rkm        (501) staff       (20)     1466 2017-12-28 05:25:04.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/scrollcontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)     1324 2018-05-26 09:29:22.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/slider.py
--rw-r--r--   0 rkm        (501) staff       (20)     1271 2018-01-25 04:51:21.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/button.py
--rw-r--r--   0 rkm        (501) staff       (20)     1605 2018-02-21 05:36:56.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/progressbar.py
--rw-r--r--   0 rkm        (501) staff       (20)     1594 2018-01-18 21:56:40.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/label.py
--rw-r--r--   0 rkm        (501) staff       (20)     2335 2018-05-17 17:50:27.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/numberinput.py
--rw-r--r--   0 rkm        (501) staff       (20)      308 2017-12-22 11:14:05.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/passwordinput.py
--rw-r--r--   0 rkm        (501) staff       (20)     1451 2018-01-18 21:56:40.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/table.py
--rw-r--r--   0 rkm        (501) staff       (20)     1303 2018-05-17 17:50:27.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/selection.py
--rw-r--r--   0 rkm        (501) staff       (20)     1926 2018-01-25 04:51:21.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/webview.py
--rw-r--r--   0 rkm        (501) staff       (20)      721 2018-01-18 21:56:40.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/optioncontainer.py
--rw-r--r--   0 rkm        (501) staff       (20)      219 2018-06-10 23:51:35.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/image.py
--rw-r--r--   0 rkm        (501) staff       (20)     2026 2018-05-26 09:29:22.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/base.py
--rw-r--r--   0 rkm        (501) staff       (20)     5966 2018-07-07 05:52:00.000000 toga-gtk-0.3.0.dev9/toga_gtk/widgets/canvas.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk.egg-info/
--rw-rw-r--   0 rkm        (501) staff       (20)     3179 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk.egg-info/PKG-INFO
--rw-rw-r--   0 rkm        (501) staff       (20)     1308 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk.egg-info/SOURCES.txt
--rw-rw-r--   0 rkm        (501) staff       (20)       69 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk.egg-info/requires.txt
--rw-rw-r--   0 rkm        (501) staff       (20)       15 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk.egg-info/top_level.txt
--rw-rw-r--   0 rkm        (501) staff       (20)        1 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/toga_gtk.egg-info/dependency_links.txt
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/tests/
--rw-r--r--   0 rkm        (501) staff       (20)     3564 2018-05-26 09:29:22.000000 toga-gtk-0.3.0.dev9/tests/test_font.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:05.000000 toga-gtk-0.3.0.dev9/tests/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)      273 2017-12-22 11:14:30.000000 toga-gtk-0.3.0.dev9/tests/test_implementation.py
-drwxr-xr-x   0 rkm        (501) staff       (20)        0 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/tests/widgets/
--rw-r--r--   0 rkm        (501) staff       (20)     8519 2017-12-23 03:47:56.000000 toga-gtk-0.3.0.dev9/tests/widgets/test_tree.py
--rw-r--r--   0 rkm        (501) staff       (20)     6736 2017-12-22 11:14:30.000000 toga-gtk-0.3.0.dev9/tests/widgets/test_table.py
--rw-r--r--   0 rkm        (501) staff       (20)        0 2017-12-22 11:14:30.000000 toga-gtk-0.3.0.dev9/tests/widgets/__init__.py
--rw-r--r--   0 rkm        (501) staff       (20)     1283 2018-06-10 23:51:35.000000 toga-gtk-0.3.0.dev9/tests/widgets/test_imageview.py
--rw-r--r--   0 rkm        (501) staff       (20)      111 2017-12-22 11:14:05.000000 toga-gtk-0.3.0.dev9/MANIFEST.in
--rw-r--r--   0 rkm        (501) staff       (20)     1731 2018-07-07 05:52:00.000000 toga-gtk-0.3.0.dev9/setup.py
--rw-r--r--   0 rkm        (501) staff       (20)       38 2018-07-07 05:55:20.000000 toga-gtk-0.3.0.dev9/setup.cfg
--rw-r--r--   0 rkm        (501) staff       (20)     1824 2017-12-22 11:14:05.000000 toga-gtk-0.3.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.394464 toga-gtk-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 01:58:52.394464 toga-gtk-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-12 01:58:52.394464 toga-gtk-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.374463 toga-gtk-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.378463 toga-gtk-0.3.1/src/toga_gtk/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.382464 toga-gtk-0.3.1/src/toga_gtk/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.382464 toga-gtk-0.3.1/src/toga_gtk/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/libs/gtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/libs/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/libs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.386463 toga-gtk-0.3.1/src/toga_gtk/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/imageview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.386463 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.386463 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/buttons/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/buttons/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/buttons/scroll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.390463 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/rows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/rows/scrollable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/rows/texticon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/internal/sourcetreemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/multilinetextinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/numberinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/optioncontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/scrollcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/splitcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/widgets/webview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/src/toga_gtk/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.382464 toga-gtk-0.3.1/src/toga_gtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 01:58:52.000000 toga-gtk-0.3.1/src/toga_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-12 01:58:52.000000 toga-gtk-0.3.1/src/toga_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:52.000000 toga-gtk-0.3.1/src/toga_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 01:58:52.000000 toga-gtk-0.3.1/src/toga_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:58:34.000000 toga-gtk-0.3.1/src/toga_gtk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 01:58:52.000000 toga-gtk-0.3.1/src/toga_gtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 01:58:52.000000 toga-gtk-0.3.1/src/toga_gtk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.390463 toga-gtk-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/test_font.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/test_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.390463 toga-gtk-0.3.1/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/widgets/test_detailedlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/widgets/test_imageview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/widgets/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/widgets/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/widgets/test_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests/widgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.390463 toga-gtk-0.3.1/tests_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:52.394464 toga-gtk-0.3.1/tests_backend/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 01:58:01.000000 toga-gtk-0.3.1/tests_backend/widgets/textinput.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/font.py` & `toga-gtk-0.3.1/src/toga_gtk/fonts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,46 @@
-from toga.constants import ITALIC, OBLIQUE, SMALL_CAPS, BOLD, SYSTEM
-import gi
+from toga.constants import (
+    BOLD,
+    ITALIC,
+    OBLIQUE,
+    SMALL_CAPS,
+    SYSTEM,
+    SYSTEM_DEFAULT_FONT_SIZE,
+)
 
-gi.require_version("Gtk", "3.0")
-from gi.repository import Gtk
-
-try:
-    gi.require_version("Pango", "1.0")
-    from gi.repository import Pango
-except ImportError:
-    Pango = None
+from .libs import Pango
 
 _FONT_CACHE = {}
 
 
-class Measure(Gtk.Widget):
-    """Gtk.Widget for Font.measure in order to create a Pango Layout
-    """
-
-    def create(self):
-        pass
-
-
 class Font:
     def __init__(self, interface):
         self.interface = interface
 
         if Pango is None:
             raise RuntimeError(
-                "'from gi.repository import Pango' failed; may need to install gir1.2-pango-1.0."
+                "'from gi.repository import Pango' failed; you may need to install gir1.2-pango-1.0."
             )
 
         try:
             font = _FONT_CACHE[self.interface]
         except KeyError:
-
             # Initialize font with properties 'None NORMAL NORMAL NORMAL 0'
             font = Pango.FontDescription()
 
             # Set font family
             family = self.interface.family
             if family != SYSTEM:
-                family = '{}, {}'.format(family, SYSTEM)  # Default to system
+                family = f"{family}, {SYSTEM}"  # Default to system
 
             font.set_family(family)
 
-            # Set font size
-            font.set_size(self.interface.size * Pango.SCALE)
+            # If this is a non-default font size, set the font size
+            if self.interface.size != SYSTEM_DEFAULT_FONT_SIZE:
+                font.set_size(self.interface.size * Pango.SCALE)
 
             # Set font style
             if self.interface.style == ITALIC:
                 font.set_style(Pango.Style.ITALIC)
             elif self.interface.style == OBLIQUE:
                 font.set_style(Pango.Style.OBLIQUE)
 
@@ -61,17 +52,17 @@
             if self.interface.weight == BOLD:
                 font.set_weight(Pango.Weight.BOLD)
 
             _FONT_CACHE[self.interface] = font
 
         self.native = font
 
-    def measure(self, text, tight=False):
-        measure_widget = Measure()
-        layout = measure_widget.create_pango_layout(text)
+    def measure(self, text, widget, tight=False):
+        layout = widget.create_pango_layout(text)
+
         layout.set_font_description(self.native)
         ink, logical = layout.get_extents()
         if tight:
             width = (ink.width / Pango.SCALE) - (ink.width * 0.2) / Pango.SCALE
             height = ink.height / Pango.SCALE
         else:
             width = (logical.width / Pango.SCALE) - (logical.width * 0.2) / Pango.SCALE
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/widgets/multilinetextinput.py` & `toga-gtk-0.3.1/src/toga_gtk/widgets/multilinetextinput.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,83 @@
-from gi.repository import Gtk
+from travertino.size import at_least
 
+from ..libs import Gtk
 from .base import Widget
 
 
 class MultilineTextInput(Widget):
     def create(self):
-        self.native = Gtk.TextView()
-        self.native.interface = self.interface
-        self.buffer = Gtk.TextBuffer()
-        self.native.set_buffer(self.buffer)
+        # Wrap the TextView in a ScrolledWindow in order to show a
+        # vertical scroll bar when necessary.
+        self.native = Gtk.ScrolledWindow()
+        self.native.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
 
-        self._placeholder = ''
-        self.native.connect("focus-in-event", self.on_focus_in)
-        self.native.connect("focus-out-event", self.on_focus_out)
-        self.tag_placholder = self.buffer.create_tag("placeholder", foreground="gray")
+        self.textview = Gtk.TextView()
+        self.buffer = Gtk.TextBuffer()
+        self.textview.set_buffer(self.buffer)
+        self.textview.set_wrap_mode(Gtk.WrapMode.WORD_CHAR)
+        self.native.add(self.textview)
+
+        self._placeholder = ""
+        self.textview.connect("focus-in-event", self.gtk_on_focus_in)
+        self.textview.connect("focus-out-event", self.gtk_on_focus_out)
+        self.tag_placeholder = self.buffer.create_tag("placeholder", foreground="gray")
 
     def set_value(self, value):
         self.buffer.set_text(value)
 
     def get_value(self):
-        return self.buffer.get_text(self.buffer.get_start_iter(), self.buffer.get_end_iter(), True)
+        return self.buffer.get_text(
+            self.buffer.get_start_iter(), self.buffer.get_end_iter(), True
+        )
 
     def set_readonly(self, value):
-        self.native.set_property('editable', not value)
-        self.native.set_property('cursor-visible', not value)
+        self.textview.set_property("editable", not value)
+        self.textview.set_property("cursor-visible", not value)
 
     def set_placeholder(self, value):
-        """ Set the placeholder text of the widget.
-        GTK.TextView does not have a placeholder option by default so we have to create one.
-        We do this with the two helper functions `on_focus_in` and `on_focus_out`.
+        """Set the placeholder text of the widget.
+
+        GTK.TextView does not have a placeholder option by default so we
+        have to create one. We do this with the two helper functions
+        `on_focus_in` and `on_focus_out`.
         """
         if self.get_value() == self._placeholder:
             self._placeholder = value
-            self.buffer.set_text(value)
-            self.buffer.apply_tag(self.tag_placholder,
-                                  self.buffer.get_start_iter(),
-                                  self.buffer.get_end_iter())  # make the placeholder text gray.
+            self.buffer.set_text(self.interface.value)
+            self.buffer.apply_tag(
+                self.tag_placeholder,
+                self.buffer.get_start_iter(),
+                self.buffer.get_end_iter(),
+            )  # make the placeholder text gray.
         else:
             self._placeholder = value
 
-    def on_focus_in(self, *args):
+    def gtk_on_focus_in(self, *args):
         if self.get_value() == self._placeholder:
             self.buffer.set_text("")
         return False
 
-    def on_focus_out(self, *args):
+    def gtk_on_focus_out(self, *args):
         if self.get_value() == "":
             self.buffer.set_text(self.interface.placeholder)
-            self.buffer.apply_tag(self.tag_placholder,
-                                  self.buffer.get_start_iter(),
-                                  self.buffer.get_end_iter())  # make the placeholder text gray.
+            self.buffer.apply_tag(
+                self.tag_placeholder,
+                self.buffer.get_start_iter(),
+                self.buffer.get_end_iter(),
+            )  # make the placeholder text gray.
         return False
 
     def rehint(self):
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
-        self.interface.intrinsic.height = at_least(self.interface.MIN_HEIGHT)
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
+        self.interface.intrinsic.height = at_least(self.interface._MIN_HEIGHT)
+
+    def set_on_change(self, handler):
+        self.interface.factory.not_implemented("MultilineTextInput.set_on_change()")
+
+    def scroll_to_bottom(self):
+        self.buffer.place_cursor(self.buffer.get_end_iter())
+        self.textview.scroll_to_mark(self.buffer.get_insert(), 0.0, True, 0.0, 0.0)
+
+    def scroll_to_top(self):
+        self.buffer.place_cursor(self.buffer.get_start_iter())
+        self.textview.scroll_to_mark(self.buffer.get_insert(), 0.0, True, 0.0, 0.0)
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/widgets/textinput.py` & `toga-gtk-0.3.1/src/toga_gtk/widgets/button.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-from gi.repository import Gtk
 from travertino.size import at_least
 
+from toga.colors import TRANSPARENT
+
+from ..libs import Gtk
 from .base import Widget
 
 
-class TextInput(Widget):
+class Button(Widget):
     def create(self):
-        self.native = Gtk.Entry()
-        self.native.interface = self.interface
-
-        self.native.connect('show', lambda event: self.rehint())
-
-    def set_readonly(self, value):
-        self.native.set_property('editable', not value)
-
-    def set_placeholder(self, value):
-        self.native.set_placeholder_text(value)
-
-    def set_alignment(self, value):
-        self.interface.factory.not_implemented('TextInput.set_alignment()')
+        self.native = Gtk.Button()
+        self.native.connect("clicked", self.gtk_clicked)
 
-    def set_font(self, value):
-        self.interface.factory.not_implemented('TextInput.set_font()')
+    def get_text(self):
+        return self.native.get_label()
 
-    def get_value(self):
-        return self.native.get_text()
+    def set_text(self, text):
+        self.native.set_label(text)
 
-    def set_value(self, value):
-        self.native.set_text(value)
+    def set_enabled(self, value):
+        self.native.set_sensitive(value)
+
+    def set_background_color(self, color):
+        # Buttons interpret TRANSPARENT backgrounds as a reset
+        if color == TRANSPARENT:
+            color = None
+        super().set_background_color(color)
 
     def rehint(self):
-        # print("REHINT", self, self._impl.get_preferred_width(), self._impl.get_preferred_height(), getattr(self, '_fixed_height', False), getattr(self, '_fixed_width', False))
+        # print("REHINT", self, self.native.get_preferred_width(), self.native.get_preferred_height())
         width = self.native.get_preferred_width()
         height = self.native.get_preferred_height()
 
-        self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
+        self.interface.intrinsic.width = at_least(width[0])
         self.interface.intrinsic.height = height[1]
 
-    def set_on_change(self, handler):
-        # No special handling required
-        pass
+    def gtk_clicked(self, event):
+        self.interface.on_press(None)
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/widgets/switch.py` & `toga-gtk-0.3.1/src/toga_gtk/widgets/label.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,35 @@
-from gi.repository import Gtk
 from travertino.size import at_least
 
+from ..libs import Gtk, gtk_alignment
 from .base import Widget
 
 
-class Switch(Widget):
+class Label(Widget):
     def create(self):
-        self._on_toggle_handler = None
+        self.native = Gtk.Label()
+        self.native.set_line_wrap(False)
 
-        self.native = Gtk.Box()
-        self.native.interface = self.interface
+    def set_alignment(self, value):
+        xalign, justify = gtk_alignment(value)
+        self.native.set_xalign(xalign)  # Aligns the whole text block within the widget.
+        self.native.set_yalign(0.5)
+        self.native.set_justify(
+            justify
+        )  # Aligns multiple lines relative to each other.
 
-        self.label = Gtk.Label(xalign=0)
-        self.label.set_line_wrap(True)
+    def get_text(self):
+        return self.native.get_text()
 
-        self.switch = Gtk.Switch()
-        self.switch.connect("notify::active", self._on_toggle)
-
-        self.native.pack_start(self.label, True, True, 0)
-        self.native.pack_start(self.switch, False, False, 0)
-        self.native.connect('show', lambda event: self.rehint())
-
-    def _on_toggle(self, widget, state):
-        if self._on_toggle_handler:
-            self._on_toggle_handler(widget)
-
-    def set_on_toggle(self, handler):
-        self._on_toggle_handler = handler
-
-    def set_label(self, label):
-        self.label.set_text(label)
-
-    def get_is_on(self):
-        return self.switch.get_active()
-
-    def set_is_on(self, value):
-        self.switch.set_active(value)
+    def set_text(self, value):
+        self.native.set_text(value)
 
     def rehint(self):
-        # print("REHINT", self, self.native.get_preferred_width(), self.native.get_preferred_height())
+        # print("REHINT", self,
+        #     self.native.get_preferred_width(), self.native.get_preferred_height(),
+        #     getattr(self, '_fixed_height', False), getattr(self, '_fixed_width', False)
+        # )
         width = self.native.get_preferred_width()
         height = self.native.get_preferred_height()
 
-        # Set intrinsic width to at least the minimum width
         self.interface.intrinsic.width = at_least(width[0])
-        # Set intrinsic height to the natural height
         self.interface.intrinsic.height = height[1]
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/widgets/scrollcontainer.py` & `toga-gtk-0.3.1/src/toga_gtk/widgets/optioncontainer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,58 @@
-from gi.repository import Gtk
-
-from toga_gtk.window import GtkViewport
-
+from ..container import TogaContainer
+from ..libs import Gtk
 from .base import Widget
 
 
-class ScrollContainer(Widget):
+class OptionContainer(Widget):
     def create(self):
-        self.native = Gtk.ScrolledWindow()
-        self.native.interface = self.interface
-
-    def set_content(self, widget):
-        self.inner_container = widget
+        # We want a single unified widget; the vbox is the representation of that widget.
+        self.native = Gtk.Notebook()
+        self.native.connect("switch-page", self.gtk_on_switch_page)
+
+    def gtk_on_switch_page(self, widget, page, page_num):
+        if self.interface.on_select:
+            self.interface.on_select(
+                self.interface, option=self.interface.content[page_num]
+            )
+
+    def add_content(self, index, text, widget):
+        sub_container = TogaContainer()
+        sub_container.content = widget
 
-        widget.viewport = GtkViewport(self.native)
+        self.native.insert_page(sub_container, Gtk.Label(label=text), index)
 
-        # Add all children to the content widget.
-        for child in widget.interface.children:
-            child._impl.container = widget
+        # Tabs aren't visible by default;
+        # tell the notebook to show all content.
+        self.native.show_all()
 
-        if self.native.get_child():
-            self.native.get_child().destroy()
+    def set_on_select(self, handler):
+        # No special handling required
+        pass
+
+    def remove_content(self, index):
+        if index == self.native.get_current_page():
+            # Don't allow removal of a selected tab
+            raise self.interface.OptionException(
+                "Currently selected option cannot be removed"
+            )
+        self.native.remove_page(index)
+
+    def set_option_enabled(self, index, enabled):
+        self.interface.factory.not_implemented("OptionContainer.set_option_enabled()")
+
+    def is_option_enabled(self, index):
+        self.interface.factory.not_implemented("OptionContainer.is_option_enabled()")
+
+    def set_option_text(self, index, value):
+        tab = self.native.get_nth_page(index)
+        self.native.set_tab_label(tab, Gtk.Label(label=value))
+
+    def get_option_text(self, index):
+        tab = self.native.get_nth_page(index)
+        return self.native.get_tab_label(tab).get_label()
 
-        self.native.add(self.inner_container.native)
-        self.native.show_all()
+    def get_current_tab_index(self):
+        return self.native.get_current_page()
 
-    def set_app(self, app):
-        if self.interface.content:
-            self.interface.content.app = app
-
-    def set_window(self, window):
-        if self.interface.content:
-            self.interface.content.window = window
-
-    def set_vertical(self, value):
-        self.native.set_policy(
-            Gtk.PolicyType.AUTOMATIC if getattr(self, 'horizontal', True) else Gtk.PolicyType.NEVER,
-            Gtk.PolicyType.AUTOMATIC if getattr(self, 'vertical', True) else Gtk.PolicyType.NEVER,
-        )
-
-    def set_horizontal(self, value):
-        self.native.set_policy(
-            Gtk.PolicyType.AUTOMATIC if getattr(self, 'horizontal', True) else Gtk.PolicyType.NEVER,
-            Gtk.PolicyType.AUTOMATIC if getattr(self, 'vertical', True) else Gtk.PolicyType.NEVER,
-        )
+    def set_current_tab_index(self, current_tab_index):
+        self.native.set_current_page(current_tab_index)
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/widgets/button.py` & `toga-gtk-0.3.1/src/toga_gtk/widgets/selection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-from gi.repository import Gtk
 from travertino.size import at_least
 
+from ..libs import Gtk
 from .base import Widget
 
 
-class Button(Widget):
+class Selection(Widget):
     def create(self):
-        self.native = Gtk.Button()
-        self.native.interface = self.interface
+        self.native = Gtk.ComboBoxText.new()
+        self.native.connect("changed", self.gtk_on_select)
 
-        self.native.connect('show', lambda event: self.rehint())
-        self.native.connect('clicked', self.on_press)
+    def gtk_on_select(self, widget):
+        if self.interface.on_select:
+            self.interface.on_select(widget)
 
-    def set_label(self, label):
-        self.native.set_label(self.interface.label)
-        self.rehint()
+    def remove_all_items(self):
+        self.native.remove_all()
 
-    def set_enabled(self, value):
-        # self._impl.set_sensitive(value)
-        self.interface.factory.not_implemented('Button.set_enabled()')
+    def add_item(self, item):
+        self.native.append_text(item)
 
-    def set_background_color(self, value):
-        self.interface.factory.not_implemented('Button.set_background_color()')
+        # Gtk.ComboBox does not select the first item, so it's done here.
+        if not self.get_selected_item():
+            self.select_item(item)
 
-    def set_on_press(self, handler):
-        # No special handling required
-        pass
+    def select_item(self, item):
+        self.native.set_active(self.interface.items.index(item))
+
+    def get_selected_item(self):
+        return self.native.get_active_text()
 
     def rehint(self):
-        # print("REHINT", self, self.native.get_preferred_width(), self.native.get_preferred_height())
-        width = self.native.get_preferred_width()
+        # width = self.native.get_preferred_width()
         height = self.native.get_preferred_height()
 
-        self.interface.intrinsic.width = at_least(width[0])
+        self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
         self.interface.intrinsic.height = height[1]
 
-    def on_press(self, event):
-        if self.interface.on_press:
-            self.interface.on_press(self.interface)
+    def set_on_select(self, handler):
+        # No special handling required
+        pass
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/widgets/numberinput.py` & `toga-gtk-0.3.1/src/toga_gtk/widgets/numberinput.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import sys
 from decimal import Decimal
 
 from travertino.size import at_least
 
-from gi.repository import Gtk
-
+from ..libs import Gtk, gtk_alignment
 from .base import Widget
 
 
 class NumberInput(Widget):
     def create(self):
         self.adjustment = Gtk.Adjustment()
 
         self.native = Gtk.SpinButton()
-        self.native.interface = self.interface
         self.native.set_adjustment(self.adjustment)
         self.native.set_numeric(True)
 
-        self.native.connect("value-changed", self._on_change)
-
-        self.rehint()
+        self.native.connect("changed", self.gtk_on_change)
 
-    def _on_change(self, widget):
-        self.interface._value = Decimal(self.native.get_value()).quantize(self.interface.step)
+    def gtk_on_change(self, widget):
+        value = widget.get_text().replace(",", ".") or 0
+        self.interface._value = Decimal(value).quantize(self.interface.step)
         if self.interface.on_change:
             self.interface.on_change(widget)
 
     def set_readonly(self, value):
         self.native.editable = not value
 
     def set_step(self, step):
@@ -51,22 +48,23 @@
     def set_value(self, value):
         if value is None:
             self.native.set_value(Decimal(0.0))
         else:
             self.native.set_value(self.interface.value)
 
     def set_alignment(self, value):
-        self.interface.factory.not_implemented('NumberInput.set_alignment()')
+        xalign, justify = gtk_alignment(value)
+        self.native.set_alignment(xalign)
 
-    def set_font(self, value):
-        self.interface.factory.not_implemented('NumberInput.set_font()')
+    def set_font(self, font):
+        self.interface.factory.not_implemented("NumberInput.set_font()")
 
     def rehint(self):
         width = self.native.get_preferred_width()
         height = self.native.get_preferred_height()
         if width and height:
-            self.interface.intrinsic.width = at_least(self.interface.MIN_WIDTH)
+            self.interface.intrinsic.width = at_least(self.interface._MIN_WIDTH)
             self.interface.intrinsic.height = height[1]
 
     def set_on_change(self, handler):
         # No special handling required.
         pass
```

### Comparing `toga-gtk-0.3.0.dev9/toga_gtk/widgets/table.py` & `toga-gtk-0.3.1/src/toga_gtk/widgets/table.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,71 @@
-from gi.repository import Gtk
-
 from .tree import Tree
 
 
 class Table(Tree):
-
-    def on_select(self, selection):
+    def gtk_on_select(self, selection):
         if self.interface.on_select:
-            tree_model, tree_iter = selection.get_selected()
+            if self.interface.multiple_select:
+                tree_model, tree_path = selection.get_selected_rows()
+                if tree_path:
+                    tree_iter = tree_model.get_iter(tree_path[-1])
+                else:
+                    tree_iter = None
+            else:
+                tree_model, tree_iter = selection.get_selected()
+
+            # Covert the tree iter into the actual row.
             if tree_iter:
                 row = tree_model.get(tree_iter, 0)[0]
             else:
                 row = None
             self.interface.on_select(None, row=row)
 
     def change_source(self, source):
         # Temporarily disconnecting the TreeStore improves performance for large
         # updates by deferring row rendering until the update is complete.
         self.treeview.set_model(None)
 
-        self.store.clear()
+        self.store.change_source(source)
 
         for i, row in enumerate(self.interface.data):
             self.insert(i, row)
 
         self.treeview.set_model(self.store)
 
-    def insert(self, index, item, **kwargs):
-        super().insert(None, index, item, **kwargs)
+    def insert(self, index, item):
+        super().insert(None, index, item)
 
     def scroll_to_row(self, row):
         return NotImplementedError
 
+    def add_column(self, heading, accessor):
+        return NotImplementedError
+
+    def remove_column(self, accessor):
+        return NotImplementedError
+
     # =================================
     # UNCHANGED METHODS (inherited from Tree)
     # They are included here only to satisfy the implementation tests, which
     # do not currently check for inherited methods.
 
     def create(self):
         super().create()
 
     def change(self, item):
         super().change(item)
 
-    def remove(self, item):
-        super().remove(item)
+    def remove(self, index, item):
+        super().remove(item, index=index, parent=None)
 
     def clear(self):
         super().clear()
 
+    def get_selection(self):
+        return super().get_selection()
+
     def set_on_select(self, handler):
         super().set_on_select(handler)
+
+    def set_on_double_click(self, handler):
+        self.interface.factory.not_implemented("Table.set_on_double_click()")
```

### Comparing `toga-gtk-0.3.0.dev9/tests/test_font.py` & `toga-gtk-0.3.1/tests/test_font.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,94 @@
-import toga
-from toga.constants import ITALIC, OBLIQUE, SMALL_CAPS, BOLD, SYSTEM, CURSIVE
-from toga_gtk import font as gtk_font
 import unittest
-import gi
+
+import toga
+from toga.constants import BOLD, CURSIVE, ITALIC, OBLIQUE, SMALL_CAPS, SYSTEM
+from toga_gtk import fonts as gtk_fonts
 
 try:
     import gi
-    gi.require_version('Gtk', '3.0')
-    from gi.repository import Gtk, Gdk
+
+    gi.require_version("Gtk", "3.0")
+    from gi.repository import Gtk
 except ImportError:
     import sys
+
     # If we're on Linux, Gtk *should* be available. If it isn't, make
     # Gtk an object... but in such a way that every test will fail,
     # because the object isn't actually the Gtk interface.
-    if sys.platform == 'linux':
+    if sys.platform == "linux":
         Gtk = object()
     else:
         Gtk = None
 
 try:
     gi.require_version("Pango", "1.0")
     from gi.repository import Pango
 except ImportError:
     Pango = None
 
 
-@unittest.skipIf(Pango is None, 'Pango import error')
-@unittest.skipIf(Gtk is None,
-                 "Can't run GTK implementation tests on a non-Linux platform")
+@unittest.skipIf(Pango is None, "Pango import error")
+@unittest.skipIf(
+    Gtk is None, "Can't run GTK implementation tests on a non-Linux platform"
+)
 class TestFontImplementation(unittest.TestCase):
     def setUp(self):
-        self.interface = None
-        self.native = None
         self.font_family = SYSTEM
         self.font_size = 12
 
-    def tearDown(self):
-        if self.native:  # Avoids 'free'ing invalid pointer
-            self.native.free()
+    def test_font_bind(self):
+        font = toga.Font(self.font_family, self.font_size)
+        font_impl = font.bind()
+
+        self.assertEqual(font._impl, font_impl)
 
     def test_font_default_has_all_attr_set(self):
-        self.interface = toga.Font(self.font_family, self.font_size)
-        self.native = self.interface._impl.native
-        self.assertEqual(self.native.get_family(), SYSTEM)
-        self.assertEqual(self.native.get_size() / Pango.SCALE, self.font_size)
-        self.assertEqual(self.native.get_style(), Pango.Style.NORMAL)
-        self.assertEqual(self.native.get_variant(), Pango.Variant.NORMAL)
-        self.assertEqual(self.native.get_weight(), Pango.Weight.NORMAL)
+        font = toga.Font(self.font_family, self.font_size)
+        native = font._impl.native
+        self.assertEqual(native.get_family(), SYSTEM)
+        self.assertEqual(native.get_size() / Pango.SCALE, self.font_size)
+        self.assertEqual(native.get_style(), Pango.Style.NORMAL)
+        self.assertEqual(native.get_variant(), Pango.Variant.NORMAL)
+        self.assertEqual(native.get_weight(), Pango.Weight.NORMAL)
 
     def test_font_size(self):
         self.font_size = 22
-        self.interface = toga.Font(self.font_family, self.font_size)
-        self.native = self.interface._impl.native
-        self.assertEqual(self.native.get_size() / Pango.SCALE, self.font_size)
+        font = toga.Font(self.font_family, self.font_size)
+        native = font._impl.native
+        self.assertEqual(native.get_size() / Pango.SCALE, self.font_size)
 
     def test_font_style_italic(self):
-        self.interface = toga.Font(
-            self.font_family, self.font_size, style=ITALIC)
-        self.native = self.interface._impl.native
-        self.assertEqual(self.native.get_style(), Pango.Style.ITALIC)
+        font = toga.Font(self.font_family, self.font_size, style=ITALIC)
+        native = font._impl.native
+        self.assertEqual(native.get_style(), Pango.Style.ITALIC)
 
     def test_font_style_oblique(self):
-        self.interface = toga.Font(
-            self.font_family, self.font_size, style=OBLIQUE)
-        self.native = self.interface._impl.native
-        self.assertEqual(self.native.get_style(), Pango.Style.OBLIQUE)
+        font = toga.Font(self.font_family, self.font_size, style=OBLIQUE)
+        native = font._impl.native
+        self.assertEqual(native.get_style(), Pango.Style.OBLIQUE)
 
     def test_font_variant_small_caps(self):
-        self.interface = toga.Font(
-            self.font_family, self.font_size, variant=SMALL_CAPS)
-        self.native = self.interface._impl.native
-        self.assertEqual(self.native.get_variant(), Pango.Variant.SMALL_CAPS)
+        font = toga.Font(self.font_family, self.font_size, variant=SMALL_CAPS)
+        native = font._impl.native
+        self.assertEqual(native.get_variant(), Pango.Variant.SMALL_CAPS)
 
     def test_font_weight_bold(self):
-        self.interface = toga.Font(
-            self.font_family, self.font_size, weight=BOLD)
-        self.native = self.interface._impl.native
-        self.assertEqual(self.native.get_weight(), Pango.Weight.BOLD)
+        font = toga.Font(self.font_family, self.font_size, weight=BOLD)
+        native = font._impl.native
+        self.assertEqual(native.get_weight(), Pango.Weight.BOLD)
 
     def test_font_cache(self):
-        self.interface = toga.Font(self.font_family, self.font_size)
-        self.impl = gtk_font.Font(self.interface)
-        self.cache = gtk_font._FONT_CACHE
-        self.assertEqual(self.cache[self.interface], self.impl.native)
+        font = toga.Font(self.font_family, self.font_size)
+        self.impl = gtk_fonts.Font(font)
+        self.cache = gtk_fonts._FONT_CACHE
+        self.assertEqual(self.cache[font], self.impl.native)
 
     def test_font_family_defaults_to_system(self):
-        self.interface = toga.Font(CURSIVE, self.font_size)
-        self.native = self.interface._impl.native
-        self.assertIn(CURSIVE, self.native.get_family())
-        self.assertIn(SYSTEM, self.native.get_family())
+        font = toga.Font(CURSIVE, self.font_size)
+        native = font._impl.native
+        self.assertIn(CURSIVE, native.get_family())
+        self.assertIn(SYSTEM, native.get_family())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `toga-gtk-0.3.0.dev9/tests/widgets/test_tree.py` & `toga-gtk-0.3.1/tests/widgets/test_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import unittest
+
 try:
     import gi
-    gi.require_version('Gtk', '3.0')
+
+    gi.require_version("Gtk", "3.0")
     from gi.repository import Gtk
 except ImportError:
     import sys
+
     # If we're on Linux, Gtk *should* be available. If it isn't, make
     # Gtk an object... but in such a way that every test will fail,
     # because the object isn't actually the Gtk interface.
-    if sys.platform == 'linux':
+    if sys.platform == "linux":
         Gtk = object()
     else:
         Gtk = None
 
 import toga
 
+from .utils import TreeModelListener
+
 
 def handle_events():
     while Gtk.events_pending():
         Gtk.main_iteration_do(blocking=False)
 
 
-@unittest.skipIf(Gtk is None, "Can't run GTK implementation tests on a non-Linux platform")
+@unittest.skipIf(
+    Gtk is None, "Can't run GTK implementation tests on a non-Linux platform"
+)
 class TestGtkTree(unittest.TestCase):
     def setUp(self):
-        self.tree = toga.Tree(
-            headings=("one", "two")
-        )
+        self.tree = toga.Tree(headings=("one", "two"))
 
         # make a shortcut for easy use
         self.gtk_tree = self.tree._impl
 
         self.window = Gtk.Window()
         self.window.add(self.tree._impl.native)
 
     def assertNodeEqual(self, node, data):
         self.assertEqual(tuple(node)[1:], data)
 
     def test_change_source(self):
-        # Clear the table directly
+        # Clear the tree directly
         self.gtk_tree.clear()
 
         # Assign pre-constructed data
-        self.tree.data = {
-            ("A1", "A2"): [],
-            ("B1", "B2"): [
-                ("B1.1", "B2.1")
-            ]
-        }
+        self.tree.data = {("A1", "A2"): [], ("B1", "B2"): [("B1.1", "B2.1")]}
 
         # Make sure the data was stored correctly
         store = self.gtk_tree.store
         self.assertNodeEqual(store[0], ("A1", "A2"))
         self.assertNodeEqual(store[1], ("B1", "B2"))
         self.assertNodeEqual(store[(1, 0)], ("B1.1", "B2.1"))
 
@@ -65,57 +65,64 @@
         self.tree.data = None
         self.assertEqual(len(store), 0)
 
         self.tree.data = ()
         self.assertEqual(len(store), 0)
 
     def test_insert_root_node(self):
+        listener = TreeModelListener(self.gtk_tree.store)
+
         # Insert a node
         node_data = ("1", "2")
         node = self.tree.data.insert(None, 0, *node_data)
 
         # Make sure it's in there
-        self.assertIsNotNone(node._impl[self.gtk_tree])
+        self.assertIsNotNone(listener.inserted_it)
 
         # Get the Gtk.TreeIter
-        tree_iter = node._impl[self.gtk_tree]
+        tree_iter = listener.inserted_it
 
         # Make sure it's a Gtk.TreeIter
         self.assertTrue(isinstance(tree_iter, Gtk.TreeIter))
 
         # Make sure it's the correct Gtk.TreeIter
         self.assertEqual(node, self.gtk_tree.store.get(tree_iter, 0)[0])
 
         # Get the Gtk.TreePath of the Gtk.TreeIter
         path = self.gtk_tree.store.get_path(tree_iter)
 
         # Make sure it's the correct Gtk.TreePath
         self.assertTrue(isinstance(path, Gtk.TreePath))
         self.assertEqual(path, Gtk.TreePath(0))
+        self.assertEqual(listener.inserted_path, Gtk.TreePath(0))
         # self.assertEqual(str(path), "0")
         # self.assertNodeEqual(path), (0,))
 
         # Make sure the node got stored correctly
         self.assertNodeEqual(self.gtk_tree.store[path], node_data)
 
     def test_insert_child_node(self):
+        listener = TreeModelListener(self.gtk_tree.store)
+
         self.tree.data = []
 
         # Insert blank node as parent
         parent = self.tree.data.insert(None, 0, *(None, None))
 
+        listener.clear()
+
         # Insert a child node
         node_data = ("1", "2")
         node = self.tree.data.insert(parent, 0, *node_data)
 
         # Make sure it's in there
-        self.assertIsNotNone(node._impl[self.gtk_tree])
+        self.assertIsNotNone(listener.inserted_path)
 
         # Get the Gtk.TreeIter
-        tree_iter = node._impl[self.gtk_tree]
+        tree_iter = listener.inserted_it
 
         # Make sure it's a Gtk.TreeIter
         self.assertTrue(isinstance(tree_iter, Gtk.TreeIter))
 
         # Make sure it's the correct Gtk.TreeIter
         self.assertEqual(node, self.gtk_tree.store.get(tree_iter, 0)[0])
 
@@ -123,81 +130,91 @@
         path = self.gtk_tree.store.get_path(tree_iter)
 
         # Make sure it's the correct Gtk.TreePath
         self.assertTrue(isinstance(path, Gtk.TreePath))
         self.assertEqual(str(path), "0:0")
         self.assertEqual(tuple(path), (0, 0))
         self.assertEqual(path, Gtk.TreePath((0, 0)))
+        self.assertEqual(listener.inserted_path, Gtk.TreePath((0, 0)))
 
         # Make sure the node got stored correctly
         self.assertNodeEqual(self.gtk_tree.store[path], node_data)
 
     def test_remove(self):
+        listener = TreeModelListener(self.gtk_tree.store)
+
         # Insert a node
         node = self.tree.data.insert(None, 0, "1", "2")
 
         # Make sure it's in there
-        self.assertIsNotNone(node._impl[self.gtk_tree])
+        self.assertIsNotNone(listener.inserted_it)
 
         # Then remove it
-        self.gtk_tree.remove(node)
+        self.gtk_tree.remove(node, index=0, parent=None)
 
         # Make sure its gone
-        self.assertIsNone(node._impl.get(self.gtk_tree, None))
+        self.assertIsNone(self.gtk_tree.store.do_get_value(listener.inserted_it, 0))
 
     def test_change(self):
+        listener = TreeModelListener(self.gtk_tree.store)
+
         # Insert a node
         node = self.tree.data.insert(None, 0, "1", "2")
 
         # Make sure it's in there
-        self.assertIsNotNone(node._impl[self.gtk_tree])
+        self.assertIsNotNone(listener.inserted_path)
+        self.assertEqual([0], listener.inserted_path.get_indices())
 
         # Change a column
         node.one = "something_changed"
-        # (not testing that self.gtk_tree.change is called. The Core API
-        # unit tests should ensure this already.)
+
+        self.assertIsNotNone(listener.changed_path)
+        self.assertIsNotNone(listener.changed_it)
 
         # Get the Gtk.TreeIter
-        tree_iter = node._impl[self.gtk_tree]
+        tree_iter = listener.changed_it
 
         # Make sure it's a Gtk.TreeIter
         self.assertTrue(isinstance(tree_iter, Gtk.TreeIter))
 
         # Make sure it's the correct Gtk.TreeIter
         self.assertEqual(node, self.gtk_tree.store.get(tree_iter, 0)[0])
 
         # Make sure the value changed
         path = self.gtk_tree.store.get_path(tree_iter)
         self.assertNodeEqual(self.gtk_tree.store[path], (node.one, node.two))
 
     def test_node_persistence_for_replacement(self):
         self.tree.data = []
-        a = self.tree.data.insert(None, 0, one="A1", two="A2")
-        b = self.tree.data.insert(None, 0, one="B1", two="B2")
+        self.tree.data.insert(None, 0, one="A1", two="A2")
+        self.tree.data.insert(None, 0, one="B1", two="B2")
 
         # B should now precede A
         # test passes if A "knows" it has moved to index 1
 
         self.assertNodeEqual(self.gtk_tree.store[0], ("B1", "B2"))
         self.assertNodeEqual(self.gtk_tree.store[1], ("A1", "A2"))
 
     def test_node_persistence_for_deletion(self):
         self.tree.data = []
         a = self.tree.data.append(None, one="A1", two="A2")
-        b = self.tree.data.append(None, one="B1", two="B2")
+        self.tree.data.append(None, one="B1", two="B2")
 
         self.tree.data.remove(a)
 
         # test passes if B "knows" it has moved to index 0
         self.assertNodeEqual(self.gtk_tree.store[0], ("B1", "B2"))
 
     def test_on_select_root_node(self):
+        listener = TreeModelListener(self.gtk_tree.store)
+
         # Insert dummy nodes
         self.tree.data = []
-        a = self.tree.data.append(None, one="A1", two="A2")
+        self.tree.data.append(None, one="A1", two="A2")
+        listener.clear()
         b = self.tree.data.append(None, one="B1", two="B2")
 
         # Create a flag
         succeed = False
 
         def on_select(tree, node):
             # Make sure the right node was selected
@@ -205,25 +222,29 @@
 
             nonlocal succeed
             succeed = True
 
         self.tree.on_select = on_select
 
         # Select node B
-        self.gtk_tree.selection.select_iter(b._impl[self.gtk_tree])
+        self.gtk_tree.selection.select_iter(listener.inserted_it)
 
         # Allow on_select to call
         handle_events()
 
         self.assertTrue(succeed)
 
     def test_on_select_child_node(self):
+        listener = TreeModelListener(self.gtk_tree.store)
+
         # Insert two nodes
         self.tree.data = []
         a = self.tree.data.append(None, one="A1", two="A2")
+        a_iter = listener.inserted_it
+        listener.clear()
         b = self.tree.data.append(a, one="B1", two="B2")
 
         # Create a flag
         succeed = False
 
         def on_select(tree, node):
             # Make sure the right node was selected
@@ -231,28 +252,30 @@
 
             nonlocal succeed
             succeed = True
 
         self.tree.on_select = on_select
 
         # Expand parent node (a) on Gtk.TreeView to allow selection
-        path = self.gtk_tree.store.get_path(a._impl[self.gtk_tree])
+        path = self.gtk_tree.store.get_path(a_iter)
         self.gtk_tree.treeview.expand_row(path, True)
 
         # Select node B
-        self.gtk_tree.selection.select_iter(b._impl[self.gtk_tree])
+        self.gtk_tree.selection.select_iter(listener.inserted_it)
         # Allow on_select to call
         handle_events()
 
         self.assertTrue(succeed)
 
     def test_on_select_deleted_node(self):
+        listener = TreeModelListener(self.gtk_tree.store)
+
         # Insert two nodes
         self.tree.data = []
-        a = self.tree.data.append(None, one="A1", two="A2")
+        self.tree.data.append(None, one="A1", two="A2")
         b = self.tree.data.append(None, one="B1", two="B2")
 
         # Create a flag
         succeed = False
 
         def on_select(tree, node):
             nonlocal succeed
@@ -265,13 +288,13 @@
             else:
                 self.assertEqual(node, None)
                 succeed = True
 
         self.tree.on_select = on_select
 
         # Select node B
-        self.gtk_tree.selection.select_iter(b._impl[self.gtk_tree])
+        self.gtk_tree.selection.select_iter(listener.inserted_it)
 
         # Allow on_select to call
         handle_events()
 
         self.assertTrue(succeed)
```

### Comparing `toga-gtk-0.3.0.dev9/tests/widgets/test_table.py` & `toga-gtk-0.3.1/tests/widgets/test_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import unittest
+
 try:
     import gi
-    gi.require_version('Gtk', '3.0')
+
+    gi.require_version("Gtk", "3.0")
     from gi.repository import Gtk
 except ImportError:
     import sys
+
     # If we're on Linux, Gtk *should* be available. If it isn't, make
     # Gtk an object... but in such a way that every test will fail,
     # because the object isn't actually the Gtk interface.
-    if sys.platform == 'linux':
+    if sys.platform == "linux":
         Gtk = object()
     else:
         Gtk = None
 
 import toga
 
+from .utils import TreeModelListener
+
 
 def handle_events():
     while Gtk.events_pending():
         Gtk.main_iteration_do(blocking=False)
 
 
-@unittest.skipIf(Gtk is None, "Can't run GTK implementation tests on a non-Linux platform")
+@unittest.skipIf(
+    Gtk is None, "Can't run GTK implementation tests on a non-Linux platform"
+)
 class TestGtkTable(unittest.TestCase):
     def setUp(self):
-        self.table = toga.Table(
-            headings=("one", "two")
-        )
+        self.table = toga.Table(headings=("one", "two"))
 
         # make a shortcut for easy use
         self.gtk_table = self.table._impl
 
         self.window = Gtk.Window()
         self.window.add(self.table._impl.native)
 
@@ -38,18 +43,15 @@
         self.assertEqual(tuple(row)[1:], data)
 
     def test_change_source(self):
         # Clear the table directly
         self.gtk_table.clear()
 
         # Assign pre-constructed data
-        self.table.data = [
-            ("A1", "A2"),
-            ("B1", "B2")
-        ]
+        self.table.data = [("A1", "A2"), ("B1", "B2")]
 
         # Make sure the data was stored correctly
         store = self.gtk_table.store
         self.assertRowEqual(store[0], ("A1", "A2"))
         self.assertRowEqual(store[1], ("B1", "B2"))
 
         # Clear the table with empty assignment
@@ -62,24 +64,26 @@
         self.table.data = None
         self.assertEqual(len(store), 0)
 
         self.table.data = ()
         self.assertEqual(len(store), 0)
 
     def test_insert(self):
+        listener = TreeModelListener(self.gtk_table.store)
+
         # Insert a row
         row_data = ("1", "2")
         INSERTED_AT = 0
         row = self.table.data.insert(INSERTED_AT, *row_data)
 
         # Make sure it's in there
-        self.assertIsNotNone(row._impl[self.gtk_table])
+        self.assertIsNotNone(listener.inserted_it)
 
         # Get the Gtk.TreeIter
-        tree_iter = row._impl[self.gtk_table]
+        tree_iter = listener.inserted_it
 
         # Make sure it's a Gtk.TreeIter
         self.assertTrue(isinstance(tree_iter, Gtk.TreeIter))
 
         # Make sure it's the correct Gtk.TreeIter
         self.assertEqual(row, self.gtk_table.store.get(tree_iter, 0)[0])
 
@@ -87,72 +91,76 @@
         path = self.gtk_table.store.get_path(tree_iter)
 
         # Make sure it's the correct Gtk.TreePath
         self.assertTrue(isinstance(path, Gtk.TreePath))
         self.assertEqual(str(path), str(INSERTED_AT))
         self.assertEqual(tuple(path), (INSERTED_AT,))
         self.assertEqual(path, Gtk.TreePath(INSERTED_AT))
+        self.assertEqual(path, listener.inserted_path)
 
         # Make sure the row got stored correctly
         result_row = self.gtk_table.store[path]
         self.assertRowEqual(result_row, row_data)
 
     def test_remove(self):
+        listener = TreeModelListener(self.gtk_table.store)
         # Insert a row
         row = self.table.data.insert(0, "1", "2")
 
         # Make sure it's in there
-        self.assertIsNotNone(row._impl[self.gtk_table])
+        self.assertIsNotNone(listener.inserted_it)
 
         # Then remove it
-        self.gtk_table.remove(row)
+        self.gtk_table.remove(index=0, item=row)
 
         # Make sure its gone
-        self.assertIsNone(row._impl.get(self.gtk_table, None))
+        self.assertIsNotNone(listener.deleted_path)
 
     def test_change(self):
+        listener = TreeModelListener(self.gtk_table.store)
+
         # Insert a row
         row = self.table.data.insert(0, "1", "2")
 
         # Make sure it's in there
-        self.assertIsNotNone(row._impl[self.gtk_table])
+        self.assertIsNotNone(listener.inserted_it)
 
         # Change a column
         row.one = "something_changed"
         # (not testing that self.gtk_table.change is called. The Core API
         # unit tests should ensure this already.)
 
         # Get the Gtk.TreeIter
-        tree_iter = row._impl[self.gtk_table]
+        tree_iter = listener.changed_it
 
         # Make sure it's a Gtk.TreeIter
         self.assertTrue(isinstance(tree_iter, Gtk.TreeIter))
 
         # Make sure it's the correct Gtk.TreeIter
         self.assertEqual(row, self.gtk_table.store.get(tree_iter, 0)[0])
 
         # Make sure the value changed
         path = self.gtk_table.store.get_path(tree_iter)
         result_row = self.gtk_table.store[path]
         self.assertRowEqual(result_row, (row.one, row.two))
 
     def test_row_persistence(self):
-        a = self.table.data.insert(0, one="A1", two="A2")
-        b = self.table.data.insert(0, one="B1", two="B2")
+        self.table.data.insert(0, one="A1", two="A2")
+        self.table.data.insert(0, one="B1", two="B2")
 
         # B should now precede A
         # tests passes if A "knows" it has moved to index 1
 
         self.assertRowEqual(self.gtk_table.store[0], ("B1", "B2"))
         self.assertRowEqual(self.gtk_table.store[1], ("A1", "A2"))
 
     def test_on_select_root_row(self):
         # Insert two dummy rows
         self.table.data = []
-        a = self.table.data.append(None, one="A1", two="A2")
+        self.table.data.append(None, one="A1", two="A2")
         b = self.table.data.append(None, one="B1", two="B2")
 
         # Create a flag
         succeed = False
 
         def on_select(table, row, *kw):
             # Make sure the right row was selected
@@ -170,14 +178,17 @@
         handle_events()
 
         self.assertTrue(succeed)
 
     def test_on_select_child_row(self):
         # Insert two nodes
         self.table.data = []
+
+        listener = TreeModelListener(self.gtk_table.store)
+
         a = self.table.data.append(None, one="A1", two="A2")
         b = self.table.data.append(a, one="B1", two="B2")
 
         # Create a flag
         succeed = False
 
         def on_select(able, row, *kw):
@@ -186,25 +197,29 @@
 
             nonlocal succeed
             succeed = True
 
         self.table.on_select = on_select
 
         # Select node B
-        self.gtk_table.selection.select_iter(b._impl[self.gtk_table])
+        self.gtk_table.selection.select_iter(listener.inserted_it)
 
         # Allow on_select to call
         handle_events()
 
         self.assertTrue(succeed)
 
     def test_on_select_deleted_node(self):
         # Insert two nodes
         self.table.data = []
-        a = self.table.data.append(None, one="A1", two="A2")
+
+        listener = TreeModelListener(self.gtk_table.store)
+
+        self.table.data.append(None, one="A1", two="A2")
+        listener.clear()
         b = self.table.data.append(None, one="B1", two="B2")
 
         # Create a flag
         succeed = False
 
         def on_select(table, row):
             nonlocal succeed
@@ -217,13 +232,13 @@
             else:
                 self.assertEqual(row, None)
                 succeed = True
 
         self.table.on_select = on_select
 
         # Select row B
-        self.gtk_table.selection.select_iter(b._impl[self.gtk_table])
+        self.gtk_table.selection.select_iter(listener.inserted_it)
 
         # Allow on_select to call
         handle_events()
 
         self.assertTrue(succeed)
```

### Comparing `toga-gtk-0.3.0.dev9/tests/widgets/test_imageview.py` & `toga-gtk-0.3.1/tests/widgets/test_imageview.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import unittest
 
 try:
     import gi
-    gi.require_version('Gtk', '3.0')
+
+    gi.require_version("Gtk", "3.0")
     from gi.repository import Gtk
 except ImportError:
     import sys
+
     # If we're on Linux, Gtk *should* be available. If it isn't, make
     # Gtk an object... but in such a way that every test will fail,
     # because the object isn't actually the Gtk interface.
-    if sys.platform == 'linux':
+    if sys.platform == "linux":
         Gtk = object()
     else:
         Gtk = None
 
 from toga_gtk.widgets.imageview import ImageView
 
 
-@unittest.skipIf(Gtk is None, "Can't run GTK implementation tests on a non-Linux platform")
+@unittest.skipIf(
+    Gtk is None, "Can't run GTK implementation tests on a non-Linux platform"
+)
 class TestGtkImageView(unittest.TestCase):
-
     def test_resize_max(self):
-
         # Scale up height bound
         self.assertEqual((500, 500), ImageView._resize_max(250, 250, 500, 1000))
 
         # Scale up width bound
         self.assertEqual((500, 500), ImageView._resize_max(250, 250, 1000, 500))
 
         # Scale down height bound
```

### Comparing `toga-gtk-0.3.0.dev9/README.rst` & `toga-gtk-0.3.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 toga-gtk
 ========
 
-A GTK+ backend for the `Toga widget toolkit`_.
+A GTK backend for the `Toga widget toolkit`_.
 
 **Toga requires Python 3**
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
 
 For more details, see the `Toga project on Github`_.
 
+.. _Toga widget toolkit: http://beeware.org/toga
+.. _the core Toga library: https://pypi.python.org/pypi/toga-core
+.. _Toga project on Github: https://github.com/beeware/toga
+
 Prerequisites
 ~~~~~~~~~~~~~
 
-This backend requires GTK+ 3.10 or later. This is the version that ships
+This backend requires GTK 3.10 or later. This is the version that ships
 starting with Ubuntu 14.04 and Fedora 20. You also need to install the Python
-3 bindings to GTK+. If you want to use the WebView widget, you'll also need to
+3 bindings to GTK. If you want to use the WebView widget, you'll also need to
 have WebKit, plus the GI bindings to WebKit installed. This means you'll need
 to install the following:
 
 * **Ubuntu 14.04** ``apt-get install python3-gi gir1.2-webkit-3.0``
 
 * **Ubuntu 16.04 / Debian 8** ``apt-get install python3-gi gir1.2-webkit2-4.0``
   or ``apt-get install python3-gi gir1.2-webkit-3.0``
-  
+
 * **Fedora** ``dnf install python3-gobject pywebkitgtk``
-  or ``yum install python3-gobject pywebkitgtk`` 
-  
-* **Arch Linux** ``pacman -S python-gobject webkit2gtk`` 
+  or ``yum install python3-gobject pywebkitgtk``
+
+* **Arch Linux** ``pacman -S python-gobject webkit2gtk``
 
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

