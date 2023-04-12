# Comparing `tmp/data2vec-0.0.2.tar.gz` & `tmp/data2vec-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2vec-0.0.2.tar", last modified: Wed Apr 12 14:07:30 2023, max compression
+gzip compressed data, was "data2vec-0.0.3.tar", last modified: Wed Apr 12 15:15:52 2023, max compression
```

## Comparing `data2vec-0.0.2.tar` & `data2vec-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:07:30.226873 data2vec-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-04-12 12:09:40.000000 data2vec-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      745 2023-04-12 14:07:30.225871 data2vec-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-12 12:09:40.000000 data2vec-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 14:07:30.211675 data2vec-0.0.2/data2vec/
--rw-rw-rw-   0        0        0       45 2023-04-12 12:09:40.000000 data2vec-0.0.2/data2vec/__init__.py
--rw-rw-rw-   0        0        0     3224 2023-04-12 13:47:23.000000 data2vec-0.0.2/data2vec/img_to_vec.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:07:30.225871 data2vec-0.0.2/data2vec.egg-info/
--rw-rw-rw-   0        0        0      745 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 14:07:30.226873 data2vec-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      925 2023-04-12 14:05:49.000000 data2vec-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:15:52.409521 data2vec-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-12 12:09:40.000000 data2vec-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2668 2023-04-12 15:15:52.408520 data2vec-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2283 2023-04-12 15:14:21.000000 data2vec-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 15:15:52.391020 data2vec-0.0.3/data2vec/
+-rw-rw-rw-   0        0        0       45 2023-04-12 12:09:40.000000 data2vec-0.0.3/data2vec/__init__.py
+-rw-rw-rw-   0        0        0     3224 2023-04-12 13:47:23.000000 data2vec-0.0.3/data2vec/img_to_vec.py
+drwxrwxrwx   0        0        0        0 2023-04-12 15:15:52.407515 data2vec-0.0.3/data2vec.egg-info/
+-rw-rw-rw-   0        0        0     2668 2023-04-12 15:15:52.000000 data2vec-0.0.3/data2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-04-12 15:15:52.000000 data2vec-0.0.3/data2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 15:15:52.000000 data2vec-0.0.3/data2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-12 15:15:52.000000 data2vec-0.0.3/data2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 15:15:52.000000 data2vec-0.0.3/data2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 15:15:52.409521 data2vec-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      853 2023-04-12 15:14:21.000000 data2vec-0.0.3/setup.py
```

### Comparing `data2vec-0.0.2/LICENSE` & `data2vec-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data2vec-0.0.2/data2vec/img_to_vec.py` & `data2vec-0.0.3/data2vec/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `data2vec-0.0.2/setup.py` & `data2vec-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='data2vec',
-    version='0.0.2',
+    version='0.0.3',
     keywords='Vector Pytorch Vector Database',
-    description='data2Vec是一种用于数据向量表征的工具，它将数据转换为向量矩阵并可以将其存储在向量数据库中。',
+    description='data2Vec是一个Python工具，用于数据向量表征。',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT License',
     url='https://github.com/xuehangcang/data2vec',
     author='Xuehang Cang',
     author_email='xuehangcang@outlook.com',
     packages=find_packages(),
```

