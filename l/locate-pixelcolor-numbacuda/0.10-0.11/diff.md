# Comparing `tmp/locate_pixelcolor_numbacuda-0.10.tar.gz` & `tmp/locate_pixelcolor_numbacuda-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locate_pixelcolor_numbacuda-0.10.tar", last modified: Wed Apr 12 00:43:06 2023, max compression
+gzip compressed data, was "locate_pixelcolor_numbacuda-0.11.tar", last modified: Wed Apr 12 00:46:45 2023, max compression
```

## Comparing `locate_pixelcolor_numbacuda-0.10.tar` & `locate_pixelcolor_numbacuda-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 00:43:06.010454 locate_pixelcolor_numbacuda-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-12 00:43:03.000000 locate_pixelcolor_numbacuda-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      197 2023-04-12 00:43:03.000000 locate_pixelcolor_numbacuda-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     1737 2023-04-12 00:43:06.010454 locate_pixelcolor_numbacuda-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-04-12 00:41:56.000000 locate_pixelcolor_numbacuda-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 00:43:06.006462 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/LICENSE
--rw-rw-rw-   0        0        0     1036 2023-04-12 00:41:56.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/README.MD
--rw-rw-rw-   0        0        0     1880 2023-04-12 00:39:36.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/__init__.py
--rw-rw-rw-   0        0        0       12 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-12 00:43:06.009454 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda.egg-info/
--rw-rw-rw-   0        0        0     1737 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-04-12 00:43:06.011450 locate_pixelcolor_numbacuda-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-04-12 00:43:05.000000 locate_pixelcolor_numbacuda-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:46:45.172691 locate_pixelcolor_numbacuda-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-12 00:46:43.000000 locate_pixelcolor_numbacuda-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      197 2023-04-12 00:46:42.000000 locate_pixelcolor_numbacuda-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     1770 2023-04-12 00:46:45.172691 locate_pixelcolor_numbacuda-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2023-04-12 00:45:56.000000 locate_pixelcolor_numbacuda-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 00:46:45.168702 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/
+-rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/LICENSE
+-rw-rw-rw-   0        0        0     1066 2023-04-12 00:45:56.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/README.MD
+-rw-rw-rw-   0        0        0     1880 2023-04-12 00:39:36.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-04-12 00:46:44.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-04-12 00:46:44.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-12 00:46:45.172691 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/
+-rw-rw-rw-   0        0        0     1770 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 00:46:45.000000 locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-04-12 00:46:45.173689 locate_pixelcolor_numbacuda-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-04-12 00:46:44.000000 locate_pixelcolor_numbacuda-0.11/setup.py
```

### Comparing `locate_pixelcolor_numbacuda-0.10/LICENSE.rst` & `locate_pixelcolor_numbacuda-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numbacuda-0.10/PKG-INFO` & `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: locate_pixelcolor_numbacuda
-Version: 0.10
+Name: locate-pixelcolor-numbacuda
+Version: 0.11
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_numbacuda
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: numpy,numba,CUDA,rgb,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,22 +16,25 @@
 License-File: LICENSE.rst
 
 
 # RGB search with numba.cuda - 10 x faster than numpy 
 
 ### pip install locate-pixelcolor-numbacuda
 
+
+```python
 from locate_pixelcolor_numbacuda import search_colors
 from a_cv_imwrite_imread_plus import open_image_in_cv
 import numpy as np
 colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
-
+```
 
 #### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
 
+```python
 picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
 coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 print(coords)
 %timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 
 
 # [[[  19   14]
@@ -41,8 +44,8 @@
 #   [6613 4524]
 #   [6614 4524]
 #   [6615 4524]]]
 # 135 ms ± 3.5 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
 
 # More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
 
-
+```
```

### Comparing `locate_pixelcolor_numbacuda-0.10/README.md` & `locate_pixelcolor_numbacuda-0.11/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # RGB search with numba.cuda - 10 x faster than numpy 
 
 ### pip install locate-pixelcolor-numbacuda
 
+
+```python
 from locate_pixelcolor_numbacuda import search_colors
 from a_cv_imwrite_imread_plus import open_image_in_cv
 import numpy as np
 colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
-
+```
 
 #### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
 
+```python
 picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
 coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 print(coords)
 %timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 
 
 # [[[  19   14]
@@ -23,8 +26,8 @@
 #   [6613 4524]
 #   [6614 4524]
 #   [6615 4524]]]
 # 135 ms ± 3.5 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
 
 # More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
 
-
+```
```

### Comparing `locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/LICENSE` & `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/LICENSE`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/README.MD` & `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/README.MD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # RGB search with numba.cuda - 10 x faster than numpy 
 
 ### pip install locate-pixelcolor-numbacuda
 
+
+```python
 from locate_pixelcolor_numbacuda import search_colors
 from a_cv_imwrite_imread_plus import open_image_in_cv
 import numpy as np
 colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
-
+```
 
 #### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
 
+```python
 picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
 coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 print(coords)
 %timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 
 
 # [[[  19   14]
@@ -23,8 +26,8 @@
 #   [6613 4524]
 #   [6614 4524]
 #   [6615 4524]]]
 # 135 ms ± 3.5 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
 
 # More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
 
-
+```
```

### Comparing `locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda/__init__.py` & `locate_pixelcolor_numbacuda-0.11/locate_pixelcolor_numbacuda/__init__.py`

 * *Files identical despite different names*

### Comparing `locate_pixelcolor_numbacuda-0.10/locate_pixelcolor_numbacuda.egg-info/PKG-INFO` & `locate_pixelcolor_numbacuda-0.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: locate-pixelcolor-numbacuda
-Version: 0.10
+Name: locate_pixelcolor_numbacuda
+Version: 0.11
 Home-page: https://github.com/hansalemaos/locate_pixelcolor_numbacuda
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: numpy,numba,CUDA,rgb,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -16,22 +16,25 @@
 License-File: LICENSE.rst
 
 
 # RGB search with numba.cuda - 10 x faster than numpy 
 
 ### pip install locate-pixelcolor-numbacuda
 
+
+```python
 from locate_pixelcolor_numbacuda import search_colors
 from a_cv_imwrite_imread_plus import open_image_in_cv
 import numpy as np
 colors=[(66,  71,  69),(62,  67,  65),(144, 155, 153),(52,  57,  55),(127, 138, 136),(53,  58,  56),(51,  56,  54),(32,  27,  18),(24,  17,   8),]
-
+```
 
 #### image'https://www.pexels.com/pt-br/foto/foto-da-raposa-sentada-no-chao-2295744/'
 
+```python
 picnp = open_image_in_cv('pexels-alex-andrews-2295744.jpg',channels_in_output=3)
 coords=search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 print(coords)
 %timeit search_colors(pic=picnp,colors=colors,threadsperblock=(18, 18,3),dtypetouse = np.int32)
 
 
 # [[[  19   14]
@@ -41,8 +44,8 @@
 #   [6613 4524]
 #   [6614 4524]
 #   [6615 4524]]]
 # 135 ms ± 3.5 ms per loop (mean ± std. dev. of 7 runs, 10 loops each)
 
 # More benchmarks: https://github.com/hansalemaos/locate_pixelcolor_cpp
 
-
+```
```

### Comparing `locate_pixelcolor_numbacuda-0.10/setup.py` & `locate_pixelcolor_numbacuda-0.11/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #change to dict
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.10'
+VERSION = '0.11'
 DESCRIPTION = "RGB search with numba.cuda - 10 x faster than numpy"
 
 # Setting up
 setup(
     name="locate_pixelcolor_numbacuda",
     version=VERSION,
     license='MIT',
```

