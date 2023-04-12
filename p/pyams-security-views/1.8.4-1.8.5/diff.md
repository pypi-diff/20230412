# Comparing `tmp/pyams_security_views-1.8.4.tar.gz` & `tmp/pyams_security_views-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_security_views-1.8.4.tar", last modified: Mon Dec 26 23:56:07 2022, max compression
+gzip compressed data, was "dist/pyams_security_views-1.8.5.tar", last modified: Wed Apr 12 16:58:00 2023, max compression
```

## Comparing `pyams_security_views-1.8.4.tar` & `pyams_security_views-1.8.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3988 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/docs/
--rwxrwxrwx   0 root         (0) root         (0)     2309 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1115 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2598 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/
--rw-rw-rw-   0 root         (0) root         (0)      894 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/api/
--rw-rw-rw-   0 root         (0) root         (0)      570 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3323 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/api/principal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    10307 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1337 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      596 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2894 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/interfaces/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9380 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo
--rw-rw-rw-   0 root         (0) root         (0)    15388 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po
--rw-rw-rw-   0 root         (0) root         (0)    10813 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/locales/pyams_security_views.pot
--rw-rw-rw-   0 root         (0) root         (0)     2135 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/login.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/skin/
--rw-rw-rw-   0 root         (0) root         (0)      571 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10446 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/skin/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      299 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/skin/templates/login-logo.pt
--rw-rw-rw-   0 root         (0) root         (0)       81 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/skin/templates/login-viewlet.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/tests/
--rw-rw-rw-   0 root         (0) root         (0)      809 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/widget/
--rw-rw-rw-   0 root         (0) root         (0)      573 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/widget/permission.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/widget/principal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7022 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3229 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/login.py
--rw-rw-rw-   0 root         (0) root         (0)     4652 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3237 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     7112 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4196 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     8987 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/group.py
--rw-rw-rw-   0 root         (0) root         (0)    20959 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/userfolder.py
--rw-rw-rw-   0 root         (0) root         (0)     5900 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     3578 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2022-12-26 23:55:47.000000 pyams_security_views-1.8.4/src/pyams_security_views/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3988 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1998 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      259 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-26 23:56:07.000000 pyams_security_views-1.8.4/src/pyams_security_views.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4070 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     2391 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2643 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/api/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/api/principal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    10432 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2894 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/interfaces/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9151 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo
+-rw-rw-rw-   0 root         (0) root         (0)    15221 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po
+-rw-rw-rw-   0 root         (0) root         (0)    10468 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/locales/pyams_security_views.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10446 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/templates/login-logo.pt
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/skin/templates/login-viewlet.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1885 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/permission.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/widget/principal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7022 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3229 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     4652 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/notifications.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4196 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/group.py
+-rw-rw-rw-   0 root         (0) root         (0)    20959 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/userfolder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2714 2023-04-12 16:57:37.000000 pyams_security_views-1.8.5/src/pyams_security_views/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4070 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 16:58:00.000000 pyams_security_views-1.8.5/src/pyams_security_views.egg-info/top_level.txt
```

### Comparing `pyams_security_views-1.8.4/LICENSE` & `pyams_security_views-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/PKG-INFO` & `pyams_security_views-1.8.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_security_views
-Version: 1.8.4
+Version: 1.8.5
 Summary: Pyramid views for PyAMS_security package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -46,14 +46,18 @@
 interface (based on PyAMS_zmi package), custom widgets and a small Cornice REST API to look for
 principals.
 
 
 Changelog
 =========
 
+1.8.5
+-----
+ - refactored Colander API schemas for better OpenAPI specifications
+
 1.8.4
 -----
  - updated login form templates
  - added support for Python 3.11
 
 1.8.3
 -----
```

### Comparing `pyams_security_views-1.8.4/docs/HISTORY.rst` & `pyams_security_views-1.8.5/docs/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.8.5
+-----
+ - refactored Colander API schemas for better OpenAPI specifications
+
 1.8.4
 -----
  - updated login form templates
  - added support for Python 3.11
 
 1.8.3
 -----
