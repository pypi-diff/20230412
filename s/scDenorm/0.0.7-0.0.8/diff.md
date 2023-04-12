# Comparing `tmp/scDenorm-0.0.7.tar.gz` & `tmp/scDenorm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scDenorm-0.0.7.tar", last modified: Thu Mar 23 06:17:29 2023, max compression
+gzip compressed data, was "scDenorm-0.0.8.tar", last modified: Wed Apr 12 11:26:57 2023, max compression
```

## Comparing `scDenorm-0.0.7.tar` & `scDenorm-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-03-23 06:17:29.000000 scDenorm-0.0.7/
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)    11357 2022-12-27 07:09:08.000000 scDenorm-0.0.7/LICENSE
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)      111 2022-09-05 16:31:43.000000 scDenorm-0.0.7/MANIFEST.in
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     3800 2023-03-23 06:17:29.000000 scDenorm-0.0.7/PKG-INFO
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     2975 2023-02-10 02:07:53.000000 scDenorm-0.0.7/README.md
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-03-23 06:17:28.000000 scDenorm-0.0.7/scDenorm/
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-03-23 03:38:52.000000 scDenorm-0.0.7/scDenorm/__init__.py
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1124 2023-03-23 03:38:52.000000 scDenorm-0.0.7/scDenorm/_modidx.py
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     6334 2023-03-23 03:38:52.000000 scDenorm-0.0.7/scDenorm/denorm.py
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-03-23 06:17:29.000000 scDenorm-0.0.7/scDenorm.egg-info/
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     3800 2023-03-23 06:17:25.000000 scDenorm-0.0.7/scDenorm.egg-info/PKG-INFO
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      336 2023-03-23 06:17:27.000000 scDenorm-0.0.7/scDenorm.egg-info/SOURCES.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-03-23 06:17:25.000000 scDenorm-0.0.7/scDenorm.egg-info/dependency_links.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       93 2023-03-23 06:17:25.000000 scDenorm-0.0.7/scDenorm.egg-info/entry_points.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2022-12-27 08:36:38.000000 scDenorm-0.0.7/scDenorm.egg-info/not-zip-safe
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       74 2023-03-23 06:17:25.000000 scDenorm-0.0.7/scDenorm.egg-info/requires.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        9 2023-03-23 06:17:25.000000 scDenorm-0.0.7/scDenorm.egg-info/top_level.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1044 2023-03-23 06:15:35.000000 scDenorm-0.0.7/settings.ini
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       38 2023-03-23 06:17:29.000000 scDenorm-0.0.7/setup.cfg
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)     2541 2022-09-05 16:31:43.000000 scDenorm-0.0.7/setup.py
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-04-12 11:26:57.000000 scDenorm-0.0.8/
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)    11357 2022-12-27 07:09:08.000000 scDenorm-0.0.8/LICENSE
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)      111 2022-09-05 16:31:43.000000 scDenorm-0.0.8/MANIFEST.in
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     3800 2023-04-12 11:26:57.000000 scDenorm-0.0.8/PKG-INFO
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     2975 2023-02-10 02:07:53.000000 scDenorm-0.0.8/README.md
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-04-12 11:26:57.000000 scDenorm-0.0.8/scDenorm/
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-04-12 11:24:01.000000 scDenorm-0.0.8/scDenorm/__init__.py
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1125 2023-04-12 11:24:01.000000 scDenorm-0.0.8/scDenorm/_modidx.py
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     6334 2023-04-12 11:24:01.000000 scDenorm-0.0.8/scDenorm/denorm.py
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-04-12 11:26:57.000000 scDenorm-0.0.8/scDenorm.egg-info/
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     3800 2023-04-12 11:26:54.000000 scDenorm-0.0.8/scDenorm.egg-info/PKG-INFO
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      336 2023-04-12 11:26:56.000000 scDenorm-0.0.8/scDenorm.egg-info/SOURCES.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-04-12 11:26:54.000000 scDenorm-0.0.8/scDenorm.egg-info/dependency_links.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       93 2023-04-12 11:26:54.000000 scDenorm-0.0.8/scDenorm.egg-info/entry_points.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2022-12-27 08:36:38.000000 scDenorm-0.0.8/scDenorm.egg-info/not-zip-safe
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       74 2023-04-12 11:26:54.000000 scDenorm-0.0.8/scDenorm.egg-info/requires.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        9 2023-04-12 11:26:54.000000 scDenorm-0.0.8/scDenorm.egg-info/top_level.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1044 2023-04-12 11:25:03.000000 scDenorm-0.0.8/settings.ini
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       38 2023-04-12 11:26:57.000000 scDenorm-0.0.8/setup.cfg
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)     2541 2022-09-05 16:31:43.000000 scDenorm-0.0.8/setup.py
```

### Comparing `scDenorm-0.0.7/LICENSE` & `scDenorm-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scDenorm-0.0.7/PKG-INFO` & `scDenorm-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scDenorm
-Version: 0.0.7
+Version: 0.0.8
 Summary: scDenorm: a denormalization tool for single-cell transcriptomics data
 Home-page: https://github.com/changebio/scDenorm
 Author: Yin Huang
 Author-email: changebio@yeah.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `scDenorm-0.0.7/README.md` & `scDenorm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scDenorm-0.0.7/scDenorm/_modidx.py` & `scDenorm-0.0.8/scDenorm/_modidx.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
                 'lib_path': 'scDenorm'},
   'syms': { 'scDenorm.denorm': { 'scDenorm.denorm.check_plot': ('scdenorm.html#check_plot', 'scDenorm/denorm.py'),
                                  'scDenorm.denorm.check_unscale': ('scdenorm.html#check_unscale', 'scDenorm/denorm.py'),
                                  'scDenorm.denorm.get_scaling_factor': ('scdenorm.html#get_scaling_factor', 'scDenorm/denorm.py'),
                                  'scDenorm.denorm.get_scaling_factor_1': ('scdenorm.html#get_scaling_factor_1', 'scDenorm/denorm.py'),
                                  'scDenorm.denorm.scdenorm': ('scdenorm.html#scdenorm', 'scDenorm/denorm.py'),
                                  'scDenorm.denorm.select_base': ('scdenorm.html#select_base', 'scDenorm/denorm.py'),
-                                 'scDenorm.denorm.unscale_mat': ('scdenorm.html#unscale_mat', 'scDenorm/denorm.py')}}}
+                                 'scDenorm.denorm.unscale_mat': ('scdenorm.html#unscale_mat', 'scDenorm/denorm.py')}}}
```

