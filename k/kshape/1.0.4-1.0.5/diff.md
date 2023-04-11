# Comparing `tmp/kshape-1.0.4.tar.gz` & `tmp/kshape-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kshape-1.0.4.tar", last modified: Wed Jan 18 00:08:50 2023, max compression
+gzip compressed data, was "dist/kshape-1.0.5.tar", last modified: Tue Apr 11 22:01:34 2023, max compression
```

## Comparing `kshape-1.0.4.tar` & `kshape-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 bogireddyteja  (1009) bogireddyteja  (1013)        0 2023-01-18 00:08:50.000000 kshape-1.0.4/
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)     1070 2023-01-18 00:03:51.000000 kshape-1.0.4/LICENSE
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)      824 2023-01-18 00:08:50.000000 kshape-1.0.4/PKG-INFO
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)    20378 2023-01-18 00:03:51.000000 kshape-1.0.4/README.md
-drwxrwxr-x   0 bogireddyteja  (1009) bogireddyteja  (1013)        0 2023-01-18 00:08:50.000000 kshape-1.0.4/kshape/
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)        0 2023-01-18 00:03:52.000000 kshape-1.0.4/kshape/__init__.py
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)     4346 2023-01-18 00:03:52.000000 kshape-1.0.4/kshape/core.py
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)     3874 2023-01-18 00:07:51.000000 kshape-1.0.4/kshape/core_gpu.py
-drwxrwxr-x   0 bogireddyteja  (1009) bogireddyteja  (1013)        0 2023-01-18 00:08:50.000000 kshape-1.0.4/kshape.egg-info/
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)      824 2023-01-18 00:08:50.000000 kshape-1.0.4/kshape.egg-info/PKG-INFO
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)      253 2023-01-18 00:08:50.000000 kshape-1.0.4/kshape.egg-info/SOURCES.txt
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)        1 2023-01-18 00:08:50.000000 kshape-1.0.4/kshape.egg-info/dependency_links.txt
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)        6 2023-01-18 00:08:50.000000 kshape-1.0.4/kshape.egg-info/requires.txt
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)        7 2023-01-18 00:08:50.000000 kshape-1.0.4/kshape.egg-info/top_level.txt
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)        1 2023-01-18 00:03:52.000000 kshape-1.0.4/kshape.egg-info/zip-safe
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)       38 2023-01-18 00:08:50.000000 kshape-1.0.4/setup.cfg
--rw-rw-r--   0 bogireddyteja  (1009) bogireddyteja  (1013)      960 2023-01-18 00:05:40.000000 kshape-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 22:01:34.000000 kshape-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-11 21:54:51.000000 kshape-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      813 2023-04-11 22:01:34.000000 kshape-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20370 2023-04-11 21:54:51.000000 kshape-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 22:01:34.000000 kshape-1.0.5/kshape/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 21:54:53.000000 kshape-1.0.5/kshape/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4627 2023-04-11 21:54:53.000000 kshape-1.0.5/kshape/core.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-04-11 21:54:53.000000 kshape-1.0.5/kshape/core_gpu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 22:01:34.000000 kshape-1.0.5/kshape.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      813 2023-04-11 22:01:34.000000 kshape-1.0.5/kshape.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-11 22:01:34.000000 kshape-1.0.5/kshape.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 22:01:34.000000 kshape-1.0.5/kshape.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 22:01:34.000000 kshape-1.0.5/kshape.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-11 22:01:34.000000 kshape-1.0.5/kshape.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 21:54:53.000000 kshape-1.0.5/kshape.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 22:01:34.000000 kshape-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-11 21:55:32.000000 kshape-1.0.5/setup.py
```

### Comparing `kshape-1.0.4/LICENSE` & `kshape-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kshape-1.0.4/PKG-INFO` & `kshape-1.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: kshape
-Version: 1.0.4
+Version: 1.0.5
 Summary: k-Shape
 Home-page: https://github.com/TheDatumOrg/kshape-python
 Author: Teja
 Author-email: tejabogireddy19@gmail.com
 License: UNKNOWN
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `kshape-1.0.4/README.md` & `kshape-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 <div align="center">
 <p>
 <img alt="PyPI - Downloads" src="https://pepy.tech/badge/kshape"> <img alt="GitHub" src="https://img.shields.io/github/license/TheDatumOrg/kshape-python"> <img alt="PyPI" src="https://img.shields.io/pypi/v/kshape"> <img alt="GitHub issues" src="https://img.shields.io/github/issues/TheDatumOrg/kshape-python"> <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/kshape">
 </p>
 </div>
 
-*k*-Shape is a highly accurate and efficient unsupervised method for univariate and multivariate time-series clustering. *k*-Shape appeared at the ***ACM SIGMOD 2015*** conference, where it was selected as one of the (2) ***best papers*** and received the inaugural ***2015 ACM SIGMOD Research Highlight Award***. An extended version appeared in the ***ACM TODS 2017*** journal. Since then, *k*-Shape has achieved state-of-the-art performance in both ***univariate*** and ***multivariate*** time-series datasets (i.e., *k*-Shape is among the fastest and most accurate time-series clustering methods, ranked in the top positions of established benchmarks with 100+ different datasets). 
+*k*-Shape is a highly accurate and efficient unsupervised method for ***univariate*** and ***multivariate*** time-series clustering. *k*-Shape appeared at the ***ACM SIGMOD 2015*** conference, where it was selected as one of the (2) ***best papers*** and received the inaugural ***2015 ACM SIGMOD Research Highlight Award***. An extended version appeared in the ***ACM TODS 2017*** journal. Since then, *k*-Shape has achieved state-of-the-art performance in both ***univariate*** and ***multivariate*** time-series datasets (i.e., *k*-Shape is among the fastest and most accurate time-series clustering methods, ranked in the top positions of established benchmarks with 100+ datasets). 
 
-*k*-Shape has been widely adopted across different scientific areas (e.g., computer science, social science, space science, engineering, econometrics, biology, neuroscience, and medicine), Fortune 100-500 enterprises (e.g., Exelon, Nokia, and many financial firms), and organizations such as the European Space Agency.
+*k*-Shape has been widely adopted across scientific areas (e.g., computer science, social science, space science, engineering, econometrics, biology, neuroscience, and medicine), Fortune 100-500 enterprises (e.g., Exelon, Nokia, and many financial firms), and organizations such as the European Space Agency.
 
 If you use *k*-Shape in your project or research, cite the following two papers:
 
 * [ACM SIGMOD 2015](https://www.paparrizos.org/papers/PaparrizosSIGMOD15.pdf)
 * [ACM TODS 2017](https://www.paparrizos.org/papers/PaparrizosTODS17.pdf)
 
 ## References
```

