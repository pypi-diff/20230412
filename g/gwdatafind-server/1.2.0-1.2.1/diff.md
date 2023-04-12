# Comparing `tmp/gwdatafind-server-1.2.0.tar.gz` & `tmp/gwdatafind-server-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdatafind-server-1.2.0.tar", last modified: Thu Apr 21 21:11:55 2022, max compression
+gzip compressed data, was "gwdatafind-server-1.2.1.tar", last modified: Wed Apr 12 18:21:20 2023, max compression
```

## Comparing `gwdatafind-server-1.2.0.tar` & `gwdatafind-server-1.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.849565 gwdatafind-server-1.2.0/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    35149 2022-03-14 19:21:54.000000 gwdatafind-server-1.2.0/LICENSE
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      175 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/MANIFEST.in
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1915 2022-04-21 21:11:55.849565 gwdatafind-server-1.2.0/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      627 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/README.md
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.845565 gwdatafind-server-1.2.0/config/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      691 2022-03-30 20:12:54.000000 gwdatafind-server-1.2.0/config/gunicorn.conf
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     6737 2022-03-30 20:12:54.000000 gwdatafind-server-1.2.0/config/gunicorn.conf.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2171 2022-03-30 20:12:54.000000 gwdatafind-server-1.2.0/config/gwdatafind-server.ini
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      386 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/config/gwdatafind-server.service
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      698 2022-03-30 20:12:54.000000 gwdatafind-server-1.2.0/config/wsgi.conf
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.845565 gwdatafind-server-1.2.0/debian/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1811 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/debian/changelog
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        2 2022-03-14 19:21:54.000000 gwdatafind-server-1.2.0/debian/compat
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1446 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/debian/control
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1048 2022-03-14 19:21:54.000000 gwdatafind-server-1.2.0/debian/copyright
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       16 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/debian/gwdatafind-server.docs
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      212 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/debian/gwdatafind-server.install
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       16 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/debian/python3-gwdatafind-server.docs
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       30 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/debian/python3-gwdatafind-server.install
--rwxrwxr-x   0 duncan    (1000) duncan    (1000)       82 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/debian/rules
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.845565 gwdatafind-server-1.2.0/debian/source/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       12 2022-03-14 19:21:54.000000 gwdatafind-server-1.2.0/debian/source/format
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.845565 gwdatafind-server-1.2.0/gwdatafind_server/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      543 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/gwdatafind_server/__init__.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.849565 gwdatafind-server-1.2.0/gwdatafind_server/api/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      200 2022-03-30 20:12:54.000000 gwdatafind-server-1.2.0/gwdatafind_server/api/__init__.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      669 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/gwdatafind_server/api/base.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1914 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/gwdatafind_server/api/utils.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)    10855 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/gwdatafind_server/api/v1.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     4216 2022-03-30 20:12:54.000000 gwdatafind-server-1.2.0/gwdatafind_server/app.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     4744 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/gwdatafind_server/authentication.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     7940 2022-03-30 20:12:54.000000 gwdatafind-server-1.2.0/gwdatafind_server/cache.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      974 2022-03-14 19:21:54.000000 gwdatafind-server-1.2.0/gwdatafind_server/config.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.845565 gwdatafind-server-1.2.0/gwdatafind_server.egg-info/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1915 2022-04-21 21:11:55.000000 gwdatafind-server-1.2.0/gwdatafind_server.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1158 2022-04-21 21:11:55.000000 gwdatafind-server-1.2.0/gwdatafind_server.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2022-04-21 21:11:55.000000 gwdatafind-server-1.2.0/gwdatafind_server.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       77 2022-04-21 21:11:55.000000 gwdatafind-server-1.2.0/gwdatafind_server.egg-info/requires.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       18 2022-04-21 21:11:55.000000 gwdatafind-server-1.2.0/gwdatafind_server.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      727 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/pyproject.toml
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     4322 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/python-gwdatafind-server.spec
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1475 2022-04-21 21:11:55.849565 gwdatafind-server-1.2.0/setup.cfg
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      196 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/setup.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2022-04-21 21:11:55.849565 gwdatafind-server-1.2.0/tests/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      702 2022-03-14 19:21:54.000000 gwdatafind-server-1.2.0/tests/cache.dat
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      369 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/tests/conftest.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       77 2022-03-14 19:21:54.000000 gwdatafind-server-1.2.0/tests/grid-mapfile
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      544 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/tests/gwdatafind-server.ini
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     4722 2022-04-21 21:09:42.000000 gwdatafind-server-1.2.0/tests/test_api_v1.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      335 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/tests/test_app.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2515 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/tests/test_authentication_scitokens.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1505 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/tests/test_authentication_x509.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      790 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/tests/test_config.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      480 2022-03-30 20:13:04.000000 gwdatafind-server-1.2.0/tests/utils.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)    35149 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/LICENSE
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      175 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/MANIFEST.in
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/PKG-INFO
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      627 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/README.md
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/config/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      691 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gunicorn.conf
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     6737 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gunicorn.conf.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2174 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gwdatafind-server.ini
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      386 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/gwdatafind-server.service
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      698 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/config/wsgi.conf
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/debian/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2079 2023-04-12 17:49:45.000000 gwdatafind-server-1.2.1/debian/changelog
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)        2 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/compat
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1446 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/control
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1048 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/copyright
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/gwdatafind-server.docs
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      212 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/gwdatafind-server.install
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       16 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/python3-gwdatafind-server.docs
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       30 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/python3-gwdatafind-server.install
+-rwxrwxr-x   0 duncan    (1001) duncan    (1001)       82 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/rules
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/debian/source/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       12 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/debian/source/format
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/gwdatafind_server/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      543 2023-04-12 17:49:45.000000 gwdatafind-server-1.2.1/gwdatafind_server/__init__.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/gwdatafind_server/api/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      200 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/__init__.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      669 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/base.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1914 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/utils.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)    11084 2023-04-11 18:10:54.000000 gwdatafind-server-1.2.1/gwdatafind_server/api/v1.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4223 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/app.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4894 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/authentication.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     8011 2023-04-06 20:05:11.000000 gwdatafind-server-1.2.1/gwdatafind_server/cache.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      974 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/gwdatafind_server/config.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.116871 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1895 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1158 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)        1 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/requires.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       18 2023-04-12 18:21:20.000000 gwdatafind-server-1.2.1/gwdatafind_server.egg-info/top_level.txt
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      727 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/pyproject.toml
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4806 2023-04-12 17:49:45.000000 gwdatafind-server-1.2.1/python-gwdatafind-server.spec
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1475 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/setup.cfg
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      196 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/setup.py
+drwxrwxr-x   0 duncan    (1001) duncan    (1001)        0 2023-04-12 18:21:20.120871 gwdatafind-server-1.2.1/tests/
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      702 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/cache.dat
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      369 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/conftest.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)       77 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/grid-mapfile
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      546 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/gwdatafind-server.ini
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     4722 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_api_v1.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      335 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_app.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     2518 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_authentication_scitokens.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)     1505 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_authentication_x509.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      790 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/test_config.py
+-rw-rw-r--   0 duncan    (1001) duncan    (1001)      480 2023-03-19 17:06:06.000000 gwdatafind-server-1.2.1/tests/utils.py
```

### Comparing `gwdatafind-server-1.2.0/LICENSE` & `gwdatafind-server-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/PKG-INFO` & `gwdatafind-server-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: gwdatafind-server
-Version: 1.2.0
+Version: 1.2.1
 Summary: The server library for the GWDataFind service
 Home-page: https://git.ligo.org/computing/gwdatafind/server
 Author: Duncan Meacher
 Author-email: duncan.meacher@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/computing/gwdatafind/server/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/gwdatafind/server/
 Project-URL: Source Code, https://git.ligo.org/computing/gwdatafind/server
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -42,9 +41,7 @@
 
 For a detailed description of how to set up and configure a datafind server, 
 please see [here](https://computing.docs.ligo.org/gwdatafind/server/configuration.html).
 
 ## Client API
 
 A detailed explination of the API can be found [here](https://computing.docs.ligo.org/gwdatafind/server/api/v1.html).
-
-
```

### Comparing `gwdatafind-server-1.2.0/README.md` & `gwdatafind-server-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/config/gunicorn.conf` & `gwdatafind-server-1.2.1/config/gunicorn.conf`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/config/gunicorn.conf.py` & `gwdatafind-server-1.2.1/config/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/config/gwdatafind-server.ini` & `gwdatafind-server-1.2.1/config/gwdatafind-server.ini`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
 # Set to Python dictionary with URL types as keys and a list of regular
 # expressions in descending order of preference.
 filter_preference = """{'^file': ['preferred', 'hdfs']}"""
 
 # Set SciTokens claims
 # SciTokens Issuer
-scitokens_issuer = "https://cilogon.org/ligo"
+scitokens_issuer = "https://cilogon.org/igwn"
 # SciTokens Audience
 scitokens_audience = ANY
 # SciTokens Scope
-scitokens_scope = "read:/frames"
+scitokens_scope = "gwdatafind.read"
 
 # authorization must be one of 'None' or 'virtual_host', or a combination
 # of 'grid-mapfile' and/or 'scitoken' with comma seperation.
 # None does not authenticate users querying the server.
 # grid-mapfile checks if the user's subject has an entry in a grid-mapfile
 # scitoken uses a SciToken for authorisation.
 # virtual_host allows for different authorization settings on different
```

### Comparing `gwdatafind-server-1.2.0/config/wsgi.conf` & `gwdatafind-server-1.2.1/config/wsgi.conf`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/debian/changelog` & `gwdatafind-server-1.2.1/debian/changelog`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+gwdatafind-server (1.2.1-1) stable; urgency=low
+
+  * Added comment handling in cache file
+  * Updated default SciToken issue and scope
+  * Added ability to search for fractional GPS times
+
+ -- Duncan Meacher <duncan.meacher@ligo.org>  Fri, 07 Apr 2023 00:00:00 +0100
+
 gwdatafind-server (1.2.0-1) stable; urgency=low
 
   * Added full SciToken authentication support
   * Updated README to point to documentation pages
   * Improved error handling
   * Updated CI tests and coverage
```

### Comparing `gwdatafind-server-1.2.0/debian/control` & `gwdatafind-server-1.2.1/debian/control`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/debian/copyright` & `gwdatafind-server-1.2.1/debian/copyright`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/__init__.py` & `gwdatafind-server-1.2.1/gwdatafind_server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 data discover mechanism for data files.
 
 Users provide a few key details as part of an HTTP(S)
 query and receive URLs that indicate the locations
 of the relevant data.
 """
 
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 from .app import GWDataFindApp
 from .config import get_config_path
 
 
 def create_app():
     """Create an instance of the application
```

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/api/base.py` & `gwdatafind-server-1.2.1/gwdatafind_server/api/base.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/api/utils.py` & `gwdatafind-server-1.2.1/gwdatafind_server/api/utils.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/api/v1.py` & `gwdatafind-server-1.2.1/gwdatafind_server/api/v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -209,14 +209,17 @@
         int(start + dur),
     ))
 
 
 @blueprint.route('<ext>/<site>/<tag>/<int:start>,<int:end>')  # for --ping
 @blueprint.route('<ext>/<site>/<tag>/<int:start>,<int:end>.json')
 @blueprint.route('<ext>/<site>/<tag>/<int:start>,<int:end>/<urltype>.json')
+@blueprint.route('<ext>/<site>/<tag>/<float:start>,<float:end>')  # for --ping
+@blueprint.route('<ext>/<site>/<tag>/<float:start>,<float:end>.json')
+@blueprint.route('<ext>/<site>/<tag>/<float:start>,<float:end>/<urltype>.json')
 @handle_errors_as_json
 @authentication.validate
 def find_urls(ext, site, tag, start, end, urltype=None):
     """Find all URLs in a given GPS time interval
     """
     return list(_find_urls(
         ext,
```

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/app.py` & `gwdatafind-server-1.2.1/gwdatafind_server/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
 
 class GWDataFindApp(Flask):
     def __init__(self, import_name, configpath, *args, **kwargs):
         super().__init__(import_name, *args, **kwargs)
 
         config = ConfigObj(configpath)
-        self.config.update(
-            # use      new key                    or old key
-            config.get("GWDataFindServer", config["LDRDataFindServer"]),
-        )
+        try:
+            self.config.update(config["GWDataFindServer"])  # new key
+        except KeyError:
+            self.config.update(config["LDRDataFindServer"])  # old key
 
         # log to file
         if self.config.get("logfile"):
             lfh = logging.FileHandler(
                 self.config["logfile"],
                 mode='w',
             )
```

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/authentication.py` & `gwdatafind-server-1.2.1/gwdatafind_server/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,22 @@
         raise RuntimeError(f"Unable to deserialize token: {exc}")
 
     enforcer = scitokens.Enforcer(
         issuer,
         audience=audience,
     )
 
-    authz, path = scope.split(":", 1)
+    # parse authz operation and path (if present)
+    try:
+        authz, path = scope.split(":", 1)
+    except ValueError:
+        authz = scope
+        path = None
+
+    # test the token
     if not enforcer.test(token, authz, path):
         raise RuntimeError("token enforcement failed")
     current_app.logger.info('User SciToken authorised.')
 
 
 AUTH_METHODS["scitoken"] = (_request_has_token, _validate_scitoken)
```

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/cache.py` & `gwdatafind-server-1.2.1/gwdatafind_server/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,16 @@
         self.logger.info(f'parsing frame cache from {self.path}')
         exclusions = {key: 0 for key in self.patterns}
         nlines = 0
         cache = {}
 
         with open(self.path, 'rb') as fobj:
             for line in fobj:
+                if line.startswith(b"#"):
+                    continue
                 # parse line
                 site, tag, path, dur, ext, segments = self._parse_line(line)
                 # determine exclusion
                 exclude = self.exclude(site, tag)
                 if exclude:  # record why excluded
                     exclusions[exclude] += 1
                     continue
```

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server/config.py` & `gwdatafind-server-1.2.1/gwdatafind_server/config.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server.egg-info/PKG-INFO` & `gwdatafind-server-1.2.1/gwdatafind_server.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: gwdatafind-server
-Version: 1.2.0
+Version: 1.2.1
 Summary: The server library for the GWDataFind service
 Home-page: https://git.ligo.org/computing/gwdatafind/server
 Author: Duncan Meacher
 Author-email: duncan.meacher@ligo.org
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://git.ligo.org/computing/gwdatafind/server/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/gwdatafind/server/
 Project-URL: Source Code, https://git.ligo.org/computing/gwdatafind/server
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -42,9 +41,7 @@
 
 For a detailed description of how to set up and configure a datafind server, 
 please see [here](https://computing.docs.ligo.org/gwdatafind/server/configuration.html).
 
 ## Client API
 
 A detailed explination of the API can be found [here](https://computing.docs.ligo.org/gwdatafind/server/api/v1.html).
-
-
```

### Comparing `gwdatafind-server-1.2.0/gwdatafind_server.egg-info/SOURCES.txt` & `gwdatafind-server-1.2.1/gwdatafind_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/pyproject.toml` & `gwdatafind-server-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/python-gwdatafind-server.spec` & `gwdatafind-server-1.2.1/python-gwdatafind-server.spec`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define srcname gwdatafind-server
-%define version 1.2.0
+%define version 1.2.1
 %define release 1
 
 Name:      python-%{srcname}
 Version:   %{version}
 Release:   %{release}%{?dist}
 Summary:   The server app for the GWDataFind service
 License:   GPLv3+
@@ -90,21 +90,28 @@
 %__mkdir -pv %{buildroot}%{_sysconfdir}/
 %__install -m 644 -p -v config/gwdatafind-server.ini %{buildroot}%{_sysconfdir}/%{srcname}.ini
 
 # systemd
 %__mkdir -pv %{buildroot}%{_unitdir}/
 %__install -m 644 -p -v config/gwdatafind-server.service %{buildroot}%{_unitdir}/%{srcname}.service
 
-%post
+%pre
+getent group gwdatafind >/dev/null || groupadd -r gwdatafind
+getent passwd gwdatafind >/dev/null || \
+    useradd -r -g gwdatafind -d %{_sharedstatedir} -s /sbin/nologin \
+    -c "Dedicated gwdatafind service account" gwdatafind
+exit 0
+
+%post -n %{srcname}
 %systemd_post %{srcname}.service
 
-%preun
+%preun -n %{srcname}
 %systemd_preun %{srcname}.service
 
-%postun
+%postun -n %{srcname}
 %systemd_postun_with_restart %{srcname}.service
 
 %clean
 rm -rf $RPM_BUILD_ROOT
 
 %files -n python%{python3_pkgversion}-%{srcname}
 %doc README.md
@@ -117,14 +124,18 @@
 %license LICENSE
 %{_datadir}/%{srcname}/
 %{_unitdir}/%{srcname}.service
 
 # -- changelog
 
 %changelog
+* Fri Apr 07 2023 Duncan Meacher <duncan.meacher@ligo.org> 1.2.1-1
+- Added comment handling in cache file
+- Updated default SciToken issue and scope
+- Added ability to search for fractional GPS times
 * Thu Apr 21 2022 Duncan Meacher <duncan.meacher@ligo.org> 1.2.0-1
 - Added full SciToken authentication support
 - Updated README to point to documentation pages
 - Improved error handling
 - Updated CI tests and coverage
 * Fri Mar 11 2022 Duncan Meacher <duncan.meacher@ligo.org> 1.1.0-1
 - Added no-authentication method with virtual hosts
```

### Comparing `gwdatafind-server-1.2.0/setup.cfg` & `gwdatafind-server-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/tests/cache.dat` & `gwdatafind-server-1.2.1/tests/cache.dat`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/tests/gwdatafind-server.ini` & `gwdatafind-server-1.2.1/tests/gwdatafind-server.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[LDRDataFindServer]
+[GWDataFindServer]
 # frame cache file
 framecachefile = tests/cache.dat
 framecachetimeout = 10
 # grid-mapfile
 authorization = grid-mapfile,scitoken
 gridmapcachefile = tests/grid-mapfile
 gridmapcachetimeout = 60
@@ -12,8 +12,8 @@
 frametype_include_pattern = .+_TEST_\d+
 filter_preference = """{'^file': ['preferred', 'hdfs']}"""
 # SciTokens Issuer
 scitokens_issuer = "test"
 # SciTokens Audience
 scitokens_audience = "TEST"
 # SciTokens Scope
-scitokens_scope = "read:/frames"
+scitokens_scope = "gwdatafind.read"
```

### Comparing `gwdatafind-server-1.2.0/tests/test_api_v1.py` & `gwdatafind-server-1.2.1/tests/test_api_v1.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/tests/test_authentication_scitokens.py` & `gwdatafind-server-1.2.1/tests/test_authentication_scitokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from gwdatafind_server import __version__ as SERVER_VERSION
 
 from utils import create_test_app
 
 TEST_ISSUER = "test"
 TEST_AUDIENCE = "TEST"
-TEST_SCOPE = "read:/frames"
+TEST_SCOPE = "gwdatafind.read"
 
 
 # -- fixtures ---------------
 
 @pytest.fixture(scope="session")  # one per suite is fine
 def private_key():
     return generate_private_key(
```

### Comparing `gwdatafind-server-1.2.0/tests/test_authentication_x509.py` & `gwdatafind-server-1.2.1/tests/test_authentication_x509.py`

 * *Files identical despite different names*

### Comparing `gwdatafind-server-1.2.0/tests/test_config.py` & `gwdatafind-server-1.2.1/tests/test_config.py`

 * *Files identical despite different names*

