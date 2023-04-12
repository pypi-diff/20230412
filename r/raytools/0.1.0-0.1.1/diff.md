# Comparing `tmp/raytools-0.1.0.tar.gz` & `tmp/raytools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raytools-0.1.0.tar", last modified: Fri Jan  6 10:24:35 2023, max compression
+gzip compressed data, was "raytools-0.1.1.tar", last modified: Wed Apr 12 12:51:41 2023, max compression
```

## Comparing `raytools-0.1.0.tar` & `raytools-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,84 @@
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.970972 raytools-0.1.0/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      153 2023-01-06 09:33:55.000000 raytools-0.1.0/HISTORY.rst
--rw-------   0 stephenwasilewski   (501) staff       (20)    14847 2020-05-19 06:53:47.000000 raytools-0.1.0/LICENSE
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      592 2023-01-04 10:03:51.000000 raytools-0.1.0/MANIFEST.in
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     2369 2023-01-04 10:35:31.000000 raytools-0.1.0/Makefile
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     3069 2023-01-06 10:24:35.971110 raytools-0.1.0/PKG-INFO
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     2159 2023-01-06 10:24:33.000000 raytools-0.1.0/README.rst
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.942207 raytools-0.1.0/docs/
--rw-------   0 stephenwasilewski   (501) staff       (20)      609 2022-12-30 12:36:11.000000 raytools-0.1.0/docs/Makefile
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.942710 raytools-0.1.0/docs/_static/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     3400 2022-06-21 11:20:16.000000 raytools-0.1.0/docs/_static/custom.css
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.943264 raytools-0.1.0/docs/_templates/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      292 2019-03-05 16:30:33.000000 raytools-0.1.0/docs/_templates/navigation.html
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       63 2022-12-30 12:16:16.000000 raytools-0.1.0/docs/cli.rst
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     5023 2023-01-06 10:24:33.000000 raytools-0.1.0/docs/conf.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      890 2022-12-30 12:17:46.000000 raytools-0.1.0/docs/evaluate.rst
--rw-------   0 stephenwasilewski   (501) staff       (20)       12 2020-05-19 06:53:47.000000 raytools-0.1.0/docs/genindex.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       28 2020-09-24 09:08:55.000000 raytools-0.1.0/docs/history.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      174 2022-12-30 12:19:13.000000 raytools-0.1.0/docs/imagetools.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      366 2022-12-30 12:28:06.000000 raytools-0.1.0/docs/index.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      157 2022-12-30 12:17:46.000000 raytools-0.1.0/docs/io.rst
--rw-------   0 stephenwasilewski   (501) staff       (20)      770 2022-12-30 12:36:11.000000 raytools-0.1.0/docs/make.bat
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      513 2022-12-30 12:17:46.000000 raytools-0.1.0/docs/mapper.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       37 2022-04-19 13:23:25.000000 raytools-0.1.0/docs/requirements.txt
--rw-------   0 stephenwasilewski   (501) staff       (20)       14 2020-05-19 06:53:47.000000 raytools-0.1.0/docs/search.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      171 2022-12-30 12:17:46.000000 raytools-0.1.0/docs/translate.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      168 2022-12-30 12:17:46.000000 raytools-0.1.0/docs/utility.rst
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.943924 raytools-0.1.0/radiance_depend/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    10244 2023-01-04 09:53:32.000000 raytools-0.1.0/radiance_depend/.DS_Store
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.948200 raytools-0.1.0/radiance_depend/linux/
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)    27864 2022-12-04 19:31:36.000000 raytools-0.1.0/radiance_depend/linux/getinfo
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)   104296 2022-12-04 19:31:31.000000 raytools-0.1.0/radiance_depend/linux/pvalue
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)    88536 2022-12-04 19:31:14.000000 raytools-0.1.0/radiance_depend/linux/rcalc
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)    73872 2022-12-04 19:31:37.000000 raytools-0.1.0/radiance_depend/linux/vwrays
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.953566 raytools-0.1.0/radiance_depend/macos/
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)    52960 2022-12-04 18:34:20.000000 raytools-0.1.0/radiance_depend/macos/getinfo
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)   109016 2022-12-04 18:34:14.000000 raytools-0.1.0/radiance_depend/macos/pvalue
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)    91352 2022-12-04 18:34:14.000000 raytools-0.1.0/radiance_depend/macos/rcalc
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)    90744 2022-12-04 18:34:16.000000 raytools-0.1.0/radiance_depend/macos/vwrays
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.956722 raytools-0.1.0/raytools/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     1157 2023-01-06 10:24:33.000000 raytools-0.1.0/raytools/__init__.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.959261 raytools-0.1.0/raytools/cal/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     5589 2022-12-04 18:29:22.000000 raytools-0.1.0/raytools/cal/rayinit.cal
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     6752 2023-01-06 10:17:52.000000 raytools-0.1.0/raytools/cli.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.961124 raytools-0.1.0/raytools/evaluate/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      782 2022-12-29 14:29:15.000000 raytools-0.1.0/raytools/evaluate/__init__.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    10957 2022-12-30 12:36:11.000000 raytools-0.1.0/raytools/evaluate/basemetricset.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    26790 2023-01-04 13:11:24.000000 raytools-0.1.0/raytools/evaluate/hvsgsm.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     7287 2022-12-30 12:36:11.000000 raytools-0.1.0/raytools/evaluate/metricset.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     3557 2022-12-30 12:37:56.000000 raytools-0.1.0/raytools/evaluate/positionindex.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    14827 2022-03-15 14:44:11.000000 raytools-0.1.0/raytools/evaluate/retina.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     8182 2023-01-04 13:24:19.000000 raytools-0.1.0/raytools/imagetools.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     6867 2023-01-05 13:38:48.000000 raytools-0.1.0/raytools/io.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.962270 raytools-0.1.0/raytools/mapper/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      579 2022-12-30 09:03:45.000000 raytools-0.1.0/raytools/mapper/__init__.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     8857 2023-01-06 06:47:52.000000 raytools-0.1.0/raytools/mapper/angularmixin.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     8682 2023-01-05 13:50:47.000000 raytools-0.1.0/raytools/mapper/mapper.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     3095 2022-12-30 09:03:45.000000 raytools-0.1.0/raytools/mapper/viewmapper.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    15902 2022-12-30 14:00:33.000000 raytools-0.1.0/raytools/translate.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     4399 2023-01-03 14:45:30.000000 raytools-0.1.0/raytools/utility.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.958961 raytools-0.1.0/raytools.egg-info/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     3069 2023-01-06 10:24:35.000000 raytools-0.1.0/raytools.egg-info/PKG-INFO
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     1602 2023-01-06 10:24:35.000000 raytools-0.1.0/raytools.egg-info/SOURCES.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)        1 2023-01-06 10:24:35.000000 raytools-0.1.0/raytools.egg-info/dependency_links.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       47 2023-01-06 10:24:35.000000 raytools-0.1.0/raytools.egg-info/entry_points.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)        1 2022-12-30 09:16:51.000000 raytools-0.1.0/raytools.egg-info/not-zip-safe
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       23 2023-01-06 10:24:35.000000 raytools-0.1.0/raytools.egg-info/requires.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)        9 2023-01-06 10:24:35.000000 raytools-0.1.0/raytools.egg-info/top_level.txt
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     1995 2023-01-06 10:23:42.000000 raytools-0.1.0/release.sh
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       23 2022-12-30 09:16:08.000000 raytools-0.1.0/requirements.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      129 2022-12-30 08:33:51.000000 raytools-0.1.0/requirements_dev.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      579 2023-01-06 10:24:35.971695 raytools-0.1.0/setup.cfg
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     2473 2023-01-06 10:24:33.000000 raytools-0.1.0/setup.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.967235 raytools-0.1.0/tests/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     8196 2022-12-30 12:07:11.000000 raytools-0.1.0/tests/.DS_Store
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     1190 2023-01-03 15:02:06.000000 raytools-0.1.0/tests/test_hvsgsm.py
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     1948 2023-01-04 07:57:50.000000 raytools-0.1.0/tests/test_imagetools.py
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     2799 2023-01-04 12:37:33.000000 raytools-0.1.0/tests/test_io.py
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     6310 2023-01-03 09:30:03.000000 raytools-0.1.0/tests/test_metric.py
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     1771 2023-01-03 15:53:10.000000 raytools-0.1.0/tests/test_retina.py
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     6320 2023-01-05 14:01:20.000000 raytools-0.1.0/tests/test_translate.py
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     1007 2023-01-03 14:59:58.000000 raytools-0.1.0/tests/test_utility.py
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     3816 2023-01-05 13:41:58.000000 raytools-0.1.0/tests/test_viewmapper.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2023-01-06 10:24:35.970743 raytools-0.1.0/tests/testdir/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)  2017560 2021-02-10 13:04:00.000000 raytools-0.1.0/tests/testdir/oct21_detail_glz_EW_desk.hdr
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       86 2022-04-19 12:46:46.000000 raytools-0.1.0/tests/testdir/v1.vf
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.247889 raytools-0.1.1/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      153 2023-02-28 13:36:55.000000 raytools-0.1.1/HISTORY.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    14847 2023-02-28 13:36:55.000000 raytools-0.1.1/LICENSE
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      592 2023-02-28 13:36:55.000000 raytools-0.1.1/MANIFEST.in
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     2369 2023-02-28 13:36:55.000000 raytools-0.1.1/Makefile
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     3049 2023-04-12 12:51:41.247940 raytools-0.1.1/PKG-INFO
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     2159 2023-04-12 12:51:40.000000 raytools-0.1.1/README.rst
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.241367 raytools-0.1.1/docs/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      609 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/Makefile
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.241483 raytools-0.1.1/docs/_static/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     3400 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/_static/custom.css
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.241605 raytools-0.1.1/docs/_templates/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      292 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/_templates/navigation.html
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       63 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/cli.rst
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     5023 2023-04-12 12:51:40.000000 raytools-0.1.1/docs/conf.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      890 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/evaluate.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       12 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/genindex.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       28 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/history.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      174 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/imagetools.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      366 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/index.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      157 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/io.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      770 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/make.bat
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      513 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/mapper.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       37 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/requirements.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       14 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/search.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      171 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/translate.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      168 2023-02-28 13:36:55.000000 raytools-0.1.1/docs/utility.rst
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.237871 raytools-0.1.1/radiance_depend/
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.242180 raytools-0.1.1/radiance_depend/linux/
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)    27864 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/linux/getinfo
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)   104296 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/linux/pvalue
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)    88536 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/linux/rcalc
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)    73872 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/linux/vwrays
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.242786 raytools-0.1.1/radiance_depend/macos/
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)    52960 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/macos/getinfo
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)   109016 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/macos/pvalue
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)    91352 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/macos/rcalc
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)    90744 2023-02-28 13:36:55.000000 raytools-0.1.1/radiance_depend/macos/vwrays
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.243505 raytools-0.1.1/raytools/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     1157 2023-04-12 12:51:40.000000 raytools-0.1.1/raytools/__init__.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.244607 raytools-0.1.1/raytools/cal/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     5589 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/cal/rayinit.cal
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     6752 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/cli.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.245304 raytools-0.1.1/raytools/evaluate/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      782 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/evaluate/__init__.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    10957 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/evaluate/basemetricset.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    26790 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/evaluate/hvsgsm.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     7287 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/evaluate/metricset.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     3557 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/evaluate/positionindex.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    14827 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/evaluate/retina.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     8662 2023-04-11 08:07:32.000000 raytools-0.1.1/raytools/imagetools.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     6867 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/io.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.245740 raytools-0.1.1/raytools/mapper/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      579 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/mapper/__init__.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    10070 2023-03-22 11:49:39.000000 raytools-0.1.1/raytools/mapper/angularmixin.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     8682 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/mapper/mapper.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     3095 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/mapper/viewmapper.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    21406 2023-04-10 13:32:26.000000 raytools-0.1.1/raytools/translate.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     4399 2023-02-28 13:36:55.000000 raytools-0.1.1/raytools/utility.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.244491 raytools-0.1.1/raytools.egg-info/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     3049 2023-04-12 12:51:41.000000 raytools-0.1.1/raytools.egg-info/PKG-INFO
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     1560 2023-04-12 12:51:41.000000 raytools-0.1.1/raytools.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)        1 2023-04-12 12:51:41.000000 raytools-0.1.1/raytools.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       47 2023-04-12 12:51:41.000000 raytools-0.1.1/raytools.egg-info/entry_points.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)        1 2023-02-28 13:37:41.000000 raytools-0.1.1/raytools.egg-info/not-zip-safe
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       23 2023-04-12 12:51:41.000000 raytools-0.1.1/raytools.egg-info/requires.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)        9 2023-04-12 12:51:41.000000 raytools-0.1.1/raytools.egg-info/top_level.txt
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     1995 2023-02-28 13:36:55.000000 raytools-0.1.1/release.sh
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       23 2023-02-28 13:36:55.000000 raytools-0.1.1/requirements.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      129 2023-02-28 13:36:55.000000 raytools-0.1.1/requirements_dev.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      579 2023-04-12 12:51:41.248169 raytools-0.1.1/setup.cfg
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     2438 2023-04-12 12:51:40.000000 raytools-0.1.1/setup.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.246626 raytools-0.1.1/tests/
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     1190 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_hvsgsm.py
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     1948 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_imagetools.py
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     2799 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_io.py
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     6310 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_metric.py
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     1771 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_retina.py
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     6320 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_translate.py
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     1007 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_utility.py
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     3816 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/test_viewmapper.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-04-12 12:51:41.247784 raytools-0.1.1/tests/testdir/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)  2017560 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/testdir/oct21_detail_glz_EW_desk.hdr
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       86 2023-02-28 13:36:55.000000 raytools-0.1.1/tests/testdir/v1.vf
```

### Comparing `raytools-0.1.0/LICENSE` & `raytools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/MANIFEST.in` & `raytools-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/Makefile` & `raytools-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/PKG-INFO` & `raytools-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: raytools
-Version: 0.1.0
+Version: 0.1.1
 Summary: working with hdr images, numpy and coordinate transformations for lighting simulation
 Home-page: https://github.com/stephanwaz/raytools
 Author: Stephen Wasilewski
 Author-email: stephanwaz@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: raytools
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 License-File: LICENSE
 
 ====================
