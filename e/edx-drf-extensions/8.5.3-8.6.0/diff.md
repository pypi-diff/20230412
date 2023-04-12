# Comparing `tmp/edx-drf-extensions-8.5.3.tar.gz` & `tmp/edx-drf-extensions-8.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-drf-extensions-8.5.3.tar", last modified: Tue Apr 11 16:18:48 2023, max compression
+gzip compressed data, was "edx-drf-extensions-8.6.0.tar", last modified: Wed Apr 12 20:38:48 2023, max compression
```

## Comparing `edx-drf-extensions-8.5.3.tar` & `edx-drf-extensions-8.6.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/
--rw-r--r--   0 runner    (1001) docker     (122)     5709 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9145 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/csrf/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/csrf/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9145 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-11 16:18:48.000000 edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.177679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12023 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    19910 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.181679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)    17320 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/edx_rest_framework_extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-11 16:18:48.185679 edx-drf-extensions-8.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-11 16:18:42.000000 edx-drf-extensions-8.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     6371 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9807 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/csrf/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/csrf/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.417087 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9807 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-12 20:38:48.000000 edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8634 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13020 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13147 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19910 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.421087 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17320 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/edx_rest_framework_extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-12 20:38:48.425087 edx-drf-extensions-8.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-12 20:38:45.000000 edx-drf-extensions-8.6.0/setup.py
```

### Comparing `edx-drf-extensions-8.5.3/CHANGELOG.rst` & `edx-drf-extensions-8.6.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,28 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.6.0] - 2023-04-12
+--------------------
+
+Added
+~~~~~
+
+* Added ``jwt_auth_check_symmetric_key``, ``jwt_auth_asymmetric_verified``, ``jwt_auth_symmetric_verified``, and ``jwt_auth_verification_failed`` custom attributes to aid in deprecation and removal of symmetric keys.
+* Added ``jwt_auth_issuer`` and ``jwt_auth_issuer_verification`` custom attributes.
+
+Changed
+~~~~~~~
+
+* Changed ``jwt_auth_verify_keys_count`` custom attribute to aid in key rotations, to instead be ``jwt_auth_verify_asymmetric_keys_count`` and ``jwt_auth_verify_all_keys_count``. The latter count is only used in the case that the token can't be verified with the asymmetric keys alone.
+
 [8.5.3] - 2023-04-11
 --------------------
 
 Fixed
 ~~~~~
 
 * (Hopefully) fixed the ability to publish edx-drf-extensions, by adding a ``long_description`` to setup.py. There was no real 8.5.1 or 8.5.2.
```

### Comparing `edx-drf-extensions-8.5.3/LICENSE.txt` & `edx-drf-extensions-8.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/PKG-INFO` & `edx-drf-extensions-8.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-drf-extensions
-Version: 8.5.3
+Version: 8.6.0
 Summary: edX extensions of Django REST Framework
 Home-page: https://github.com/openedx/edx-drf-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -94,14 +94,28 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.6.0] - 2023-04-12
+--------------------
+
+Added
+~~~~~
+
+* Added ``jwt_auth_check_symmetric_key``, ``jwt_auth_asymmetric_verified``, ``jwt_auth_symmetric_verified``, and ``jwt_auth_verification_failed`` custom attributes to aid in deprecation and removal of symmetric keys.
+* Added ``jwt_auth_issuer`` and ``jwt_auth_issuer_verification`` custom attributes.
+
+Changed
+~~~~~~~
+
+* Changed ``jwt_auth_verify_keys_count`` custom attribute to aid in key rotations, to instead be ``jwt_auth_verify_asymmetric_keys_count`` and ``jwt_auth_verify_all_keys_count``. The latter count is only used in the case that the token can't be verified with the asymmetric keys alone.
+
 [8.5.3] - 2023-04-11
 --------------------
 
 Fixed
 ~~~~~
 
 * (Hopefully) fixed the ability to publish edx-drf-extensions, by adding a ``long_description`` to setup.py. There was no real 8.5.1 or 8.5.2.
