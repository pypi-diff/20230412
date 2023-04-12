# Comparing `tmp/jupyterlab_nvdashboard-0.8.0a22112312.tar.gz` & `tmp/jupyterlab_nvdashboard-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_nvdashboard-0.8.0a22112312.tar", last modified: Wed Nov 23 09:54:51 2022, max compression
+gzip compressed data, was "jupyterlab_nvdashboard-0.9.0a0.tar", last modified: Wed Apr 12 13:49:57 2023, max compression
```

## Comparing `jupyterlab_nvdashboard-0.8.0a22112312.tar` & `jupyterlab_nvdashboard-0.9.0a0.tar`

### file list

```diff
@@ -1,51 +1,48 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3686 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2991 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/install.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyter-config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyter-config/jupyterlab_nvdashboard.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      536 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/_version.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4514 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/cpu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16066 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/gpu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      833 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/handlers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2723 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/package.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9731 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/685.192016e9795f5c470d4e.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6749 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/remoteEntry.129b3fa4c4fb94482a0f.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2022-11-23 09:54:49.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/style.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2452 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1287 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3686 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1338 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2581 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/package.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/setup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5531 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/src/dashboard.tsx
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/src/handler.ts
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/src/index.ts
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/style/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2092 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/base.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/expansion-card-variant-dark.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/expansion-card-variant-light.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/index.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/index.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      555 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/tsconfig.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2969 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/tslint.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.175469 jupyterlab_nvdashboard-0.9.0a0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3677 2023-04-12 13:49:57.175469 jupyterlab_nvdashboard-0.9.0a0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2991 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/install.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.171469 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      536 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/_version.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.171469 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/apps/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/apps/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4514 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/apps/cpu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16066 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/apps/gpu.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.171469 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2723 2023-04-12 13:49:56.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/package.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.171469 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9732 2023-04-12 13:49:56.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/685.3f6908ec089d538ddf74.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2023-04-12 13:49:56.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6751 2023-04-12 13:49:56.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/remoteEntry.723954f9a80907c3d192.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-12 13:49:55.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/style.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2452 2023-04-12 13:49:56.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1287 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.171469 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3677 2023-04-12 13:49:57.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1260 2023-04-12 13:49:57.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-12 13:49:57.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-04-12 13:49:57.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-12 13:49:57.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-04-12 13:49:57.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-04-12 13:49:57.000000 jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2581 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/package.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-04-12 13:49:57.175469 jupyterlab_nvdashboard-0.9.0a0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2966 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.175469 jupyterlab_nvdashboard-0.9.0a0/src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5531 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/src/dashboard.tsx
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/src/handler.ts
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/src/index.ts
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 13:49:57.175469 jupyterlab_nvdashboard-0.9.0a0/style/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2092 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/style/base.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/style/expansion-card-variant-dark.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/style/expansion-card-variant-light.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/style/index.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/style/index.js
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      555 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/tsconfig.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2969 2023-04-12 13:43:44.000000 jupyterlab_nvdashboard-0.9.0a0/tslint.json
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/LICENSE` & `jupyterlab_nvdashboard-0.9.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/PKG-INFO` & `jupyterlab_nvdashboard-0.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nvdashboard
-Version: 0.8.0a22112312
+Version: 0.9.0a0
 Summary: A JupyterLab extension for displaying GPU usage dashboards
 Home-page: https://github.com/rapidsai/jupyterlab-nvdashboard
 Author: NVDashboard Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
@@ -106,9 +106,7 @@
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab_nvdashboard
 ```
 
 Releases for both packages are handled by [gpuCI](https://gpuci.gpuopenanalytics.com/job/rapidsai/job/gpuci/job/jupyterlab-nvdashboard/). Nightly builds are triggered when a push to a versioned branch occurs (i.e. `branch-0.5`). Stable builds are triggered when a push to the `main` branch occurs.
-
-
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/README.md` & `jupyterlab_nvdashboard-0.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/__init__.py` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/cpu.py` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/apps/cpu.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/gpu.py` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/apps/gpu.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/package.json` & `jupyterlab_nvdashboard-0.9.0a0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.9.0'"}*

