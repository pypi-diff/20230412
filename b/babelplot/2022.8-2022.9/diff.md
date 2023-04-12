# Comparing `tmp/babelplot-2022.8.tar.gz` & `tmp/babelplot-2022.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babelplot-2022.8.tar", last modified: Wed Jul 13 17:25:19 2022, max compression
+gzip compressed data, was "babelplot-2022.9.tar", last modified: Tue Nov 29 10:11:10 2022, max compression
```

## Comparing `babelplot-2022.8.tar` & `babelplot-2022.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/
--rw-r--r--   0 eric      (1000) users      (984)       66 2022-07-11 08:51:06.000000 babelplot-2022.8/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     2601 2022-07-13 17:25:19.303590 babelplot-2022.8/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2022-02-23 16:31:24.000000 babelplot-2022.8/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 babelplot-2022.8/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     1783 2022-04-04 13:36:59.000000 babelplot-2022.8/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/
--rw-r--r--   0 eric      (1000) users      (984)     1795 2022-04-06 08:30:21.000000 babelplot-2022.8/babelplot/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/backend/
--rw-r--r--   0 eric      (1000) users      (984)     4995 2022-07-13 15:29:53.000000 babelplot-2022.8/babelplot/backend/bokeh_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/backend/brick/
--rw-r--r--   0 eric      (1000) users      (984)     3283 2022-07-13 07:40:40.000000 babelplot-2022.8/babelplot/backend/brick/html.py
--rw-r--r--   0 eric      (1000) users      (984)     1696 2022-07-11 09:29:18.000000 babelplot-2022.8/babelplot/backend/gr_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/backend/helper/
--rw-r--r--   0 eric      (1000) users      (984)     4485 2022-04-06 07:31:23.000000 babelplot-2022.8/babelplot/backend/helper/creation.py
--rw-r--r--   0 eric      (1000) users      (984)     8660 2022-04-21 14:22:29.000000 babelplot-2022.8/babelplot/backend/helper/validation.py
--rw-r--r--   0 eric      (1000) users      (984)    15831 2022-07-13 17:19:39.000000 babelplot-2022.8/babelplot/backend/matplotlib_.py
--rw-r--r--   0 eric      (1000) users      (984)    10123 2022-07-13 17:05:34.000000 babelplot-2022.8/babelplot/backend/plotly_.py
--rw-r--r--   0 eric      (1000) users      (984)     2203 2022-04-08 08:53:12.000000 babelplot-2022.8/babelplot/backend/runtime.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/backend/specification/
--rw-r--r--   0 eric      (1000) users      (984)     3340 2022-04-20 15:21:18.000000 babelplot-2022.8/babelplot/backend/specification/implemented.py
--rw-r--r--   0 eric      (1000) users      (984)    14000 2022-07-13 13:25:34.000000 babelplot-2022.8/babelplot/backend/specification/plot.py
--rw-r--r--   0 eric      (1000) users      (984)     3996 2022-07-13 08:09:08.000000 babelplot-2022.8/babelplot/backend/vedo_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/brick/
--rw-r--r--   0 eric      (1000) users      (984)     2008 2022-04-21 14:04:43.000000 babelplot-2022.8/babelplot/brick/enum.py
--rw-r--r--   0 eric      (1000) users      (984)     2039 2022-04-20 15:16:40.000000 babelplot-2022.8/babelplot/brick/log.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/documentation/
--rw-r--r--   0 eric      (1000) users      (984)     5974 2022-07-13 17:14:41.000000 babelplot-2022.8/babelplot/documentation/gallery-matplotlib.py
--rw-r--r--   0 eric      (1000) users      (984)     6066 2022-07-13 17:14:06.000000 babelplot-2022.8/babelplot/documentation/gallery-plotly.py
--rw-r--r--   0 eric      (1000) users      (984)     4979 2022-07-12 13:35:56.000000 babelplot-2022.8/babelplot/figure.py
--rw-r--r--   0 eric      (1000) users      (984)     4867 2022-04-08 08:50:48.000000 babelplot-2022.8/babelplot/help.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/test/
--rw-r--r--   0 eric      (1000) users      (984)     2924 2022-07-13 16:35:42.000000 babelplot-2022.8/babelplot/test/test_backends.py
--rw-r--r--   0 eric      (1000) users      (984)     3278 2022-07-13 17:21:55.000000 babelplot-2022.8/babelplot/test/test_matplotlib.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot/type/
--rw-r--r--   0 eric      (1000) users      (984)     4371 2022-07-11 09:03:25.000000 babelplot-2022.8/babelplot/type/base.py
--rw-r--r--   0 eric      (1000) users      (984)     3110 2022-04-20 15:21:18.000000 babelplot-2022.8/babelplot/type/dimension.py
--rw-r--r--   0 eric      (1000) users      (984)     8289 2022-07-13 17:08:28.000000 babelplot-2022.8/babelplot/type/figure.py
--rw-r--r--   0 eric      (1000) users      (984)     4814 2022-07-12 12:11:09.000000 babelplot-2022.8/babelplot/type/frame.py
--rw-r--r--   0 eric      (1000) users      (984)     3722 2022-04-21 14:07:23.000000 babelplot-2022.8/babelplot/type/plot.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-07-13 17:25:19.303590 babelplot-2022.8/babelplot.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     2601 2022-07-13 17:25:19.000000 babelplot-2022.8/babelplot.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1010 2022-07-13 17:25:19.000000 babelplot-2022.8/babelplot.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2022-07-13 17:25:19.000000 babelplot-2022.8/babelplot.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       27 2022-07-13 17:25:19.000000 babelplot-2022.8/babelplot.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2022-07-13 17:25:19.000000 babelplot-2022.8/babelplot.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-04-04 12:16:02.000000 babelplot-2022.8/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2022-07-13 17:25:19.303590 babelplot-2022.8/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     4472 2022-07-13 17:23:55.000000 babelplot-2022.8/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.901756 babelplot-2022.9/
+-rw-r--r--   0 eric      (1000) users      (984)       66 2022-07-11 08:51:06.000000 babelplot-2022.9/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     2601 2022-11-29 10:11:10.901756 babelplot-2022.9/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2022-02-23 16:31:24.000000 babelplot-2022.9/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 babelplot-2022.9/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     1783 2022-04-04 13:36:59.000000 babelplot-2022.9/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.898423 babelplot-2022.9/babelplot/
+-rw-r--r--   0 eric      (1000) users      (984)     1795 2022-04-06 08:30:21.000000 babelplot-2022.9/babelplot/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.898423 babelplot-2022.9/babelplot/backend/
+-rw-r--r--   0 eric      (1000) users      (984)     4995 2022-07-13 15:29:53.000000 babelplot-2022.9/babelplot/backend/bokeh_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.898423 babelplot-2022.9/babelplot/backend/brick/
+-rw-r--r--   0 eric      (1000) users      (984)     3283 2022-07-13 07:40:40.000000 babelplot-2022.9/babelplot/backend/brick/html.py
+-rw-r--r--   0 eric      (1000) users      (984)     1696 2022-07-11 09:29:18.000000 babelplot-2022.9/babelplot/backend/gr_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.898423 babelplot-2022.9/babelplot/backend/helper/
+-rw-r--r--   0 eric      (1000) users      (984)     4485 2022-04-06 07:31:23.000000 babelplot-2022.9/babelplot/backend/helper/creation.py
+-rw-r--r--   0 eric      (1000) users      (984)     8660 2022-04-21 14:22:29.000000 babelplot-2022.9/babelplot/backend/helper/validation.py
+-rw-r--r--   0 eric      (1000) users      (984)    15831 2022-07-13 17:19:39.000000 babelplot-2022.9/babelplot/backend/matplotlib_.py
+-rw-r--r--   0 eric      (1000) users      (984)    10119 2022-10-13 12:40:05.000000 babelplot-2022.9/babelplot/backend/plotly_.py
+-rw-r--r--   0 eric      (1000) users      (984)     2203 2022-04-08 08:53:12.000000 babelplot-2022.9/babelplot/backend/runtime.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.901756 babelplot-2022.9/babelplot/backend/specification/
+-rw-r--r--   0 eric      (1000) users      (984)     3340 2022-04-20 15:21:18.000000 babelplot-2022.9/babelplot/backend/specification/implemented.py
+-rw-r--r--   0 eric      (1000) users      (984)    14000 2022-07-13 13:25:34.000000 babelplot-2022.9/babelplot/backend/specification/plot.py
+-rw-r--r--   0 eric      (1000) users      (984)     3996 2022-07-13 08:09:08.000000 babelplot-2022.9/babelplot/backend/vedo_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.901756 babelplot-2022.9/babelplot/brick/
+-rw-r--r--   0 eric      (1000) users      (984)     2008 2022-04-21 14:04:43.000000 babelplot-2022.9/babelplot/brick/enum.py
+-rw-r--r--   0 eric      (1000) users      (984)     2039 2022-04-20 15:16:40.000000 babelplot-2022.9/babelplot/brick/log.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.901756 babelplot-2022.9/babelplot/documentation/
+-rw-r--r--   0 eric      (1000) users      (984)     5974 2022-07-13 17:14:41.000000 babelplot-2022.9/babelplot/documentation/gallery-matplotlib.py
+-rw-r--r--   0 eric      (1000) users      (984)     6066 2022-07-13 17:14:06.000000 babelplot-2022.9/babelplot/documentation/gallery-plotly.py
+-rw-r--r--   0 eric      (1000) users      (984)     4979 2022-07-12 13:35:56.000000 babelplot-2022.9/babelplot/figure.py
+-rw-r--r--   0 eric      (1000) users      (984)     4867 2022-04-08 08:50:48.000000 babelplot-2022.9/babelplot/help.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.901756 babelplot-2022.9/babelplot/test/
+-rw-r--r--   0 eric      (1000) users      (984)     2924 2022-07-13 16:35:42.000000 babelplot-2022.9/babelplot/test/test_backends.py
+-rw-r--r--   0 eric      (1000) users      (984)     3278 2022-07-13 17:21:55.000000 babelplot-2022.9/babelplot/test/test_matplotlib.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.901756 babelplot-2022.9/babelplot/type/
+-rw-r--r--   0 eric      (1000) users      (984)     4371 2022-07-11 09:03:25.000000 babelplot-2022.9/babelplot/type/base.py
+-rw-r--r--   0 eric      (1000) users      (984)     3110 2022-04-20 15:21:18.000000 babelplot-2022.9/babelplot/type/dimension.py
+-rw-r--r--   0 eric      (1000) users      (984)     8289 2022-07-13 17:08:28.000000 babelplot-2022.9/babelplot/type/figure.py
+-rw-r--r--   0 eric      (1000) users      (984)     4814 2022-07-12 12:11:09.000000 babelplot-2022.9/babelplot/type/frame.py
+-rw-r--r--   0 eric      (1000) users      (984)     3722 2022-04-21 14:07:23.000000 babelplot-2022.9/babelplot/type/plot.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2022-11-29 10:11:10.898423 babelplot-2022.9/babelplot.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     2601 2022-11-29 10:11:10.000000 babelplot-2022.9/babelplot.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1010 2022-11-29 10:11:10.000000 babelplot-2022.9/babelplot.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2022-11-29 10:11:10.000000 babelplot-2022.9/babelplot.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       27 2022-11-29 10:11:10.000000 babelplot-2022.9/babelplot.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2022-11-29 10:11:10.000000 babelplot-2022.9/babelplot.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-04-04 12:16:02.000000 babelplot-2022.9/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2022-11-29 10:11:10.901756 babelplot-2022.9/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     4465 2022-11-29 10:01:30.000000 babelplot-2022.9/setup.py
```

### Comparing `babelplot-2022.8/PKG-INFO` & `babelplot-2022.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babelplot
-Version: 2022.8
+Version: 2022.9
 Summary: A Meta Plotting Library That Speaks Several Backends
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/babelplot
 Author: Eric Debreuve
 Author-email: eric.debreuve@univ-cotedazur.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/babelplot/-/wikis/HOME
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/babelplot
```

### Comparing `babelplot-2022.8/README-COPYRIGHT-utf8.txt` & `babelplot-2022.9/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/README-LICENCE-utf8.txt` & `babelplot-2022.9/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/README.rst` & `babelplot-2022.9/README.rst`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/__init__.py` & `babelplot-2022.9/babelplot/__init__.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/bokeh_.py` & `babelplot-2022.9/babelplot/backend/bokeh_.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/brick/html.py` & `babelplot-2022.9/babelplot/backend/brick/html.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/gr_.py` & `babelplot-2022.9/babelplot/backend/gr_.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/helper/creation.py` & `babelplot-2022.9/babelplot/backend/helper/creation.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/helper/validation.py` & `babelplot-2022.9/babelplot/backend/helper/validation.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/matplotlib_.py` & `babelplot-2022.9/babelplot/backend/matplotlib_.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/plotly_.py` & `babelplot-2022.9/babelplot/backend/plotly_.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,18 +76,18 @@
 def _NewFrame(*_, **__) -> backend_frame_h:
     """"""
     return None
 
 
 def _AdjustLayout(figure: figure_t, /) -> None:
     """"""
+    title_postfix = ""
+
     n_rows, n_cols = figure.shape
     if (n_rows > 1) or (n_cols > 1):
-        title_postfix = ""
-
         frame_titles = (n_rows * n_cols) * [""]
         arranged_plots = [n_cols * [None] for _ in range(n_rows)]
         for frame, (row, col) in zip(figure.frames, figure.locations):
             if frame.title is not None:
                 frame_titles[row * n_cols + col] = frame.title
             for plot in frame.plots:
                 if plot.title is not None:
```