-raytools (0.1.0)
+raytools (0.1.1)
 ====================
 
 .. image:: https://img.shields.io/pypi/v/raytools?style=flat-square
     :target: https://pypi.org/project/raytools
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/l/raytools?style=flat-square
@@ -80,9 +79,7 @@
 =======
 
 0.1.0 (2023-01-06)
 ------------------
 
 * First release on PyPI.
 * basic library and image metric CLI split off from raytraverse
-
-
```

### Comparing `raytools-0.1.0/README.rst` & `raytools-0.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ====================
-raytools (0.1.0)
+raytools (0.1.1)
 ====================
 
 .. image:: https://img.shields.io/pypi/v/raytools?style=flat-square
     :target: https://pypi.org/project/raytools
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/l/raytools?style=flat-square
```

### Comparing `raytools-0.1.0/docs/Makefile` & `raytools-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/docs/_static/custom.css` & `raytools-0.1.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/docs/conf.py` & `raytools-0.1.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 author = u"Stephen Wasilewski"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = "0.1.0"
+version = "0.1.1"
 # The full version, including alpha/beta/rc tags.
-release = "0.1.0"
+release = "0.1.1"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'en'
```

### Comparing `raytools-0.1.0/docs/evaluate.rst` & `raytools-0.1.1/docs/evaluate.rst`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/docs/make.bat` & `raytools-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/docs/mapper.rst` & `raytools-0.1.1/docs/mapper.rst`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/linux/getinfo` & `raytools-0.1.1/radiance_depend/linux/getinfo`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/linux/pvalue` & `raytools-0.1.1/radiance_depend/linux/pvalue`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/linux/rcalc` & `raytools-0.1.1/radiance_depend/linux/rcalc`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/linux/vwrays` & `raytools-0.1.1/radiance_depend/linux/vwrays`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/macos/getinfo` & `raytools-0.1.1/radiance_depend/macos/getinfo`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/macos/pvalue` & `raytools-0.1.1/radiance_depend/macos/pvalue`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/macos/rcalc` & `raytools-0.1.1/radiance_depend/macos/rcalc`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/radiance_depend/macos/vwrays` & `raytools-0.1.1/radiance_depend/macos/vwrays`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/__init__.py` & `raytools-0.1.1/raytools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 
 """Top-level package for raytools."""
 
 __author__ = """Stephen Wasilewski"""
 __email__ = 'stephanwaz@gmail.com'
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 __all__ = ['evaluate', 'io', 'imagetools', 'mapper',
            'translate', 'utility']
 
 from raytools import *
 
 
 def set_raypath(basefile=__file__, subd="cal"):
