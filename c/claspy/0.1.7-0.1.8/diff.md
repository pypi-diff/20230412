# Comparing `tmp/claspy-0.1.7.tar.gz` & `tmp/claspy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claspy-0.1.7.tar", last modified: Wed Apr 12 08:02:33 2023, max compression
+gzip compressed data, was "claspy-0.1.8.tar", last modified: Wed Apr 12 08:51:24 2023, max compression
```

## Comparing `claspy-0.1.7.tar` & `claspy-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.903123 claspy-0.1.7/
--rw-r--r--   0 ermshaua   (501) staff       (20)     1500 2023-02-18 10:38:44.000000 claspy-0.1.7/LICENSE
--rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:02:33.903329 claspy-0.1.7/PKG-INFO
--rw-r--r--   0 ermshaua   (501) staff       (20)     4084 2023-03-29 19:08:59.000000 claspy-0.1.7/README.md
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.894555 claspy-0.1.7/claspy/
--rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-18 10:41:51.000000 claspy-0.1.7/claspy/__init__.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    16928 2023-04-11 17:01:12.000000 claspy-0.1.7/claspy/clasp.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     4495 2023-02-26 13:47:51.000000 claspy-0.1.7/claspy/data_loader.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6456 2023-03-05 16:43:36.000000 claspy-0.1.7/claspy/distance.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    15830 2023-04-12 07:38:40.000000 claspy-0.1.7/claspy/nearest_neighbour.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6099 2023-02-25 09:43:02.000000 claspy-0.1.7/claspy/scoring.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    14897 2023-04-12 07:43:17.000000 claspy-0.1.7/claspy/segmentation.py
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.902375 claspy-0.1.7/claspy/tests/
--rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-20 16:05:58.000000 claspy-0.1.7/claspy/tests/__init__.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2560 2023-04-12 07:27:07.000000 claspy-0.1.7/claspy/tests/clasp_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6600 2023-02-24 12:09:02.000000 claspy-0.1.7/claspy/tests/evaluation.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2569 2023-04-12 07:25:30.000000 claspy-0.1.7/claspy/tests/nearest_neighbour_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2937 2023-04-12 07:43:17.000000 claspy-0.1.7/claspy/tests/segmentation_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     1683 2023-02-28 15:56:43.000000 claspy-0.1.7/claspy/utils.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2918 2023-04-03 15:59:10.000000 claspy-0.1.7/claspy/validation.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6991 2023-02-28 19:59:17.000000 claspy-0.1.7/claspy/window_size.py
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:02:33.898413 claspy-0.1.7/claspy.egg-info/
--rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/PKG-INFO
--rw-r--r--   0 ermshaua   (501) staff       (20)      585 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/SOURCES.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/dependency_links.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/not-zip-safe
--rw-r--r--   0 ermshaua   (501) staff       (20)      137 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/requires.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        7 2023-04-12 08:02:33.000000 claspy-0.1.7/claspy.egg-info/top_level.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)     1560 2023-04-12 07:45:54.000000 claspy-0.1.7/pyproject.toml
--rw-r--r--   0 ermshaua   (501) staff       (20)       79 2023-04-12 08:02:33.904149 claspy-0.1.7/setup.cfg
--rw-r--r--   0 ermshaua   (501) staff       (20)     1376 2023-04-12 07:43:17.000000 claspy-0.1.7/setup.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.498036 claspy-0.1.8/
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1500 2023-02-18 10:38:44.000000 claspy-0.1.8/LICENSE
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:51:24.498260 claspy-0.1.8/PKG-INFO
+-rw-r--r--   0 ermshaua   (501) staff       (20)     4084 2023-03-29 19:08:59.000000 claspy-0.1.8/README.md
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.489254 claspy-0.1.8/claspy/
+-rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-18 10:41:51.000000 claspy-0.1.8/claspy/__init__.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    16924 2023-04-12 08:45:16.000000 claspy-0.1.8/claspy/clasp.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     4495 2023-02-26 13:47:51.000000 claspy-0.1.8/claspy/data_loader.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6456 2023-03-05 16:43:36.000000 claspy-0.1.8/claspy/distance.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    15830 2023-04-12 07:38:40.000000 claspy-0.1.8/claspy/nearest_neighbour.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6099 2023-02-25 09:43:02.000000 claspy-0.1.8/claspy/scoring.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    14897 2023-04-12 07:43:17.000000 claspy-0.1.8/claspy/segmentation.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.496604 claspy-0.1.8/claspy/tests/
+-rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-20 16:05:58.000000 claspy-0.1.8/claspy/tests/__init__.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2560 2023-04-12 07:27:07.000000 claspy-0.1.8/claspy/tests/clasp_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6600 2023-02-24 12:09:02.000000 claspy-0.1.8/claspy/tests/evaluation.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2569 2023-04-12 07:25:30.000000 claspy-0.1.8/claspy/tests/nearest_neighbour_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2937 2023-04-12 07:43:17.000000 claspy-0.1.8/claspy/tests/segmentation_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1683 2023-02-28 15:56:43.000000 claspy-0.1.8/claspy/utils.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2918 2023-04-03 15:59:10.000000 claspy-0.1.8/claspy/validation.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6991 2023-02-28 19:59:17.000000 claspy-0.1.8/claspy/window_size.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.492299 claspy-0.1.8/claspy.egg-info/
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/PKG-INFO
+-rw-r--r--   0 ermshaua   (501) staff       (20)      585 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/SOURCES.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/dependency_links.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/not-zip-safe
+-rw-r--r--   0 ermshaua   (501) staff       (20)      137 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/requires.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        7 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/top_level.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1560 2023-04-12 08:44:56.000000 claspy-0.1.8/pyproject.toml
+-rw-r--r--   0 ermshaua   (501) staff       (20)       79 2023-04-12 08:51:24.498849 claspy-0.1.8/setup.cfg
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1376 2023-04-12 07:43:17.000000 claspy-0.1.8/setup.py
```

### Comparing `claspy-0.1.7/LICENSE` & `claspy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/PKG-INFO` & `claspy-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claspy
-Version: 0.1.7
+Version: 0.1.8
 Home-page: https://github.com/ermshaua/claspy
 Author: Arik Ermshaus
 Author-email: Arik Ermshaus <ermshaua@informatik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Arik Ermshaus
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: claspy Version: 0.1.7 Home-page: https://
+Metadata-Version: 2.1 Name: claspy Version: 0.1.8 Home-page: https://
 github.com/ermshaua/claspy Author: Arik Ermshaus Author-email: Arik Ermshaus
 informatik.hu-berlin.de> License: BSD 3-Clause License Copyright (c) 2023, Arik
 Ermshaus Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `claspy-0.1.7/README.md` & `claspy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/clasp.py` & `claspy-0.1.8/claspy/clasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         while self.knn.offsets.shape[0] // n_jobs < self.min_seg_size and n_jobs != 1:
             n_jobs -= 1
 
         bin_size = self.knn.offsets.shape[0] // n_jobs
 
         for idx in range(n_jobs):
             start = max(idx * bin_size, self.min_seg_size)
-            end = min((idx + 1) * bin_size, self.knn.offsets.shape[0] - self.min_seg_size + self.window_size - 1)
+            end = min((idx + 1) * bin_size, self.knn.offsets.shape[0] - self.min_seg_size + self.window_size)
             if end > start: pranges.append((start, end))
 
         self.profile = _parallel_profile(self.knn.offsets, pranges, self.window_size, self.score)
 
         self.is_fitted = True
         return self
```

