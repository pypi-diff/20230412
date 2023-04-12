# Comparing `tmp/decorrelation-0.0.4.tar.gz` & `tmp/decorrelation-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decorrelation-0.0.4.tar", last modified: Mon Jan 16 06:06:38 2023, max compression
+gzip compressed data, was "decorrelation-0.1.0.tar", last modified: Wed Apr 12 21:43:20 2023, max compression
```

## Comparing `decorrelation-0.0.4.tar` & `decorrelation-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 06:06:38.610025 decorrelation-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    33253 2023-01-16 06:06:00.000000 decorrelation-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-16 06:06:00.000000 decorrelation-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-16 06:06:38.610025 decorrelation-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-01-16 06:06:00.000000 decorrelation-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 06:06:38.606025 decorrelation-0.0.4/decorrelation/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-16 06:06:00.000000 decorrelation-0.0.4/decorrelation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-16 06:06:00.000000 decorrelation-0.0.4/decorrelation/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-01-16 06:06:00.000000 decorrelation-0.0.4/decorrelation/co.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-16 06:06:00.000000 decorrelation-0.0.4/decorrelation/pl.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-16 06:06:00.000000 decorrelation-0.0.4/decorrelation/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-01-16 06:06:00.000000 decorrelation-0.0.4/decorrelation/shp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 06:06:38.610025 decorrelation-0.0.4/decorrelation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-16 06:06:38.000000 decorrelation-0.0.4/decorrelation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-16 06:06:38.000000 decorrelation-0.0.4/decorrelation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 06:06:38.000000 decorrelation-0.0.4/decorrelation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-16 06:06:38.000000 decorrelation-0.0.4/decorrelation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 06:06:37.000000 decorrelation-0.0.4/decorrelation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-16 06:06:38.000000 decorrelation-0.0.4/decorrelation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-16 06:06:38.000000 decorrelation-0.0.4/decorrelation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-16 06:06:00.000000 decorrelation-0.0.4/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 06:06:38.610025 decorrelation-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-01-16 06:06:00.000000 decorrelation-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:43:20.165218 decorrelation-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    33253 2023-04-12 21:42:51.000000 decorrelation-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 21:42:51.000000 decorrelation-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-12 21:43:20.165218 decorrelation-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-12 21:42:51.000000 decorrelation-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:43:20.165218 decorrelation-0.1.0/decorrelation/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/co.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/pl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-12 21:42:51.000000 decorrelation-0.1.0/decorrelation/shp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:43:20.165218 decorrelation-0.1.0/decorrelation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:43:19.000000 decorrelation-0.1.0/decorrelation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 21:43:20.000000 decorrelation-0.1.0/decorrelation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-12 21:42:51.000000 decorrelation-0.1.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 21:43:20.165218 decorrelation-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-12 21:42:51.000000 decorrelation-0.1.0/setup.py
```

### Comparing `decorrelation-0.0.4/LICENSE` & `decorrelation-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decorrelation-0.0.4/PKG-INFO` & `decorrelation-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorrelation
-Version: 0.0.4
+Version: 0.1.0
 Summary: An InSAR postprocessing tool
 Home-page: https://github.com/kanglcn/decorrelation
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,18 @@
 
 [Documentation](https://kanglcn.github.io/decorrelation)
 
 > InSAR postprocessing tool
 
 ## Install
 
+Install
+[CuPy](https://docs.cupy.dev/en/stable/install.html#installation) first,
+then:
+
 With conda:
 
 ``` bash
 conda install -c conda-forge decorrelation
 ```
 
 With pip:
@@ -57,14 +61,17 @@
 import decorrelation as dc
 ```
 
 Please refer to the
 [Documentation](https://kanglcn.github.io/decorrelation) for detailed
 usage.
 
+**Warning!!!** This package is under intensive development. API is
+subjected to change without any noticement.
+
 ## Contact us
 
 - Most discussion happens on
   [GitHub](https://github.com/kanglcn/decorrelation). Feel free to [open
   an issue](https://github.com/kanglcn/decorrelation/issues/new) or
   comment on any open issue or pull request.
 - use github
```

### Comparing `decorrelation-0.0.4/README.md` & `decorrelation-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 [Documentation](https://kanglcn.github.io/decorrelation)
 
 > InSAR postprocessing tool
 
 ## Install
 
+Install
+[CuPy](https://docs.cupy.dev/en/stable/install.html#installation) first,
+then:
+
 With conda:
 
 ``` bash
 conda install -c conda-forge decorrelation
 ```
 
 With pip:
@@ -35,14 +39,17 @@
 import decorrelation as dc
 ```
 
 Please refer to the
 [Documentation](https://kanglcn.github.io/decorrelation) for detailed
 usage.
 
+**Warning!!!** This package is under intensive development. API is
+subjected to change without any noticement.
+
 ## Contact us
 
 - Most discussion happens on
   [GitHub](https://github.com/kanglcn/decorrelation). Feel free to [open
   an issue](https://github.com/kanglcn/decorrelation/issues/new) or
   comment on any open issue or pull request.
 - use github
```

### Comparing `decorrelation-0.0.4/decorrelation/_modidx.py` & `decorrelation-0.1.0/decorrelation/_modidx.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/decorrelation',
                 'doc_host': 'https://kanglcn.github.io',
                 'git_url': 'https://github.com/kanglcn/decorrelation',
                 'lib_path': 'decorrelation'},
   'syms': { 'decorrelation.co': { 'decorrelation.co.emperical_co': ('API/co.html#emperical_co', 'decorrelation/co.py'),
                                   'decorrelation.co.emperical_co_sp': ('API/co.html#emperical_co_sp', 'decorrelation/co.py'),
+                                  'decorrelation.co.isPD': ('API/co.html#ispd', 'decorrelation/co.py'),
                                   'decorrelation.co.nearestPD': ('API/co.html#nearestpd', 'decorrelation/co.py'),
-                                  'decorrelation.co.regularize_spectral': ('API/co.html#regularize_spectral', 'decorrelation/co.py'),
-                                  'decorrelation.co.wherePD': ('API/co.html#wherepd', 'decorrelation/co.py')},
-            'decorrelation.pl': {'decorrelation.pl.emi': ('API/pl.html#emi', 'decorrelation/pl.py')},
+                                  'decorrelation.co.regularize_spectral': ('API/co.html#regularize_spectral', 'decorrelation/co.py')},
+            'decorrelation.pl': { 'decorrelation.pl.emi': ('API/pl.html#emi', 'decorrelation/pl.py'),
+                                  'decorrelation.pl.temp_coh': ('API/pl.html#temp_coh', 'decorrelation/pl.py')},
             'decorrelation.plot': {'decorrelation.plot.bg_alpha': ('API/plot.html#bg_alpha', 'decorrelation/plot.py')},
-            'decorrelation.shp': {'decorrelation.shp.ks_test': ('API/shp.html#ks_test', 'decorrelation/shp.py')}}}
+            'decorrelation.shp': {'decorrelation.shp.ks_test': ('API/shp.html#ks_test', 'decorrelation/shp.py')}}}
```

### Comparing `decorrelation-0.0.4/decorrelation/co.py` & `decorrelation-0.1.0/decorrelation/co.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/API/co.ipynb.
 
 # %% auto 0