```

### Comparing `raytools-0.1.0/raytools/cal/rayinit.cal` & `raytools-0.1.1/raytools/cal/rayinit.cal`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/cli.py` & `raytools-0.1.1/raytools/cli.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/evaluate/__init__.py` & `raytools-0.1.1/raytools/evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/evaluate/basemetricset.py` & `raytools-0.1.1/raytools/evaluate/basemetricset.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/evaluate/hvsgsm.py` & `raytools-0.1.1/raytools/evaluate/hvsgsm.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/evaluate/metricset.py` & `raytools-0.1.1/raytools/evaluate/metricset.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/evaluate/positionindex.py` & `raytools-0.1.1/raytools/evaluate/positionindex.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/evaluate/retina.py` & `raytools-0.1.1/raytools/evaluate/retina.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/imagetools.py` & `raytools-0.1.1/raytools/imagetools.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,33 +14,37 @@
 
 from raytools import translate, io
 from raytools.evaluate import MetricSet, retina
 from raytools.mapper.viewmapper import ViewMapper
 
 
 def array_uv2ang(imarray):
-    res = imarray.shape[-1]
-    vm = ViewMapper(viewangle=180)
-    pixelxyz = vm.pixelrays(res)
+    resx = imarray.shape[-2]
+    resy = imarray.shape[-1]
+    if resx > resy:
+        vm = ViewMapper(viewangle=360)
+    else:
+        vm = ViewMapper(viewangle=180)
+    img, pixelxyz, mask, _, _ = vm.init_img(resy, features=len(imarray.shape), indices=False)
     uv = vm.xyz2uv(pixelxyz.reshape(-1, 3))
-    mask = vm.in_view(pixelxyz, indices=False)
-    ij = translate.uv2ij(uv[mask], res)
+    ij = translate.uv2ij(uv[mask], resy)
     if len(imarray.shape) == 3:
-        img = np.zeros((3, res*res))
+        img = np.zeros((3, resx*resy))
         img[:, mask] = imarray[:, ij[:, 0], ij[:, 1]]
-        return img.reshape(3, res, res)
+        return img.reshape(3, resx, resy)
     else:
-        img = np.zeros(res*res)
+        img = np.zeros(resx*resy)
         img[mask] = imarray[ij[:, 0], ij[:, 1]]
-        return img.reshape(res, res)
+        return img.reshape(resx, resy)
 
 
-def hdr_uv2ang(imgf, **kwargs):
+def hdr_uv2ang(imgf, outf=None, **kwargs):
+    if outf is None:
+        outf = imgf.rsplit(".", 1)[0] + "_ang.hdr"
     imarray = io.hdr2carray(imgf)
-    outf = imgf.rsplit(".", 1)[0] + "_ang.hdr"
     img = array_uv2ang(imarray)
     io.carray2hdr(img, outf)
     return outf
 
 
 def array_ang2uv(imarray, vm=None):
     if vm is None:
@@ -51,22 +55,23 @@
     pxy = vm.ray2pixel(xyz, imarray.shape[-1])
     if len(imarray.shape) == 3:
         return imarray[:, pxy[:, 0], pxy[:, 1]].reshape(3, res, res)
     else:
         return imarray[pxy[:, 0], pxy[:, 1]].reshape(res, res)
 
 
-def hdr_ang2uv(imgf, useview=True):
+def hdr_ang2uv(imgf, useview=True, outf=None):
+    if outf is None:
+        outf = imgf.rsplit(".", 1)[0] + "_uv.hdr"
     vm = None
     if useview:
         vm = hdr2vm(imgf)
     if vm is None:
         vm = ViewMapper(viewangle=180)
     imarray = io.hdr2carray(imgf)
-    outf = imgf.rsplit(".", 1)[0] + "_uv.hdr"
     img = array_ang2uv(imarray, vm)
     io.carray2hdr(img, outf)
     return outf
 
 
 def hdr2vol(imgf, vm=None):
     ar = io.hdr2array(imgf)
@@ -85,14 +90,26 @@
     vp = vl[-1].split()
     view_angle = float(vp[vp.index("-vh") + 1])
     vd = vp.index("-vd")
     view_dir = [float(vp[i]) for i in range(vd + 1, vd + 4)]
     return ViewMapper(view_dir, view_angle)
 
 
+def img_size(imgf):
+    hd = cst.pipeline([f"getinfo -d {imgf}"]).strip().split()
+    x = 1
+    y = 1
+    for i in range(2, len(hd)):
+        if 'X' in hd[i - 1]:
+            x = int(hd[i])
+        elif 'Y' in hd[i - 1]:
+            y = int(hd[i])
+    return x, y
+
+
 def hdr2vm(imgf, vpt=False):
     """hdr to ViewMapper"""
     header, err = cst.pipeline([f"getinfo {imgf}"], caperr=True)
     try:
         err = err.decode("utf-8")
     except AttributeError:
         pass
@@ -115,34 +132,27 @@
             view_dir = [float(vp[i]) for i in range(vd + 1, vd + 4)]
         try:
             vpi = vp.index("-vp")
         except ValueError:
             view_pt = [0.0, 0.0, 0.0]
         else:
             view_pt = [float(vp[i]) for i in range(vpi + 1, vpi + 4)]
-        hd = cst.pipeline([f"getinfo -d {imgf}"]).strip().split()
-        x = 1
-        y = 1
-        for i in range(2, len(hd)):
-            if 'X' in hd[i - 1]:
-                x = float(hd[i])
-            elif 'Y' in hd[i - 1]:
-                y = float(hd[i])
+        x, y = img_size(imgf)
         vm = ViewMapper(view_dir, view_angle * x / y)
     else:
         view_pt = None
         vm = None
     if vpt:
         return vm, view_pt
     else:
         return vm
 
 
 def normalize_peak(v, o, l, scale=179, peaka=6.7967e-05, peakt=1e5, peakr=4,
-                   blursun=False, blurtol=0.75):
+                   blursun=False, blurtol=0.75, returnall=True):
     """consolidate the brightest pixels represented by v, o, l up into a single
     source, correcting the area while maintaining equal energy
 
     Parameters
     ----------
     v: np.array
         shape (N, 3), direction vectors of pixels (x, y, z) normalized
@@ -160,14 +170,16 @@
         ratio, from peak pixel value to lowest value to include when aggregating
         partially visible sun.
     blursun: bool, optional
         whether to correct area and luminance according to human PSF
     blurtol: float, optional
         when checking for su visibility this enables an averaging of near peak values
         whick could be an artifact from pfilt. set to 1 to disable.
+    returnall: bool, optional
+        if true, return complete v, o, l. if false, only return peak
 
     Returns
     -------
     v: np.array
         shape (N, 3), direction vectors of pixels (x, y, z) normalized
     o: np.array
         shape (N,), solid angles of pixels (steradians)
@@ -216,17 +228,23 @@
         vol = np.delete(np.hstack((v, o[:, None], l[:, None])), pc, axis=0)
         # then add new consolidated ray back to output v, o, l
         v = np.vstack((vol[:, 0:3], pv))
         if blursun:
             cf = np.atleast_1d(retina.blur_sun(peaka, peakl))[0]
         else:
             cf = 1
-        o = np.concatenate((vol[:, 3], [peaka*cf]))
-        l = np.concatenate((vol[:, 4], [peakl/cf]))
-    return v, o, l
+        pvol = (pv.ravel(), peaka*cf, peakl/cf)
+        o = np.concatenate((vol[:, 3], [pvol[1]]))
+        l = np.concatenate((vol[:, 4], [pvol[2]]))
+    else:
+        pvol = np.zeros(5)
+    if returnall:
+        return v, o, l
+    else:
+        return pvol
 
 
 def imgmetric(imgf, metrics, peakn=False, scale=179, threshold=2000., lowlight=False,
               **peakwargs):
     vm = hdr2vm(imgf)
     if vm is None:
         vm = ViewMapper(viewangle=180)
```

