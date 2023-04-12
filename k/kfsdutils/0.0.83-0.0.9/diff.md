# Comparing `tmp/kfsdutils-0.0.83.tar.gz` & `tmp/kfsdutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsdutils-0.0.83.tar", last modified: Wed Apr 12 01:18:34 2023, max compression
+gzip compressed data, was "kfsdutils-0.0.9.tar", last modified: Sat Feb 12 00:07:52 2022, max compression
```

## Comparing `kfsdutils-0.0.83.tar` & `kfsdutils-0.0.9.tar`

### file list

```diff
@@ -1,92 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.201397 kfsdutils-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 01:18:34.197396 kfsdutils-0.0.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.189396 kfsdutils-0.0.83/kfsdutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.189396 kfsdutils-0.0.83/kfsdutils/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/core/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/core/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/templates/browser.html
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/templates/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/tests/test_apibrowserview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/docs/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/docs/views/apibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/endpoints/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/endpoints/handlers/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/handlers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/handlers/core/basehandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/endpoints/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/renderers/kubefacetstext.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/endpoints/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/serializers/basemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/endpoints/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.193396 kfsdutils-0.0.83/kfsdutils/apps/endpoints/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/endpoints/views/baseview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.197396 kfsdutils-0.0.83/kfsdutils/apps/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.197396 kfsdutils-0.0.83/kfsdutils/apps/frontend/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/handlers/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/handlers/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/handlers/tokenuser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.197396 kfsdutils-0.0.83/kfsdutils/apps/frontend/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/permissions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/permissions/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.197396 kfsdutils-0.0.83/kfsdutils/apps/frontend/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/views/baseformview.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/views/basetemplateview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/frontend/views/baseview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.197396 kfsdutils-0.0.83/kfsdutils/apps/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/middleware/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/middleware/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/middleware/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.197396 kfsdutils-0.0.83/kfsdutils/apps/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/models/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/kfsdutils/apps/models/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:18:34.189396 kfsdutils-0.0.83/kfsdutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 01:18:34.000000 kfsdutils-0.0.83/kfsdutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-12 01:18:34.000000 kfsdutils-0.0.83/kfsdutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:18:34.000000 kfsdutils-0.0.83/kfsdutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:18:33.000000 kfsdutils-0.0.83/kfsdutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 01:18:34.000000 kfsdutils-0.0.83/kfsdutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 01:18:34.000000 kfsdutils-0.0.83/kfsdutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 01:18:34.201397 kfsdutils-0.0.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-12 01:18:22.000000 kfsdutils-0.0.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    34378 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/kfsdutils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/kfsdutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/kfsdutils/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/kfsdutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/kfsdutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-12 00:07:52.000000 kfsdutils-0.0.9/kfsdutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-12 00:07:52.511787 kfsdutils-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-02-12 00:07:39.000000 kfsdutils-0.0.9/setup.py
```

### Comparing `kfsdutils-0.0.83/LICENSE` & `kfsdutils-0.0.9/LICENSE`

 * *Files identical despite different names*