### Comparing `scDenorm-0.0.7/scDenorm/denorm.py` & `scDenorm-0.0.8/scDenorm/denorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     scaling_factors = diags(scaling_factors)
     counts = scaling_factors*scaled_counts
     if rint:
         counts=counts.rint()
     return counts,success_cells
 
 def select_base(x,cont=1,cutoff=0.05,plot=False):
-    for b in [np.e,2,10,1]:
+    for b in [np.e,1,2,10]:
         if check_unscale(x,b,cont,cutoff,plot):
             break
     return b
 
 def check_unscale(x,base=np.e,cont=1,cutoff=0.05,plot=True):
     if base!=1:
         x=base**x-cont
```

### Comparing `scDenorm-0.0.7/scDenorm.egg-info/PKG-INFO` & `scDenorm-0.0.8/scDenorm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scDenorm
-Version: 0.0.7
+Version: 0.0.8
 Summary: scDenorm: a denormalization tool for single-cell transcriptomics data
 Home-page: https://github.com/changebio/scDenorm
 Author: Yin Huang
 Author-email: changebio@yeah.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `scDenorm-0.0.7/settings.ini` & `scDenorm-0.0.8/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = scDenorm
 lib_name = %(repo)s
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = scDenorm
 nbs_path = nbs
```

### Comparing `scDenorm-0.0.7/setup.py` & `scDenorm-0.0.8/setup.py`

 * *Files identical despite different names*

