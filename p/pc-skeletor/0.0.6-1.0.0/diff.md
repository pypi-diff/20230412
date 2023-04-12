# Comparing `tmp/pc_skeletor-0.0.6.tar.gz` & `tmp/pc_skeletor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PC-Skeletor/PC-Skeletor/dist/tmpg3dw4bqm/pc_skeletor-0.0.6.tar", last modified: Tue Nov 22 16:42:28 2022, max compression
+gzip compressed data, was "/home/runner/work/pc-skeletor/pc-skeletor/dist/.tmp-cx504pkn/pc_skeletor-1.0.0.tar", last modified: Wed Apr 12 16:19:26 2023, max compression
```

## Comparing `pc_skeletor-0.0.6.tar` & `pc_skeletor-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (116)     1089 2022-11-22 16:42:16.000000 pc_skeletor-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     6964 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor/
--rw-r--r--   0 runner    (1001) docker     (116)       87 2022-11-22 16:42:17.000000 pc_skeletor-0.0.6/pc_skeletor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3289 2022-11-22 16:42:17.000000 pc_skeletor-0.0.6/pc_skeletor/download.py
--rw-r--r--   0 runner    (1001) docker     (116)    13306 2022-11-22 16:42:17.000000 pc_skeletor-0.0.6/pc_skeletor/skeletor.py
--rw-r--r--   0 runner    (1001) docker     (116)      702 2022-11-22 16:42:17.000000 pc_skeletor-0.0.6/pc_skeletor/test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2131 2022-11-22 16:42:17.000000 pc_skeletor-0.0.6/pc_skeletor/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6964 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      330 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/pc_skeletor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-22 16:42:28.000000 pc_skeletor-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    10558 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor/
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/pc_skeletor/L1.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/pc_skeletor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9556 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/pc_skeletor/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/pc_skeletor/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23617 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/pc_skeletor/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/pc_skeletor/point2skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9011 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/pc_skeletor/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10558 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/pc_skeletor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:19:26.000000 pc_skeletor-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4136 2023-04-12 16:19:18.000000 pc_skeletor-1.0.0/tests/test_lbc.py
```

### Comparing `pc_skeletor-0.0.6/LICENSE` & `pc_skeletor-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pc_skeletor-0.0.6/pc_skeletor/download.py` & `pc_skeletor-1.0.0/pc_skeletor/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 
 # Built-in/Generic Imports
 # ...
 
 # Libs
 import os
 from zipfile import ZipFile
-from tqdm import tqdm
 import urllib.request
+import glob
+
+from tqdm import tqdm
 
 # Own modules
 # ...
 
 EXISTS = True
 NON_EXIST = False
 
@@ -78,27 +80,50 @@
         else:
             return NON_EXIST
 
     def download_tree_dataset(self, output_path: str = os.path.abspath(__file__), overwrite: bool = False):
 
         self.url = 'https://faubox.rrze.uni-erlangen.de/dl/fiY7DMQ5TgQwoA1LvedgRu/tree.zip'
 
-        self.dataset_name ='tree'
+        self.dataset_name = 'tree'
 
         existence = self.__check_existence(output_directory=output_path, dataset_name=self.dataset_name)
 
         if existence == NON_EXIST:
             self.filename = download(url=self.url, output_dir=self.data_path, overwrite=overwrite)
             extract(filename=self.filename, output_dir=self.data_path)
         else:
             print('Dataset {} already exists at location {}'.format(self.dataset_name, self.data_path))
 
         self.file_path = os.path.abspath(
             os.path.join(self.data_path, self.url.split('/')[-1].split('.zip')[0] + '.ply'))
         return self.file_path
 
+    def download_semantic_tree_dataset(self, output_path: str = os.path.abspath(__file__), overwrite: bool = False):
+
+        self.url = 'https://faubox.rrze.uni-erlangen.de/dl/fiCVjuo7hpxcacu1dWEmr9/semantic_tree.zip'
+
+        self.dataset_name = 'semantic tree'
+
+        existence = self.__check_existence(output_directory=output_path, dataset_name=self.dataset_name)
+
+        if existence == NON_EXIST:
+            self.filename = download(url=self.url, output_dir=self.data_path, overwrite=overwrite)
+            extract(filename=self.filename, output_dir=self.data_path)
+        else:
+            print('Dataset {} already exists at location {}'.format(self.dataset_name, self.data_path))
+
+        self.file_paths = glob.glob(
+            os.path.join(self.data_path, self.url.split('/')[-1].split('.zip')[0] + '/*' + '.ply'))
+        return self.file_paths
+
 
 if __name__ == '__main__':
     downloader = Dataset()
-    downloader.download_tree_dataset()
+    file = downloader.download_tree_dataset()
+
+    print('Saved at {}'.format(downloader.dataset_path))
+
+    downloader = Dataset()
+    file1, file2 = downloader.download_semantic_tree_dataset()
 
     print('Saved at {}'.format(downloader.dataset_path))
```

