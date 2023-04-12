# Comparing `tmp/kmspy-0.0.8.tar.gz` & `tmp/kmspy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmspy-0.0.8.tar", last modified: Sun Jan  1 23:45:33 2023, max compression
+gzip compressed data, was "kmspy-0.0.9.tar", last modified: Mon Jan  2 03:40:44 2023, max compression
```

## Comparing `kmspy-0.0.8.tar` & `kmspy-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-01 23:45:33.934214 kmspy-0.0.8/
--rw-rw-r--   0 kms       (1001) kms       (1003)      382 2023-01-01 23:45:33.932941 kmspy-0.0.8/PKG-INFO
--rw-rw-r--   0 kms       (1001) kms       (1003)        0 2022-09-20 05:46:56.000000 kmspy-0.0.8/README.md
-drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-01 23:45:33.876422 kmspy-0.0.8/kmspy/
--rw-rw-r--   0 kms       (1001) kms       (1003)      117 2023-01-01 23:43:20.000000 kmspy-0.0.8/kmspy/__init__.py
-drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-01 23:45:33.905722 kmspy-0.0.8/kmspy/data/
--rw-rw-r--   0 kms       (1001) kms       (1003)       90 2022-12-28 04:32:46.000000 kmspy-0.0.8/kmspy/data/__init__.py
--rw-rw-r--   0 kms       (1001) kms       (1003)     6462 2023-01-01 23:43:50.000000 kmspy-0.0.8/kmspy/data/dataset.py
--rw-rw-r--   0 kms       (1001) kms       (1003)    12437 2023-01-01 23:43:00.000000 kmspy-0.0.8/kmspy/data/prefetch_generator.py
-drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-01 23:45:33.914037 kmspy-0.0.8/kmspy/multiprocessing/
--rw-rw-r--   0 kms       (1001) kms       (1003)       28 2022-12-27 04:29:25.000000 kmspy-0.0.8/kmspy/multiprocessing/__init__.py
--rw-rw-r--   0 kms       (1001) kms       (1003)     2828 2022-12-28 04:51:40.000000 kmspy-0.0.8/kmspy/multiprocessing/process.py
-drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-01 23:45:33.921919 kmspy-0.0.8/kmspy/utils/
--rw-rw-r--   0 kms       (1001) kms       (1003)       46 2022-12-28 04:33:10.000000 kmspy-0.0.8/kmspy/utils/__init__.py
--rw-rw-r--   0 kms       (1001) kms       (1003)     1857 2022-12-28 04:35:05.000000 kmspy-0.0.8/kmspy/utils/_utils.py
-drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-01 23:45:33.894702 kmspy-0.0.8/kmspy.egg-info/
--rw-rw-r--   0 kms       (1001) kms       (1003)      382 2023-01-01 23:45:33.000000 kmspy-0.0.8/kmspy.egg-info/PKG-INFO
--rw-rw-r--   0 kms       (1001) kms       (1003)      403 2023-01-01 23:45:33.000000 kmspy-0.0.8/kmspy.egg-info/SOURCES.txt
--rw-rw-r--   0 kms       (1001) kms       (1003)        1 2023-01-01 23:45:33.000000 kmspy-0.0.8/kmspy.egg-info/dependency_links.txt
--rw-rw-r--   0 kms       (1001) kms       (1003)        6 2023-01-01 23:45:33.000000 kmspy-0.0.8/kmspy.egg-info/requires.txt
--rw-rw-r--   0 kms       (1001) kms       (1003)       12 2023-01-01 23:45:33.000000 kmspy-0.0.8/kmspy.egg-info/top_level.txt
--rw-rw-r--   0 kms       (1001) kms       (1003)       38 2023-01-01 23:45:33.934965 kmspy-0.0.8/setup.cfg
--rw-rw-r--   0 kms       (1001) kms       (1003)      607 2023-01-01 23:43:07.000000 kmspy-0.0.8/setup.py
-drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-01 23:45:33.929346 kmspy-0.0.8/tests/
--rw-rw-r--   0 kms       (1001) kms       (1003)        0 2022-09-20 05:44:16.000000 kmspy-0.0.8/tests/__init__.py
--rw-rw-r--   0 kms       (1001) kms       (1003)        0 2022-09-20 05:44:09.000000 kmspy-0.0.8/tests/test.py
+drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-02 03:40:44.559561 kmspy-0.0.9/
+-rw-rw-r--   0 kms       (1001) kms       (1003)      382 2023-01-02 03:40:44.557875 kmspy-0.0.9/PKG-INFO
+-rw-rw-r--   0 kms       (1001) kms       (1003)        0 2022-09-20 05:46:56.000000 kmspy-0.0.9/README.md
+drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-02 03:40:44.492843 kmspy-0.0.9/kmspy/
+-rw-rw-r--   0 kms       (1001) kms       (1003)      117 2023-01-02 03:40:03.000000 kmspy-0.0.9/kmspy/__init__.py
+drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-02 03:40:44.523285 kmspy-0.0.9/kmspy/data/
+-rw-rw-r--   0 kms       (1001) kms       (1003)       90 2022-12-28 04:32:46.000000 kmspy-0.0.9/kmspy/data/__init__.py
+-rw-rw-r--   0 kms       (1001) kms       (1003)     6462 2023-01-01 23:43:50.000000 kmspy-0.0.9/kmspy/data/dataset.py
+-rw-rw-r--   0 kms       (1001) kms       (1003)    12476 2023-01-02 03:39:48.000000 kmspy-0.0.9/kmspy/data/prefetch_generator.py
+drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-02 03:40:44.532686 kmspy-0.0.9/kmspy/multiprocessing/
+-rw-rw-r--   0 kms       (1001) kms       (1003)       28 2022-12-27 04:29:25.000000 kmspy-0.0.9/kmspy/multiprocessing/__init__.py
+-rw-rw-r--   0 kms       (1001) kms       (1003)     2828 2022-12-28 04:51:40.000000 kmspy-0.0.9/kmspy/multiprocessing/process.py
+drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-02 03:40:44.544904 kmspy-0.0.9/kmspy/utils/
+-rw-rw-r--   0 kms       (1001) kms       (1003)       46 2022-12-28 04:33:10.000000 kmspy-0.0.9/kmspy/utils/__init__.py
+-rw-rw-r--   0 kms       (1001) kms       (1003)     1857 2022-12-28 04:35:05.000000 kmspy-0.0.9/kmspy/utils/_utils.py
+drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-02 03:40:44.511663 kmspy-0.0.9/kmspy.egg-info/
+-rw-rw-r--   0 kms       (1001) kms       (1003)      382 2023-01-02 03:40:44.000000 kmspy-0.0.9/kmspy.egg-info/PKG-INFO
+-rw-rw-r--   0 kms       (1001) kms       (1003)      403 2023-01-02 03:40:44.000000 kmspy-0.0.9/kmspy.egg-info/SOURCES.txt
+-rw-rw-r--   0 kms       (1001) kms       (1003)        1 2023-01-02 03:40:44.000000 kmspy-0.0.9/kmspy.egg-info/dependency_links.txt
+-rw-rw-r--   0 kms       (1001) kms       (1003)        6 2023-01-02 03:40:44.000000 kmspy-0.0.9/kmspy.egg-info/requires.txt
+-rw-rw-r--   0 kms       (1001) kms       (1003)       12 2023-01-02 03:40:44.000000 kmspy-0.0.9/kmspy.egg-info/top_level.txt
+-rw-rw-r--   0 kms       (1001) kms       (1003)       38 2023-01-02 03:40:44.560486 kmspy-0.0.9/setup.cfg
+-rw-rw-r--   0 kms       (1001) kms       (1003)      607 2023-01-02 03:40:08.000000 kmspy-0.0.9/setup.py
+drwxrwxr-x   0 kms       (1001) kms       (1003)        0 2023-01-02 03:40:44.553391 kmspy-0.0.9/tests/
+-rw-rw-r--   0 kms       (1001) kms       (1003)        0 2022-09-20 05:44:16.000000 kmspy-0.0.9/tests/__init__.py
+-rw-rw-r--   0 kms       (1001) kms       (1003)        0 2022-09-20 05:44:09.000000 kmspy-0.0.9/tests/test.py
```

### Comparing `kmspy-0.0.8/kmspy/data/dataset.py` & `kmspy-0.0.9/kmspy/data/dataset.py`

 * *Files identical despite different names*

### Comparing `kmspy-0.0.8/kmspy/data/prefetch_generator.py` & `kmspy-0.0.9/kmspy/data/prefetch_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
                 # results에서 꺼낼 데이터도 없고, unit도 모두 종료된 상태
                 raise StopIteration
             if (self._next_idx in self.results if self.ordered else self.results):
                 # self.ordered=True 이면, self.results에서 next_idx를 꺼내고
                 # self.ordered=False 이면, popitem(False)로 가장 오래된 데이터부터 꺼냄
                 item = self.results.pop(self._next_idx) if self.ordered else self.results.popitem(False)[1]
                 if item is NoOutput:
+                    self._next_idx +=1
                     continue
                 else:
                     self._pendding = False
                     self._next_idx +=1
                     return item
             else:
                 # unit에서 데이터가 준비될때까지 대기하기 위해서 진입하는 조건문
```

### Comparing `kmspy-0.0.8/kmspy/multiprocessing/process.py` & `kmspy-0.0.9/kmspy/multiprocessing/process.py`

 * *Files identical despite different names*

### Comparing `kmspy-0.0.8/kmspy/utils/_utils.py` & `kmspy-0.0.9/kmspy/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `kmspy-0.0.8/setup.py` & `kmspy-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kmspy",
-    version="0.0.8",
+    version="0.0.9",
     author="KMS",
     author_email="su4651@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