### Comparing `raytools-0.1.0/raytools/io.py` & `raytools-0.1.1/raytools/io.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/mapper/__init__.py` & `raytools-0.1.1/raytools/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/mapper/angularmixin.py` & `raytools-0.1.1/raytools/mapper/angularmixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,62 +114,93 @@
         ang = self.radians(vec) - tol
         mask = ang < (self._chordfactor * self.viewangle * np.pi / 360)
         if indices:
             return np.unravel_index(np.arange(ang.size)[mask], vec.shape[:-1])
         else:
             return mask
 
-    def header(self, pt=(0, 0, 0), **kwargs):
+    def header(self, pt=(0, 0, 0), viewproj='vta', **kwargs):
         if np.allclose(self.dxyz, (0, 0, 1)):
             vup = "0 1 0"
         else:
             vup = "0 0 1"
-        return ('VIEW= -vta -vv {0} -vh {0} -vd {1} {2} {3} -vp {4} {5} '
-                '{6} -vu {7}'.format(self.viewangle, *self.dxyz, *pt, vup))
+        return ('VIEW= -{8} -vv {0} -vh {0} -vd {1} {2} {3} -vp {4} {5} '
+                '{6} -vu {7}'.format(self.viewangle, *self.dxyz, *pt, vup,
+                                     viewproj))
 