### Comparing `babelplot-2022.8/babelplot/backend/runtime.py` & `babelplot-2022.9/babelplot/backend/runtime.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/specification/implemented.py` & `babelplot-2022.9/babelplot/backend/specification/implemented.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/specification/plot.py` & `babelplot-2022.9/babelplot/backend/specification/plot.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/backend/vedo_.py` & `babelplot-2022.9/babelplot/backend/vedo_.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/brick/enum.py` & `babelplot-2022.9/babelplot/brick/enum.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/brick/log.py` & `babelplot-2022.9/babelplot/brick/log.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/documentation/gallery-matplotlib.py` & `babelplot-2022.9/babelplot/documentation/gallery-matplotlib.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/documentation/gallery-plotly.py` & `babelplot-2022.9/babelplot/documentation/gallery-plotly.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/figure.py` & `babelplot-2022.9/babelplot/figure.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/help.py` & `babelplot-2022.9/babelplot/help.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/test/test_backends.py` & `babelplot-2022.9/babelplot/test/test_backends.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/test/test_matplotlib.py` & `babelplot-2022.9/babelplot/test/test_matplotlib.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/type/base.py` & `babelplot-2022.9/babelplot/type/base.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/type/dimension.py` & `babelplot-2022.9/babelplot/type/dimension.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/type/figure.py` & `babelplot-2022.9/babelplot/type/figure.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/type/frame.py` & `babelplot-2022.9/babelplot/type/frame.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot/type/plot.py` & `babelplot-2022.9/babelplot/type/plot.py`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/babelplot.egg-info/PKG-INFO` & `babelplot-2022.9/babelplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babelplot
-Version: 2022.8
+Version: 2022.9
 Summary: A Meta Plotting Library That Speaks Several Backends
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/babelplot
 Author: Eric Debreuve
 Author-email: eric.debreuve@univ-cotedazur.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/babelplot/-/wikis/HOME
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/babelplot
```

### Comparing `babelplot-2022.8/babelplot.egg-info/SOURCES.txt` & `babelplot-2022.9/babelplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `babelplot-2022.8/setup.py` & `babelplot-2022.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 PYPI_NAME = "babelplot"
 DESCRIPTION = "A Meta Plotting Library That Speaks Several Backends"
 KEYWORDS = "plot, library"
 TOPIC = "Scientific/Engineering"
 SUBTOPIC = "Visualization"
 AUDIENCE = "Science/Research"
 LICENSE = "CeCILL-2.1"
-VERSION = (2022, 8)  # /!\ str(2021.10) -> "2021.1"
+VERSION = (2022, 9)  # /!\ str(2021.10) -> "2021.1"
 STATUS = "3 - Alpha"
 PY_VERSION = "3.10"
 
 REPOSITORY_NAME = "babelplot"
 REPOSITORY_USER = "eric.debreuve"
 REPOSITORY_SITE = "src.koda.cnrs.fr"
 DOCUMENTATION_SITE = "-/wikis/HOME"
@@ -75,15 +75,15 @@
 version = f"{VERSION[0]}.{VERSION[1]}"
 
 folders = [IMPORT_NAME]
 excluded_folders = (f"{IMPORT_NAME}.documentation.api", f"{IMPORT_NAME}.documentation.wiki")
 for node in (HERE / IMPORT_NAME).rglob("*"):
     if node.is_dir() and not str(node).startswith("."):
         node = node.relative_to(HERE)
-        node = str(node).replace("/", ".")
+        node = ".".join(node.parts)
         if not (
             (node in excluded_folders)
             or any(node.startswith(_fld + ".") for _fld in excluded_folders)
         ):
             folders.append(node)
 folders = sorted(folders)
 if PACKAGES != folders:
```