```

### Comparing `edx-drf-extensions-8.5.3/README.rst` & `edx-drf-extensions-8.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/csrf/api/v1/views.py` & `edx-drf-extensions-8.6.0/csrf/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/csrf/tests/test_api.py` & `edx-drf-extensions-8.6.0/csrf/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/docs/conf.py` & `edx-drf-extensions-8.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/PKG-INFO` & `edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-drf-extensions
-Version: 8.5.3
+Version: 8.6.0
 Summary: edX extensions of Django REST Framework
 Home-page: https://github.com/openedx/edx-drf-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -94,14 +94,28 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.6.0] - 2023-04-12
+--------------------
+
+Added
+~~~~~
+
+* Added ``jwt_auth_check_symmetric_key``, ``jwt_auth_asymmetric_verified``, ``jwt_auth_symmetric_verified``, and ``jwt_auth_verification_failed`` custom attributes to aid in deprecation and removal of symmetric keys.
+* Added ``jwt_auth_issuer`` and ``jwt_auth_issuer_verification`` custom attributes.
+
+Changed
+~~~~~~~
+
+* Changed ``jwt_auth_verify_keys_count`` custom attribute to aid in key rotations, to instead be ``jwt_auth_verify_asymmetric_keys_count`` and ``jwt_auth_verify_all_keys_count``. The latter count is only used in the case that the token can't be verified with the asymmetric keys alone.
+
 [8.5.3] - 2023-04-11
 --------------------
 
 Fixed
 ~~~~~
 
 * (Hopefully) fixed the ability to publish edx-drf-extensions, by adding a ``long_description`` to setup.py. There was no real 8.5.1 or 8.5.2.
```

### Comparing `edx-drf-extensions-8.5.3/edx_drf_extensions.egg-info/SOURCES.txt` & `edx-drf-extensions-8.6.0/edx_drf_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/authentication.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/authentication.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/cookies.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/decoder.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/decoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -169,26 +169,84 @@
     _verify_version(token_version)
     _set_is_restricted(token)
     _set_filters(token)
     return token
 
 
 def _verify_jwt_signature(token, jwt_issuer, decode_symmetric_token):
+    """
+    Verifies the JWT signature. Raises InvalidTokenError in the event of an error.
+
+    Arguments:
+        token (str): JWT to be decoded.
+        jwt_issuer (dict): A dict of JWT issuer related settings, containing the symmetric key.
+        decode_symmetric_token (bool): Whether to decode symmetric tokens or not. Pass False for asymmetric tokens only
+    """
+    # .. custom_attribute_name: jwt_auth_check_symmetric_key
+    # .. custom_attribute_description: True if symmetric keys will also be used for checking
+    #   the JWT signature, and False if only asymmetric keys will be used.
+    set_custom_attribute('jwt_auth_check_symmetric_key', decode_symmetric_token)
+
+    # For observability purposes, we will first try asymmetric keys only to verify
+    #   that we no longer need the symmetric key. However, if this fails, we will
+    #   continue on to the original code path and try all keys (including symmetric)
+    #   and add monitoring to let us know. This is meant to be temporary, until we
+    #   can fully retire code paths for symmetric keys, as part of
+    #   DEPR: Symmetric JWTs: https://github.com/openedx/public-engineering/issues/83
+
+    # Use add_symmetric_keys=False to only include asymmetric keys at first
+    key_set = _get_signing_jwk_key_set(jwt_issuer, add_symmetric_keys=False)
+    # .. custom_attribute_name: jwt_auth_verify_asymmetric_keys_count
+    # .. custom_attribute_description: Number of JWT verification keys in use for this
+    #   verification. Should be same as number of asymmetric public keys. This is
+    #   intended to aid in key rotations; once the average count stabilizes at a
+    #   higher number after adding a public key, it should be safe to change the secret key.
+    set_custom_attribute('jwt_auth_verify_asymmetric_keys_count', len(key_set))
+
+    try:
+        _ = JWS().verify_compact(token, key_set)
+        # .. custom_attribute_name: jwt_auth_asymmetric_verified
+        # .. custom_attribute_description: Whether the JWT was successfully verified
+        #   using an asymmetric key.
+        set_custom_attribute('jwt_auth_asymmetric_verified', True)
+        return
+    except Exception:  # pylint: disable=broad-except
+        # Continue to the old code path of trying all keys
+        pass
+
+    # The following is the original code that includes both the symmetric and asymmetric keys
+    #   as requested with the decode_symmetric_token argument. Note that the check against
+    #   the asymmetric keys here is redundant and unnecessary, but this code is temporary and
+    #   will be simplified once symmetric keys have been fully retired.
+
     key_set = _get_signing_jwk_key_set(jwt_issuer, add_symmetric_keys=decode_symmetric_token)