-    def init_img(self, res=512, pt=(0, 0, 0), features=1, **kwargs):
+    @staticmethod
+    def _process_viewproj(a):
+        a = a.lower()
+        if a[0:2] == 'vt':
+            a = a[-1]
+        a = a[0]
+        if a in ('a', 'f'):  # angular fisheye
+            return 'vta'
+        else:  # Shirley-Chiu square/rectangle
+            return 'vuv'
+
+    def init_img(self, res=512, pt=(0, 0, 0), features=1, viewproj='vta', indices=True,
+                 **kwargs):
         """Initialize an image array with vectors and mask
 
         Parameters
         ----------
         res: int, optional
             image array resolution
         pt: tuple, optional
             view point for image header
+        features: int, optional
+            when greater than 1 initialize img array with N output channels
+        viewproj: str, optional
+            output view projection chose from::
+
+                angular: '[Aa]*', 'vta', 'fish*'
+                shirley chiu: '[Uu]*', 'square'
 
         Returns
         -------
         img: np.array
             zero array of shape (res*self.aspect, res)
         vecs: np.array
             direction vectors corresponding to each pixel (img.size, 3)
         mask: np.array
             indices of flattened img that are in view
         mask2: np.array None
             if features > 1, use mask 2 fro color images
         header: str
         """