### Comparing `kshape-1.0.4/kshape/core.py` & `kshape-1.0.5/kshape/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,17 @@
         if idx[i] == j:
             args.append([x[i], cur_center])
     _a = pool.map(collect_shift, args)
     pool.close()
 
     a = np.array(_a)
     if len(a) == 0:
-        return np.zeros((x.shape[1]))
+        indices = np.random.choice(x.shape[0], 1)
+        return np.squeeze(x[indices].copy())
+        #return np.zeros((x.shape[1]))
 
     columns = a.shape[1]
     y = zscore(a, axis=1, ddof=1)
 
     s = np.dot(y[:, :, 0].transpose(), y[:, :, 0])
     p = np.empty((columns, columns))
     p.fill(1.0/columns)
@@ -125,15 +127,17 @@
         centroids = x[indices].copy()
     distances = np.empty((m, k))
     
     for it in range(max_iter):
         old_idx = idx
 
         for j in range(k):
-            centroids[j] = np.expand_dims(_extract_shape(idx, x, j, centroids[j]), axis=1)
+            for d in range(x.shape[2]):
+                centroids[j, :, d] = _extract_shape(idx, np.expand_dims(x[:, :, d], axis=2), j, np.expand_dims(centroids[j, :, d], axis=1))
+                #centroids[j] = np.expand_dims(_extract_shape(idx, x, j, centroids[j]), axis=1)
 
         pool = multiprocessing.Pool()
         args = []
         for p in range(m):
             for q in range(k):
                 args.append([x[p, :], centroids[q, :]])
         result = pool.map(_ncc_c_3dim, args)
```

### Comparing `kshape-1.0.4/kshape/core_gpu.py` & `kshape-1.0.5/kshape/core_gpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,17 @@
             if torch.sum(cur_center)==0:
                 opt_x = x[i]
             else:
                 opt_x = _sbd(cur_center, x[i])
             _a.append(opt_x)
             
     if len(_a) == 0:
-        return torch.zeros((x.shape[1]))
+        indices = torch.randperm(x.shape[0])[:1]
+        return torch.squeeze(x[indices].clone())
+        #return torch.zeros((x.shape[1]))
 
     a = torch.stack(_a)
     
     columns = a.shape[1]
     y = zscore(a, axis=1, ddof=1)
     
     s = y[:, :, 0].transpose(0, 1).mm(y[:, :, 0])
@@ -93,15 +95,17 @@
         indices = torch.randperm(x.shape[0])[:k]
         centroids = x[indices].clone()
     distances = torch.empty(m, k, device="cuda")
 
     for it in range(max_iter):
         old_idx = idx
         for j in range(k):
-            centroids[j] = torch.unsqueeze(_extract_shape(idx, x, j, centroids[j]), dim=1)
+            for d in range(x.shape[2]):
+                centroids[j, :, d] = _extract_shape(idx, torch.unsqueeze(x[:, :, d], axis=2), j, torch.unsqueeze(centroids[j, :, d], axis=1))
+                #centroids[j] = torch.unsqueeze(_extract_shape(idx, x, j, centroids[j]), dim=1)
             
         for i, ts in enumerate(x):
             for c, ct in enumerate(centroids):
                 dist = 1 - _ncc_c_3dim(ts, ct).max()
                 distances[i, c] = dist
         
         idx = distances.argmin(1)
```

### Comparing `kshape-1.0.4/kshape.egg-info/PKG-INFO` & `kshape-1.0.5/kshape.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: kshape
-Version: 1.0.4
+Version: 1.0.5
 Summary: k-Shape
 Home-page: https://github.com/TheDatumOrg/kshape-python
 Author: Teja
 Author-email: tejabogireddy19@gmail.com
 License: UNKNOWN
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `kshape-1.0.4/setup.py` & `kshape-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
```