```diff
@@ -30,19 +30,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/rapidsai/jupyterlab-nvdashboard",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.129b3fa4c4fb94482a0f.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "jupyterlab_nvdashboard/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -74,9 +69,9 @@
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/685.192016e9795f5c470d4e.js` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/685.3f6908ec089d538ddf74.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 (self.webpackChunkjupyterlab_nvdashboard = self.webpackChunkjupyterlab_nvdashboard || []).push([
     [685], {
         685: (e, n, t) => {
             "use strict";
             t.r(n), t.d(n, {
                 default: () => x
             });
-            var a, i = t(503),
-                o = t(169),
-                r = t(19),
-                s = t(579),
+            var a, i = t(210),
+                o = t(859),
+                r = t(671),
+                s = t(878),
                 d = t(526),
                 c = t(992),
                 l = t(271),
                 u = t(456);
             class h extends o.MainAreaWidget {
                 constructor() {
                     super({
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/remoteEntry.129b3fa4c4fb94482a0f.js` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/remoteEntry.723954f9a80907c3d192.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, d, s, f, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, d, f, s, p, c, h, v = {
             217: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(685).then((() => () => t(685))),
                         "./extension": () => t.e(685).then((() => () => t(685))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         b = {};
 
     function g(e) {
         var r = b[e];
@@ -43,78 +43,78 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        685: "192016e9795f5c470d4e",
+        685: "3f6908ec089d538ddf74",
         747: "8e5d43e699c27568a49a"
     } [e] + ".js?v=" + {
-        685: "192016e9795f5c470d4e",
+        685: "3f6908ec089d538ddf74",
         747: "8e5d43e699c27568a49a"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-nvdashboard:", g.l = (t, n, a, o) => {
+    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-nvdashboard:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== a)
+            if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var s = l[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+                    var f = l[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, g.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         g.S = {};
         var e = {},
             r = {};
         g.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 g.o(g.S, t) || (g.S[t] = {});
-                var o = g.S[t],
+                var a = g.S[t],
                     i = "jupyterlab-nvdashboard",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var a = o[e] = o[e] || {},
-                        u = a[r];
-                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
+                    var o = a[e] = a[e] || {},
+                        u = o[r];
+                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => g.e(685).then((() => () => g(685))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-nvdashboard", "0.8.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-nvdashboard", "0.9.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -128,151 +128,151 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 u = (typeof i)[0];
-            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
-                if ("u" == s) {
-                    if (!l || "u" != f) return !1
+                var d, f, s = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
+                if ("u" == f) {
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (f == s)
+                    if (s == f)
                         if (u <= n) {
                             if (d != e[u]) return !1
                         } else {
-                            if (a ? d > e[u] : d < e[u]) return !1;
+                            if (o ? d > e[u] : d < e[u]) return !1;
                             d != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (a || u <= n) return !1;
+                else if ("s" != s && "n" != s) {
+                    if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < f != a) return !1;
+                    if (u <= n || f < s != o) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != s && "n" != s && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = g.S[e];
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
-        var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), s(e[t][a])
-    }, s = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, a) {
-        var o = g.I(r);
-        return o && o.then ? o.then(e.bind(e, r, g.S[r], t, n, a)) : e(r, g.S[r], t, n)
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
+        var o = u(e, t);
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
+    }, f = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, o) {
+        var a = g.I(r);
+        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), p = {}, c = {
-        19: () => f("default", "@jupyterlab/coreutils", [1, 5, 5, 0]),
-        169: () => f("default", "@jupyterlab/apputils", [1, 3, 5, 0]),
-        271: () => f("default", "react", [1, 17, 0, 1]),
-        456: () => f("default", "react-dom", [1, 17, 0, 1]),
-        503: () => f("default", "@jupyterlab/application", [1, 3, 5, 0]),
-        526: () => f("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        579: () => f("default", "@jupyterlab/services", [1, 6, 5, 0]),
-        992: () => f("default", "@lumino/widgets", [1, 1, 33, 0])
+        210: () => s("default", "@jupyterlab/application", [1, 3, 5, 3]),
+        271: () => s("default", "react", [1, 17, 0, 1]),
+        456: () => s("default", "react-dom", [1, 17, 0, 1]),
+        526: () => s("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        671: () => s("default", "@jupyterlab/coreutils", [1, 5, 5, 3]),
+        859: () => s("default", "@jupyterlab/apputils", [1, 3, 5, 3]),
+        878: () => s("default", "@jupyterlab/services", [1, 6, 5, 3]),
+        992: () => s("default", "@lumino/widgets", [1, 1, 33, 0])
     }, h = {
-        685: [19, 169, 271, 456, 503, 526, 579, 992]
+        685: [210, 271, 456, 526, 671, 859, 878, 992]
     }, g.f.consumes = (e, r) => {
         g.o(h, e) && h[e].forEach((e => {
             if (g.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete p[e], g.m[e] = t => {
                         throw delete g.c[e], r
                     }
                 };
             try {
-                var a = c[e]();
-                a.then ? r.push(p[e] = a.then(t).catch(n)) : t(a)
+                var o = c[e]();
+                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             837: 0
         };
         g.f.j = (r, t) => {
             var n = g.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var o = g.p + g.u(r),
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var a = g.p + g.u(r),
                         i = new Error;
-                    g.l(o, (t => {
+                    g.l(a, (t => {
                         if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
-                                o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) g.o(i, n) && (g.m[n] = i[n]);
                     u && u(g)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], g.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], g.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkjupyterlab_nvdashboard = self.webpackChunkjupyterlab_nvdashboard || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var m = g(217);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-nvdashboard"] = m
 })();
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/server.py` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/server.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/PKG-INFO` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-nvdashboard
-Version: 0.8.0a22112312
+Version: 0.9.0a0
 Summary: A JupyterLab extension for displaying GPU usage dashboards
 Home-page: https://github.com/rapidsai/jupyterlab-nvdashboard
 Author: NVDashboard Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
@@ -106,9 +106,7 @@
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab_nvdashboard
 ```
 
 Releases for both packages are handled by [gpuCI](https://gpuci.gpuopenanalytics.com/job/rapidsai/job/gpuci/job/jupyterlab-nvdashboard/). Nightly builds are triggered when a push to a versioned branch occurs (i.e. `branch-0.5`). Stable builds are triggered when a push to the `main` branch occurs.
-
-
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/SOURCES.txt` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,34 +5,32 @@
 package.json
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tsconfig.json
 tslint.json
-jupyter-config/jupyterlab_nvdashboard.json
 jupyterlab_nvdashboard/__init__.py
 jupyterlab_nvdashboard/_version.py
-jupyterlab_nvdashboard/handlers.py
 jupyterlab_nvdashboard/server.py
 jupyterlab_nvdashboard/utils.py
 jupyterlab_nvdashboard.egg-info/PKG-INFO
 jupyterlab_nvdashboard.egg-info/SOURCES.txt
 jupyterlab_nvdashboard.egg-info/dependency_links.txt
 jupyterlab_nvdashboard.egg-info/entry_points.txt
 jupyterlab_nvdashboard.egg-info/not-zip-safe
 jupyterlab_nvdashboard.egg-info/requires.txt
 jupyterlab_nvdashboard.egg-info/top_level.txt
 jupyterlab_nvdashboard/apps/__init__.py
 jupyterlab_nvdashboard/apps/cpu.py
 jupyterlab_nvdashboard/apps/gpu.py
 jupyterlab_nvdashboard/labextension/package.json
-jupyterlab_nvdashboard/labextension/static/685.192016e9795f5c470d4e.js
+jupyterlab_nvdashboard/labextension/static/685.3f6908ec089d538ddf74.js
 jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js
-jupyterlab_nvdashboard/labextension/static/remoteEntry.129b3fa4c4fb94482a0f.js
+jupyterlab_nvdashboard/labextension/static/remoteEntry.723954f9a80907c3d192.js
 jupyterlab_nvdashboard/labextension/static/style.js
 jupyterlab_nvdashboard/labextension/static/third-party-licenses.json
 src/dashboard.tsx
 src/handler.ts
 src/index.ts
 style/base.css
 style/expansion-card-variant-dark.svg
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/package.json` & `jupyterlab_nvdashboard-0.9.0a0/jupyterlab_nvdashboard/labextension/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.723954f9a80907c3d192.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.9.0'"}*

```diff
@@ -30,14 +30,19 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/rapidsai/jupyterlab-nvdashboard",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.723954f9a80907c3d192.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "jupyterlab_nvdashboard/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -69,9 +74,9 @@
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/setup.py` & `jupyterlab_nvdashboard-0.9.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     ]
 }
 
 labext_name = "jupyterlab-nvdashboard"
 
 data_files_spec = [
     ("share/jupyter/labextensions/%s" % labext_name, lab_path, "**"),
-    ("share/jupyter/labextensions/%s" % labext_name, HERE, "install.json"),("etc/jupyter/jupyter_server_config.d",
-     "jupyter-config", "jupyterlab_nvdashboard.json"),
-
+    ("share/jupyter/labextensions/%s" % labext_name, HERE, "install.json"),
 ]
 
 cmdclass = create_cmdclass("jsdeps",
     package_data_spec=package_data_spec,
     data_files_spec=data_files_spec
 )
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/src/dashboard.tsx` & `jupyterlab_nvdashboard-0.9.0a0/src/dashboard.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/src/handler.ts` & `jupyterlab_nvdashboard-0.9.0a0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/src/index.ts` & `jupyterlab_nvdashboard-0.9.0a0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/style/base.css` & `jupyterlab_nvdashboard-0.9.0a0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/tsconfig.json` & `jupyterlab_nvdashboard-0.9.0a0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22112312/tslint.json` & `jupyterlab_nvdashboard-0.9.0a0/tslint.json`

 * *Files identical despite different names*