-    # .. custom_attribute_name: jwt_auth_verify_keys_count
+    # .. custom_attribute_name: jwt_auth_verify_all_keys_count
     # .. custom_attribute_description: Number of JWT verification keys in use for this
     #   verification. Should be same as number of asymmetric public keys, plus one if
     #   a symmetric key secret is set. This is intended to aid in key rotations; once
     #   the average count stabilizes at a higher number after adding a public key, it
     #   should be safe to change the secret key.
-    set_custom_attribute('jwt_auth_verify_keys_count', len(key_set))
+    set_custom_attribute('jwt_auth_verify_all_keys_count', len(key_set))
 
     try:
         _ = JWS().verify_compact(token, key_set)
+        # .. custom_attribute_name: jwt_auth_symmetric_verified
+        # .. custom_attribute_description: Whether the JWT was successfully verified
+        #   using a symmetric key.
+        # Note: Rather than using a single custom attribute like ``jwt_auth_verified``
+        #   with values of 'symmetric' or 'asymmetric', we use two separate custom
+        #   attribute names (e.g. jwt_auth_symmetric_verified and jwt_auth_asymmetric_verified),
+        #   so that if each of these were set separately in the same request, they
+        #   wouldn't clobber each other.
+        set_custom_attribute('jwt_auth_symmetric_verified', True)
+        return
     except Exception as token_error:
+        # .. custom_attribute_name: jwt_auth_verification_failed
+        # .. custom_attribute_description: True if the JWT token verification failed.
+        set_custom_attribute('jwt_auth_verification_failed', True)
         logger.exception('Token verification failed.')
         exc_info = sys.exc_info()
         raise jwt.InvalidTokenError(exc_info[2]) from token_error
 
 
 def _decode_and_verify_token(token, jwt_issuer):
     """
@@ -212,16 +270,27 @@
         audience=jwt_issuer['AUDIENCE'],
         issuer=jwt_issuer['ISSUER'],
         algorithms=[api_settings.JWT_ALGORITHM],
     )
 
     # TODO (ARCH-204): verify issuer manually until it is properly configured.
     token_issuer = decoded_token.get('iss')
+    # .. custom_attribute_name: jwt_auth_issuer
+    # .. custom_attribute_description: Value set to the JWT auth issuer.
+    set_custom_attribute('jwt_auth_issuer', token_issuer)
     issuer_matched = any(issuer['ISSUER'] == token_issuer for issuer in get_jwt_issuers())
-    if not issuer_matched:
+    if token_issuer == jwt_issuer['ISSUER']:
+        # .. custom_attribute_name: jwt_auth_issuer_verification
+        # .. custom_attribute_description: Depending on issuer verification, the value will
+        #   be one of: matches-first-issuer, matches-later-issuer, or no-match.
+        set_custom_attribute('jwt_auth_issuer_verification', 'matches-first-issuer')
+    elif issuer_matched:
+        set_custom_attribute('jwt_auth_issuer_verification', 'matches-later-issuer')
+    else:
+        set_custom_attribute('jwt_auth_issuer_verification', 'no-match')
         logger.info('Token decode failed due to mismatched issuer [%s]', token_issuer)
         raise jwt.InvalidTokenError('%s is not a valid issuer.' % token_issuer)
 
     return decoded_token
 
 
 def _get_signing_jwk_key_set(jwt_issuer, add_symmetric_keys=True):
```

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/middleware.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,28 +196,46 @@
         """
         Validates that a valid asymmetric token is properly decoded
         """
         token = generate_asymmetric_jwt_token(self.payload)
         self.assertEqual(get_asymmetric_only_jwt_decode_handler(token), self.payload)
 
     @mock.patch('edx_rest_framework_extensions.auth.jwt.decoder.set_custom_attribute')
-    def test_keyset_size_monitoring(self, mock_set_custom_attribute):
+    def test_keyset_size_and_other_monitoring(self, mock_set_custom_attribute):
         """
