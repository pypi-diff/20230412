# Comparing `tmp/xfact-0.3.54.tar.gz` & `tmp/xfact-0.3.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfact-0.3.54.tar", last modified: Thu Apr  6 02:54:14 2023, max compression
+gzip compressed data, was "xfact-0.3.56.tar", last modified: Wed Apr 12 02:40:16 2023, max compression
```

## Comparing `xfact-0.3.54.tar` & `xfact-0.3.56.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.945128 xfact-0.3.54/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-06 02:53:40.000000 xfact-0.3.54/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-06 02:54:14.945128 xfact-0.3.54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-06 02:53:40.000000 xfact-0.3.54/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-06 02:53:40.000000 xfact-0.3.54/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 02:54:14.945128 xfact-0.3.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-06 02:53:41.000000 xfact-0.3.54/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/xfact/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/xfact/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/config/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/xfact/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/logs/comet_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/logs/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/xfact/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/xfact/nlp/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/datasets/fever_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/datasets/snli_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/deardr_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/xfact/nlp/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/inference/prefix_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/nlp/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.945128 xfact-0.3.54/src/xfact/registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/registry/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/registry/registrable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-06 02:53:40.000000 xfact-0.3.54/src/xfact/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:54:14.941128 xfact-0.3.54/src/xfact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-06 02:54:14.000000 xfact-0.3.54/src/xfact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-06 02:54:14.000000 xfact-0.3.54/src/xfact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:54:14.000000 xfact-0.3.54/src/xfact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-06 02:54:14.000000 xfact-0.3.54/src/xfact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 02:54:14.000000 xfact-0.3.54/src/xfact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.899397 xfact-0.3.56/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 02:39:49.000000 xfact-0.3.56/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 02:40:16.899397 xfact-0.3.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-12 02:39:49.000000 xfact-0.3.56/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 02:39:49.000000 xfact-0.3.56/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 02:40:16.899397 xfact-0.3.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-12 02:39:50.000000 xfact-0.3.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.895397 xfact-0.3.56/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.895397 xfact-0.3.56/src/xfact/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.899397 xfact-0.3.56/src/xfact/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/config/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.899397 xfact-0.3.56/src/xfact/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/logs/comet_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/logs/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.899397 xfact-0.3.56/src/xfact/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.899397 xfact-0.3.56/src/xfact/nlp/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/datasets/fever_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/datasets/snli_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/deardr_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.899397 xfact-0.3.56/src/xfact/nlp/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/inference/prefix_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/nlp/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.899397 xfact-0.3.56/src/xfact/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/registry/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/registry/registrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-12 02:39:49.000000 xfact-0.3.56/src/xfact/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:40:16.895397 xfact-0.3.56/src/xfact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 02:40:16.000000 xfact-0.3.56/src/xfact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-12 02:40:16.000000 xfact-0.3.56/src/xfact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:40:16.000000 xfact-0.3.56/src/xfact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 02:40:16.000000 xfact-0.3.56/src/xfact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 02:40:16.000000 xfact-0.3.56/src/xfact.egg-info/top_level.txt
```

### Comparing `xfact-0.3.54/README.md` & `xfact-0.3.56/README.md`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/setup.py` & `xfact-0.3.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install = [req for req in reqs if not req.startswith("git+git://")]
 depends = [req.replace("git+git://", "git+http://") for req in reqs if req.startswith("git+git://")]
 
 
 setup(
     name='xfact',
-    version='0.3.54',
+    version='0.3.56',
     author='James Thorne',
     author_email='james@jamesthorne.com',
     description='xfact',
     long_description="readme",
     python_requires='>=3.8',
     packages=["xfact",
               "xfact.nlp",
```

### Comparing `xfact-0.3.54/src/xfact/config/args.py` & `xfact-0.3.56/src/xfact/config/args.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/logs/comet_callback.py` & `xfact-0.3.56/src/xfact/logs/comet_callback.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/logs/logs.py` & `xfact-0.3.56/src/xfact/logs/logs.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/data_utils.py` & `xfact-0.3.56/src/xfact/nlp/data_utils.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/dataset.py` & `xfact-0.3.56/src/xfact/nlp/dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/datasets/fever_dataset.py` & `xfact-0.3.56/src/xfact/nlp/datasets/fever_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/datasets/snli_dataset.py` & `xfact-0.3.56/src/xfact/nlp/datasets/snli_dataset.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/deardr_trainer.py` & `xfact-0.3.56/src/xfact/nlp/deardr_trainer.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/inference/prefix_decoder.py` & `xfact-0.3.56/src/xfact/nlp/inference/prefix_decoder.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/model.py` & `xfact-0.3.56/src/xfact/nlp/model.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/post_processing.py` & `xfact-0.3.56/src/xfact/nlp/post_processing.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/reader.py` & `xfact-0.3.56/src/xfact/nlp/reader.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/nlp/scoring.py` & `xfact-0.3.56/src/xfact/nlp/scoring.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/registry/module.py` & `xfact-0.3.56/src/xfact/registry/module.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/registry/registrable.py` & `xfact-0.3.56/src/xfact/registry/registrable.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact/train.py` & `xfact-0.3.56/src/xfact/train.py`

 * *Files identical despite different names*

### Comparing `xfact-0.3.54/src/xfact.egg-info/SOURCES.txt` & `xfact-0.3.56/src/xfact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

