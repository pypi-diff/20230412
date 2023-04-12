# Comparing `tmp/domino-composite-0.261.tar.gz` & `tmp/domino-composite-0.262.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-composite-0.261.tar", last modified: Wed Apr 12 15:40:27 2023, max compression
+gzip compressed data, was "domino-composite-0.262.tar", last modified: Wed Apr 12 15:41:44 2023, max compression
```

## Comparing `domino-composite-0.261.tar` & `domino-composite-0.262.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:40:27.421901 domino-composite-0.261/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-04-12 15:40:27.421901 domino-composite-0.261/PKG-INFO
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:40:27.417901 domino-composite-0.261/domino/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.261/domino/__init__.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      444 2022-11-23 14:10:19.000000 domino-composite-0.261/domino/agg.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.261/domino/categorical_analysis.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50813 2023-03-31 15:44:13.000000 domino-composite-0.261/domino/core.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.261/domino/deseasonaliser.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3667 2023-03-31 11:02:48.000000 domino-composite-0.261/domino/filtering.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.261/domino/plsr.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    13677 2023-04-04 09:10:15.000000 domino-composite-0.261/domino/prediction.py
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5673 2023-04-12 15:38:45.000000 domino-composite-0.261/domino/util.py
-drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:40:27.421901 domino-composite-0.261/domino_composite.egg-info/
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-04-12 15:40:27.000000 domino-composite-0.261/domino_composite.egg-info/PKG-INFO
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-04-12 15:40:27.000000 domino-composite-0.261/domino_composite.egg-info/SOURCES.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-04-12 15:40:27.000000 domino-composite-0.261/domino_composite.egg-info/dependency_links.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-04-12 15:40:27.000000 domino-composite-0.261/domino_composite.egg-info/requires.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-04-12 15:40:27.000000 domino-composite-0.261/domino_composite.egg-info/top_level.txt
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-04-12 15:40:27.421901 domino-composite-0.261/setup.cfg
--rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-04-12 15:38:55.000000 domino-composite-0.261/setup.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:41:44.497071 domino-composite-0.262/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-04-12 15:41:44.497071 domino-composite-0.262/PKG-INFO
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:41:44.497071 domino-composite-0.262/domino/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2022-11-23 14:01:08.000000 domino-composite-0.262/domino/__init__.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      444 2022-11-23 14:10:19.000000 domino-composite-0.262/domino/agg.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     2702 2022-11-23 14:10:17.000000 domino-composite-0.262/domino/categorical_analysis.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    50813 2023-03-31 15:44:13.000000 domino-composite-0.262/domino/core.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4248 2023-01-30 10:05:05.000000 domino-composite-0.262/domino/deseasonaliser.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     3667 2023-03-31 11:02:48.000000 domino-composite-0.262/domino/filtering.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     4784 2023-04-03 16:12:11.000000 domino-composite-0.262/domino/plsr.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)    13677 2023-04-04 09:10:15.000000 domino-composite-0.262/domino/prediction.py
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     5671 2023-04-12 15:41:15.000000 domino-composite-0.262/domino/util.py
+drwxr-xr-x   0 ox5324   (243050) imk-tro  (44470)        0 2023-04-12 15:41:44.497071 domino-composite-0.262/domino_composite.egg-info/
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)     1213 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/PKG-INFO
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      382 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/SOURCES.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        1 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/dependency_links.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       62 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/requires.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)        7 2023-04-12 15:41:44.000000 domino-composite-0.262/domino_composite.egg-info/top_level.txt
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)       38 2023-04-12 15:41:44.497071 domino-composite-0.262/setup.cfg
+-rw-r--r--   0 ox5324   (243050) imk-tro  (44470)      728 2023-04-12 15:41:24.000000 domino-composite-0.262/setup.py
```

### Comparing `domino-composite-0.261/PKG-INFO` & `domino-composite-0.262/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.261
+Version: 0.262
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.261/domino/categorical_analysis.py` & `domino-composite-0.262/domino/categorical_analysis.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.261/domino/core.py` & `domino-composite-0.262/domino/core.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.261/domino/deseasonaliser.py` & `domino-composite-0.262/domino/deseasonaliser.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.261/domino/filtering.py` & `domino-composite-0.262/domino/filtering.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.261/domino/plsr.py` & `domino-composite-0.262/domino/plsr.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.261/domino/prediction.py` & `domino-composite-0.262/domino/prediction.py`

 * *Files identical despite different names*

### Comparing `domino-composite-0.261/domino/util.py` & `domino-composite-0.262/domino/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,12 +142,12 @@
     if infer_offset:
         offsets={v:indices[v].attrs[attr_kw] for v in indices.data_vars}
     
     da_arr=[]
     for v in indices.data_vars:
         da=indices[v]
         l=offsets[v]
-        if type(l)====np.int_:
+        if type(l)==np.int_:
             l=int(l) #datetime can't handle np.ints, no idea why not.
         da_arr.append(offset_time_dim(da,-l,offset_unit,offset_dim=dim))
     ds=xr.merge(da_arr)
     return ds
```

### Comparing `domino-composite-0.261/domino_composite.egg-info/PKG-INFO` & `domino-composite-0.262/domino_composite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-composite
-Version: 0.261
+Version: 0.262
 Summary: A package for compositing atmospheric datasets
 Home-page: https://github.com/joshdorrington/domino
 Author: Josh Dorrington
 Author-email: joshua.dorrington@kit.edu
 License: bsd-3-clause
 Description-Content-Type: text/markdown
```

### Comparing `domino-composite-0.261/setup.py` & `domino-composite-0.262/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("/data/ox5324/Domino/readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='domino-composite',
-    version='0.261',
+    version='0.262',
     author='Josh Dorrington',
     author_email='joshua.dorrington@kit.edu',
     description='A package for compositing atmospheric datasets',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/joshdorrington/domino',
     license='bsd-3-clause',
```