### Comparing `claspy-0.1.7/claspy/data_loader.py` & `claspy-0.1.8/claspy/data_loader.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/distance.py` & `claspy-0.1.8/claspy/distance.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/nearest_neighbour.py` & `claspy-0.1.8/claspy/nearest_neighbour.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/scoring.py` & `claspy-0.1.8/claspy/scoring.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/segmentation.py` & `claspy-0.1.8/claspy/segmentation.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/tests/clasp_test.py` & `claspy-0.1.8/claspy/tests/clasp_test.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/tests/evaluation.py` & `claspy-0.1.8/claspy/tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/tests/nearest_neighbour_test.py` & `claspy-0.1.8/claspy/tests/nearest_neighbour_test.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/tests/segmentation_test.py` & `claspy-0.1.8/claspy/tests/segmentation_test.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/utils.py` & `claspy-0.1.8/claspy/utils.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/validation.py` & `claspy-0.1.8/claspy/validation.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy/window_size.py` & `claspy-0.1.8/claspy/window_size.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/claspy.egg-info/PKG-INFO` & `claspy-0.1.8/claspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claspy
-Version: 0.1.7
+Version: 0.1.8
 Home-page: https://github.com/ermshaua/claspy
 Author: Arik Ermshaus
 Author-email: Arik Ermshaus <ermshaua@informatik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Arik Ermshaus
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: claspy Version: 0.1.7 Home-page: https://
+Metadata-Version: 2.1 Name: claspy Version: 0.1.8 Home-page: https://
 github.com/ermshaua/claspy Author: Arik Ermshaus Author-email: Arik Ermshaus
 informatik.hu-berlin.de> License: BSD 3-Clause License Copyright (c) 2023, Arik
 Ermshaus Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `claspy-0.1.7/claspy.egg-info/SOURCES.txt` & `claspy-0.1.8/claspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claspy-0.1.7/pyproject.toml` & `claspy-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "claspy"
 
-version = "0.1.7"
+version = "0.1.8"
 
 description = ""
 readme = "README.md"
 authors = [
     {name = "Arik Ermshaus", email = "ermshaua@informatik.hu-berlin.de"}
 ]
 keywords = [
```

### Comparing `claspy-0.1.7/setup.py` & `claspy-0.1.8/setup.py`

 * *Files identical despite different names*