```

### Comparing `pyams_security_views-1.8.4/docs/README.rst` & `pyams_security_views-1.8.5/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/setup.py` & `pyams_security_views-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.8.4'
+version = '1.8.5'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
+    'cornice_swagger',
     'pyams_i18n_views',
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
 
 setup(name='pyams_security_views',
@@ -59,14 +60,15 @@
       # uncomment this to be able to run tests with setup.py
       test_suite="pyams_security_views.tests.test_utilsdocs.test_suite",
       tests_require=tests_require,
       extras_require=dict(test=tests_require),
       install_requires=[
           'setuptools',
           # -*- Extra requirements: -*-
+          'colander',
           'cornice',
           'persistent',
           'pyams_file',
           'pyams_i18n',
           'pyams_security',
           'pyams_site',
           'pyams_skin',
```

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/api/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/api/principal.py` & `pyams_security_views-1.8.5/src/pyams_security_views/api/principal.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,93 +13,98 @@
 """PyAMS_security_views.api.principal module
 
 This module only provides a small Cornice API to search for principals.
 """
 
 import sys
 
-from colander import MappingSchema, SchemaNode, SequenceSchema, String
+from colander import MappingSchema, SchemaNode, SequenceSchema, String, drop
 from cornice import Service
-from cornice.validators import colander_querystring_validator
+from cornice.validators import colander_validator
 from pyramid.httpexceptions import HTTPOk
 
 from pyams_security.interfaces import ISecurityManager
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_security.rest import check_cors_origin, set_cors_headers
 from pyams_security_views.interfaces import REST_PRINCIPALS_SEARCH_ROUTE
 from pyams_utils.registry import query_utility
+from pyams_utils.rest import BaseResponseSchema, STATUS, rest_responses
 
 
 __docformat__ = 'restructuredtext'
 
-from pyams_security_views import _  # pylint: disable=ungrouped-imports
-
 
 TEST_MODE = sys.argv[-1].endswith('/test')
 
 
-class PrincipalsSearchQuerySchema(MappingSchema):
-    """Principals search schema"""
+class PrincipalsSearchQuery(MappingSchema):
+    """Principals search query"""
     term = SchemaNode(String(),
-                      description=_("Principals search string"))
+                      description="Principals search string")
 
 
-class PrincipalResultSchema(MappingSchema):
+class Principal(MappingSchema):
     """Principal result schema"""
     id = SchemaNode(String(),
-                    description=_("Principal ID"))
+                    description="Principal ID")
     text = SchemaNode(String(),
-                      description=_("Principal title"))
+                      description="Principal title")
 
 
-class PrincipalsSearchResults(SequenceSchema):
+class PrincipalsList(SequenceSchema):
     """Principals search results interface"""
-    result = PrincipalResultSchema()
+    result = Principal()
 
 
-class PrincipalsSearchResultsSchema(MappingSchema):
+class PrincipalsSearchResults(BaseResponseSchema):
     """Principals search results schema"""
-    results = PrincipalsSearchResults(description=_("Results list"))
-
+    results = PrincipalsList(description="List of principals matching input term",
+                             missing=drop)
 
-search_responses = {
-    HTTPOk.code: PrincipalsSearchResultsSchema(description=_("Search results")),
-}
-if TEST_MODE:
-    service_params = {}
-else:
-    service_params = {
-        'response_schemas': search_responses
-    }
 
+principals_service = Service(name=REST_PRINCIPALS_SEARCH_ROUTE,
+                             pyramid_route=REST_PRINCIPALS_SEARCH_ROUTE,
+                             description="Principals management")
 
-service = Service(name=REST_PRINCIPALS_SEARCH_ROUTE,
-                  pyramid_route=REST_PRINCIPALS_SEARCH_ROUTE,
-                  description="Principals management")
 
-
-@service.options(validators=(check_cors_origin, set_cors_headers),
-                 **service_params)
+@principals_service.options(validators=(check_cors_origin, set_cors_headers))
 def principals_options(request):  # pylint: disable=unused-argument
     """Principals service options"""
     return ''
 
 
-@service.get(permission=VIEW_SYSTEM_PERMISSION,
-             schema=PrincipalsSearchQuerySchema(),
-             validators=(check_cors_origin, colander_querystring_validator, set_cors_headers),
-             **service_params)
+class PrincipalsSearchRequest(MappingSchema):
+    """Principals search request"""
+    querystring = PrincipalsSearchQuery()
+
+
+class PrincipalsGetterResponse(MappingSchema):
+    """Principals getter response"""
+    body = PrincipalsSearchResults()
+
+
+principals_get_responses = rest_responses.copy()
+principals_get_responses[HTTPOk.code] = PrincipalsGetterResponse(
+    description="Search results")
+
+
+@principals_service.get(permission=VIEW_SYSTEM_PERMISSION,
+                        schema=PrincipalsSearchRequest(),
+                        validators=(check_cors_origin, colander_validator, set_cors_headers),
+                        response_schemas=principals_get_responses)
 def get_principals(request):
     """Returns list of principals matching given query"""
-    if TEST_MODE:
-        query = request.params.get('term')
-    else:
-        query = request.validated.get('term')
+    params = request.params if TEST_MODE else request.validated.get('querystring', {})
+    query = params.get('term')
     if not query:
-        return []
+        return {
+            'status': STATUS.ERROR.value,
+            'message': "Missing arguments"
+        }
     manager = query_utility(ISecurityManager)
     return {
+        'status': STATUS.SUCCESS.value,
         'results': [{
             'id': principal.id,
             'text': principal.title
         } for principal in manager.find_principals(query)]
     }
```

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/doctests/README.rst` & `pyams_security_views-1.8.5/src/pyams_security_views/doctests/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     >>> config = setUp(hook_zca=True)
     >>> config.registry.settings['zodbconn.uri'] = 'memory://'
 
     >>> from pyramid_zodbconn import includeme as include_zodbconn
     >>> include_zodbconn(config)
     >>> from cornice import includeme as include_cornice
     >>> include_cornice(config)
+    >>> from cornice_swagger import includeme as include_swagger
+    >>> include_swagger(config)
     >>> from pyams_utils import includeme as include_utils
     >>> include_utils(config)
     >>> from pyams_viewlet import includeme as include_viewlet
     >>> include_viewlet(config)
     >>> from pyams_site import includeme as include_site
     >>> include_site(config)
     >>> from pyams_security import includeme as include_security
@@ -140,26 +142,27 @@
             multiple="multiple"
             size="1"
             data-placeholder="No selected principal"
             data-ajax--url="/api/security/principals"
             readonly="readonly">
             <option></option>
     </select>
-    <input name="form.widgets.managers-empty-marker" type="hidden" value="1"/>
+    <input name="form.widgets.managers-empty-marker" type="hidden" value="1" />
 
     >>> output = form.render()
 
 
 Principals searching API
 ------------------------
 
     >>> from pyams_security_views.api.principal import get_principals
     >>> request = DummyRequest(params={'term': 'admin'})
     >>> pprint.pprint(get_principals(request))
-    {'results': [{'id': 'system:admin', 'text': 'System manager authentication'}]}
+    {'results': [{'id': 'system:admin', 'text': 'System manager authentication'}],
+     'status': 'success'}
 
 
 Login form configuration edit form
 ----------------------------------
 
     >>> request = DummyRequest(context=app)
     >>> alsoProvides(request, IAdminLayer)
@@ -233,15 +236,15 @@
                     </label>
                     <div class="col-sm-9 col-md-8">
                         <div class="form-widget ">
                             <input type="password"
                                    id="login_form-widgets-password"
                                    name="login_form.widgets.password"
                                    class="form-control password-widget required password-field"
-                                   value="*****"/>
+                                   value="*****" />
                         </div>
                     </div>
                 </div>
             </fieldset>
             <footer>
                 <button
                     type="submit"
```

#### html2text {}

```diff
@@ -1,62 +1,64 @@
 ============================ PyAMS security views package
 ============================ Introduction ------------ This package is composed
 of a set of utility functions, usable into any Pyramid application. >>> import
 pprint >>> from pyramid.testing import setUp, tearDown, DummyRequest >>> config
 = setUp(hook_zca=True) >>> config.registry.settings['zodbconn.uri'] = 'memory:/
 /' >>> from pyramid_zodbconn import includeme as include_zodbconn >>>
 include_zodbconn(config) >>> from cornice import includeme as include_cornice
->>> include_cornice(config) >>> from pyams_utils import includeme as
-include_utils >>> include_utils(config) >>> from pyams_viewlet import includeme
-as include_viewlet >>> include_viewlet(config) >>> from pyams_site import
-includeme as include_site >>> include_site(config) >>> from pyams_security
-import includeme as include_security >>> include_security(config) >>> from
-pyams_form import includeme as include_form >>> include_form(config) >>> from
-pyams_skin import includeme as include_skin >>> include_skin(config) >>> from
-pyams_zmi import includeme as include_zmi >>> include_zmi(config) >>> from
-pyams_security_views import includeme as include_security_views >>>
-include_security_views(config) >>> from pyams_i18n_views import includeme as
-include_i18n_view >>> include_i18n_view(config) >>> from pyams_utils.registry
-import get_utility, set_local_registry >>> registry = config.registry >>>
-set_local_registry(registry) >>> from pyams_site.generations import
-upgrade_site >>> request = DummyRequest() >>> app = upgrade_site(request)
-Upgrading PyAMS timezone to generation 1... Upgrading PyAMS security to
-generation 2... >>> from zope.traversing.interfaces import BeforeTraverseEvent
->>> from pyams_utils.registry import handle_site_before_traverse >>>
-handle_site_before_traverse(BeforeTraverseEvent(app, request)) >>> from
-pyams_security.interfaces import ISecurityManager >>> sm = get_utility
-(ISecurityManager) Security manager properties edit form ----------------------
---------------- >>> from zope.interface import alsoProvides >>> from
-pyams_zmi.interfaces import IAdminLayer >>> request = DummyRequest(context=app)
->>> alsoProvides(request, IAdminLayer) >>> from
+>>> include_cornice(config) >>> from cornice_swagger import includeme as
+include_swagger >>> include_swagger(config) >>> from pyams_utils import
+includeme as include_utils >>> include_utils(config) >>> from pyams_viewlet
+import includeme as include_viewlet >>> include_viewlet(config) >>> from
+pyams_site import includeme as include_site >>> include_site(config) >>> from
+pyams_security import includeme as include_security >>> include_security
+(config) >>> from pyams_form import includeme as include_form >>> include_form
+(config) >>> from pyams_skin import includeme as include_skin >>> include_skin
+(config) >>> from pyams_zmi import includeme as include_zmi >>> include_zmi
+(config) >>> from pyams_security_views import includeme as
+include_security_views >>> include_security_views(config) >>> from
+pyams_i18n_views import includeme as include_i18n_view >>> include_i18n_view
+(config) >>> from pyams_utils.registry import get_utility, set_local_registry
+>>> registry = config.registry >>> set_local_registry(registry) >>> from
+pyams_site.generations import upgrade_site >>> request = DummyRequest() >>> app
+= upgrade_site(request) Upgrading PyAMS timezone to generation 1... Upgrading
+PyAMS security to generation 2... >>> from zope.traversing.interfaces import
+BeforeTraverseEvent >>> from pyams_utils.registry import
+handle_site_before_traverse >>> handle_site_before_traverse(BeforeTraverseEvent
+(app, request)) >>> from pyams_security.interfaces import ISecurityManager >>>
+sm = get_utility(ISecurityManager) Security manager properties edit form ------
+------------------------------- >>> from zope.interface import alsoProvides >>>
+from pyams_zmi.interfaces import IAdminLayer >>> request = DummyRequest
+(context=app) >>> alsoProvides(request, IAdminLayer) >>> from
 pyams_security_views.zmi.manager import SecurityPropertiesEditForm >>> form =
 SecurityPropertiesEditForm(sm, request) >>> form.update() >>> form.widgets.keys
 () odict_keys(['credentials_plugins_names', 'authentication_plugins_names',
 'directory_plugins_names']) >>> print(form.widgets
 ['credentials_plugins_names'].render())
 >>> print(form.widgets['authentication_plugins_names'].render())
  System manager authentication
  internal service
   >>> output = form.render() Principals searching API -----------------------
 - >>> from pyams_security_views.api.principal import get_principals >>> request
 = DummyRequest(params={'term': 'admin'}) >>> pprint.pprint(get_principals
 (request)) {'results': [{'id': 'system:admin', 'text': 'System manager
-authentication'}]} Login form configuration edit form -------------------------
---------- >>> request = DummyRequest(context=app) >>> alsoProvides(request,
-IAdminLayer) >>> from pyams_security_views.zmi.login import
-LoginFormConfigurationForm >>> form = LoginFormConfigurationForm(app, request)
->>> form.update() >>> form.widgets.keys() odict_keys(['logo', 'header',
-'header_renderer', 'footer', 'footer_renderer']) >>> output = form.render()
-Login form ---------- >>> from pyams_layer.interfaces import IPyAMSLayer >>>
-from pyams_security_views.skin.login import LoginForm >>> request =
-DummyRequest(is_xhr=False, params={ ... 'login_form.widgets.login': 'admin',
-... 'login_form.widgets.password': 'admin', ... 'login_form.buttons.login':
-'Connect' ... }) >>> alsoProvides(request, IPyAMSLayer) >>> form = LoginForm
-(app, request) >>> form.update() >>> form.widgets.keys() odict_keys(['hash',
-'login', 'password']) >>> output = form.render() >>> print(output)
+authentication'}], 'status': 'success'} Login form configuration edit form ----
+------------------------------ >>> request = DummyRequest(context=app) >>>
+alsoProvides(request, IAdminLayer) >>> from pyams_security_views.zmi.login
+import LoginFormConfigurationForm >>> form = LoginFormConfigurationForm(app,
+request) >>> form.update() >>> form.widgets.keys() odict_keys(['logo',
+'header', 'header_renderer', 'footer', 'footer_renderer']) >>> output =
+form.render() Login form ---------- >>> from pyams_layer.interfaces import
+IPyAMSLayer >>> from pyams_security_views.skin.login import LoginForm >>>
+request = DummyRequest(is_xhr=False, params={ ... 'login_form.widgets.login':
+'admin', ... 'login_form.widgets.password': 'admin', ...
+'login_form.buttons.login': 'Connect' ... }) >>> alsoProvides(request,
+IPyAMSLayer) >>> form = LoginForm(app, request) >>> form.update() >>>
+form.widgets.keys() odict_keys(['hash', 'login', 'password']) >>> output =
+form.render() >>> print(output)
 ***** You must authenticate *****
  Please enter valid credentials
  Login
 [admin               ]
  Password
 [********************]
   Connect Reset
```

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/include.py` & `pyams_security_views-1.8.5/src/pyams_security_views/include.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/interfaces/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/interfaces/login.py` & `pyams_security_views-1.8.5/src/pyams_security_views/interfaces/login.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo` & `pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -218,23 +218,14 @@
 
 msgid "Plug-in properties"
 msgstr "Propriétés du module"
 
 msgid "Plug-in: {}"
 msgstr "Module : {}"
 
-msgid "Principal ID"
-msgstr "ID du mandataire"
-
-msgid "Principal title"
-msgstr "Libellé du mandataire"
-
-msgid "Principals search string"
-msgstr "Requête de recherche des mandataires"
-
 msgid "Properties"
 msgstr "Propriétés"
 
 msgid "Re-enable user profile"
 msgstr "Ré-activer le compte"
 
 msgid "Redirection hash"
@@ -245,17 +236,14 @@
 
 msgid "Refresh secret"
 msgstr "Réinitialiser le secret"
 
 msgid "Reset"
 msgstr "Annuler"
 
-msgid "Results list"
-msgstr "Liste de résultats"
-
 msgid "Roles are not defined for this context!"
 msgstr "Aucun rôle n'est défini dans ce contexte !"
 
 msgid "Search into folder"
 msgstr "Rechercher dans le dossier"
 
 msgid "Search results"
```

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po` & `pyams_security_views-1.8.5/src/pyams_security_views/locales/fr/LC_MESSAGES/pyams_security_views.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2022-05-16 10:51+0200\n"
+"POT-Creation-Date: 2023-04-12 16:00+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 3.10.dev0\n"
 
 #: src/pyams_security_views/widget/principal.py:71
 msgid "No selected principal"
 msgstr "Aucun mandataire sélectionné"
 
-#: src/pyams_security_views/zmi/rest.py:50
-#: src/pyams_security_views/zmi/rest.py:60
+#: src/pyams_security_views/zmi/rest.py:51
+#: src/pyams_security_views/zmi/rest.py:61
 msgid "CORS configuration"
 msgstr "Configuration CORS"
 
-#: src/pyams_security_views/zmi/rest.py:91
+#: src/pyams_security_views/zmi/rest.py:96
 msgid ""
 "If you disable CORS origins check, any CORS request will be accepted.\n"
 "Otherwise, only origins specified below will be allowed.\n"
 "Please note that you don't have to set main site URL(s) below, only "
 "\"external\" URLs have to be defined."
 msgstr ""
-"Si vous désactivez le contrôle sur l'origine des requêtes, toutes les requêtes "
-"CORS seront acceptées !\n"
-"Dans le cas contraire, seules les requêtes dont l'origine est indiquée ci-dessous "
-"seront acceptées.\n"
-"Veuillez noter que vous n'avez pas à indiquer l'URL d'accès au site, celle-ci "
-"sera toujours acceptée ; seules les origines \"externes\" doivent être précisées."
+"Si vous désactivez le contrôle sur l'origine des requêtes, toutes les "
+"requêtes CORS seront acceptées !\n"
+"Dans le cas contraire, seules les requêtes dont l'origine est indiquée ci-"
+"dessous seront acceptées.\n"
+"Veuillez noter que vous n'avez pas à indiquer l'URL d'accès au site, celle-"
+"ci sera toujours acceptée ; seules les origines \"externes\" doivent être "
+"précisées."
 
 #: src/pyams_security_views/zmi/notifications.py:50
 msgid "Notifications"
 msgstr "Notifications"
 
 #: src/pyams_security_views/zmi/notifications.py:60
 msgid "Notifications settings"
@@ -56,38 +57,39 @@
 "Elles sont notamment nécessaires pour prendre en charge leur processus "
 "d'enregistrement, aussi bien lorsqu'il s'agit d'une inscription publique (si "
 "vous activez cette option) que dans le cadre d'un enregistrement par un "
 "administrateur.\n"
 "Les applications peuvent également envoyer des messages dans le cadre de "
 "leur processus de fonctionnement normal."
 
-#: src/pyams_security_views/zmi/policy.py:58
-#: src/pyams_security_views/zmi/policy.py:68
+#: src/pyams_security_views/zmi/policy.py:59
+#: src/pyams_security_views/zmi/policy.py:98
+#: src/pyams_security_views/zmi/policy.py:112
 msgid "User roles"
 msgstr "Habilitations"
 
-#: src/pyams_security_views/zmi/policy.py:69
+#: src/pyams_security_views/zmi/policy.py:67
 msgid "Granted object roles"
 msgstr "Rôles accordés aux utilisateurs"
 
-#: src/pyams_security_views/zmi/policy.py:107
+#: src/pyams_security_views/zmi/policy.py:128
 msgid "Roles are not defined for this context!"
 msgstr "Aucun rôle n'est défini dans ce contexte !"
 
-#: src/pyams_security_views/zmi/policy.py:120
+#: src/pyams_security_views/zmi/policy.py:141
 msgid "Security policy"
 msgstr "Politique de sécurité"
 
-#: src/pyams_security_views/zmi/policy.py:130
+#: src/pyams_security_views/zmi/policy.py:151
 #: src/pyams_security_views/zmi/manager.py:48
 #: src/pyams_security_views/zmi/manager.py:69
 msgid "Security manager"
 msgstr "Gestionnaire de sécurité"
 
-#: src/pyams_security_views/zmi/policy.py:131
+#: src/pyams_security_views/zmi/policy.py:152
 msgid "Security policy management"
 msgstr "Paramètres de la politique de sécurité"
 
 #: src/pyams_security_views/zmi/login.py:45
 msgid "Login form"
 msgstr "Page de connexion"
 
@@ -153,21 +155,21 @@
 msgid "New plug-in properties"
 msgstr "Propriétés du nouveau module"
 
 #: src/pyams_security_views/zmi/plugin/__init__.py:97
 msgid "Specified prefix is already used!"
 msgstr "Le préfixe indiqué est déjà utilisé !"
 
-#: src/pyams_security_views/zmi/plugin/__init__.py:135
-#: src/pyams_security_views/zmi/plugin/__init__.py:162
+#: src/pyams_security_views/zmi/plugin/__init__.py:136
+#: src/pyams_security_views/zmi/plugin/__init__.py:163
 #, python-format
 msgid "Plug-in: {}"
 msgstr "Module : {}"
 
-#: src/pyams_security_views/zmi/plugin/__init__.py:164
+#: src/pyams_security_views/zmi/plugin/__init__.py:165
 msgid "Plug-in properties"
 msgstr "Propriétés du module"
 
 #: src/pyams_security_views/zmi/plugin/group.py:65
 msgid "Add groups folder..."
 msgstr "Ajouter un dossier de groupes..."
 
@@ -225,15 +227,14 @@
 msgstr "Le mot de passe est renseigné"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:194
 msgid "Account is activated"
 msgstr "Le profil est activé"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:217
-#: src/pyams_security_views/api/principal.py:65
 msgid "Search results"
 msgstr "Résultats de la recherche"
 
 #: src/pyams_security_views/zmi/plugin/userfolder.py:238
 msgid "Add user"
 msgstr "Ajouter un utilisateur"
 
@@ -347,46 +348,30 @@
 msgstr ""
 "<strong>Prenez soin de bien redéfinir le mot de passe lorsque vous utilisez "
 "certains navigateurs qui forcent l'auto-complétion !!!</strong><br />En "
 "effaçant le mot de passe, le compte restera actif mais sans possibilité de "
 "se connecter (il restera utilisable pour des tâches internes) ; en indiquant "
 "la valeur '*****', le mot de passe ne sera pas modifié..."
 
-#: src/pyams_security_views/api/principal.py:43
-msgid "Principals search string"
-msgstr "Requête de recherche des mandataires"
-
-#: src/pyams_security_views/api/principal.py:49
-msgid "Principal ID"
-msgstr "ID du mandataire"
-
-#: src/pyams_security_views/api/principal.py:51
-msgid "Principal title"
-msgstr "Libellé du mandataire"
-
-#: src/pyams_security_views/api/principal.py:61
-msgid "Results list"
-msgstr "Liste de résultats"
-
-#: src/pyams_security_views/skin/login.py:81
+#: src/pyams_security_views/skin/login.py:83
 msgid "You must authenticate"
 msgstr "Vous devez vous authentifier !"
 
-#: src/pyams_security_views/skin/login.py:82
+#: src/pyams_security_views/skin/login.py:84
 msgid "Please enter valid credentials"
 msgstr "Paramètres de connexion"
 
-#: src/pyams_security_views/skin/login.py:150
+#: src/pyams_security_views/skin/login.py:153
 msgid ""
 "Missing security manager utility. Please contact your system administrator!"
 msgstr ""
 "Aucun gestionnaire de sécurité n'est disponible. Veuillez contacter votre "
 "administrateur !"
 
-#: src/pyams_security_views/skin/login.py:156
+#: src/pyams_security_views/skin/login.py:159
 msgid "Invalid credentials!"
 msgstr "Vos paramètres de connexion sont incorrects !"
 
 #: src/pyams_security_views/interfaces/login.py:34
 msgid "Login logo"
 msgstr "Logo de connexion"
 
@@ -443,14 +428,26 @@
 msgid "Reset"
 msgstr "Annuler"
 
 #: src/pyams_security_views/interfaces/login.py:91
 msgid "Cancel"
 msgstr "Annuler"
 
+#~ msgid "Principals search string"
+#~ msgstr "Requête de recherche des mandataires"
+
+#~ msgid "Principal ID"
+#~ msgstr "ID du mandataire"
+
+#~ msgid "Principal title"
+#~ msgstr "Libellé du mandataire"
+
+#~ msgid "Results list"
+#~ msgstr "Liste de résultats"
+
 #~ msgid "Groups folder plug-in"
 #~ msgstr "Groupes d'utilisateurs"
 
 #~ msgid "System authentication plug-in"
 #~ msgstr "Utilisateur système"
 
 #~ msgid "Users folder plug-in"
```

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/locales/pyams_security_views.pot` & `pyams_security_views-1.8.5/src/pyams_security_views/locales/pyams_security_views.pot`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2022-05-16 10:51+0200\n"
+"POT-Creation-Date: 2023-04-12 16:00+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
 #: ./src/pyams_security_views/widget/principal.py:71
 msgid "No selected principal"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/rest.py:50
-#: ./src/pyams_security_views/zmi/rest.py:60
+#: ./src/pyams_security_views/zmi/rest.py:51
+#: ./src/pyams_security_views/zmi/rest.py:61
 msgid "CORS configuration"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/rest.py:91
+#: ./src/pyams_security_views/zmi/rest.py:96
 msgid ""
 "If you disable CORS origins check, any CORS request will be accepted.\n"
 "Otherwise, only origins specified below will be allowed.\n"
 "Please note that you don't have to set main site URL(s) below, only \"external\" URLs have to be defined."
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/notifications.py:50
@@ -42,38 +42,39 @@
 
 #: ./src/pyams_security_views/zmi/notifications.py:85
 msgid ""
 "Notifications are used to send messages to users during their registration process.\n"
 "Applications can also send messages during their normal process."
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/policy.py:58
-#: ./src/pyams_security_views/zmi/policy.py:68
+#: ./src/pyams_security_views/zmi/policy.py:59
+#: ./src/pyams_security_views/zmi/policy.py:98
+#: ./src/pyams_security_views/zmi/policy.py:112
 msgid "User roles"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/policy.py:69
+#: ./src/pyams_security_views/zmi/policy.py:67
 msgid "Granted object roles"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/policy.py:107
+#: ./src/pyams_security_views/zmi/policy.py:128
 msgid "Roles are not defined for this context!"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/policy.py:120
+#: ./src/pyams_security_views/zmi/policy.py:141
 msgid "Security policy"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/policy.py:130
+#: ./src/pyams_security_views/zmi/policy.py:151
 #: ./src/pyams_security_views/zmi/manager.py:48
 #: ./src/pyams_security_views/zmi/manager.py:69
 msgid "Security manager"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/policy.py:131
+#: ./src/pyams_security_views/zmi/policy.py:152
 msgid "Security policy management"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/login.py:45
 msgid "Login form"
 msgstr ""
 
@@ -131,21 +132,21 @@
 msgid "New plug-in properties"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/__init__.py:97
 msgid "Specified prefix is already used!"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:135
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:162
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:136
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:163
 #, python-format
 msgid "Plug-in: {}"
 msgstr ""
 
-#: ./src/pyams_security_views/zmi/plugin/__init__.py:164
+#: ./src/pyams_security_views/zmi/plugin/__init__.py:165
 msgid "Plug-in properties"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/group.py:65
 msgid "Add groups folder..."
 msgstr ""
 
@@ -203,15 +204,14 @@
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:194
 msgid "Account is activated"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:217
-#: ./src/pyams_security_views/api/principal.py:65
 msgid "Search results"
 msgstr ""
 
 #: ./src/pyams_security_views/zmi/plugin/userfolder.py:238
 msgid "Add user"
 msgstr ""
 
@@ -310,44 +310,28 @@
 msgid ""
 "<strong>Be careful to redefine the password when using some browsers which "
 "are forcing autocompletion!!!</strong><br />Clearing the password will keep "
 "the plug-in active but without the option to log-in with this account; "
 "setting the password value to '*****' will leave the password as-is..."
 msgstr ""
 
-#: ./src/pyams_security_views/api/principal.py:43
-msgid "Principals search string"
-msgstr ""
-
-#: ./src/pyams_security_views/api/principal.py:49
-msgid "Principal ID"
-msgstr ""
-
-#: ./src/pyams_security_views/api/principal.py:51
-msgid "Principal title"
-msgstr ""
-
-#: ./src/pyams_security_views/api/principal.py:61
-msgid "Results list"
-msgstr ""
-
-#: ./src/pyams_security_views/skin/login.py:81
+#: ./src/pyams_security_views/skin/login.py:83
 msgid "You must authenticate"
 msgstr ""
 
-#: ./src/pyams_security_views/skin/login.py:82
+#: ./src/pyams_security_views/skin/login.py:84
 msgid "Please enter valid credentials"
 msgstr ""
 
-#: ./src/pyams_security_views/skin/login.py:150
+#: ./src/pyams_security_views/skin/login.py:153
 msgid ""
 "Missing security manager utility. Please contact your system administrator!"
 msgstr ""
 
-#: ./src/pyams_security_views/skin/login.py:156
+#: ./src/pyams_security_views/skin/login.py:159
 msgid "Invalid credentials!"
 msgstr ""
 
 #: ./src/pyams_security_views/interfaces/login.py:34
 msgid "Login logo"
 msgstr ""
```

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/login.py` & `pyams_security_views-1.8.5/src/pyams_security_views/login.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/site.py` & `pyams_security_views-1.8.5/src/pyams_security_views/site.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/skin/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/skin/login.py` & `pyams_security_views-1.8.5/src/pyams_security_views/skin/login.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/tests/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/tests/test_utilsdocs.py` & `pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/tests/test_utilsdocstrings.py` & `pyams_security_views-1.8.5/src/pyams_security_views/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/widget/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/widget/interfaces.py` & `pyams_security_views-1.8.5/src/pyams_security_views/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/widget/permission.py` & `pyams_security_views-1.8.5/src/pyams_security_views/widget/permission.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/widget/principal.py` & `pyams_security_views-1.8.5/src/pyams_security_views/widget/principal.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/interfaces.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/login.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/login.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/manager.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/notifications.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/notifications.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/__init__.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/admin.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/admin.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/group.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/group.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/plugin/userfolder.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/plugin/userfolder.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/policy.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/policy.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/rest.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views/zmi/widget.py` & `pyams_security_views-1.8.5/src/pyams_security_views/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views.egg-info/PKG-INFO` & `pyams_security_views-1.8.5/src/pyams_security_views.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-security-views
-Version: 1.8.4
+Version: 1.8.5
 Summary: Pyramid views for PyAMS_security package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
 Platform: UNKNOWN
@@ -46,14 +46,18 @@
 interface (based on PyAMS_zmi package), custom widgets and a small Cornice REST API to look for
 principals.
 
 
 Changelog
 =========
 
+1.8.5
+-----
+ - refactored Colander API schemas for better OpenAPI specifications
+
 1.8.4
 -----
  - updated login form templates
  - added support for Python 3.11
 
 1.8.3
 -----
```

### Comparing `pyams_security_views-1.8.4/src/pyams_security_views.egg-info/SOURCES.txt` & `pyams_security_views-1.8.5/src/pyams_security_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