-__all__ = ['emperical_co', 'emperical_co_sp', 'wherePD', 'nearestPD', 'regularize_spectral']
+__all__ = ['emperical_co', 'emperical_co_sp', 'isPD', 'nearestPD', 'regularize_spectral']
 
-# %% ../nbs/API/co.ipynb 5
+# %% ../nbs/API/co.ipynb 4
 import cupy as cp
 from typing import Union
 
-# %% ../nbs/API/co.ipynb 7
+# %% ../nbs/API/co.ipynb 6
 _emperical_co_kernel = cp.ElementwiseKernel(
     'raw T rslc, raw bool is_shp, int32 nlines, int32 width, int32 nimages, int32 az_half_win, int32 r_half_win',
     'raw T cov, raw T coh',
     '''
     if (i >= nlines*width) return;
     int az_win = 2*az_half_win+1;
     int r_win = 2*r_half_win+1;
@@ -59,15 +59,15 @@
             coh[(i*nimages+m)*nimages+j] = _cov/_amp2_m;
         }
     }
     ''',
     name = 'emperical_co_kernel',reduce_dims = False,no_return=True
 )
 
-# %% ../nbs/API/co.ipynb 8
+# %% ../nbs/API/co.ipynb 7
 def emperical_co(rslc:cp.ndarray, # rslc stack, dtype: `cupy.complexfloating`
                  is_shp:cp.ndarray, # shp bool, dtype: `cupy.bool`
                  block_size:int=128, # the CUDA block size, it only affects the calculation speed
                 )-> tuple[cp.ndarray,cp.ndarray]: # the covariance and coherence matrix `cov` and `coh`
     '''
     Maximum likelihood covariance estimator.
     '''
@@ -79,27 +79,27 @@
     cov = cp.empty((nlines,width,nimages,nimages),dtype=rslc.dtype)
     coh = cp.empty((nlines,width,nimages,nimages),dtype=rslc.dtype)
 
     _emperical_co_kernel(rslc, is_shp, cp.int32(nlines),cp.int32(width),cp.int32(nimages),
                     cp.int32(az_half_win),cp.int32(r_half_win),cov,coh,size = nlines*width,block_size=block_size)
     return cov,coh
 