+        viewproj = self._process_viewproj(viewproj)
         if features > 1:
-            img = np.zeros((features, res*self.aspect, res))
-        else:
-            img = np.zeros((res*self.aspect, res))
-        vecs = self.pixelrays(res)
-        if self.aspect == 2:
-            mask = self.in_view(vecs[0:res])
-            mask2 = self.ivm.in_view(vecs[res:])
-            mask = (np.concatenate((mask[0], mask2[0] + res)),
-                    np.concatenate((mask[1], mask2[1])))
+            img = np.zeros((features, res * self.aspect, res))
         else:
-            mask = self.in_view(vecs)
-        header = self.header(pt, **kwargs)
-        if features > 1:
-            mask2 = (np.tile(np.arange(features), len(mask[0])),
-                     np.repeat(mask[0], features), np.repeat(mask[1], features))
+            img = np.zeros((res * self.aspect, res))
+        header = self.header(pt, viewproj=viewproj, **kwargs)
+        mask = None
+        mask2 = None
+        if viewproj == 'vta':
+            vecs = self.pixelrays(res)
+            if self.aspect == 2:
+                mask = self.in_view(vecs[0:res], indices=indices)
+                mask2 = self.ivm.in_view(vecs[res:], indices=indices)
+                if indices:
+                    mask = (np.concatenate((mask[0], mask2[0] + res)),
+                            np.concatenate((mask[1], mask2[1])))
+                else:
+                    mask = np.concatenate((mask, mask2))
+            else:
+                mask = self.in_view(vecs, indices=indices)
+
+            if features > 1 and indices:
+                mask2 = (np.tile(np.arange(features), len(mask[0])),
+                         np.repeat(mask[0], features), np.repeat(mask[1], features))
+            else:
+                mask2 = mask
         else:
-            mask2 = mask
+            uv = translate.bin2uv(np.arange(res * res * self.aspect), res)
+            vecs = self.uv2xyz(uv).reshape(self.aspect * res, res, 3)
         return img, vecs, mask, mask2, header
 
     def add_vecs_to_img(self, img, v, channels=(1, 0, 0), grow=0, fisheye=True,
                         mask=None):
         res = img.shape[-1]
         if fisheye:
             if self.aspect == 2:
```

### Comparing `raytools-0.1.0/raytools/mapper/mapper.py` & `raytools-0.1.1/raytools/mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/mapper/viewmapper.py` & `raytools-0.1.1/raytools/mapper/viewmapper.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools/translate.py` & `raytools-0.1.1/raytools/translate.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # =======================================================================
 
 """functions for translating between coordinate spaces and resolutions"""
 
 import numpy as np
 from scipy.ndimage import gaussian_filter, uniform_filter
 from scipy.spatial import cKDTree
-
+from scipy import stats
 
 def norm(v):
     """normalize 2D array of vectors along last dimension"""
     return v/np.linalg.norm(v, axis=-1).reshape(-1, 1)
 
 
 def norm1(v):
@@ -391,14 +391,181 @@
     elif radius is not None:
         if gauss:
             samps = gaussian_filter(samps, radius)
         else:
             samps = uniform_filter(samps, int(radius))
     return samps
 