-        Validates that a custom attribute is recorded for the keyset size.
+        Validates a variety of custom attributes are recorded, including the keyset size.
         """
-        token = generate_asymmetric_jwt_token(self.payload)
+        asymmetric_token = generate_asymmetric_jwt_token(self.payload)
+        symmetric_token = generate_jwt_token(self.payload)
 
         # The secret key is included by default making a list of length 2, but for
         # asymmetric-only there is only 1 key in the keyset.
-        self.assertEqual(jwt_decode_handler(token), self.payload)
-        self.assertEqual(get_asymmetric_only_jwt_decode_handler(token), self.payload)
+        self.assertEqual(jwt_decode_handler(asymmetric_token), self.payload)
+        self.assertEqual(get_asymmetric_only_jwt_decode_handler(asymmetric_token), self.payload)
+        self.assertEqual(jwt_decode_handler(symmetric_token), self.payload)
 
         assert mock_set_custom_attribute.call_args_list == [
-            mock.call('jwt_auth_verify_keys_count', 2),
-            mock.call('jwt_auth_verify_keys_count', 1),
+            mock.call('jwt_auth_check_symmetric_key', True),
+            mock.call('jwt_auth_verify_asymmetric_keys_count', 1),
+            mock.call('jwt_auth_asymmetric_verified', True),
+            mock.call('jwt_auth_issuer', 'test-issuer-1'),
+            mock.call('jwt_auth_issuer_verification', 'matches-first-issuer'),
+
+            mock.call('jwt_auth_check_symmetric_key', False),
+            mock.call('jwt_auth_verify_asymmetric_keys_count', 1),
+            mock.call('jwt_auth_asymmetric_verified', True),
+            mock.call('jwt_auth_issuer', 'test-issuer-1'),
+            mock.call('jwt_auth_issuer_verification', 'matches-first-issuer'),
+
+            mock.call('jwt_auth_check_symmetric_key', True),
+            mock.call('jwt_auth_verify_asymmetric_keys_count', 1),
+            mock.call('jwt_auth_verify_all_keys_count', 2),
+            mock.call('jwt_auth_symmetric_verified', True),
+            mock.call('jwt_auth_issuer', 'test-issuer-1'),
+            mock.call('jwt_auth_issuer_verification', 'matches-first-issuer'),
         ]
 
 
 def _jwt_decode_handler_with_defaults(token):  # pylint: disable=unused-argument
     """
     Accepts anything as a token and returns a fake JWT payload with defaults.
     """
```

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/jwt/tests/utils.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/authentication.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/auth/session/tests/test_authentication.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/config.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/config.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/middleware.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/paginators.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/permissions.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/settings.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_middleware.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_paginators.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_permissions.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/edx_rest_framework_extensions/tests/test_settings.py` & `edx-drf-extensions-8.6.0/edx_rest_framework_extensions/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/requirements/constraints.txt` & `edx-drf-extensions-8.6.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.5.3/setup.py` & `edx-drf-extensions-8.6.0/setup.py`

 * *Files identical despite different names*