-# %% ../nbs/API/co.ipynb 20
+# %% ../nbs/API/co.ipynb 16
 # I is int32* or int64*
 _emperical_co_sp_kernel = cp.ElementwiseKernel(
-    'raw T rslc, raw I sp_idx, raw bool is_shp_sp, int32 nlines, int32 width, int32 nimages, int32 az_half_win, int32 r_half_win, int32 num_sp',
+    'raw T rslc, raw I az_idx, raw I r_idx, raw bool is_shp_sp, int32 nlines, int32 width, int32 nimages, int32 az_half_win, int32 r_half_win, int32 num_sp',
     'raw T cov, raw T coh',
     '''
     if (i >= num_sp) return;
     int az_win = 2*az_half_win+1;
     int r_win = 2*r_half_win+1;
     int win = az_win*r_win;
     
-    int ref_az = sp_idx[i*2];
-    int ref_r = sp_idx[i*2+1];
+    int ref_az = az_idx[i];
+    int ref_r = r_idx[i];
 
     int sec_az, sec_r;
 
     int m,j; // index of each coherence matrix
     int k,l; // index of search window
     T _cov; // covariance
     float _amp2_m; // sum of amplitude square for image i
@@ -136,44 +136,46 @@
             coh[(i*nimages+m)*nimages+j] = _cov/_amp2_m;
         }
     }
     ''',
     name = 'emperical_co_sp_kernel',reduce_dims = False,no_return=True
 )
 
-# %% ../nbs/API/co.ipynb 21
+# %% ../nbs/API/co.ipynb 17
 def emperical_co_sp(rslc:cp.ndarray, # rslc stack, dtype: `cupy.complexfloating`
-                    sp_idx:cp.ndarray, # index of sparse data, dtype: `cupy.int`, shape: [n_sp,2]
+                    sp_idx:cp.ndarray, # index of sparse data [azimuth_index, range_index], dtype: `cupy.int`, shape: (n_sp,2)
                     is_shp_sp:cp.ndarray, # shp bool, dtype: `cupy.bool`
                     block_size:int=128, # the CUDA block size, it only affects the calculation speed
                    )-> tuple[cp.ndarray,cp.ndarray]: # the covariance and coherence matrix `cov` and `coh`
     '''
     Maximum likelihood covariance estimator for sparse data.
     '''
     nlines, width, nimages = rslc.shape
     az_win, r_win = is_shp_sp.shape[-2:]
     az_half_win = (az_win-1)//2
     r_half_win = (r_win-1)//2
-    num_sp = sp_idx.shape[0]
+    az_idx = sp_idx[0]; r_idx = sp_idx[1]
+    num_sp = az_idx.shape[0]
+
     
     cov = cp.empty((num_sp,nimages,nimages),dtype=rslc.dtype)
     coh = cp.empty((num_sp,nimages,nimages),dtype=rslc.dtype)
 
