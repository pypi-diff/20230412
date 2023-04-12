# Comparing `tmp/matej-libs-0.1.tar.gz` & `tmp/matej-libs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matej-libs-0.1.tar", last modified: Wed Apr 12 15:35:47 2023, max compression
+gzip compressed data, was "matej-libs-0.1.1.tar", last modified: Wed Apr 12 16:02:41 2023, max compression
```

## Comparing `matej-libs-0.1.tar` & `matej-libs-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:47.401325 matej-libs-0.1/
--rw-rw-rw-   0        0        0    35823 2023-02-15 23:50:40.000000 matej-libs-0.1/LICENSE
--rw-rw-rw-   0        0        0      400 2023-04-12 15:35:47.401325 matej-libs-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-12 15:32:19.000000 matej-libs-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:47.365325 matej-libs-0.1/matej/
--rw-rw-rw-   0        0        0     1525 2023-04-12 13:28:06.000000 matej-libs-0.1/matej/__init__.py
--rw-rw-rw-   0        0        0    17946 2023-04-06 16:38:42.000000 matej-libs-0.1/matej/argparse.py
--rw-rw-rw-   0        0        0      686 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/callable.py
--rw-rw-rw-   0        0        0     5145 2023-02-16 22:11:29.000000 matej-libs-0.1/matej/collections.py
--rw-rw-rw-   0        0        0     1184 2023-02-15 15:30:46.000000 matej-libs-0.1/matej/colour.py
--rw-rw-rw-   0        0        0    12591 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/config.py
--rw-rw-rw-   0        0        0     9100 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/enum.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:47.373327 matej-libs-0.1/matej/gui/
--rw-rw-rw-   0        0        0        0 2021-06-16 12:56:36.000000 matej-libs-0.1/matej/gui/__init__.py
--rw-rw-rw-   0        0        0    25450 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/gui/pyqt.py
--rw-rw-rw-   0        0        0      846 2021-06-16 12:56:36.000000 matej-libs-0.1/matej/gui/tkinter.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:47.383324 matej-libs-0.1/matej/math/
--rw-rw-rw-   0        0        0     3834 2023-02-15 15:30:46.000000 matej-libs-0.1/matej/math/__init__.py
--rw-rw-rw-   0        0        0    16358 2023-02-04 12:38:06.000000 matej-libs-0.1/matej/math/calculator.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:47.388326 matej-libs-0.1/matej/nn/
--rw-rw-rw-   0        0        0        0 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/nn/__init__.py
--rw-rw-rw-   0        0        0      501 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/nn/torch.py
--rw-rw-rw-   0        0        0     1204 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/parallel.py
--rw-rw-rw-   0        0        0     5289 2023-03-17 22:07:57.000000 matej-libs-0.1/matej/regedit.py
--rw-rw-rw-   0        0        0      648 2021-06-16 12:56:36.000000 matej-libs-0.1/matej/string.py
--rw-rw-rw-   0        0        0     1611 2023-04-12 13:24:32.000000 matej-libs-0.1/matej/web.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:35:47.400326 matej-libs-0.1/matej_libs.egg-info/
--rw-rw-rw-   0        0        0      400 2023-04-12 15:35:47.000000 matej-libs-0.1/matej_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-04-12 15:35:47.000000 matej-libs-0.1/matej_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:35:47.000000 matej-libs-0.1/matej_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-12 15:35:47.000000 matej-libs-0.1/matej_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 15:35:47.000000 matej-libs-0.1/matej_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-04-12 15:35:47.402325 matej-libs-0.1/setup.cfg
--rw-rw-rw-   0        0        0      545 2023-02-15 23:54:57.000000 matej-libs-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:02:41.127548 matej-libs-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-02-15 23:50:40.000000 matej-libs-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      620 2023-04-12 16:02:41.127548 matej-libs-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-12 15:32:19.000000 matej-libs-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 16:02:41.114548 matej-libs-0.1.1/matej/
+-rw-rw-rw-   0        0        0     1525 2023-04-12 13:28:06.000000 matej-libs-0.1.1/matej/__init__.py
+-rw-rw-rw-   0        0        0    17946 2023-04-06 16:38:42.000000 matej-libs-0.1.1/matej/argparse.py
+-rw-rw-rw-   0        0        0      686 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/callable.py
+-rw-rw-rw-   0        0        0     5145 2023-02-16 22:11:29.000000 matej-libs-0.1.1/matej/collections.py
+-rw-rw-rw-   0        0        0     1184 2023-02-15 15:30:46.000000 matej-libs-0.1.1/matej/colour.py
+-rw-rw-rw-   0        0        0    12591 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/config.py
+-rw-rw-rw-   0        0        0     9100 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/enum.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:02:41.116548 matej-libs-0.1.1/matej/gui/
+-rw-rw-rw-   0        0        0        0 2021-06-16 12:56:36.000000 matej-libs-0.1.1/matej/gui/__init__.py
+-rw-rw-rw-   0        0        0    25450 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/gui/pyqt.py
+-rw-rw-rw-   0        0        0      846 2021-06-16 12:56:36.000000 matej-libs-0.1.1/matej/gui/tkinter.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:02:41.117548 matej-libs-0.1.1/matej/math/
+-rw-rw-rw-   0        0        0     3834 2023-02-15 15:30:46.000000 matej-libs-0.1.1/matej/math/__init__.py
+-rw-rw-rw-   0        0        0    16358 2023-02-04 12:38:06.000000 matej-libs-0.1.1/matej/math/calculator.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:02:41.118548 matej-libs-0.1.1/matej/nn/
+-rw-rw-rw-   0        0        0        0 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/nn/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/nn/torch.py
+-rw-rw-rw-   0        0        0     1204 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/parallel.py
+-rw-rw-rw-   0        0        0     5289 2023-03-17 22:07:57.000000 matej-libs-0.1.1/matej/regedit.py
+-rw-rw-rw-   0        0        0      648 2021-06-16 12:56:36.000000 matej-libs-0.1.1/matej/string.py
+-rw-rw-rw-   0        0        0     1611 2023-04-12 13:24:32.000000 matej-libs-0.1.1/matej/web.py
+drwxrwxrwx   0        0        0        0 2023-04-12 16:02:41.127548 matej-libs-0.1.1/matej_libs.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-04-12 16:02:41.000000 matej-libs-0.1.1/matej_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2023-04-12 16:02:41.000000 matej-libs-0.1.1/matej_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 16:02:41.000000 matej-libs-0.1.1/matej_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-12 16:02:41.000000 matej-libs-0.1.1/matej_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 16:02:41.000000 matej-libs-0.1.1/matej_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-04-12 16:02:41.128548 matej-libs-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      565 2023-04-12 16:02:36.000000 matej-libs-0.1.1/setup.py
```

### Comparing `matej-libs-0.1/LICENSE` & `matej-libs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/__init__.py` & `matej-libs-0.1.1/matej/__init__.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/argparse.py` & `matej-libs-0.1.1/matej/argparse.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/callable.py` & `matej-libs-0.1.1/matej/callable.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/collections.py` & `matej-libs-0.1.1/matej/collections.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/colour.py` & `matej-libs-0.1.1/matej/colour.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/config.py` & `matej-libs-0.1.1/matej/config.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/enum.py` & `matej-libs-0.1.1/matej/enum.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/gui/pyqt.py` & `matej-libs-0.1.1/matej/gui/pyqt.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/gui/tkinter.py` & `matej-libs-0.1.1/matej/gui/tkinter.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/math/__init__.py` & `matej-libs-0.1.1/matej/math/__init__.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/math/calculator.py` & `matej-libs-0.1.1/matej/math/calculator.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/parallel.py` & `matej-libs-0.1.1/matej/parallel.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/regedit.py` & `matej-libs-0.1.1/matej/regedit.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/string.py` & `matej-libs-0.1.1/matej/string.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej/web.py` & `matej-libs-0.1.1/matej/web.py`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/matej_libs.egg-info/SOURCES.txt` & `matej-libs-0.1.1/matej_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matej-libs-0.1/setup.py` & `matej-libs-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
-version = "0.1"
+version = "0.1.1"
 
 setup(
 	name='matej-libs',
 	version=version,
 	author="Matej Vitek",
 	author_email="matej.vitek.business@gmail.com",
+	description="Collection of Python utility libraries.",
+	long_description=open('README.md', encoding='utf-8').read(),
 	url='https://github.com/MatejVitek/Python-Libraries',
-	download_url=f'https://github.com/MatejVitek/Python-Libraries/archive/refs/tags/v{version}.tar.gz',
 	packages=find_packages(),
 	python_requires='>=3.8',
 	install_requires=['numpy'],
 	extras_require={
 		'google-drive': ['requests'],
 		'config': ['ruamel.yaml'],
 		'parallel': ['joblib']
```