+####################################
+# 1D non-uniform signal processing #
+####################################
+
+
+def weighted_quantile(d, weights=None, q=0.5, t=0.0):
+    """calculate weighted quantiles on 1d data
+
+    Parameters
+    ----------
+    d : np.array
+        data (flattens array)
+    q : np.array
+        quantiles (N,)
+    weights : np.array
+        weights
+    t : float
+        threshold for inclusion
+
+    Returns
+    -------
+    result : np.array
+        shape (N,)
+
+    """
+    if weights is None:
+        return np.quantile(d, q)
+    else:
+        d = np.asarray(d).ravel()
+        si = np.argsort(d)
+        d = d[si]
+        w = np.asarray(weights).ravel()[si]
+        d = d[w > t]
+        w = w[w > t]
+        cw = np.cumsum(w)
+        cw = cw - cw[0]
+        midp = np.asarray(q) * cw[-1]
+        li = np.searchsorted(cw, midp, side='right') - 1
+        ri = np.where(np.isclose(q, 1), li, li+1)
+        try:
+            dn = np.where(np.isclose(q, 1), 1, (cw[ri] - cw[li]))
+        except IndexError as ex:
+            result = np.quantile(d, q)
+        else:
+            result = d[li] + (d[ri] - d[li]) * (midp - cw[li])/dn
+        return result
+
+
+def weighted_median(d, weights=None, t=0.0):
+    """convinience function with different signature"""
+    return weighted_quantile(d, q=.5, weights=weights, t=t)
+
+
+def non_uniform_gaussian_filter(x, y, xr=None, sigma=None, sscale=1.0,
+                                bw=500, amethod='mean'):
+    """apply a guassian filter to non-uniformly spaced data
+
+    Parameters
+    ----------
+    x : np.array
+        1d source data (N,)
+    y : np.array
+        data to smooth (M,N)
+    xr : np.array
+        coordinates along x to resample (R,). if none, uses x directly
+    sigma : float
+        if None applies scotts rule (x.size**0.2)
+    sscale : float
+        extra factor to apply to sigma
+    bw : int
+        1/2 bandwidth for kernel (in # of samples) use for N > 10000
+    amethod : Union[str, np.array]
+        averaging method, can be 'mean', 'median', or array like of quantiles. if more
+        than one quantile y must contain only one feature
+
+    Returns
+    -------
+    mu : np.array
+        shape (M,), or (R,) if resample
+    """
+    if amethod == 'mean':
+        afunc = np.average
+        akwargs = dict(axis=1)
+    elif amethod == 'median':
+        afunc = weighted_median
+        akwargs = {}
+    else:
+        try:
+            q = np.atleast_1d(amethod).ravel().astype(float)
+        except (TypeError, ValueError):
+            raise ValueError(f"'{amethod}' is not a valid option, must be "
+                             f"'mean' or array-like of quantiles")
+        if not np.all((q >= 0) & (q <= 1)):
+            raise ValueError(f"quantiles must all be in [0,1] not {q}")
+        if y.size > max(y.shape) and len(q) > 1:
+            raise ValueError(f"y must only have one dimension when calculating "
+                             f"more than 1 quantile")
+        afunc = weighted_quantile
+        akwargs = dict(q=q)
+
+    def _nugf_x(x0, xp, yp, sp):
+        """average yp spaced by xp at x0 for a sigma=sp"""
+        n = stats.norm(loc=x0, scale=sp)
+        weights = n.pdf(xp)
+        if np.sum(weights) > 0:
+            mu = afunc(yp, weights=weights, **akwargs)
+        else:
+            # fall back to linear interpolation
+            mui = np.searchsorted(xp, x0)[0]
+            if mui == len(xp):
+                mu = yp[:, -1]
+            elif mui == 0:
+                mu = yp[:, 0]
+            else:
+                mu = np.average((yp[:, mui], yp[:, mui-1]), axis=0,
+                                weights=(x0-xp[mui-1], xp[mui]-x0))
+            if 'q' in akwargs:
+                mu = np.full(len(akwargs['q']), mu)
+        return mu
+
+    def _nugf_i(i, xp, yp, sp):
+        """average yp spaced by xp at index i for a sigma=sp"""
+        return _nugf_x(xp[i[0]], xp, yp, sp)
+
+    def _nugf_x_bw(x0, xp, yp, sp):
+        """average yp spaced by xp at x0 for a sigma=sp with limited
+        bandwidth"""
+        i = np.searchsorted(xp, x0)
+        i2 = np.clip((i - bw, i + bw), 0, len(xp)).astype(int).ravel()
+        return _nugf_x(x0, xp[i2[0]:i2[1]], yp[:, i2[0]:i2[1]], sp)
+
+    def _nugf_i_bw(i, xp, yp, sp):
+        """average yp spaced by xp at index i for a sigma=sp with limited
+        bandwidth"""
+        i2 = np.clip((i - bw, i + bw), 0, len(xp)).astype(int).ravel()
+        return _nugf_x(xp[i], xp[i2[0]:i2[1]], yp[:, i2[0]:i2[1]], sp)
+
+    y = np.atleast_2d(y)
+    # sort data if necessary
+    if not np.all(x[:-1] <= x[1:]):
+        sorti = np.argsort(x, kind='stable')
+        x = x[sorti]
+        y = y[:, sorti]
+        inv_sort = np.argsort(sorti, kind='stable')
+    else:
+        inv_sort = None
+    if sigma is None:
+        sigma = np.sqrt(np.cov(x) * len(x) ** (-.4))
+    sigma *= sscale
+    if bw is None and xr is None:  # no bandwidth and self
+        nugf = _nugf_i
+        idxs = np.arange(x.size)
+    elif bw is None:  # no bandwidth, resample
+        nugf = _nugf_x
+        idxs = xr
+    elif xr is None:  # bandwidth on self
+        nugf = _nugf_i_bw
+        idxs = np.arange(x.size)
+    else:  # bandwidth on resample
+        nugf = _nugf_x_bw
+        idxs = xr
+    amu = np.apply_along_axis(nugf, 0, idxs.reshape(1, -1), x, y, sigma)
+    # sort back unless already sorted or resampled
+    if inv_sort is not None and resample is None:
+        amu = amu[inv_sort]
+    return amu
+
 
 ####################
 # vector rotations #
 ####################
 
 def rmtx_elem(theta, axis=2, degrees=True):
     if degrees:
