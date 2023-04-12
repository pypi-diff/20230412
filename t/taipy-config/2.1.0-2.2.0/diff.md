# Comparing `tmp/taipy-config-2.1.0.tar.gz` & `tmp/taipy-config-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-config-2.1.0.tar", last modified: Tue Jan 31 09:57:49 2023, max compression
+gzip compressed data, was "taipy-config-2.2.0.tar", last modified: Wed Apr 12 08:49:33 2023, max compression
```

## Comparing `taipy-config-2.1.0.tar` & `taipy-config-2.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.040584 taipy-config-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-01-31 09:57:36.000000 taipy-config-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-31 09:57:36.000000 taipy-config-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-01-31 09:57:49.040584 taipy-config-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-01-31 09:57:36.000000 taipy-config-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 09:57:49.040584 taipy-config-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-01-31 09:57:36.000000 taipy-config-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.032584 taipy-config-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.036584 taipy-config-2.1.0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.036584 taipy-config-2.1.0/src/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/_base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/_config_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/_json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/_toml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.036584 taipy-config-2.1.0/src/taipy/config/checker/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.036584 taipy-config-2.1.0/src/taipy/config/checker/_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/_checkers/_auth_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/_checkers/_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/checker/issue_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.040584 taipy-config-2.1.0/src/taipy/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/_classproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/_config_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/_template_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/_validate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/common/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    33812 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.040584 taipy-config-2.1.0/src/taipy/config/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.040584 taipy-config-2.1.0/src/taipy/config/global_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/global_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/global_app/global_app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/section.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/unique_section.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.040584 taipy-config-2.1.0/src/taipy/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-01-31 09:57:36.000000 taipy-config-2.1.0/src/taipy/logger/_taipy_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:57:49.040584 taipy-config-2.1.0/src/taipy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-01-31 09:57:49.000000 taipy-config-2.1.0/src/taipy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-01-31 09:57:49.000000 taipy-config-2.1.0/src/taipy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 09:57:49.000000 taipy-config-2.1.0/src/taipy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 09:57:42.000000 taipy-config-2.1.0/src/taipy_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-31 09:57:49.000000 taipy-config-2.1.0/src/taipy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-31 09:57:49.000000 taipy-config-2.1.0/src/taipy_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.866582 taipy-config-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-12 08:49:19.000000 taipy-config-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 08:49:19.000000 taipy-config-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-12 08:49:33.866582 taipy-config-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-12 08:49:19.000000 taipy-config-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:49:33.866582 taipy-config-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 08:49:19.000000 taipy-config-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.846582 taipy-config-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.850582 taipy-config-2.2.0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.854582 taipy-config-2.2.0/src/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_config_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/_toml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.854582 taipy-config-2.2.0/src/taipy/config/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.858582 taipy-config-2.2.0/src/taipy/config/checker/_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/_auth_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/checker/issue_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_config_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_template_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/_validate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/common/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33812 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/config/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/config/global_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/global_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/global_app/global_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/unique_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.862582 taipy-config-2.2.0/src/taipy/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-12 08:49:19.000000 taipy-config-2.2.0/src/taipy/logger/_taipy_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:33.866582 taipy-config-2.2.0/src/taipy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:49:25.000000 taipy-config-2.2.0/src/taipy_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 08:49:33.000000 taipy-config-2.2.0/src/taipy_config.egg-info/top_level.txt
```

### Comparing `taipy-config-2.1.0/LICENSE` & `taipy-config-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/PKG-INFO` & `taipy-config-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.1.0
+Version: 2.2.0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.1.0/README.md` & `taipy-config-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/setup.py` & `taipy-config-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/__init__.py` & `taipy-config-2.2.0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/__init__.py` & `taipy-config-2.2.0/src/taipy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/_base_serializer.py` & `taipy-config-2.2.0/src/taipy/config/_base_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/_config.py` & `taipy-config-2.2.0/src/taipy/config/_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/_config_comparator.py` & `taipy-config-2.2.0/src/taipy/config/_config_comparator.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/_json_serializer.py` & `taipy-config-2.2.0/src/taipy/config/_json_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/_toml_serializer.py` & `taipy-config-2.2.0/src/taipy/config/_toml_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/__init__.py` & `taipy-config-2.2.0/src/taipy/config/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/_checker.py` & `taipy-config-2.2.0/src/taipy/config/checker/_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/_checkers/__init__.py` & `taipy-config-2.2.0/src/taipy/config/checker/_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/_checkers/_auth_config_checker.py` & `taipy-config-2.2.0/src/taipy/config/checker/_checkers/_auth_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/_checkers/_config_checker.py` & `taipy-config-2.2.0/src/taipy/config/checker/_checkers/_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py` & `taipy-config-2.2.0/src/taipy/config/checker/_checkers/_gLobal_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/issue.py` & `taipy-config-2.2.0/src/taipy/config/checker/issue.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/checker/issue_collector.py` & `taipy-config-2.2.0/src/taipy/config/checker/issue_collector.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/_argparser.py` & `taipy-config-2.2.0/src/taipy/config/common/_argparser.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/_classproperty.py` & `taipy-config-2.2.0/src/taipy/config/common/_classproperty.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/_config_blocker.py` & `taipy-config-2.2.0/src/taipy/config/common/_config_blocker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/_repr_enum.py` & `taipy-config-2.2.0/src/taipy/config/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/_template_handler.py` & `taipy-config-2.2.0/src/taipy/config/common/_template_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/_validate_id.py` & `taipy-config-2.2.0/src/taipy/config/common/_validate_id.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/frequency.py` & `taipy-config-2.2.0/src/taipy/config/common/frequency.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/common/scope.py` & `taipy-config-2.2.0/src/taipy/config/common/scope.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/config.py` & `taipy-config-2.2.0/src/taipy/config/config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/config.pyi` & `taipy-config-2.2.0/src/taipy/config/config.pyi`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/exceptions/__init__.py` & `taipy-config-2.2.0/src/taipy/config/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/exceptions/exceptions.py` & `taipy-config-2.2.0/src/taipy/config/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/global_app/global_app_config.py` & `taipy-config-2.2.0/src/taipy/config/global_app/global_app_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/section.py` & `taipy-config-2.2.0/src/taipy/config/section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/config/unique_section.py` & `taipy-config-2.2.0/src/taipy/config/unique_section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/logger/__init__.py` & `taipy-config-2.2.0/src/taipy/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy/logger/_taipy_logger.py` & `taipy-config-2.2.0/src/taipy/logger/_taipy_logger.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.1.0/src/taipy_config.egg-info/PKG-INFO` & `taipy-config-2.2.0/src/taipy_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.1.0
+Version: 2.2.0
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.1.0/src/taipy_config.egg-info/SOURCES.txt` & `taipy-config-2.2.0/src/taipy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

