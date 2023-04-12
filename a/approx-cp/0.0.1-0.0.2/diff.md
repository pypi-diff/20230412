# Comparing `tmp/approx-cp-0.0.1.tar.gz` & `tmp/approx-cp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approx-cp-0.0.1.tar", last modified: Wed Apr 12 18:38:08 2023, max compression
+gzip compressed data, was "approx-cp-0.0.2.tar", last modified: Wed Apr 12 18:53:53 2023, max compression
```

## Comparing `approx-cp-0.0.1.tar` & `approx-cp-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:38:08.657579 approx-cp-0.0.1/
--rw-r--r--   0 javierabad   (501) staff       (20)     7438 2023-04-12 18:38:08.657648 approx-cp-0.0.1/PKG-INFO
--rw-r--r--   0 javierabad   (501) staff       (20)     6880 2023-04-12 16:35:37.000000 approx-cp-0.0.1/README.md
--rw-r--r--   0 javierabad   (501) staff       (20)       86 2023-04-12 16:35:37.000000 approx-cp-0.0.1/pyproject.toml
--rw-r--r--   0 javierabad   (501) staff       (20)       78 2023-04-12 18:38:08.657870 approx-cp-0.0.1/setup.cfg
--rw-r--r--   0 javierabad   (501) staff       (20)     1202 2023-04-12 18:33:33.000000 approx-cp-0.0.1/setup.py
-drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:38:08.654675 approx-cp-0.0.1/src/
-drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:38:08.656166 approx-cp-0.0.1/src/acp/
--rw-r--r--   0 javierabad   (501) staff       (20)        0 2023-04-12 16:35:37.000000 approx-cp-0.0.1/src/acp/__init__.py
--rw-r--r--   0 javierabad   (501) staff       (20)     9393 2023-04-12 18:27:24.000000 approx-cp-0.0.1/src/acp/experiments.py
--rw-r--r--   0 javierabad   (501) staff       (20)     6290 2023-04-12 18:26:47.000000 approx-cp-0.0.1/src/acp/methods.py
--rw-r--r--   0 javierabad   (501) staff       (20)    20187 2023-04-12 18:27:00.000000 approx-cp-0.0.1/src/acp/models.py
--rw-r--r--   0 javierabad   (501) staff       (20)    10590 2023-04-12 18:27:04.000000 approx-cp-0.0.1/src/acp/others.py
--rw-r--r--   0 javierabad   (501) staff       (20)    13557 2023-04-12 17:54:51.000000 approx-cp-0.0.1/src/acp/utils.py
--rw-r--r--   0 javierabad   (501) staff       (20)    13791 2023-04-12 18:27:17.000000 approx-cp-0.0.1/src/acp/wrapper.py
-drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:38:08.656862 approx-cp-0.0.1/src/approx_cp.egg-info/
--rw-r--r--   0 javierabad   (501) staff       (20)     7438 2023-04-12 18:38:08.000000 approx-cp-0.0.1/src/approx_cp.egg-info/PKG-INFO
--rw-r--r--   0 javierabad   (501) staff       (20)      461 2023-04-12 18:38:08.000000 approx-cp-0.0.1/src/approx_cp.egg-info/SOURCES.txt
--rw-r--r--   0 javierabad   (501) staff       (20)        1 2023-04-12 18:38:08.000000 approx-cp-0.0.1/src/approx_cp.egg-info/dependency_links.txt
--rw-r--r--   0 javierabad   (501) staff       (20)      102 2023-04-12 18:38:08.000000 approx-cp-0.0.1/src/approx_cp.egg-info/requires.txt
--rw-r--r--   0 javierabad   (501) staff       (20)       16 2023-04-12 18:38:08.000000 approx-cp-0.0.1/src/approx_cp.egg-info/top_level.txt
-drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:38:08.657158 approx-cp-0.0.1/src/third_party/
-drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:38:08.657482 approx-cp-0.0.1/src/third_party/RAPS/
--rw-r--r--   0 javierabad   (501) staff       (20)    23347 2023-04-12 16:35:37.000000 approx-cp-0.0.1/src/third_party/RAPS/RAPS_conformal.py
--rw-r--r--   0 javierabad   (501) staff       (20)        0 2023-04-12 16:35:37.000000 approx-cp-0.0.1/src/third_party/RAPS/__init__.py
--rw-r--r--   0 javierabad   (501) staff       (20)        0 2023-04-12 16:35:37.000000 approx-cp-0.0.1/src/third_party/__init__.py
+drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:53:53.881073 approx-cp-0.0.2/
+-rw-r--r--   0 javierabad   (501) staff       (20)     4527 2023-04-12 18:53:53.881141 approx-cp-0.0.2/PKG-INFO
+-rw-r--r--   0 javierabad   (501) staff       (20)     3969 2023-04-12 18:51:44.000000 approx-cp-0.0.2/README.md
+-rw-r--r--   0 javierabad   (501) staff       (20)       86 2023-04-12 16:35:37.000000 approx-cp-0.0.2/pyproject.toml
+-rw-r--r--   0 javierabad   (501) staff       (20)       78 2023-04-12 18:53:53.881343 approx-cp-0.0.2/setup.cfg
+-rw-r--r--   0 javierabad   (501) staff       (20)     1202 2023-04-12 18:53:38.000000 approx-cp-0.0.2/setup.py
+drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:53:53.877911 approx-cp-0.0.2/src/
+drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:53:53.879897 approx-cp-0.0.2/src/acp/
+-rw-r--r--   0 javierabad   (501) staff       (20)        0 2023-04-12 16:35:37.000000 approx-cp-0.0.2/src/acp/__init__.py
+-rw-r--r--   0 javierabad   (501) staff       (20)     9393 2023-04-12 18:27:24.000000 approx-cp-0.0.2/src/acp/experiments.py
+-rw-r--r--   0 javierabad   (501) staff       (20)     6290 2023-04-12 18:26:47.000000 approx-cp-0.0.2/src/acp/methods.py
+-rw-r--r--   0 javierabad   (501) staff       (20)    20187 2023-04-12 18:27:00.000000 approx-cp-0.0.2/src/acp/models.py
+-rw-r--r--   0 javierabad   (501) staff       (20)    10590 2023-04-12 18:27:04.000000 approx-cp-0.0.2/src/acp/others.py
+-rw-r--r--   0 javierabad   (501) staff       (20)    13557 2023-04-12 17:54:51.000000 approx-cp-0.0.2/src/acp/utils.py
+-rw-r--r--   0 javierabad   (501) staff       (20)    13791 2023-04-12 18:27:17.000000 approx-cp-0.0.2/src/acp/wrapper.py
+drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:53:53.880569 approx-cp-0.0.2/src/approx_cp.egg-info/
+-rw-r--r--   0 javierabad   (501) staff       (20)     4527 2023-04-12 18:53:53.000000 approx-cp-0.0.2/src/approx_cp.egg-info/PKG-INFO
+-rw-r--r--   0 javierabad   (501) staff       (20)      461 2023-04-12 18:53:53.000000 approx-cp-0.0.2/src/approx_cp.egg-info/SOURCES.txt
+-rw-r--r--   0 javierabad   (501) staff       (20)        1 2023-04-12 18:53:53.000000 approx-cp-0.0.2/src/approx_cp.egg-info/dependency_links.txt
+-rw-r--r--   0 javierabad   (501) staff       (20)      102 2023-04-12 18:53:53.000000 approx-cp-0.0.2/src/approx_cp.egg-info/requires.txt
+-rw-r--r--   0 javierabad   (501) staff       (20)       16 2023-04-12 18:53:53.000000 approx-cp-0.0.2/src/approx_cp.egg-info/top_level.txt
+drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:53:53.880718 approx-cp-0.0.2/src/third_party/
+drwxr-xr-x   0 javierabad   (501) staff       (20)        0 2023-04-12 18:53:53.880981 approx-cp-0.0.2/src/third_party/RAPS/
+-rw-r--r--   0 javierabad   (501) staff       (20)    23347 2023-04-12 16:35:37.000000 approx-cp-0.0.2/src/third_party/RAPS/RAPS_conformal.py
+-rw-r--r--   0 javierabad   (501) staff       (20)        0 2023-04-12 16:35:37.000000 approx-cp-0.0.2/src/third_party/RAPS/__init__.py
+-rw-r--r--   0 javierabad   (501) staff       (20)        0 2023-04-12 16:35:37.000000 approx-cp-0.0.2/src/third_party/__init__.py
```

### Comparing `approx-cp-0.0.1/setup.py` & `approx-cp-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="approx-cp",
-    version="0.0.1",
+    version="0.0.2",
     description="Python implementation of Approximate full Conformal Prediction (ACP)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cambridge-mlg/acp",
     author="Javier Abad",
     author_email="javier.abadmartinez@ai.ethz.ch",
     classifiers=[
```

### Comparing `approx-cp-0.0.1/src/acp/experiments.py` & `approx-cp-0.0.2/src/acp/experiments.py`

 * *Files identical despite different names*

### Comparing `approx-cp-0.0.1/src/acp/methods.py` & `approx-cp-0.0.2/src/acp/methods.py`

 * *Files identical despite different names*

### Comparing `approx-cp-0.0.1/src/acp/models.py` & `approx-cp-0.0.2/src/acp/models.py`

 * *Files identical despite different names*

### Comparing `approx-cp-0.0.1/src/acp/others.py` & `approx-cp-0.0.2/src/acp/others.py`

 * *Files identical despite different names*

### Comparing `approx-cp-0.0.1/src/acp/utils.py` & `approx-cp-0.0.2/src/acp/utils.py`

 * *Files identical despite different names*

### Comparing `approx-cp-0.0.1/src/acp/wrapper.py` & `approx-cp-0.0.2/src/acp/wrapper.py`

 * *Files identical despite different names*

### Comparing `approx-cp-0.0.1/src/third_party/RAPS/RAPS_conformal.py` & `approx-cp-0.0.2/src/third_party/RAPS/RAPS_conformal.py`

 * *Files identical despite different names*

