# Comparing `tmp/Termighty-0.0.9.tar.gz` & `tmp/Termighty-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Termighty-0.0.9.tar", last modified: Fri Jul 26 17:49:17 2019, max compression
+gzip compressed data, was "Termighty-3.0.1.tar", last modified: Wed Apr 12 17:47:10 2023, max compression
```

## Comparing `Termighty-0.0.9.tar` & `Termighty-3.0.1.tar`

### file list

```diff
@@ -1,18 +1,40 @@
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2019-07-26 17:49:17.000000 Termighty-0.0.9/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      832 2019-07-26 17:49:17.000000 Termighty-0.0.9/PKG-INFO
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       40 2019-07-24 15:22:53.000000 Termighty-0.0.9/setup.cfg
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1228 2019-07-26 17:49:14.000000 Termighty-0.0.9/setup.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2019-07-26 17:49:17.000000 Termighty-0.0.9/Termighty/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)       40 2019-07-26 17:48:41.000000 Termighty-0.0.9/Termighty/__init__.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2019-07-26 17:49:17.000000 Termighty-0.0.9/Termighty/utils/
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)    26047 2019-07-26 17:37:25.000000 Termighty-0.0.9/Termighty/utils/charrays.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)    10770 2019-07-26 17:37:18.000000 Termighty-0.0.9/Termighty/utils/utils.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     1476 2019-07-26 17:41:11.000000 Termighty-0.0.9/Termighty/utils/config.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     8654 2019-07-26 17:33:26.000000 Termighty-0.0.9/Termighty/utils/exceptions.py
--rw-rw-r--   0 gabriel   (1000) gabriel   (1000)       95 2019-07-26 17:48:35.000000 Termighty-0.0.9/Termighty/utils/__init__.py
-drwxr-xr-x   0 gabriel   (1000) gabriel   (1000)        0 2019-07-26 17:49:17.000000 Termighty-0.0.9/Termighty/obj/
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     2668 2019-07-26 17:48:18.000000 Termighty-0.0.9/Termighty/obj/Terminal.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)    10723 2019-07-26 17:46:46.000000 Termighty-0.0.9/Termighty/obj/Charray.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)      110 2019-07-26 17:36:55.000000 Termighty-0.0.9/Termighty/obj/__init__.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)    12347 2019-07-26 17:46:47.000000 Termighty-0.0.9/Termighty/obj/String.py
--rw-r--r--   0 gabriel   (1000) gabriel   (1000)     6668 2019-07-26 17:19:48.000000 Termighty-0.0.9/Termighty/obj/Char.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.499442 Termighty-3.0.1/
+-rw-rw-rw-   0        0        0    35823 2022-09-11 20:43:48.000000 Termighty-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      596 2023-04-12 17:47:10.499442 Termighty-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2022-09-11 20:43:48.000000 Termighty-3.0.1/README.md
+-rw-rw-rw-   0        0        0      105 2022-09-18 20:12:03.000000 Termighty-3.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-12 17:47:10.500947 Termighty-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2022-09-18 20:11:40.000000 Termighty-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.322399 Termighty-3.0.1/source/
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.356899 Termighty-3.0.1/source/Termighty.egg-info/
+-rw-rw-rw-   0        0        0      596 2023-04-12 17:47:10.000000 Termighty-3.0.1/source/Termighty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-04-12 17:47:10.000000 Termighty-3.0.1/source/Termighty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:47:10.000000 Termighty-3.0.1/source/Termighty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 17:47:10.000000 Termighty-3.0.1/source/Termighty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-12 17:47:10.000000 Termighty-3.0.1/source/Termighty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.360900 Termighty-3.0.1/source/termighty/
+-rw-rw-rw-   0        0        0      115 2022-09-11 20:43:48.000000 Termighty-3.0.1/source/termighty/__init__.py
+-rw-rw-rw-   0        0        0      403 2022-09-17 22:33:08.000000 Termighty-3.0.1/source/termighty/config.ini
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.368399 Termighty-3.0.1/source/termighty/data/
+-rw-rw-rw-   0        0        0     7971 2022-09-17 14:02:53.000000 Termighty-3.0.1/source/termighty/data/keymaps.json
+-rw-rw-rw-   0        0        0    66090 2022-09-11 20:43:48.000000 Termighty-3.0.1/source/termighty/data/rgb.json
+-rw-rw-rw-   0        0        0      216 2022-09-11 20:43:48.000000 Termighty-3.0.1/source/termighty/data/styles.json
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.397899 Termighty-3.0.1/source/termighty/obj/
+-rw-rw-rw-   0        0        0       54 2022-09-11 20:43:48.000000 Termighty-3.0.1/source/termighty/obj/__init__.py
+-rw-rw-rw-   0        0        0    15095 2022-09-18 18:49:31.000000 Termighty-3.0.1/source/termighty/obj/color.py
+-rw-rw-rw-   0        0        0    17757 2022-09-18 14:21:27.000000 Termighty-3.0.1/source/termighty/obj/string.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.438488 Termighty-3.0.1/source/termighty/settings/
+-rw-rw-rw-   0        0        0       80 2022-09-11 20:43:48.000000 Termighty-3.0.1/source/termighty/settings/__init__.py
+-rw-rw-rw-   0        0        0     1737 2022-09-17 22:33:43.000000 Termighty-3.0.1/source/termighty/settings/config.py
+-rw-rw-rw-   0        0        0     1010 2022-09-18 14:22:15.000000 Termighty-3.0.1/source/termighty/settings/data.py
+-rw-rw-rw-   0        0        0     1469 2022-09-11 20:43:48.000000 Termighty-3.0.1/source/termighty/settings/system.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.486026 Termighty-3.0.1/source/termighty/utils/
+-rw-rw-rw-   0        0        0       97 2022-09-18 19:41:57.000000 Termighty-3.0.1/source/termighty/utils/__init__.py
+-rw-rw-rw-   0        0        0    44886 2022-09-18 18:29:32.000000 Termighty-3.0.1/source/termighty/utils/key_processor.py
+-rw-rw-rw-   0        0        0    10167 2022-09-18 18:29:32.000000 Termighty-3.0.1/source/termighty/utils/listener.py
+-rw-rw-rw-   0        0        0     6754 2022-09-17 20:42:16.000000 Termighty-3.0.1/source/termighty/utils/term.py
+-rw-rw-rw-   0        0        0     5787 2022-09-17 13:34:43.000000 Termighty-3.0.1/source/termighty/utils/term_old.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:47:10.496435 Termighty-3.0.1/source/termighty/widgets/
+-rw-rw-rw-   0        0        0       68 2022-09-12 19:41:55.000000 Termighty-3.0.1/source/termighty/widgets/__init__.py
+-rw-rw-rw-   0        0        0    16825 2022-09-18 19:12:33.000000 Termighty-3.0.1/source/termighty/widgets/text_box.py
+-rw-rw-rw-   0        0        0    16064 2022-09-18 19:42:23.000000 Termighty-3.0.1/source/termighty/widgets/text_editor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

