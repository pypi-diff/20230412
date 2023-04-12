# Comparing `tmp/jupyterlab_nvdashboard-0.8.0a22103111.tar.gz` & `tmp/jupyterlab_nvdashboard-0.8.0a22112312.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_nvdashboard-0.8.0a22103111.tar", last modified: Mon Oct 31 16:14:29 2022, max compression
+gzip compressed data, was "jupyterlab_nvdashboard-0.8.0a22112312.tar", last modified: Wed Nov 23 09:54:51 2022, max compression
```

## Comparing `jupyterlab_nvdashboard-0.8.0a22103111.tar` & `jupyterlab_nvdashboard-0.8.0a22112312.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3394 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2699 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/install.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.432949 jupyterlab_nvdashboard-0.8.0a22103111/jupyter-config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyter-config/jupyterlab_nvdashboard.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.432949 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      536 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/_version.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/apps/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/apps/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4514 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/apps/cpu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16066 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/apps/gpu.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      833 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/handlers.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2723 2022-10-31 16:14:28.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/package.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9731 2022-10-31 16:14:28.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/685.192016e9795f5c470d4e.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2022-10-31 16:14:28.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6749 2022-10-31 16:14:28.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/remoteEntry.129b3fa4c4fb94482a0f.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2022-10-31 16:14:27.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/style.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2452 2022-10-31 16:14:28.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1287 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3394 2022-10-31 16:14:29.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1338 2022-10-31 16:14:29.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-10-31 16:14:29.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2022-10-31 16:14:29.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-10-31 16:14:29.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2022-10-31 16:14:29.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2022-10-31 16:14:29.000000 jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2581 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/package.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/setup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5531 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/src/dashboard.tsx
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/src/handler.ts
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/src/index.ts
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-31 16:14:29.436949 jupyterlab_nvdashboard-0.8.0a22103111/style/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2092 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/style/base.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/style/expansion-card-variant-dark.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/style/expansion-card-variant-light.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/style/index.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/style/index.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      555 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/tsconfig.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2969 2022-10-31 16:04:34.000000 jupyterlab_nvdashboard-0.8.0a22103111/tslint.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3686 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2991 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      205 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/install.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyter-config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyter-config/jupyterlab_nvdashboard.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      536 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      459 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/_version.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4514 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/cpu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16066 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/gpu.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      833 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/handlers.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2723 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/package.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9731 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/685.192016e9795f5c470d4e.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6749 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/remoteEntry.129b3fa4c4fb94482a0f.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      165 2022-11-23 09:54:49.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/style.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2452 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1287 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.326450 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3686 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1338 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      147 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-23 09:54:50.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       23 2022-11-23 09:54:51.000000 jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2581 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/package.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      157 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5531 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/src/dashboard.tsx
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1109 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/src/handler.ts
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/src/index.ts
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-23 09:54:51.330451 jupyterlab_nvdashboard-0.8.0a22112312/style/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2092 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/base.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/expansion-card-variant-dark.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      362 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/expansion-card-variant-light.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/index.css
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/style/index.js
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      555 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/tsconfig.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2969 2022-11-23 09:47:19.000000 jupyterlab_nvdashboard-0.8.0a22112312/tslint.json
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/LICENSE` & `jupyterlab_nvdashboard-0.8.0a22112312/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/PKG-INFO` & `jupyterlab_nvdashboard-0.8.0a22112312/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nvdashboard
-Version: 0.8.0a22103111
+Version: 0.8.0a22112312
 Summary: A JupyterLab extension for displaying GPU usage dashboards
 Home-page: https://github.com/rapidsai/jupyterlab-nvdashboard
 Author: NVDashboard Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
