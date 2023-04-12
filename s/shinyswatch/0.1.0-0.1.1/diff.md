# Comparing `tmp/shinyswatch-0.1.0.tar.gz` & `tmp/shinyswatch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinyswatch-0.1.0.tar", last modified: Wed Apr 12 17:24:30 2023, max compression
+gzip compressed data, was "shinyswatch-0.1.1.tar", last modified: Wed Apr 12 17:31:41 2023, max compression
```

## Comparing `shinyswatch-0.1.0.tar` & `shinyswatch-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,100 @@
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:24:30.894209 shinyswatch-0.1.0/
--rw-r--r--   0 barret     (502) staff       (20)     1067 2023-03-29 18:28:41.000000 shinyswatch-0.1.0/LICENSE
--rw-r--r--   0 barret     (502) staff       (20)       36 2023-04-06 16:37:13.000000 shinyswatch-0.1.0/MANIFEST.in
--rw-r--r--   0 barret     (502) staff       (20)     2429 2023-04-12 17:24:30.894317 shinyswatch-0.1.0/PKG-INFO
--rw-r--r--   0 barret     (502) staff       (20)     1179 2023-04-11 21:01:32.000000 shinyswatch-0.1.0/README.md
--rw-r--r--   0 barret     (502) staff       (20)     1956 2023-04-12 17:24:30.894679 shinyswatch-0.1.0/setup.cfg
--rw-r--r--   0 barret     (502) staff       (20)       38 2023-03-23 14:55:23.000000 shinyswatch-0.1.0/setup.py
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:24:30.893024 shinyswatch-0.1.0/shinyswatch/
--rw-r--r--   0 barret     (502) staff       (20)      120 2023-04-11 21:01:57.000000 shinyswatch-0.1.0/shinyswatch/__init__.py
--rw-r--r--   0 barret     (502) staff       (20)      991 2023-04-06 16:37:13.000000 shinyswatch-0.1.0/shinyswatch/_assert.py
--rw-r--r--   0 barret     (502) staff       (20)     2941 2023-04-12 13:19:08.000000 shinyswatch-0.1.0/shinyswatch/_theme.py
--rw-r--r--   0 barret     (502) staff       (20)      584 2023-04-06 16:37:13.000000 shinyswatch-0.1.0/shinyswatch/_themes.py
--rw-r--r--   0 barret     (502) staff       (20)        0 2023-03-23 14:55:23.000000 shinyswatch-0.1.0/shinyswatch/py.typed
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:24:30.894071 shinyswatch-0.1.0/shinyswatch.egg-info/
--rw-r--r--   0 barret     (502) staff       (20)     2429 2023-04-12 17:24:30.000000 shinyswatch-0.1.0/shinyswatch.egg-info/PKG-INFO
--rw-r--r--   0 barret     (502) staff       (20)      369 2023-04-12 17:24:30.000000 shinyswatch-0.1.0/shinyswatch.egg-info/SOURCES.txt
--rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-12 17:24:30.000000 shinyswatch-0.1.0/shinyswatch.egg-info/dependency_links.txt
--rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-12 17:24:30.000000 shinyswatch-0.1.0/shinyswatch.egg-info/not-zip-safe
--rw-r--r--   0 barret     (502) staff       (20)      369 2023-04-12 17:24:30.000000 shinyswatch-0.1.0/shinyswatch.egg-info/requires.txt
--rw-r--r--   0 barret     (502) staff       (20)       12 2023-04-12 17:24:30.000000 shinyswatch-0.1.0/shinyswatch.egg-info/top_level.txt
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.958611 shinyswatch-0.1.1/
+-rw-r--r--   0 barret     (502) staff       (20)     1067 2023-03-29 18:28:41.000000 shinyswatch-0.1.1/LICENSE
+-rw-r--r--   0 barret     (502) staff       (20)      216 2023-04-12 17:30:44.000000 shinyswatch-0.1.1/MANIFEST.in
+-rw-r--r--   0 barret     (502) staff       (20)     2429 2023-04-12 17:31:41.958757 shinyswatch-0.1.1/PKG-INFO
+-rw-r--r--   0 barret     (502) staff       (20)     1179 2023-04-11 21:01:32.000000 shinyswatch-0.1.1/README.md
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.923027 shinyswatch-0.1.1/docs/
+-rw-r--r--   0 barret     (502) staff       (20)      638 2023-04-11 20:37:32.000000 shinyswatch-0.1.1/docs/Makefile
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.916098 shinyswatch-0.1.1/docs/build/
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.916402 shinyswatch-0.1.1/docs/build/html/
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.923404 shinyswatch-0.1.1/docs/build/html/_sources/
+-rw-r--r--   0 barret     (502) staff       (20)      792 2023-04-12 13:21:09.000000 shinyswatch-0.1.1/docs/build/html/_sources/index.rst
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.923788 shinyswatch-0.1.1/docs/build/html/_sources/reference/
+-rw-r--r--   0 barret     (502) staff       (20)       95 2023-04-12 13:34:05.000000 shinyswatch-0.1.1/docs/build/html/_sources/reference/shinyswatch.theme.rst
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.925467 shinyswatch-0.1.1/docs/build/html/_static/
+-rw-r--r--   0 barret     (502) staff       (20)    30784 2023-04-12 13:39:56.000000 shinyswatch-0.1.1/docs/build/html/_static/bootswatch.png
+-rw-r--r--   0 barret     (502) staff       (20)      286 2023-04-11 20:40:59.000000 shinyswatch-0.1.1/docs/build/html/_static/file.png
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.925831 shinyswatch-0.1.1/docs/build/html/_static/images/
+-rw-r--r--   0 barret     (502) staff       (20)     7601 2023-04-11 20:45:27.000000 shinyswatch-0.1.1/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0 barret     (502) staff       (20)       90 2023-04-11 20:40:59.000000 shinyswatch-0.1.1/docs/build/html/_static/minus.png
+-rw-r--r--   0 barret     (502) staff       (20)       90 2023-04-11 20:40:59.000000 shinyswatch-0.1.1/docs/build/html/_static/plus.png
+-rw-r--r--   0 barret     (502) staff       (20)       70 2023-04-12 16:47:04.000000 shinyswatch-0.1.1/docs/modules.rst
+-rw-r--r--   0 barret     (502) staff       (20)      156 2023-04-12 16:47:04.000000 shinyswatch-0.1.1/docs/shinyswatch.rst
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.927252 shinyswatch-0.1.1/docs/source/
+-rw-r--r--   0 barret     (502) staff       (20)     3778 2023-04-12 13:38:51.000000 shinyswatch-0.1.1/docs/source/conf.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.928211 shinyswatch-0.1.1/docs/source/images/
+-rw-r--r--   0 barret     (502) staff       (20)    17879 2023-04-12 13:38:59.000000 shinyswatch-0.1.1/docs/source/images/bootswatch copy.png
+-rw-r--r--   0 barret     (502) staff       (20)    30784 2023-04-12 13:39:56.000000 shinyswatch-0.1.1/docs/source/images/bootswatch.png
+-rw-r--r--   0 barret     (502) staff       (20)      792 2023-04-12 13:21:09.000000 shinyswatch-0.1.1/docs/source/index.rst
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.928673 shinyswatch-0.1.1/docs/source/reference/
+-rw-r--r--   0 barret     (502) staff       (20)       95 2023-04-12 13:34:05.000000 shinyswatch-0.1.1/docs/source/reference/shinyswatch.theme.rst
+-rw-r--r--   0 barret     (502) staff       (20)     1956 2023-04-12 17:31:41.959311 shinyswatch-0.1.1/setup.cfg
+-rw-r--r--   0 barret     (502) staff       (20)       38 2023-03-23 14:55:23.000000 shinyswatch-0.1.1/setup.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.931944 shinyswatch-0.1.1/shinyswatch/
+-rw-r--r--   0 barret     (502) staff       (20)      120 2023-04-12 17:31:09.000000 shinyswatch-0.1.1/shinyswatch/__init__.py
+-rw-r--r--   0 barret     (502) staff       (20)      991 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/_assert.py
+-rw-r--r--   0 barret     (502) staff       (20)     2941 2023-04-12 13:19:08.000000 shinyswatch-0.1.1/shinyswatch/_theme.py
+-rw-r--r--   0 barret     (502) staff       (20)      584 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/_themes.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.920858 shinyswatch-0.1.1/shinyswatch/bsw5/
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.933840 shinyswatch-0.1.1/shinyswatch/bsw5/cerulean/
+-rw-r--r--   0 barret     (502) staff       (20)   241305 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/cerulean/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.934678 shinyswatch-0.1.1/shinyswatch/bsw5/cosmo/
+-rw-r--r--   0 barret     (502) staff       (20)   228137 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/cosmo/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.935328 shinyswatch-0.1.1/shinyswatch/bsw5/cyborg/
+-rw-r--r--   0 barret     (502) staff       (20)   239795 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/cyborg/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.936090 shinyswatch-0.1.1/shinyswatch/bsw5/darkly/
+-rw-r--r--   0 barret     (502) staff       (20)   244211 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/darkly/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.936561 shinyswatch-0.1.1/shinyswatch/bsw5/flatly/
+-rw-r--r--   0 barret     (502) staff       (20)   240774 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/flatly/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.937325 shinyswatch-0.1.1/shinyswatch/bsw5/journal/
+-rw-r--r--   0 barret     (502) staff       (20)   238362 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/journal/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.937913 shinyswatch-0.1.1/shinyswatch/bsw5/litera/
+-rw-r--r--   0 barret     (502) staff       (20)   240358 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/litera/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.938639 shinyswatch-0.1.1/shinyswatch/bsw5/lumen/
+-rw-r--r--   0 barret     (502) staff       (20)   245474 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/lumen/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.939173 shinyswatch-0.1.1/shinyswatch/bsw5/lux/
+-rw-r--r--   0 barret     (502) staff       (20)   229679 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/lux/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.940246 shinyswatch-0.1.1/shinyswatch/bsw5/materia/
+-rw-r--r--   0 barret     (502) staff       (20)   268868 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/materia/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.941115 shinyswatch-0.1.1/shinyswatch/bsw5/minty/
+-rw-r--r--   0 barret     (502) staff       (20)   239411 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/minty/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.942160 shinyswatch-0.1.1/shinyswatch/bsw5/morph/
+-rw-r--r--   0 barret     (502) staff       (20)   264987 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/morph/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.943232 shinyswatch-0.1.1/shinyswatch/bsw5/pulse/
+-rw-r--r--   0 barret     (502) staff       (20)   231184 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/pulse/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.945299 shinyswatch-0.1.1/shinyswatch/bsw5/quartz/
+-rw-r--r--   0 barret     (502) staff       (20)   275083 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/quartz/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.946305 shinyswatch-0.1.1/shinyswatch/bsw5/sandstone/
+-rw-r--r--   0 barret     (502) staff       (20)   241171 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/sandstone/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.947005 shinyswatch-0.1.1/shinyswatch/bsw5/simplex/
+-rw-r--r--   0 barret     (502) staff       (20)   241660 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/simplex/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.947767 shinyswatch-0.1.1/shinyswatch/bsw5/sketchy/
+-rw-r--r--   0 barret     (502) staff       (20)   245207 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/sketchy/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.948423 shinyswatch-0.1.1/shinyswatch/bsw5/slate/
+-rw-r--r--   0 barret     (502) staff       (20)   253193 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/slate/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.949296 shinyswatch-0.1.1/shinyswatch/bsw5/solar/
+-rw-r--r--   0 barret     (502) staff       (20)   239224 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/solar/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.951368 shinyswatch-0.1.1/shinyswatch/bsw5/spacelab/
+-rw-r--r--   0 barret     (502) staff       (20)   242824 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/spacelab/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.952086 shinyswatch-0.1.1/shinyswatch/bsw5/superhero/
+-rw-r--r--   0 barret     (502) staff       (20)   239767 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/superhero/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.952863 shinyswatch-0.1.1/shinyswatch/bsw5/united/
+-rw-r--r--   0 barret     (502) staff       (20)   237981 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/united/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.953585 shinyswatch-0.1.1/shinyswatch/bsw5/vapor/
+-rw-r--r--   0 barret     (502) staff       (20)   256498 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/vapor/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.954064 shinyswatch-0.1.1/shinyswatch/bsw5/yeti/
+-rw-r--r--   0 barret     (502) staff       (20)   249497 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/yeti/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.954861 shinyswatch-0.1.1/shinyswatch/bsw5/zephyr/
+-rw-r--r--   0 barret     (502) staff       (20)   246162 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/zephyr/bootswatch.min.css
+-rw-r--r--   0 barret     (502) staff       (20)        0 2023-03-23 14:55:23.000000 shinyswatch-0.1.1/shinyswatch/py.typed
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.933637 shinyswatch-0.1.1/shinyswatch.egg-info/
+-rw-r--r--   0 barret     (502) staff       (20)     2429 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/PKG-INFO
+-rw-r--r--   0 barret     (502) staff       (20)     1988 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/SOURCES.txt
+-rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/dependency_links.txt
+-rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/not-zip-safe
+-rw-r--r--   0 barret     (502) staff       (20)      369 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/requires.txt
+-rw-r--r--   0 barret     (502) staff       (20)       12 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/top_level.txt
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.958105 shinyswatch-0.1.1/tests/
+-rw-r--r--   0 barret     (502) staff       (20)     6148 2023-03-29 18:47:46.000000 shinyswatch-0.1.1/tests/.DS_Store
+-rw-r--r--   0 barret     (502) staff       (20)       33 2023-03-29 18:42:55.000000 shinyswatch-0.1.1/tests/__init__.py
+-rw-r--r--   0 barret     (502) staff       (20)      474 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/tests/test_themes.py
```

### Comparing `shinyswatch-0.1.0/LICENSE` & `shinyswatch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.0/PKG-INFO` & `shinyswatch-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
 Home-page: https://github.com/schloerke/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schloerke/py-shinyswatch/issues
 Project-URL: Source Code, https://github.com/schloerke/py-shinyswatch
```

### Comparing `shinyswatch-0.1.0/README.md` & `shinyswatch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.0/setup.cfg` & `shinyswatch-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.0/shinyswatch/_assert.py` & `shinyswatch-0.1.1/shinyswatch/_assert.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.0/shinyswatch/_theme.py` & `shinyswatch-0.1.1/shinyswatch/_theme.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.0/shinyswatch/_themes.py` & `shinyswatch-0.1.1/shinyswatch/_themes.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.0/shinyswatch.egg-info/PKG-INFO` & `shinyswatch-0.1.1/shinyswatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.1.0
+Version: 0.1.1
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
 Home-page: https://github.com/schloerke/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schloerke/py-shinyswatch/issues
 Project-URL: Source Code, https://github.com/schloerke/py-shinyswatch
```

