# Comparing `tmp/closedai-0.0.2.tar.gz` & `tmp/closedai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "closedai-0.0.2.tar", last modified: Sat Mar 25 21:05:06 2023, max compression
+gzip compressed data, was "closedai-0.0.3.tar", last modified: Wed Apr 12 03:09:08 2023, max compression
```

## Comparing `closedai-0.0.2.tar` & `closedai-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:05:06.450126 closedai-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-25 21:04:52.000000 closedai-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-25 21:05:06.450126 closedai-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-25 21:04:52.000000 closedai-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-25 21:04:52.000000 closedai-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 21:05:06.450126 closedai-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-25 21:04:52.000000 closedai-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:05:06.446126 closedai-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:05:06.446126 closedai-0.0.2/src/closedai/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-25 21:04:52.000000 closedai-0.0.2/src/closedai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:05:06.450126 closedai-0.0.2/src/closedai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-25 21:05:06.000000 closedai-0.0.2/src/closedai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-25 21:05:06.000000 closedai-0.0.2/src/closedai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 21:05:06.000000 closedai-0.0.2/src/closedai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-25 21:05:06.000000 closedai-0.0.2/src/closedai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-25 21:05:06.000000 closedai-0.0.2/src/closedai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:09:08.814946 closedai-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 03:08:57.000000 closedai-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-12 03:09:08.814946 closedai-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 03:08:57.000000 closedai-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-12 03:08:57.000000 closedai-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 03:09:08.814946 closedai-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-12 03:08:57.000000 closedai-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:09:08.814946 closedai-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:09:08.814946 closedai-0.0.3/src/closedai/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:09:08.814946 closedai-0.0.3/src/closedai/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/pipelines/pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/pipelines/pipeline_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/pipelines/pipeline_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-12 03:08:57.000000 closedai-0.0.3/src/closedai/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:09:08.814946 closedai-0.0.3/src/closedai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-12 03:09:08.000000 closedai-0.0.3/src/closedai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-12 03:09:08.000000 closedai-0.0.3/src/closedai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:09:08.000000 closedai-0.0.3/src/closedai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 03:09:08.000000 closedai-0.0.3/src/closedai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 03:09:08.000000 closedai-0.0.3/src/closedai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 03:09:08.000000 closedai-0.0.3/src/closedai.egg-info/top_level.txt
```

### Comparing `closedai-0.0.2/LICENSE` & `closedai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `closedai-0.0.2/setup.py` & `closedai-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,20 @@
             if line.startswith("__version__"):
                 delim = '"' if '"' in line else "'"
                 return line.split(delim)[1]
     raise RuntimeError("Unable to find version string.")
 
 
 requirements = [
-    "huggingface_hub>=0.12.0",
+    "fastapi>=0.63.0",
+    "pydantic>=1.8.1",
+    "uvicorn[standard]>=0.13.4",
+    "openai",
+    "fire",
+    "packaging>=20.0",
 ]
 
 extras = {}
 extras["quality"] = ["black~=23.1", "ruff>=0.0.241"]
 
 setup(
     name="closedai",
@@ -28,8 +33,14 @@
     author="Nathan Raw",
     author_email="naterawdata@gmail.com",
     license="Apache",
     install_requires=requirements,
     extras_require=extras,
     package_dir={"": "src"},
     packages=find_packages("src"),
+    # add console script
+    entry_points={
+        "console_scripts": [
+            "closedai=closedai.cli_main:main",
+        ],
+    },
 )
```

