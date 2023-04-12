# Comparing `tmp/tendril-utils-db-0.5.0.tar.gz` & `tmp/tendril-utils-db-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-utils-db-0.5.0.tar", last modified: Tue Apr 11 18:44:21 2023, max compression
+gzip compressed data, was "tendril-utils-db-0.5.1.tar", last modified: Wed Apr 12 17:42:18 2023, max compression
```

## Comparing `tendril-utils-db-0.5.0.tar` & `tendril-utils-db-0.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.5.0/alembic.ini
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.929615 tendril-utils-db-0.5.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.921615 tendril-utils-db-0.5.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.5.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.5.0/src/tendril/config/db.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/config/db_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.0/src/tendril/db/controllers/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.933615 tendril-utils-db-0.5.0/src/tendril/db/migration/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/README
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/env.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/script.py.mako
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril/db/migration/versions/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.0/src/tendril/db/migration/versions/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.0/src/tendril/db/models/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.5.0/src/tendril/utils/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9578 2023-04-11 18:42:19.000000 tendril-utils-db-0.5.0/src/tendril/utils/db.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-11 18:44:21.000000 tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-11 18:44:21.937615 tendril-utils-db-0.5.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/README.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.5.1/alembic.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.506977 tendril-utils-db-0.5.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.502977 tendril-utils-db-0.5.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.5.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.5.1/src/tendril/config/db.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/config/db_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.1/src/tendril/db/controllers/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/db/migration/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/README
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/env.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/script.py.mako
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/db/migration/versions/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/versions/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.1/src/tendril/db/models/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.5.1/src/tendril/utils/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    10197 2023-04-12 17:41:29.000000 tendril-utils-db-0.5.1/src/tendril/utils/db.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/tox.ini
```

### Comparing `tendril-utils-db-0.5.0/.gitignore` & `tendril-utils-db-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/.readthedocs.yml` & `tendril-utils-db-0.5.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/.travis.yml` & `tendril-utils-db-0.5.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/LICENSE` & `tendril-utils-db-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/PKG-INFO` & `tendril-utils-db-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.5.0
+Version: 0.5.1
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
```

### Comparing `tendril-utils-db-0.5.0/README.rst` & `tendril-utils-db-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/alembic.ini` & `tendril-utils-db-0.5.1/alembic.ini`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/Makefile` & `tendril-utils-db-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/_static/custom.css` & `tendril-utils-db-0.5.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/_static/favicon.ico` & `tendril-utils-db-0.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/_static/logo.png` & `tendril-utils-db-0.5.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/_static/logo_packed.png` & `tendril-utils-db-0.5.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/_templates/about.html` & `tendril-utils-db-0.5.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/conf.py` & `tendril-utils-db-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/index.rst` & `tendril-utils-db-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/docs/installation.rst` & `tendril-utils-db-0.5.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/setup.py` & `tendril-utils-db-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/src/tendril/config/__init__.py` & `tendril-utils-db-0.5.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/src/tendril/config/db.py` & `tendril-utils-db-0.5.1/src/tendril/config/db.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/src/tendril/config/db_core.py` & `tendril-utils-db-0.5.1/src/tendril/config/db_core.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/src/tendril/db/migration/env.py` & `tendril-utils-db-0.5.1/src/tendril/db/migration/env.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/src/tendril/utils/db.py` & `tendril-utils-db-0.5.1/src/tendril/utils/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -205,15 +205,21 @@
     dependence to any degree. It adds both the ``updated_at`` and
     ``created_at`` columns.
     """
     pass
 
 
 _default_prefixes = ['tendril']
-_excluded_prefixes = ['tendril.schema']
+_excluded_prefixes = ['tendril.schema',  # Cannot always be safely imported. Has no models.
+                      'tendril.interests',  # Cannot be safely imported before authn. Models must reside in tendril.db.models.  # noqa
+                      'tendril.config',  # Can never contain models. Should be safe to import though.
+                      'tendril.db',      # Can never contain models. Should be safe to import though.
+                      'tendril.common',  # Can never contain models. Should be safe to import though.
+                      'tendril.utils',   # Can never contain models. Should be safe to import though.
+                      ]
 _user_models_prefix = ['tendril.db.models']
 
 
 def get_metadata(prefixes=DATABASE_PACKAGE_PREFIXES):
     """
     This function populates the database metadata with all the models used
     by the application. The models are imported from <prefix>.*.db.models,
```

### Comparing `tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/PKG-INFO` & `tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.5.0
+Version: 0.5.1
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
```

### Comparing `tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/SOURCES.txt` & `tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/src/tendril_utils_db.egg-info/requires.txt` & `tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/tests/coveralls.py` & `tendril-utils-db-0.5.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.0/tox.ini` & `tendril-utils-db-0.5.1/tox.ini`

 * *Files identical despite different names*