@@ -410,15 +577,15 @@
 
 
 def rotate_elem(v, theta, axis=2, degrees=True):
     rmtx = rmtx_elem(theta, axis=axis, degrees=degrees)
     return np.einsum('ij,kj->ki', rmtx, v)
 
 
-def rmtx_yp(v):
+def rmtx_yp(v, keepdims=False):
     """generate a pair of rotation matrices to transform from vector v to
     z, enforcing a z-up in the source space and a y-up in the destination. If
     v is z, returns pair of identity matrices, if v is -z returns pair of 180
     degree rotation matrices.
 
     Parameters
     ----------
@@ -465,14 +632,17 @@
     p = -tp[:, 0]
     cp = np.cos(p)
     sp = np.sin(p)
     pmtx = np.stack(((o, z, z), (z, cp, sp), (z, -sp, cp))).T
     pmtx[e] = np.eye(3)
     pmtx[ne] = np.array([(1, 0, 0), (0, -1, 0), (0, 0, -1)])
 
+    if keepdims:
+        return ymtx, pmtx
+
     return np.squeeze(ymtx), np.squeeze(pmtx)
 
 
 def cull_vectors(vecs, tol):
     """return mask to cull duplicate vectors within tolerance
 
     Parameters
```

### Comparing `raytools-0.1.0/raytools/utility.py` & `raytools-0.1.1/raytools/utility.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/raytools.egg-info/PKG-INFO` & `raytools-0.1.1/raytools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: raytools
-Version: 0.1.0
+Version: 0.1.1
 Summary: working with hdr images, numpy and coordinate transformations for lighting simulation
 Home-page: https://github.com/stephanwaz/raytools
 Author: Stephen Wasilewski
 Author-email: stephanwaz@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Keywords: raytools
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 License-File: LICENSE
 
 ====================
-raytools (0.1.0)
+raytools (0.1.1)
 ====================
 
 .. image:: https://img.shields.io/pypi/v/raytools?style=flat-square
     :target: https://pypi.org/project/raytools
     :alt: PyPI
 
 .. image:: https://img.shields.io/pypi/l/raytools?style=flat-square
@@ -80,9 +79,7 @@
 =======
 
 0.1.0 (2023-01-06)
 ------------------
 
 * First release on PyPI.
 * basic library and image metric CLI split off from raytraverse
-
-
```

### Comparing `raytools-0.1.0/raytools.egg-info/SOURCES.txt` & `raytools-0.1.1/raytools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 docs/mapper.rst
 docs/requirements.txt
 docs/search.rst
 docs/translate.rst
 docs/utility.rst
 docs/_static/custom.css
 docs/_templates/navigation.html
-radiance_depend/.DS_Store
 radiance_depend/linux/getinfo
 radiance_depend/linux/pvalue
 radiance_depend/linux/rcalc
 radiance_depend/linux/vwrays
 radiance_depend/macos/getinfo
 radiance_depend/macos/pvalue
 radiance_depend/macos/rcalc
@@ -54,15 +53,14 @@
 raytools/evaluate/metricset.py
 raytools/evaluate/positionindex.py
 raytools/evaluate/retina.py
 raytools/mapper/__init__.py
 raytools/mapper/angularmixin.py
 raytools/mapper/mapper.py
 raytools/mapper/viewmapper.py
-tests/.DS_Store
 tests/test_hvsgsm.py
 tests/test_imagetools.py
 tests/test_io.py
 tests/test_metric.py
 tests/test_retina.py
 tests/test_translate.py
 tests/test_utility.py
```

### Comparing `raytools-0.1.0/release.sh` & `raytools-0.1.1/release.sh`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/setup.cfg` & `raytools-0.1.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1
 commit = False
 tag = False
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `raytools-0.1.0/setup.py` & `raytools-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 radexec = [rade for rade in radexec if
            shutil.which(os.path.basename(rade)) is None]
 if len(radexec) > 0:
     data_files = [('bin', radexec)]
 else:
     data_files = []
-print(data_files, file=sys.stderr)
 package_data = {"raytools": ["cal/*.cal"]}
 
 setup(
     author="Stephen Wasilewski",
     author_email='stephanwaz@gmail.com',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -69,10 +68,10 @@
     packages=find_packages(),
     data_files=data_files,
     package_data=package_data,
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/stephanwaz/raytools',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
     )
```

### Comparing `raytools-0.1.0/tests/test_hvsgsm.py` & `raytools-0.1.1/tests/test_hvsgsm.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/test_imagetools.py` & `raytools-0.1.1/tests/test_imagetools.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/test_io.py` & `raytools-0.1.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/test_metric.py` & `raytools-0.1.1/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/test_retina.py` & `raytools-0.1.1/tests/test_retina.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/test_translate.py` & `raytools-0.1.1/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/test_utility.py` & `raytools-0.1.1/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/test_viewmapper.py` & `raytools-0.1.1/tests/test_viewmapper.py`

 * *Files identical despite different names*

### Comparing `raytools-0.1.0/tests/testdir/oct21_detail_glz_EW_desk.hdr` & `raytools-0.1.1/tests/testdir/oct21_detail_glz_EW_desk.hdr`

 * *Files identical despite different names*

