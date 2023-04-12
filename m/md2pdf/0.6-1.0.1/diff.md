# Comparing `tmp/md2pdf-0.6.tar.gz` & `tmp/md2pdf-1.0.1.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2pdf-0.6.tar", last modified: Fri Apr  7 14:33:47 2023, max compression
+gzip compressed data, was "md2pdf-1.0.1.linux-x86_64.tar", last modified: Wed Apr 12 08:51:45 2023, max compression
```

## Comparing `md2pdf-0.6.tar` & `md2pdf-1.0.1.linux-x86_64.tar`

### file list

```diff
@@ -1,26 +1,41 @@
-drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-07 14:33:47.295627 md2pdf-0.6/
--rw-r--r--   0 maupetit  (1000) fun       (5000)     1064 2021-01-21 19:55:29.000000 md2pdf-0.6/LICENSE
--rw-r--r--   0 maupetit  (1000) fun       (5000)      148 2021-01-21 19:55:29.000000 md2pdf-0.6/MANIFEST.in
--rw-r--r--   0 maupetit  (1000) fun       (5000)     1166 2023-04-07 14:33:47.295627 md2pdf-0.6/PKG-INFO
--rw-r--r--   0 maupetit  (1000) fun       (5000)     3467 2021-01-21 19:55:29.000000 md2pdf-0.6/README.md
-drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-07 14:33:47.295627 md2pdf-0.6/md2pdf/
--rw-r--r--   0 maupetit  (1000) fun       (5000)      210 2023-04-07 14:25:24.000000 md2pdf-0.6/md2pdf/__init__.py
--rwxr-xr-x   0 maupetit  (1000) fun       (5000)      787 2023-04-07 14:17:27.000000 md2pdf-0.6/md2pdf/__main__.py
--rw-r--r--   0 maupetit  (1000) fun       (5000)     1393 2023-04-07 14:17:27.000000 md2pdf-0.6/md2pdf/core.py
--rw-r--r--   0 maupetit  (1000) fun       (5000)       69 2021-01-21 19:55:29.000000 md2pdf-0.6/md2pdf/exceptions.py
-drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-07 14:33:47.295627 md2pdf-0.6/md2pdf.egg-info/
--rw-r--r--   0 maupetit  (1000) fun       (5000)     1166 2023-04-07 14:33:47.000000 md2pdf-0.6/md2pdf.egg-info/PKG-INFO
--rw-r--r--   0 maupetit  (1000) fun       (5000)      415 2023-04-07 14:33:47.000000 md2pdf-0.6/md2pdf.egg-info/SOURCES.txt
--rw-r--r--   0 maupetit  (1000) fun       (5000)        1 2023-04-07 14:33:47.000000 md2pdf-0.6/md2pdf.egg-info/dependency_links.txt
--rw-r--r--   0 maupetit  (1000) fun       (5000)       49 2023-04-07 14:33:47.000000 md2pdf-0.6/md2pdf.egg-info/entry_points.txt
--rw-r--r--   0 maupetit  (1000) fun       (5000)       28 2023-04-07 14:33:47.000000 md2pdf-0.6/md2pdf.egg-info/requires.txt
--rw-r--r--   0 maupetit  (1000) fun       (5000)       13 2023-04-07 14:33:47.000000 md2pdf-0.6/md2pdf.egg-info/top_level.txt
--rw-r--r--   0 maupetit  (1000) fun       (5000)       96 2021-01-21 19:55:29.000000 md2pdf-0.6/requirements-dev.txt
--rw-r--r--   0 maupetit  (1000) fun       (5000)       28 2021-01-21 19:55:29.000000 md2pdf-0.6/requirements.txt
--rw-r--r--   0 maupetit  (1000) fun       (5000)      319 2023-04-07 14:33:47.295627 md2pdf-0.6/setup.cfg
--rw-r--r--   0 maupetit  (1000) fun       (5000)     2222 2023-04-07 14:17:27.000000 md2pdf-0.6/setup.py
-drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-07 14:33:47.295627 md2pdf-0.6/tests/
--rw-r--r--   0 maupetit  (1000) fun       (5000)        0 2021-01-21 19:55:29.000000 md2pdf-0.6/tests/__init__.py
--rw-r--r--   0 maupetit  (1000) fun       (5000)      164 2021-01-21 19:55:29.000000 md2pdf-0.6/tests/defaults.py
--rw-r--r--   0 maupetit  (1000) fun       (5000)     1866 2021-01-21 19:55:29.000000 md2pdf-0.6/tests/test_cli.py
--rw-r--r--   0 maupetit  (1000) fun       (5000)      617 2021-01-21 19:55:29.000000 md2pdf-0.6/tests/test_core.py
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.564437 ./home/maupetit/Work/perso/md2pdf/venv/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.564437 ./home/maupetit/Work/perso/md2pdf/venv/bin/
+-rwxr-xr-x   0 maupetit  (1000) fun       (5000)      986 2023-04-12 08:51:45.564437 ./home/maupetit/Work/perso/md2pdf/venv/bin/md2pdf
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.552436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      225 2023-04-12 08:51:13.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__init__.py
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      787 2023-04-07 14:17:27.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__main__.py
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__pycache__/
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      395 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      855 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__pycache__/__main__.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)     1382 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__pycache__/core.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      352 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      198 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__pycache__/version.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)     1393 2023-04-07 14:17:27.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/core.py
+-rw-r--r--   0 maupetit  (1000) fun       (5000)       69 2021-01-21 19:55:29.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/exceptions.py
+-rw-r--r--   0 maupetit  (1000) fun       (5000)       22 2023-04-12 08:51:13.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/version.py
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.552436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/
+-rw-r--r--   0 maupetit  (1000) fun       (5000)     1074 2023-04-12 08:51:45.548436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/PKG-INFO
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      433 2023-04-12 08:51:45.548436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/SOURCES.txt
+-rw-r--r--   0 maupetit  (1000) fun       (5000)        1 2023-04-12 08:51:45.548436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/dependency_links.txt
+-rw-r--r--   0 maupetit  (1000) fun       (5000)       49 2023-04-12 08:51:45.548436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/entry_points.txt
+-rw-r--r--   0 maupetit  (1000) fun       (5000)       28 2023-04-12 08:51:45.548436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/requires.txt
+-rw-r--r--   0 maupetit  (1000) fun       (5000)       13 2023-04-12 08:51:45.548436 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/top_level.txt
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/
+-rw-r--r--   0 maupetit  (1000) fun       (5000)        0 2021-01-21 19:55:29.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/__init__.py
+drwxr-xr-x   0 maupetit  (1000) fun       (5000)        0 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/__pycache__/
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      177 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      304 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/__pycache__/defaults.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)     2323 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/__pycache__/test_cli.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)     1025 2023-04-12 08:51:45.544437 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/__pycache__/test_core.cpython-310.pyc
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      164 2021-01-21 19:55:29.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/defaults.py
+-rw-r--r--   0 maupetit  (1000) fun       (5000)     1866 2021-01-21 19:55:29.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/test_cli.py
+-rw-r--r--   0 maupetit  (1000) fun       (5000)      617 2021-01-21 19:55:29.000000 ./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/test_core.py
```

### Comparing `md2pdf-0.6/PKG-INFO` & `./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf-1.0.1.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2pdf
-Version: 0.6
+Version: 1.0.1
 Summary: md2pdf, a Markdown to PDF conversion tool
 Home-page: UNKNOWN
 Author: Julien Maupetit
 Author-email: julien@maupetit.net
 License: MIT
 Keywords: markdown converter css pdf
 Platform: UNKNOWN
@@ -15,19 +15,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `md2pdf-0.6/md2pdf/__main__.py` & `./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/__main__.py`

 * *Files identical despite different names*

### Comparing `md2pdf-0.6/md2pdf/core.py` & `./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/md2pdf/core.py`

 * *Files identical despite different names*

### Comparing `md2pdf-0.6/tests/test_cli.py` & `./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `md2pdf-0.6/tests/test_core.py` & `./home/maupetit/Work/perso/md2pdf/venv/lib/python3.10/site-packages/tests/test_core.py`

 * *Files identical despite different names*