-    _emperical_co_sp_kernel(rslc, sp_idx, is_shp_sp, cp.int32(nlines),cp.int32(width),cp.int32(nimages),
+    _emperical_co_sp_kernel(rslc, az_idx, r_idx, is_shp_sp, cp.int32(nlines),cp.int32(width),cp.int32(nimages),
                     cp.int32(az_half_win),cp.int32(r_half_win),cp.int32(num_sp),cov,coh,size = num_sp,block_size=block_size)
     return cov,coh
 
-# %% ../nbs/API/co.ipynb 28
-def wherePD(co:cp.ndarray, # absolute value of complex coherence/covariance stack
+# %% ../nbs/API/co.ipynb 25
+def isPD(co:cp.ndarray, # absolute value of complex coherence/covariance stack
          )-> cp.ndarray: # bool array indicating wheather coherence/covariance is positive define
     L = cp.linalg.cholesky(co)
-    isPD = cp.isfinite(L).all(axis=(-2,-1))
-    return isPD
+    is_PD = cp.isfinite(L).all(axis=(-2,-1))
+    return is_PD
 
-# %% ../nbs/API/co.ipynb 29
+# %% ../nbs/API/co.ipynb 32
 '''
     The method is presented in [1]. John D'Errico implented it in MATLAB [2] under BSD
     Licence and [3] implented it with Python/Numpy based on [2] also under BSD Licence.
     This is a cupy implentation with stack of matrix supported.
 
     [1] N.J. Higham, "Computing a nearest symmetric positive semidefinite
     matrix" (1988): https://doi.org/10.1016/0024-3795(88)90223-6
```

### Comparing `decorrelation-0.0.4/decorrelation/shp.py` & `decorrelation-0.1.0/decorrelation/shp.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,27 +69,28 @@
             p2 = p;
         }
         return p;
     }
     ''',)
 
 # %% ../nbs/API/shp.ipynb 7
-def ks_test(rmli_stack:cp.ndarray, # the rmli stack, dtype: cupy.floating
+def ks_test(rmli:cp.ndarray, # the rmli stack, dtype: cupy.floating
             az_half_win:int, # SHP identification half search window size in azimuth direction
             r_half_win:int, # SHP identification half search window size in range direction
             block_size:int=128, # the CUDA block size, it only affects the calculation speed
-           ) -> tuple : # the KS test statistics `dist` and p value `p`
+           ) -> tuple[cp.ndarray,cp.ndarray] : # the KS test statistics `dist` and p value `p`
     '''
-    SHP identification based on Two-Sample Kolmogorov-Smirnov Test
+    SHP identification based on Two-Sample Kolmogorov-Smirnov Test.
     '''
+    sorted_rmli = cp.sort(rmli,axis=-1) # In fact, this step is most time consuming, consider move it out
     az_win = 2*az_half_win+1
     r_win = 2*r_half_win+1
-    nlines = rmli_stack.shape[0]
-    width = rmli_stack.shape[1]
-    nimages = rmli_stack.shape[-1]
-    dist = cp.empty((nlines,width,az_win,r_win),dtype=rmli_stack.dtype)
-    p = cp.empty((nlines,width,az_win,r_win),dtype=rmli_stack.dtype)
+    nlines = rmli.shape[0]
+    width = rmli.shape[1]
+    nimages = rmli.shape[-1]
+    dist = cp.empty((nlines,width,az_win,r_win),dtype=rmli.dtype)
+    p = cp.empty((nlines,width,az_win,r_win),dtype=rmli.dtype)
 
-    _ks_test_kernel(rmli_stack,cp.int32(nlines),cp.int32(width),cp.int32(nimages),
+    _ks_test_kernel(sorted_rmli,cp.int32(nlines),cp.int32(width),cp.int32(nimages),
                     cp.int32(az_half_win),cp.int32(r_half_win),dist,p,
                     size=width*nlines*r_win*az_win,block_size=block_size)
     return dist,p
```

### Comparing `decorrelation-0.0.4/decorrelation.egg-info/PKG-INFO` & `decorrelation-0.1.0/decorrelation.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decorrelation
-Version: 0.0.4
+Version: 0.1.0
 Summary: An InSAR postprocessing tool
 Home-page: https://github.com/kanglcn/decorrelation
 Author: kanglcn
 Author-email: kanglcn@gmail.com
 License: GNU General Public License v3.0 only
 Keywords: InSAR PS DS CUDA
 Classifier: Development Status :: 4 - Beta
@@ -27,14 +27,18 @@
 
 [Documentation](https://kanglcn.github.io/decorrelation)
 
 > InSAR postprocessing tool
 
 ## Install
 
+Install
+[CuPy](https://docs.cupy.dev/en/stable/install.html#installation) first,
+then:
+
 With conda:
 
 ``` bash
 conda install -c conda-forge decorrelation
 ```
 
 With pip:
@@ -57,14 +61,17 @@
 import decorrelation as dc
 ```
 
 Please refer to the
 [Documentation](https://kanglcn.github.io/decorrelation) for detailed
 usage.
 
+**Warning!!!** This package is under intensive development. API is
+subjected to change without any noticement.
+
 ## Contact us
 
 - Most discussion happens on
   [GitHub](https://github.com/kanglcn/decorrelation). Feel free to [open
   an issue](https://github.com/kanglcn/decorrelation/issues/new) or
   comment on any open issue or pull request.
 - use github
```

### Comparing `decorrelation-0.0.4/settings.ini` & `decorrelation-0.1.0/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = decorrelation
 lib_name = decorrelation
-version = 0.0.4
+version = 0.1.0
 min_python = 3.7
 license = gpl3
 doc_path = docs
 lib_path = decorrelation
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -21,18 +21,19 @@
 author_email = kanglcn@gmail.com
 copyright = 2022 onwards, kanglcn
 description = An InSAR postprocessing tool
 keywords = InSAR PS DS CUDA
 language = English
 status = 3
 user = kanglcn
-requirements = numpy scipy matplotlib
+requirements = numpy scipy matplotlib zarr dask colorcet
 dev_requirements = nbdev pre-commit
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 label_groups = {"feature":"New Features", "enhancement":"Features improved", "breaking": "Breaking Changes", "bug":"Bugs Squashed", "documentation":"Improvements to documentation", "deprecation":"Features deprecation", "packaging":"(For Developer) Packaging"}
+custom_quarto_yml = True
```

### Comparing `decorrelation-0.0.4/setup.py` & `decorrelation-0.1.0/setup.py`

 * *Files identical despite different names*