@@ -14,19 +14,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# jupyterlab_nvdashboard
+# JupyterLab NVDashboard
+
+![GPU Dashboard](demo.gif)
 
 ![Github Actions Status](https://github.com/rapidsai/jupyterlab-nvdashboard/workflows/Build/badge.svg)
 
-A JupyterLab extension for displaying GPU usage dashboards
+NVDashboard is a JupyterLab extension for displaying GPU usage dashboards. It enables JupyterLab users to visualize system hardware metrics within the same interactive environment they use for development. Supported metrics include:
+
+- GPU-compute utilization
+- GPU-memory consumption
+- PCIe throughput
+- NVLink throughput
 
 
 This extension is composed of a Python package named `jupyterlab_nvdashboard`
 for the server extension and a NPM package named `jupyterlab-nvdashboard`
 for the frontend extension.
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/README.md` & `jupyterlab_nvdashboard-0.8.0a22112312/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,19 @@
-# jupyterlab_nvdashboard
+# JupyterLab NVDashboard
+
+![GPU Dashboard](demo.gif)
 
 ![Github Actions Status](https://github.com/rapidsai/jupyterlab-nvdashboard/workflows/Build/badge.svg)
 
-A JupyterLab extension for displaying GPU usage dashboards
+NVDashboard is a JupyterLab extension for displaying GPU usage dashboards. It enables JupyterLab users to visualize system hardware metrics within the same interactive environment they use for development. Supported metrics include:
+
+- GPU-compute utilization
+- GPU-memory consumption
+- PCIe throughput
+- NVLink throughput
 
 
 This extension is composed of a Python package named `jupyterlab_nvdashboard`
 for the server extension and a NPM package named `jupyterlab-nvdashboard`
 for the frontend extension.
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/__init__.py` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/apps/cpu.py` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/cpu.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/apps/gpu.py` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/apps/gpu.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/handlers.py` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/package.json` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/685.192016e9795f5c470d4e.js` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/685.192016e9795f5c470d4e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/747.8e5d43e699c27568a49a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/remoteEntry.129b3fa4c4fb94482a0f.js` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/remoteEntry.129b3fa4c4fb94482a0f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard/server.py` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard/server.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/PKG-INFO` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-nvdashboard
-Version: 0.8.0a22103111
+Version: 0.8.0a22112312
 Summary: A JupyterLab extension for displaying GPU usage dashboards
 Home-page: https://github.com/rapidsai/jupyterlab-nvdashboard
 Author: NVDashboard Contributors
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
@@ -14,19 +14,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# jupyterlab_nvdashboard
+# JupyterLab NVDashboard
+
+![GPU Dashboard](demo.gif)
 
 ![Github Actions Status](https://github.com/rapidsai/jupyterlab-nvdashboard/workflows/Build/badge.svg)
 
-A JupyterLab extension for displaying GPU usage dashboards
+NVDashboard is a JupyterLab extension for displaying GPU usage dashboards. It enables JupyterLab users to visualize system hardware metrics within the same interactive environment they use for development. Supported metrics include:
+
+- GPU-compute utilization
+- GPU-memory consumption
+- PCIe throughput
+- NVLink throughput
 
 
 This extension is composed of a Python package named `jupyterlab_nvdashboard`
 for the server extension and a NPM package named `jupyterlab-nvdashboard`
 for the frontend extension.
```

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/jupyterlab_nvdashboard.egg-info/SOURCES.txt` & `jupyterlab_nvdashboard-0.8.0a22112312/jupyterlab_nvdashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/package.json` & `jupyterlab_nvdashboard-0.8.0a22112312/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/setup.py` & `jupyterlab_nvdashboard-0.8.0a22112312/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/src/dashboard.tsx` & `jupyterlab_nvdashboard-0.8.0a22112312/src/dashboard.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/src/handler.ts` & `jupyterlab_nvdashboard-0.8.0a22112312/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/src/index.ts` & `jupyterlab_nvdashboard-0.8.0a22112312/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/style/base.css` & `jupyterlab_nvdashboard-0.8.0a22112312/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/tsconfig.json` & `jupyterlab_nvdashboard-0.8.0a22112312/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nvdashboard-0.8.0a22103111/tslint.json` & `jupyterlab_nvdashboard-0.8.0a22112312/tslint.json`

 * *Files identical despite different names*

