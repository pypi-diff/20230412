# Comparing `tmp/ipydrawio-export-1.2.2.tar.gz` & `tmp/ipydrawio-export-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipydrawio-export-1.2.2.tar", last modified: Tue Nov  8 14:39:20 2022, max compression
+gzip compressed data, was "ipydrawio-export-1.3.0.tar", last modified: Tue Apr 11 21:51:05 2023, max compression
```

## Comparing `ipydrawio-export-1.2.2.tar` & `ipydrawio-export-1.3.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.831557 ipydrawio-export-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-11-08 14:39:20.831557 ipydrawio-export-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/_/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/_/ipydrawio-pdf/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-08 14:39:06.000000 ipydrawio-export-1.2.2/_/ipydrawio-pdf/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/
--rw-r--r--   0 runner    (1001) docker     (121)     5485 2022-11-08 14:39:06.000000 ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/385.92b16e78cc4802eb266f.js
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-11-08 14:39:06.000000 ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/568.3ea8d02d5f8c77cec1bd.js
--rw-r--r--   0 runner    (1001) docker     (121)     7212 2022-11-08 14:39:06.000000 ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/remoteEntry.aaae5653dd69b7dedcd0.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-08 14:39:05.000000 ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-08 14:39:06.000000 ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-11-08 14:39:20.831557 ipydrawio-export-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/src/ipydrawio_export/
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/src/ipydrawio_export/etc/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/etc/install.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/src/ipydrawio_export/etc/jupyter_notebook_config.d/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/etc/jupyter_notebook_config.d/ipydrawio-export.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/src/ipydrawio_export/etc/jupyter_server_config.d/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/etc/jupyter_server_config.d/ipydrawio-export.json
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13765 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/serverextension.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.831557 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-08 14:37:31.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-11-08 14:37:31.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-11-08 14:37:31.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/app.json
--rw-r--r--   0 runner    (1001) docker     (121)    18717 2022-11-08 14:37:31.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/export.js
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-11-08 14:37:31.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/package.json
--rw-r--r--   0 runner    (1001) docker     (121)    51935 2022-11-08 14:38:22.000000 ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.827557 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-11-08 14:39:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-11-08 14:39:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 14:39:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-08 14:39:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 14:39:19.000000 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-08 14:39:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-08 14:39:20.000000 ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.831557 ipydrawio-export-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:20.831557 ipydrawio-export-1.2.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/fixtures/a.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10765 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/fixtures/b.png
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/fixtures/empty.dio
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/fixtures/empty.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1786 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-11-08 14:37:20.000000 ipydrawio-export-1.2.2/tests/test_serverextension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.148645 ipydrawio-export-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-11 21:51:05.148645 ipydrawio-export-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.108645 ipydrawio-export-1.3.0/_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.112645 ipydrawio-export-1.3.0/_/ipydrawio-pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-11 21:51:00.000000 ipydrawio-export-1.3.0/_/ipydrawio-pdf/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.120645 ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-11 21:51:00.000000 ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/385.1639e823caa9b50aada5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-11 21:51:00.000000 ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/568.c1c4c11fee97c25006f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-11 21:51:00.000000 ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/remoteEntry.a38839e484daf1046bb6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 21:50:55.000000 ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 21:51:00.000000 ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-11 21:51:05.160646 ipydrawio-export-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.108645 ipydrawio-export-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.128645 ipydrawio-export-1.3.0/src/ipydrawio_export/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.132645 ipydrawio-export-1.3.0/src/ipydrawio_export/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/etc/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.132645 ipydrawio-export-1.3.0/src/ipydrawio_export/etc/jupyter_notebook_config.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/etc/jupyter_notebook_config.d/ipydrawio-export.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.132645 ipydrawio-export-1.3.0/src/ipydrawio_export/etc/jupyter_server_config.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/etc/jupyter_server_config.d/ipydrawio-export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16124 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/serverextension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.108645 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.136645 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 21:49:24.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-11 21:49:24.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-11 21:49:24.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/app.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-04-11 21:49:24.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/export.js
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-11 21:49:24.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    80716 2023-04-11 21:50:45.000000 ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.132645 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-11 21:51:02.000000 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-11 21:51:04.000000 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:02.000000 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-11 21:51:02.000000 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:02.000000 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-11 21:51:02.000000 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 21:51:02.000000 ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.144646 ipydrawio-export-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:05.148645 ipydrawio-export-1.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/fixtures/a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/fixtures/b.png
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/fixtures/empty.dio
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/fixtures/empty.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-11 21:49:16.000000 ipydrawio-export-1.3.0/tests/test_serverextension.py
```

### Comparing `ipydrawio-export-1.2.2/LICENSE.txt` & `ipydrawio-export-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydrawio-export-1.2.2/PKG-INFO` & `ipydrawio-export-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ipydrawio-export
-Version: 1.2.2
+Version: 1.3.0
 Summary: PDF export for Drawio diagrams in JupyterLab
 Home-page: https://ipydrawio.rtfd.io
 Author: ipydrawio Contributors
 Author-email: ripxl@example.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/deathbeds/ipydrawio/issues
-Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://app.codecov.io/gh/deathbeds/ipydrawio
 Project-URL: Documentation, https://ipydrawio.rtfd.io
 Project-URL: Source Code, https://github.com/deathbeds/ipydrawio
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # IPyDrawio Export
 
 [![docs][docs-badge]][docs] [![binder-badge][]][binder]
@@ -125,15 +124,15 @@
 
 This work is licensed under the [Apache-2.0] License.
 
 The vendored code from [@jgraph/draw-image-export2][] is also licensed under the
 [Apache-2.0][draw2-license] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -142,28 +141,28 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [@jgraph/draw-image-export2]: https://github.com/jgraph/draw-image-export2
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-export/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-export/LICENSE.txt
 [draw2-license]:
   https://github.com/jgraph/draw-image-export2/blob/master/LICENSE
 [serverext]:
   https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Distributing%20Jupyter%20Extensions%20as%20Python%20Packages.html
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-export
 [pypi]: https://pypi.org/project/ipydrawio-export
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-export
 [conda]: https://anaconda.org/conda-forge/ipydrawio-export
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-export-1.2.2/README.md` & `ipydrawio-export-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 This work is licensed under the [Apache-2.0] License.
 
 The vendored code from [@jgraph/draw-image-export2][] is also licensed under the
 [Apache-2.0][draw2-license] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -107,28 +107,28 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [@jgraph/draw-image-export2]: https://github.com/jgraph/draw-image-export2
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-export/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-export/LICENSE.txt
 [draw2-license]:
   https://github.com/jgraph/draw-image-export2/blob/master/LICENSE
 [serverext]:
   https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Distributing%20Jupyter%20Extensions%20as%20Python%20Packages.html
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-export
 [pypi]: https://pypi.org/project/ipydrawio-export
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-export
 [conda]: https://anaconda.org/conda-forge/ipydrawio-export
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-export-1.2.2/_/ipydrawio-pdf/package.json` & `ipydrawio-export-1.3.0/_/ipydrawio-pdf/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9152777777777779%*

 * *Differences: {"'devDependencies'": "{'@deathbeds/ipydrawio': '^1.3.0', '@jupyterlab/builder': '^3.6.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a38839e484daf1046bb6.js'}}",*

 * * "'version'": "'1.3.0'"}*

```diff
@@ -2,25 +2,25 @@
     "bugs": {
         "url": "https://github.com/deathbeds/ipydrawio/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.1.0"
     },
     "devDependencies": {
-        "@deathbeds/ipydrawio": "^1.2.2",
-        "@jupyterlab/builder": "^3.4.0"
+        "@deathbeds/ipydrawio": "^1.3.0",
+        "@jupyterlab/builder": "^3.6.1"
     },
     "files": [
         "{lib,schema,style,src}/**/*.{ts,tsx,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,css}"
     ],
     "homepage": "https://ipydrawio.rtfd.io",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.aaae5653dd69b7dedcd0.js"
+            "load": "static/remoteEntry.a38839e484daf1046bb6.js"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "ipydrawio-export"
                 },
                 "managers": [
@@ -36,9 +36,9 @@
                 "bundled": false,
                 "singleton": true
             }
         }
     },
     "main": "lib/index.js",
     "name": "@deathbeds/ipydrawio-pdf",
-    "version": "1.2.2"
+    "version": "1.3.0"
 }
```

### Comparing `ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/385.92b16e78cc4802eb266f.js` & `ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/385.1639e823caa9b50aada5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,16 @@
 (self.webpackChunk_deathbeds_ipydrawio_pdf = self.webpackChunk_deathbeds_ipydrawio_pdf || []).push([
     [385], {
         656: (t, e, i) => {
             i.d(e, {
                 C: () => s,
                 M: () => r
             });
-            var n = i(267);
-            const s = new(i(978).LabIcon)({
+            var n = i(67);
+            const s = new(i(502).LabIcon)({
                     name: "drawio:pdf",
                     svgstr: n.DRAWIO_ICON_SVG.replace(n.DRAWIO_ICON_CLASS_RE, "jp-icon-contrast2")
                 }),
                 r = {
                     ext: ".pdf",
                     format: "base64",
                     factoryName: "Diagram (PDF)",
@@ -28,17 +28,17 @@
                     exporter: async (t, e, i) => null
                 }
         },
         385: (t, e, i) => {
             i.r(e), i.d(e, {
                 default: () => v
             });
-            var n = i(169),
-                s = i(436),
-                r = i(267),
+            var n = i(33),
+                s = i(583),
+                r = i(67),
                 o = i(656),
                 a = i(271),
                 d = i.n(a);
 
             function l(t) {
                 const {
                     provisioning: e,
@@ -96,15 +96,15 @@
                     }
                     set provisioning(t) {
                         this._provisioning !== t && (this._provisioning = t, this.stateChanged.emit(void 0))
                     }
                 }
                 t.Model = e
             }(p || (p = {}));
-            var u, c = i(19);
+            var u, c = i(142);
             class h {
                 constructor() {
                     this.exportPDF = async (t, e, i) => {
                         await this.fetchStatus();
                         let n = this.exportUrl(i);
                         if (null == n) return null;
                         const s = t.adapter.toXML();
@@ -206,15 +206,15 @@
             i.d(e, {
                 sr: () => a,
                 OF: () => d,
                 NS: () => r,
                 iR: () => s,
                 Uu: () => o
             });
-            const n = JSON.parse('{"name":"@deathbeds/ipydrawio-pdf","version":"1.2.2","homepage":"https://ipydrawio.rtfd.io","bugs":{"url":"https://github.com/deathbeds/ipydrawio/issues"},"main":"lib/index.js","files":["{lib,schema,style,src}/**/*.{ts,tsx,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,css}"],"dependencies":{"@jupyterlab/application":"^3.1.0"},"devDependencies":{"@deathbeds/ipydrawio":"^1.2.2","@jupyterlab/builder":"^3.4.0"},"jupyterlab":{"extension":"lib/plugin.js","outputDir":"../../py_packages/ipydrawio-export/_/ipydrawio-pdf","sharedPackages":{"@deathbeds/ipydrawio":{"bundled":false,"singleton":true}},"discovery":{"server":{"base":{"name":"ipydrawio-export"},"managers":["pip","conda"]}}}}'),
+            const n = JSON.parse('{"name":"@deathbeds/ipydrawio-pdf","version":"1.3.0","homepage":"https://ipydrawio.rtfd.io","bugs":{"url":"https://github.com/deathbeds/ipydrawio/issues"},"main":"lib/index.js","files":["{lib,schema,style,src}/**/*.{ts,tsx,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,css}"],"dependencies":{"@jupyterlab/application":"^3.1.0"},"devDependencies":{"@deathbeds/ipydrawio":"^1.3.0","@jupyterlab/builder":"^3.6.1"},"jupyterlab":{"extension":"lib/plugin.js","outputDir":"../../py_packages/ipydrawio-export/_/ipydrawio-pdf","sharedPackages":{"@deathbeds/ipydrawio":{"bundled":false,"singleton":true}},"discovery":{"server":{"base":{"name":"ipydrawio-export"},"managers":["pip","conda"]}}}}'),
                 s = i.t(n, 2),
                 r = s.name,
                 o = `${r}:plugin`,
                 a = "ipydrawio-pdf";
             var d;
             ! function(t) {
                 t.provision = `${a}:provision`
```

### Comparing `ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/568.3ea8d02d5f8c77cec1bd.js` & `ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/568.c1c4c11fee97c25006f5.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -15,16 +15,16 @@
                 p = i(656)
         },
         656: (e, a, i) => {
             i.d(a, {
                 C: () => p,
                 M: () => d
             });
-            var s = i(267);
-            const p = new(i(978).LabIcon)({
+            var s = i(67);
+            const p = new(i(502).LabIcon)({
                     name: "drawio:pdf",
                     svgstr: s.DRAWIO_ICON_SVG.replace(s.DRAWIO_ICON_CLASS_RE, "jp-icon-contrast2")
                 }),
                 d = {
                     ext: ".pdf",
                     format: "base64",
                     factoryName: "Diagram (PDF)",
@@ -45,15 +45,15 @@
             i.d(a, {
                 sr: () => o,
                 OF: () => t,
                 NS: () => d,
                 iR: () => p,
                 Uu: () => r
             });
-            const s = JSON.parse('{"name":"@deathbeds/ipydrawio-pdf","version":"1.2.2","homepage":"https://ipydrawio.rtfd.io","bugs":{"url":"https://github.com/deathbeds/ipydrawio/issues"},"main":"lib/index.js","files":["{lib,schema,style,src}/**/*.{ts,tsx,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,css}"],"dependencies":{"@jupyterlab/application":"^3.1.0"},"devDependencies":{"@deathbeds/ipydrawio":"^1.2.2","@jupyterlab/builder":"^3.4.0"},"jupyterlab":{"extension":"lib/plugin.js","outputDir":"../../py_packages/ipydrawio-export/_/ipydrawio-pdf","sharedPackages":{"@deathbeds/ipydrawio":{"bundled":false,"singleton":true}},"discovery":{"server":{"base":{"name":"ipydrawio-export"},"managers":["pip","conda"]}}}}'),
+            const s = JSON.parse('{"name":"@deathbeds/ipydrawio-pdf","version":"1.3.0","homepage":"https://ipydrawio.rtfd.io","bugs":{"url":"https://github.com/deathbeds/ipydrawio/issues"},"main":"lib/index.js","files":["{lib,schema,style,src}/**/*.{ts,tsx,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,css}"],"dependencies":{"@jupyterlab/application":"^3.1.0"},"devDependencies":{"@deathbeds/ipydrawio":"^1.3.0","@jupyterlab/builder":"^3.6.1"},"jupyterlab":{"extension":"lib/plugin.js","outputDir":"../../py_packages/ipydrawio-export/_/ipydrawio-pdf","sharedPackages":{"@deathbeds/ipydrawio":{"bundled":false,"singleton":true}},"discovery":{"server":{"base":{"name":"ipydrawio-export"},"managers":["pip","conda"]}}}}'),
                 p = i.t(s, 2),
                 d = p.name,
                 r = `${d}:plugin`,
                 o = "ipydrawio-pdf";
             var t;
             ! function(e) {
                 e.provision = `${o}:provision`
```

### Comparing `ipydrawio-export-1.2.2/_/ipydrawio-pdf/static/remoteEntry.aaae5653dd69b7dedcd0.js` & `ipydrawio-export-1.3.0/_/ipydrawio-pdf/static/remoteEntry.a38839e484daf1046bb6.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, u, d, f, l, s, p, c, h, v, b, y = {
+    var e, r, t, o, n, a, i, u, f, l, d, s, p, c, h, v, b, y = {
             188: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(258), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(258), t.e(385)]).then((() => () => t(385)))
+                        "./index": () => Promise.all([t.e(851), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(851), t.e(385)]).then((() => () => t(385)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var o = "default",
@@ -54,37 +54,37 @@
         return a.default = () => t, m.d(n, a), n
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        258: "84e04da02f6a739ec481",
-        385: "92b16e78cc4802eb266f",
-        568: "3ea8d02d5f8c77cec1bd"
+        385: "1639e823caa9b50aada5",
+        568: "c1c4c11fee97c25006f5",
+        851: "91bf67e7c4cb4ae61178"
     } [e] + ".js?v=" + {
-        258: "84e04da02f6a739ec481",
-        385: "92b16e78cc4802eb266f",
-        568: "3ea8d02d5f8c77cec1bd"
+        385: "1639e823caa9b50aada5",
+        568: "c1c4c11fee97c25006f5",
+        851: "91bf67e7c4cb4ae61178"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, o = "@deathbeds/ipydrawio-pdf:", m.l = (e, r, n, a) => {
         if (t[e]) t[e].push(r);
         else {
             var i, u;
             if (void 0 !== n)
-                for (var d = document.getElementsByTagName("script"), f = 0; f < d.length; f++) {
-                    var l = d[f];
-                    if (l.getAttribute("src") == e || l.getAttribute("data-webpack") == o + n) {
-                        i = l;
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var d = f[l];
+                    if (d.getAttribute("src") == e || d.getAttribute("data-webpack") == o + n) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", o + n), i.src = e), t[e] = [r];
             var s = (r, o) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = t[e];
@@ -115,19 +115,19 @@
                 var a = m.S[t],
                     i = "@deathbeds/ipydrawio-pdf",
                     u = [];
                 return "default" === t && ((e, r, t, o) => {
                     var n = a[e] = a[e] || {},
                         u = n[r];
                     (!u || !u.loaded && (1 != !u.eager ? o : i > u.from)) && (n[r] = {
-                        get: () => Promise.all([m.e(258), m.e(568)]).then((() => () => m(568))),
+                        get: () => Promise.all([m.e(851), m.e(568)]).then((() => () => m(568))),
                         from: i,
                         eager: !1
                     })
-                })("@deathbeds/ipydrawio-pdf", "1.2.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@deathbeds/ipydrawio-pdf", "1.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -162,79 +162,79 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var o = 1, n = 1; n < e.length; n++) o--, t += "u" == (typeof(u = e[n]))[0] ? "-" : (o > 0 ? "." : "") + (o = 2, u);
             return t
         }
         var a = [];
         for (n = 1; n < e.length; n++) {
             var u = e[n];
-            a.push(0 === u ? "not(" + d() + ")" : 1 === u ? "(" + d() + " || " + d() + ")" : 2 === u ? a.pop() + " " + a.pop() : i(u))
+            a.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? a.pop() + " " + a.pop() : i(u))
         }
-        return d();
+        return f();
 
-        function d() {
+        function f() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, u = (e, r) => {
         if (0 in e) {
             r = n(r);
             var t = e[0],
                 o = t < 0;
             o && (t = -t - 1);
-            for (var a = 0, i = 1, d = !0;; i++, a++) {
-                var f, l, s = i < e.length ? (typeof e[i])[0] : "";
-                if (a >= r.length || "o" == (l = (typeof(f = r[a]))[0])) return !d || ("u" == s ? i > t && !o : "" == s != o);
-                if ("u" == l) {
-                    if (!d || "u" != s) return !1
-                } else if (d)
-                    if (s == l)
+            for (var a = 0, i = 1, f = !0;; i++, a++) {
+                var l, d, s = i < e.length ? (typeof e[i])[0] : "";
+                if (a >= r.length || "o" == (d = (typeof(l = r[a]))[0])) return !f || ("u" == s ? i > t && !o : "" == s != o);
+                if ("u" == d) {
+                    if (!f || "u" != s) return !1
+                } else if (f)
+                    if (s == d)
                         if (i <= t) {
-                            if (f != e[i]) return !1
+                            if (l != e[i]) return !1
                         } else {
-                            if (o ? f > e[i] : f < e[i]) return !1;
-                            f != e[i] && (d = !1)
+                            if (o ? l > e[i] : l < e[i]) return !1;
+                            l != e[i] && (f = !1)
                         }
                 else if ("s" != s && "n" != s) {
                     if (o || i <= t) return !1;
-                    d = !1, i--
+                    f = !1, i--
                 } else {
-                    if (i <= t || l < s != o) return !1;
-                    d = !1
-                } else "s" != s && "n" != s && (d = !1, i--)
+                    if (i <= t || d < s != o) return !1;
+                    f = !1
+                } else "s" != s && "n" != s && (f = !1, i--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? u(h, r) : !c())
         }
         return !!c()
-    }, d = (e, r) => {
+    }, f = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, f = (e, r) => {
+    }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, l = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(o) + ")", s = (e, r, t, o) => {
-        var n = f(e, t);
-        return u(o, n) || "undefined" != typeof console && console.warn && console.warn(l(e, t, n, o)), p(e[t][n])
+    }, d = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(o) + ")", s = (e, r, t, o) => {
+        var n = l(e, t);
+        return u(o, n) || "undefined" != typeof console && console.warn && console.warn(d(e, t, n, o)), p(e[t][n])
     }, p = e => (e.loaded = 1, e.get()), c = (e => function(r, t, o, n) {
         var a = m.I(r);
         return a && a.then ? a.then(e.bind(e, r, m.S[r], t, o, n)) : e(r, m.S[r], t, o)
-    })(((e, r, t, o) => (d(e, t), s(r, 0, t, o)))), h = {}, v = {
-        267: () => c("default", "@deathbeds/ipydrawio", [1, 1, 2, 2]),
-        978: () => c("default", "@jupyterlab/ui-components", [1, 3, 5, 0]),
-        19: () => c("default", "@jupyterlab/coreutils", [1, 5, 5, 0]),
-        169: () => c("default", "@jupyterlab/apputils", [1, 3, 5, 0]),
+    })(((e, r, t, o) => (f(e, t), s(r, 0, t, o)))), h = {}, v = {
+        67: () => c("default", "@deathbeds/ipydrawio", [1, 1, 3, 0]),
+        502: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        33: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
         271: () => c("default", "react", [1, 17, 0, 1]),
-        436: () => c("default", "@jupyterlab/statusbar", [1, 3, 5, 0])
+        583: () => c("default", "@jupyterlab/statusbar", [1, 3, 6, 3])
     }, b = {
-        258: [267, 978],
-        385: [19, 169, 271, 436]
+        385: [33, 142, 271, 583],
+        851: [67, 502]
     }, m.f.consumes = (e, r) => {
         m.o(b, e) && b[e].forEach((e => {
             if (m.o(h, e)) return r.push(h[e]);
             var t = r => {
                     h[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
@@ -255,15 +255,15 @@
         var e = {
             863: 0
         };
         m.f.j = (r, t) => {
             var o = m.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (258 != r) {
+                else if (851 != r) {
                 var n = new Promise(((t, n) => o = e[r] = [t, n]));
                 t.push(o[2] = n);
                 var a = m.p + m.u(r),
                     i = new Error;
                 m.l(a, (t => {
                     if (m.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
@@ -271,20 +271,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + a + ")", i.name = "ChunkLoadError", i.type = n, i.request = a, o[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var o, n, [a, i, u] = t,
-                    d = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
                     for (o in i) m.o(i, o) && (m.m[o] = i[o]);
                     u && u(m)
                 }
-                for (r && r(t); d < a.length; d++) n = a[d], m.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); f < a.length; f++) n = a[f], m.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_deathbeds_ipydrawio_pdf = self.webpackChunk_deathbeds_ipydrawio_pdf || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var w = m(188);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@deathbeds/ipydrawio-pdf"] = w
 })();
```

### Comparing `ipydrawio-export-1.2.2/setup.cfg` & `ipydrawio-export-1.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -6,49 +6,48 @@
 url = https://ipydrawio.rtfd.io
 author = ipydrawio Contributors
 author_email = ripxl@example.com
 license = Apache-2.0
 license_files = LICENSE.txt
 project_urls = 
 	Bug Tracker = https://github.com/deathbeds/ipydrawio/issues
-	Changelog = https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+	Changelog = https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 	Coverage = https://app.codecov.io/gh/deathbeds/ipydrawio
 	Documentation = https://ipydrawio.rtfd.io
 	Source Code = https://github.com/deathbeds/ipydrawio
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: Jupyter
 	Framework :: Jupyter :: JupyterLab :: 3
 	Framework :: Jupyter :: JupyterLab :: Extensions
 	Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 	Topic :: Multimedia :: Graphics :: Presentation
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
-	ipydrawio ==1.2.2
+	ipydrawio ==1.3.0
 	lxml
 	pillow
-	pypdf2
+	pypdf
 	requests_cache
 
 [options.packages.find]
 where = 
 	src
 
 [options.entry_points]
@@ -59,29 +58,21 @@
 test = 
 	pytest
 	pytest-console-scripts
 
 [aliases]
 test = pytest
 
-[flake8]
-exclude = .git,__pycache__,envs,.ipynb_checkpoints,.mypy_cache
-max-line-length = 88
-ignore = E203
-
-[isort]
-combine_as_imports = True
-include_trailing_comma = True
-line_length = 88
-multi_line_output = 3
-
 [coverage:run]
 branch = True
 source_pkgs = 
 	ipydrawio_export
 concurrency = multiprocessing
 parallel = True
 
+[coverage:html]
+show_contexts = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ipydrawio-export-1.2.2/setup.py` & `ipydrawio-export-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""dynamic setup information for setuptools, also see package.json and setup.cfg"""
+"""dynamic setup information for setuptools, also see package.json and setup.cfg."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -37,22 +37,22 @@
         if path.is_dir():
             continue
         parent = path.parent.relative_to(package_json.parent).as_posix()
         FILES += [
             (
                 f"""{SHARE}/{pkg["name"]}/{parent}""",
                 [str(path.relative_to(HERE).as_posix())],
-            )
+            ),
         ]
 
 for app in ["server", "notebook"]:
     FILES += [
         (
             f"etc/jupyter/jupyter_{app}_config.d",
             [f"src/ipydrawio_export/etc/jupyter_{app}_config.d/ipydrawio-export.json"],
-        )
+        ),
     ]
 
 if __name__ == "__main__":
     import setuptools
 
     setuptools.setup(version=__js__["version"], data_files=FILES)
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/__init__.py` & `ipydrawio-export-1.3.0/src/ipydrawio_export/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""programmatic drawio export"""
+"""programmatic drawio export."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,21 +18,20 @@
 
 from ._version import __ext__, __js__, __prefix__, __version__
 from .manager import DRAWIO_STATIC, IPyDrawioExportManager
 from .serverextension import load_jupyter_server_extension
 
 
 def _jupyter_labextension_paths():
-    """static paths to link for interactive installation"""
-    exts = _ipydrawio_labextension_paths(prefix=__prefix__, extensions=__ext__)
-    return exts
+    """Static paths to link for interactive installation."""
+    return _ipydrawio_labextension_paths(prefix=__prefix__, extensions=__ext__)
 
 
 def _jupyter_server_extension_paths():
-    """python module to load as extension"""
+    """Python module to load as extension."""
     return [{"module": "ipydrawio_export"}]
 
 
 __all__ = [
     "__js__",
     "__version__",
     "_jupyter_labextension_paths",
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/_version.py` & `ipydrawio-export-1.3.0/src/ipydrawio_export/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""source of truth for ipydrawio version"""
+"""source of truth for ipydrawio version."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 # Copyright 2020 jupyterlab-drawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/app.py` & `ipydrawio-export-1.3.0/src/ipydrawio_export/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""CLI for ipydrawio-export"""
+"""CLI for ipydrawio-export."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,32 +15,38 @@
 # limitations under the License.
 
 import base64
 import json
 from pathlib import Path
 
 import traitlets as T
-from jupyter_core.application import base_flags
+from ipydrawio.app import TRIMMED_FLAGS
 from tornado import ioloop
 from traitlets.config import Application
 
 from ._version import __version__
 from .constants import IPYNB_METADATA
 from .manager import IPyDrawioExportManager
 
 
 class BaseApp(Application):
+    """The base app for ``ipydrawio-export`` apps."""
+
     version = __version__
 
+    flags = TRIMMED_FLAGS
+
     @property
     def description(self):  # pragma: no cover
         return self.__doc__.splitlines()[0].strip()
 
 
 class ManagedApp(BaseApp):
+    """an ``ipydrawio-export`` app with a manager."""
+
     drawio_manager: IPyDrawioExportManager = T.Instance(IPyDrawioExportManager)
     io_loop = T.Instance(ioloop.IOLoop)
 
     @T.default("io_loop")
     def _default_io_loop(self):
         return ioloop.IOLoop.current()
 
@@ -57,20 +63,23 @@
         def _stop():
             self.io_loop.stop()
 
         self.io_loop.add_callback(_stop)
 
 
 class ProvisionApp(ManagedApp):
-    """pre-provision drawio export tools"""
 
-    show_workdir = T.Bool(False).tag(config=True)
+    """pre-provision drawio export tools."""
+
+    show_workdir = T.Bool(False, help="also print out the working location").tag(
+        config=True,
+    )
 
     flags = dict(
-        **base_flags,
+        **TRIMMED_FLAGS,
         workdir=(
             {"ProvisionApp": {"show_workdir": True}},
             "Print the export working directory",
         ),
     )
 
     async def start_async(self):
@@ -82,15 +91,16 @@
             try:
                 await self.drawio_manager.provision(force=True)
             finally:
                 self.stop()
 
 
 class PDFApp(ManagedApp):
-    """export a drawio as PDF"""
+
+    """export a drawio diagram as a PDF."""
 
     dio_files = T.Tuple()
 
     def parse_command_line(self, argv=None):
         super().parse_command_line(argv)
         self.dio_files = [Path(p).resolve() for p in self.extra_args]
 
@@ -100,15 +110,15 @@
             await self.drawio_manager.start_server()
             pdf_requests = []
             for dio in self.dio_files:
                 # TODO: handle more request params
                 pdf_request = {}
                 if dio.name.endswith(".png"):
                     pdf_request["xml"] = base64.b64encode(dio.read_bytes()).decode(
-                        "utf-8"
+                        "utf-8",
                     )
                 elif dio.name.endswith(".ipynb"):
                     meta = json.loads(dio.read_text(encoding="utf-8"))["metadata"]
                     pdf_request["xml"] = meta[IPYNB_METADATA]["xml"]
                 else:
                     pdf_request["xml"] = dio.read_text(encoding="utf-8")
 
@@ -124,20 +134,21 @@
                 self.log.warning("Writing %s bytes to %s", len(pdf_bytes), out)
                 out.write_bytes(pdf_bytes)
         finally:
             self.stop()
 
 
 class DrawioExportApp(BaseApp):
-    """ipydrawio export tools"""
+
+    """``ipydrawio`` export tools."""
 
     name = "ipydrawio-export"
-    subcommands = dict(
-        provision=(ProvisionApp, ProvisionApp.__doc__.splitlines()[0]),
-        pdf=(PDFApp, PDFApp.__doc__.splitlines()[0]),
-    )
+    subcommands = {
+        "provision": (ProvisionApp, ProvisionApp.__doc__.splitlines()[0]),
+        "pdf": (PDFApp, PDFApp.__doc__.splitlines()[0]),
+    }
 
 
 main = launch_instance = DrawioExportApp.launch_instance
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/handlers.py` & `ipydrawio-export-1.3.0/src/ipydrawio_export/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""tornado handlers for managing and communicating with drawio export server"""
+"""tornado handlers for managing and communicating with drawio export server."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,15 +26,15 @@
 
     def initialize(self, manager: IPyDrawioExportManager):
         self.manager = manager
 
 
 class PDFHandler(BaseHandler):
     @authenticated
-    async def post(self, url=None):
+    async def post(self, url=None):  # noqa: ARG002
         params = {k: v[-1] for k, v in self.request.arguments.items()}
         params.pop("_xsrf", None)
         pdf = await self.manager.pdf([params])
         self.finish(pdf)
 
 
 class StatusHandler(BaseHandler):
@@ -49,15 +49,15 @@
     async def post(self):
         await self.manager.provision()
         status = await self.manager.status()
         self.finish(status)
 
 
 def add_handlers(app):
-    """Add ipydrawio routes to the notebook server web application"""
+    """Add ipydrawio routes to the notebook server web application."""
     ns_url = ujoin(app.base_url, "ipydrawio")
     pdf_url = ujoin(ns_url, "export", r"(?P<url>.*)")
     status_url = ujoin(ns_url, "status")
     provision_url = ujoin(ns_url, "provision")
 
     opts = {"manager": app.drawio_manager}
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/manager.py` & `ipydrawio-export-1.3.0/src/ipydrawio_export/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""drawio export manager"""
+"""``ipdrawio-export`` manager."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,134 +28,164 @@
 from concurrent.futures import ThreadPoolExecutor
 from io import BytesIO
 from pathlib import Path
 
 import lxml.etree as E
 from jupyterlab.commands import get_app_dir
 from PIL import Image
+from pypdf import PdfMerger, PdfReader, PdfWriter
 from requests import Session
 from requests_cache import CachedSession
 from tornado.concurrent import run_on_executor
 from traitlets import Bool, Dict, Instance, Int, Unicode, default
 from traitlets.config import LoggingConfigurable
 
-try:
-    from PyPDF2 import PdfMerger, PdfReader, PdfWriter
-except ImportError:  # pragma: no cover
-    from PyPDF2 import (
-        PdfFileMerger as PdfMerger,
-        PdfFileReader as PdfReader,
-        PdfFileWriter as PdfWriter,
-    )
-
 from .constants import (
+    DOT_CHROMIUM,
     DRAWIO_APP,
+    DRAWIO_EXPORT_JS,
+    ENV_DRAWIO_NODE_ENV,
+    ENV_DRAWIO_PORT,
+    ENV_DRAWIO_SERVER_URL,
     ENV_IPYDRAWIO_DATA_DIR,
+    ENV_IPYDRAWIO_PORT,
+    ENV_IPYDRAWIO_PUPPETEER_CACHE_DIR,
     ENV_JUPYTER_DATA_DIR,
+    ENV_PUPPETEER_CACHE_DIR,
     PNG_DRAWIO_INFO,
+    PUPPETEER_INSTALL,
     WORK_DIR,
 )
 
+# http error code
+FOUR_HUNDRED = 400
+
 VEND = Path(__file__).parent / "vendor/draw-image-export2"
 
 DRAWIO_STATIC = (Path(get_app_dir()) / DRAWIO_APP).resolve()
 
 JLPM = Path(shutil.which("jlpm")).resolve()
 
 NODE = Path(
-    shutil.which("node") or shutil.which("node.exe") or shutil.which("node.cmd")
+    shutil.which("node") or shutil.which("node.exe") or shutil.which("node.cmd"),
 ).resolve()
 
 
 class IPyDrawioExportManager(LoggingConfigurable):
-    """manager of (currently) another node-based server"""
 
-    drawio_server_url = Unicode().tag(config=True)
-    drawio_port = Int().tag(config=True)
-    drawing_name = Unicode("drawing.dio.xml").tag(config=True)
-    core_params = Dict().tag(config=True)
-    drawio_export_workdir = Unicode().tag(config=True)
-    pdf_cache = Unicode(allow_none=True).tag(config=True)
-    attach_xml = Bool().tag(config=True)
-    attachment_name = Unicode("diagram.drawio").tag(config=True)
+    """manager of (currently) another node-based server."""
+
+    drawio_server_url = Unicode(help="URL for the drawio server").tag(config=True)
+    drawio_port = Int(help="port for the drawio server").tag(config=True)
+    drawing_name = Unicode("drawing.dio.xml", help="name for temporary XML").tag(
+        config=True,
+    )
+    core_params = Dict(help="URL parameters for export").tag(config=True)
+    drawio_export_workdir = Unicode(help="working directory for the drawio server").tag(
+        config=True,
+    )
+    pdf_cache = Unicode(
+        allow_none=True,
+        help="path to cache for generated PDF pages",
+    ).tag(config=True)
+    attach_xml = Bool(help="attach source XML to PDF document").tag(config=True)
+    attachment_name = Unicode("diagram.drawio", help="name of document to attach").tag(
+        config=True,
+    )
+    init_wait_sec = Int(2, help="time to wait until contacting drawio server").tag(
+        config=True,
+    )
+    export_retries = Int(5, help="number of retries for export").tag(config=True)
     is_provisioning = Bool(False)
     is_starting = Bool(False)
-    init_wait_sec = Int(2).tag(config=True)
     _server = Instance(subprocess.Popen, allow_none=True)
     _session = Instance(Session)
 
     executor = ThreadPoolExecutor(1)
 
     def initialize(self):
         atexit.register(self.stop_server)
 
     @run_on_executor
     def _pdf(self, pdf_request):
         """TODO: enable more customization... I guess over HTTP headers?
-        X-JPYDIO-embed: 1
+        X-JPYDIO-embed: 1.
         """
         data = dict(pdf_request)
         data.update(**self.core_params)
+
+        retries = self.export_retries
         status_code = None
-        pdf_text = None
         res = None
-
-        retries = 3
+        pdf_text = None
 
         while retries:
-            status_code = None
-
             if self._server.returncode is not None:  # pragma: no cover
                 self.start_server()
                 time.sleep(self.init_wait_sec)
             try:
-                self.log.warning(f"[ipydrawio-export] exporting ({retries} retries)...")
+                self.log.warning(
+                    "[ipydrawio-export] exporting (%s retries remaining)...",
+                    retries,
+                )
                 res = self._session.post(self.url, timeout=None, data=data)
                 pdf_text = res.text
+                pdf_text_len = len(res.text)
                 status_code = res.status_code
+                self.log.info(
+                    "[ipydrawio-export] ... %s response: %s bytes",
+                    status_code,
+                    pdf_text_len,
+                )
             except Exception as err:  # pragma: no cover
                 self.log.warning(f"[ipydrawio-export] Pre-HTTP Error: {err}")
-                time.sleep((3 - retries) * self.init_wait_sec)
+                time.sleep((self.export_retries - retries) * self.init_wait_sec)
 
             if status_code is not None:
-                if status_code <= 400:
+                if status_code <= FOUR_HUNDRED:
                     break
-                elif res:  # pragma: no cover
+
+                if res:  # pragma: no cover
                     self.log.warning(
-                        f"[ipydrawio-export] HTTP {res.status_code}: {res.text}"
+                        f"[ipydrawio-export] HTTP {res.status_code}: {res.text}",
                     )
-                else:  # pragma: no cover
-                    self.log.warning("[ipydrawio-export] retrying...")
 
-            retries -= 1  # pragma: no cover
+                status_code = None
+                res = None
+                pdf_text = None
+
+                self.log.warning(
+                    "[ipydrawio-export] retrying, %s remaining...",
+                    retries,
+                )
 
-        if res:
-            self.log.debug(f"[ipydrawio-export] {len(res.text)} bytes")
+            retries -= 1  # pragma: no cover
 
         if pdf_text and self.attach_xml and self.attachments:
             self.log.info(
-                f"[ipydrawio-export] attaching drawio XML as {self.attachment_name}"
+                "[ipydrawio-export] attaching drawio XML as %s",
+                self.attachment_name,
             )
             with tempfile.TemporaryDirectory() as td:
                 tdp = Path(td)
                 output_pdf = tdp / "original.pdf"
                 output_pdf.write_bytes(b64decode(pdf_text))
                 final_pdf = tdp / "final.pdf"
                 final = PdfWriter()
-                final.appendPagesFromReader(PdfReader(str(output_pdf), "rb"))
+                final.append_pages_from_reader(PdfReader(str(output_pdf), "rb"))
                 xml = pdf_request["xml"]
                 if hasattr(xml, "encode"):
                     xml = xml.encode("utf-8")
-                final.addAttachment(self.attachment_name, xml)
+                final.add_attachment(self.attachment_name, xml)
                 with final_pdf.open("wb") as fpt:
                     final.write(fpt)
 
                 pdf_text = b64encode(final_pdf.read_bytes())
                 self.log.debug(
-                    f"[ipydrawio-export] {len(pdf_text)} bytes (with attachment)"
+                    f"[ipydrawio-export] {len(pdf_text)} bytes (with attachment)",
                 )
 
         return pdf_text
 
     @run_on_executor
     def _merge(self, pdf_requests):
         tree = E.fromstring("""<mxfile version="13.3.6"></mxfile>""")
@@ -173,17 +203,20 @@
                 if wrote:
                     merger.append(PdfReader(str(next_pdf)))
             output_pdf = tdp / "output.pdf"
             final_pdf = tdp / "final.pdf"
             merger.write(str(output_pdf))
             composite_xml = E.tostring(tree).decode("utf-8")
             final = PdfWriter()
-            final.appendPagesFromReader(PdfReader(str(output_pdf), "rb"))
+            final.append_pages_from_reader(PdfReader(str(output_pdf), "rb"))
             if self.attach_xml:
-                final.addAttachment(self.attachment_name, composite_xml.encode("utf-8"))
+                final.add_attachment(
+                    self.attachment_name,
+                    composite_xml.encode("utf-8"),
+                )
             with final_pdf.open("wb") as fpt:
                 final.write(fpt)
             return b64encode(final_pdf.read_bytes()).decode("utf-8")
 
     async def pdf(self, pdf_requests):
         if not self._server:  # pragma: no cover
             await self.start_server()
@@ -214,15 +247,21 @@
 
     @property
     def url(self):
         return f"http://localhost:{self.drawio_port}"
 
     @default("drawio_port")
     def _default_drawio_port(self):
-        port = self.get_unused_port()
+        port = os.environ.get(
+            ENV_IPYDRAWIO_PORT,
+            os.environ.get(ENV_DRAWIO_PORT),
+        )
+        if port is None:
+            self.log.debug("[ipydrawio-export] getting unused port...")
+            port = self.get_unused_port()
         self.log.debug(f"[ipydrawio-export] port: {port}")
         return port
 
     @default("drawio_server_url")
     def _default_drawio_server_url(self):
         url = DRAWIO_STATIC.as_uri()
         self.log.debug(f"[ipydrawio-export] URL: {url}")
@@ -235,15 +274,15 @@
             return CachedSession(self.pdf_cache, allowable_methods=["POST"])
 
         self.log.debug("[ipydrawio-export] requests session: regular")
         return Session()
 
     @default("core_params")
     def _default_core_params(self):
-        return dict(format="pdf", base64="1")
+        return {"format": "pdf", "base64": "1"}
 
     @default("drawio_export_workdir")
     def _default_drawio_export_workdir(self):
         data_root = Path(sys.prefix) / "share/jupyter"
 
         if ENV_JUPYTER_DATA_DIR in os.environ:
             data_root = Path(os.environ[ENV_JUPYTER_DATA_DIR])
@@ -292,39 +331,40 @@
         elif tag == "{http://www.w3.org/2000/svg}svg":
             diagrams = E.fromstring(node.attrib["content"]).xpath("//diagram")
             for diagram in diagrams:
                 yield diagram
 
     def _start_process(self):
         env = dict(os.environ)
-        env_updates = dict(
-            PORT=str(self.drawio_port),
-            DRAWIO_SERVER_URL=self.drawio_server_url,
-            NODE_ENV="production",
-        )
-        env.update(env_updates)
+        env_updates = {
+            ENV_DRAWIO_PORT: self.drawio_port,
+            ENV_DRAWIO_SERVER_URL: self.drawio_server_url,
+            ENV_DRAWIO_NODE_ENV: "production",
+            ENV_PUPPETEER_CACHE_DIR: self.drawio_export_chromium,
+        }
+        env.update({k: f"{v}" for k, v in env_updates.items()})
 
         self.log.debug(f"[ipydrawio-export] extra env: {env_updates}")
 
-        args = [NODE, self.drawio_export_app / "export.js"]
+        args = [NODE, self.drawio_export_app / DRAWIO_EXPORT_JS]
         self._server = subprocess.Popen([*map(str, args)], env=env)
         return self._server
 
     async def start_server(self):
         self.stop_server()
         self.log.debug("[ipydrawio-export] starting")
         self.is_starting = True
 
         if not self.is_provisioned:  # pragma: no cover
             await self.provision()
 
         self._start_process()
 
         self.log.warning(
-            f"[ipydrawio-export] waiting {self.init_wait_sec}s for server to start"
+            f"[ipydrawio-export] waiting {self.init_wait_sec}s for server to start",
         )
 
         await asyncio.sleep(self.init_wait_sec)
 
         self.log.warning("[ipydrawio-export] server started")
 
         self.is_starting = False
@@ -342,20 +382,36 @@
         return Path(self.drawio_export_workdir) / VEND.name
 
     @property
     def drawio_export_node_modules(self):
         return self.drawio_export_app / "node_modules"
 
     @property
+    def drawio_export_chromium(self):
+        cache_dir = os.environ.get(
+            ENV_IPYDRAWIO_PUPPETEER_CACHE_DIR,
+            os.environ.get(ENV_PUPPETEER_CACHE_DIR),
+        )
+        if cache_dir is None:
+            cache_dir = self.drawio_export_app / DOT_CHROMIUM
+        return Path(cache_dir)
+
+    @property
+    def drawio_export_puppeteer(self):
+        return self.drawio_export_node_modules / "puppeteer"
+
+    @property
     def drawio_export_integrity(self):
         return self.drawio_export_node_modules / ".yarn-integrity"
 
     @run_on_executor
     def provision(self, force=False):  # pragma: no cover
         self.is_provisioning = True
+        env = dict(**os.environ)
+        env[ENV_PUPPETEER_CACHE_DIR] = str(self.drawio_export_chromium)
         if not self.drawio_export_app.exists():
             if not self.drawio_export_app.parent.exists():
                 self.drawio_export_app.parent.mkdir(parents=True)
             self.log.info(
                 "[ipydrawio-export] initializing drawio export app %s",
                 self.drawio_export_app,
             )
@@ -368,16 +424,28 @@
 
         if not self.drawio_export_node_modules.exists() or force:
             self.log.info(
                 "[ipydrawio-export] installing drawio export dependencies %s",
                 self.drawio_export_app,
             )
             subprocess.check_call(
-                [str(JLPM), "--silent", "--ignore-optional"],
+                [str(JLPM), "--silent", "--ignore-scripts", "--no-optional"],
                 cwd=str(self.drawio_export_app),
+                env=env,
+            )
+
+        if not self.drawio_export_chromium.exists() or force:
+            self.log.info(
+                "[ipydrawio-export] installing puppeteer %s",
+                self.drawio_export_chromium,
+            )
+            subprocess.check_call(
+                [str(NODE), PUPPETEER_INSTALL],
+                cwd=str(self.drawio_export_puppeteer),
+                env=env,
             )
         self.is_provisioning = False
 
     def get_unused_port(self):
         """Get an unused port by trying to listen to any random port.
 
         Probably could introduce race conditions if inside a tight loop.
@@ -386,18 +454,18 @@
         sock.bind(("localhost", 0))
         sock.listen(1)
         port = sock.getsockname()[1]
         sock.close()
         return port
 
     def attachments(self, pdf_path):
-        """iterate over the name, attachment pairs in the PDF"""
+        """Iterate over the name, attachment pairs in the PDF."""
         reader = PdfReader(str(pdf_path), "rb")
         attachments = []
         try:
             attachments = reader.trailer["/Root"]["/Names"]["/EmbeddedFiles"]["/Names"]
         except KeyError:
             pass
         for i, name in enumerate(attachments, 1):
             if not isinstance(name, str):
                 continue
-            yield name, attachments[i].getObject()["/EF"]["/F"].getData()
+            yield name, attachments[i].get_object()["/EF"]["/F"].get_data()
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/serverextension.py` & `ipydrawio-export-1.3.0/src/ipydrawio_export/serverextension.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""add drawio support to a running jupyter application"""
+"""add drawio support to a running jupyter application."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,17 +18,18 @@
 
 from ._version import __version__
 from .handlers import add_handlers
 from .manager import IPyDrawioExportManager
 
 
 def load_jupyter_server_extension(app):
-    """create a IPyDrawioExportManager and add handlers"""
+    """Create a IPyDrawioExportManager and add handlers."""
     app.add_traits(
         drawio_manager=traitlets.Instance(
-            IPyDrawioExportManager, help="a drawio export service"
-        )
+            IPyDrawioExportManager,
+            help="a drawio export service",
+        ),
     )
     manager = app.drawio_manager = IPyDrawioExportManager(parent=app, log=app.log)
     manager.initialize()
     add_handlers(app)
     app.log.warning(f"[ipydrawio] initialized: v{__version__}")
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/LICENSE` & `ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/README.md` & `ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # draw-image-export2
 The current server-side PNG/PDF export implementation using Node, Puppeteer and Chrome headless
 
 ## Running the service (this is your instructions, not the next section)
 * npm install
 * npm start
 
+Then add export=http://localhost:8000 (hostname and port as needed) as an URL parameter to use that service
+for development and testing.
+
 ## Updating internal draw.io versions (internal only)
 
 * su chrome
 * cd ~/draw-image-export2
 * git pull
 * npm install
 * forever restartall
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/app.json` & `ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/app.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/export.js` & `ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/export.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,674 +1,768 @@
 const express = require('express');
-const bodyParser = require('body-parser');
 const morgan = require('morgan');
 const winston = require('winston');
 const compression = require('compression');
 const puppeteer = require('puppeteer');
 const zlib = require('zlib');
-const fetch = require('node-fetch');
+//const fetch = (...args) => import('node-fetch').then(({default: fetch}) => fetch(...args));
 const crc = require('crc');
 const PDFDocument = require('pdf-lib').PDFDocument;
-
-const MAX_AREA = 15000 * 15000;
-const PNG_CHUNK_IDAT = 1229209940;
-var DOMParser = require('xmldom').DOMParser;
-
-const PORT = process.env.PORT || 8000
-
-const app = express();
-
-//Max request size is 10 MB
-app.use(bodyParser.urlencoded({
-    extended: false,
-    limit: '10mb'
-}));
-app.use(bodyParser.json({
-    limit: '10mb'
-}));
-
-app.use(compression({
-    threshold: 10,
-}));
-
-//Enable request logging using morgan and Apache combined format
-app.use(morgan('combined'));
-
-const logger = winston.createLogger({
-    level: 'info',
-    format: winston.format.json(),
-    transports: [
-        //
-        // - Write to all logs with level `info` and below to `combined.log` 
-        // - Write all logs error (and below) to `error.log`.
-        //
-        new winston.transports.File({
-            filename: 'error.log',
-            level: 'error'
-        }),
-        new winston.transports.File({
-            filename: 'combined.log'
-        })
-    ],
-    exceptionHandlers: [
-        new winston.transports.File({
-            filename: 'exceptions.log'
-        })
-    ]
-});
-
-//If we're not in production then log to the `console` also
-if (process.env.NODE_ENV !== 'production') {
-    logger.add(new winston.transports.Console({
-        format: winston.format.simple()
-    }));
+const fs = require("fs").promises;
+const os = require("os");
+const path = require("path");
+const childProcess = require('child_process');
+let cluster = false;
+
+const NO_CLUSTER = process.env.NO_CLUSTER === '1';
+
+if (!NO_CLUSTER) {
+    cluster = require('cluster');
+    //Force windows to do RR scheduling
+    cluster.schedulingPolicy = cluster.SCHED_RR;
 }
 
-// NOTE: Key length must not be longer than 79 bytes (not checked)
-function writePngWithText(origBuff, key, text, compressed, base64encoded) {
-    var isDpi = key == 'dpi';
-    var inOffset = 0;
-    var outOffset = 0;
-    var data = text;
-    var dataLen = isDpi ? 9 : key.length + data.length + 1; //we add 1 zeros with non-compressed data, for pHYs it's 2 of 4-byte-int + 1 byte
-
-    //prepare compressed data to get its size
-    if (compressed) {
-        data = zlib.deflateRawSync(encodeURIComponent(text));
-        dataLen = key.length + data.length + 2; //we add 2 zeros with compressed data
+if (!NO_CLUSTER && cluster.isMaster) {
+    // Count the machine's CPUs
+    let cpuCount = process.env.WORKER_POOL_SIZE || os.cpus().length;
+
+    // Create a worker for each CPU
+    for (let i = 0; i < cpuCount; i++) {
+        cluster.fork();
     }
 
-    var outBuff = Buffer.allocUnsafe(origBuff.length + dataLen + 4); //4 is the header size "zTXt", "tEXt" or "pHYs"
+    // Listen for dying workers
+    cluster.on('exit', function(worker) {
+        // Replace the dead worker,
+        console.log('Worker %d died, restarting...', worker.id);
+        cluster.fork();
+    });
+} else {
+    const MAX_AREA = 20000 * 20000;
+    const PNG_CHUNK_IDAT = 1229209940;
+    const {
+        JSDOM
+    } = require("jsdom");
+
+    const PORT = process.env.PORT || 8000
+
+    const app = express();
+
+    //Max request size is 10 MB
+    app.use(express.urlencoded({
+        extended: false,
+        limit: '10mb'
+    }));
+    app.use(express.json({
+        limit: '10mb'
+    }));
 
-    try {
-        var magic1 = origBuff.readUInt32BE(inOffset);
-        inOffset += 4;
-        var magic2 = origBuff.readUInt32BE(inOffset);
-        inOffset += 4;
+    app.use(compression({
+        threshold: 10,
+    }));
 
-        if (magic1 != 0x89504e47 && magic2 != 0x0d0a1a0a) {
-            throw new Error("PNGImageDecoder0");
-        }
+    //Enable request logging using morgan and Apache combined format
+    app.use(morgan('combined'));
 
-        outBuff.writeUInt32BE(magic1, outOffset);
-        outOffset += 4;
-        outBuff.writeUInt32BE(magic2, outOffset);
-        outOffset += 4;
-    } catch (e) {
-        logger.error(e.message, {
-            stack: e.stack
-        });
-        throw new Error("PNGImageDecoder1");
+    const logger = winston.createLogger({
+        level: 'info',
+        format: winston.format.json(),
+        transports: [
+            //
+            // - Write to all logs with level `info` and below to `combined.log` 
+            // - Write all logs error (and below) to `error.log`.
+            //
+            new winston.transports.File({
+                filename: 'error.log',
+                level: 'error'
+            }),
+            new winston.transports.File({
+                filename: 'combined.log'
+            })
+        ],
+        exceptionHandlers: [
+            new winston.transports.File({
+                filename: 'exceptions.log'
+            })
+        ]
+    });
+
+    //If we're not in production then log to the `console` also
+    if (process.env.NODE_ENV !== 'production') {
+        logger.add(new winston.transports.Console({
+            format: winston.format.simple()
+        }));
     }
 
-    try {
-        while (inOffset < origBuff.length) {
-            var length = origBuff.readInt32BE(inOffset);
-            inOffset += 4;
-            var type = origBuff.readInt32BE(inOffset)
-            inOffset += 4;
-
-            if (type == PNG_CHUNK_IDAT) {
-                // Insert zTXt chunk before IDAT chunk
-                outBuff.writeInt32BE(dataLen, outOffset);
-                outOffset += 4;
+    // NOTE: Key length must not be longer than 79 bytes (not checked)
+    function writePngWithText(origBuff, key, text, compressed, base64encoded) {
+        var isDpi = key == 'dpi';
+        var inOffset = 0;
+        var outOffset = 0;
+        var data = text;
+        var dataLen = isDpi ? 9 : key.length + data.length + 1; //we add 1 zeros with non-compressed data, for pHYs it's 2 of 4-byte-int + 1 byte
+
+        //prepare compressed data to get its size
+        if (compressed) {
+            data = zlib.deflateRawSync(encodeURIComponent(text));
+            dataLen = key.length + data.length + 2; //we add 2 zeros with compressed data
+        }
 
-                var typeSignature = isDpi ? 'pHYs' : (compressed ? "zTXt" : "tEXt");
-                outBuff.write(typeSignature, outOffset);
+        var outBuff = Buffer.allocUnsafe(origBuff.length + dataLen + 4); //4 is the header size "zTXt", "tEXt" or "pHYs"
 
-                outOffset += 4;
+        try {
+            var magic1 = origBuff.readUInt32BE(inOffset);
+            inOffset += 4;
+            var magic2 = origBuff.readUInt32BE(inOffset);
+            inOffset += 4;
 
-                if (isDpi) {
-                    var dpm = Math.round(parseInt(text) / 0.0254) || 3937; //One inch is equal to exactly 0.0254 meters. 3937 is 100dpi
+            if (magic1 != 0x89504e47 && magic2 != 0x0d0a1a0a) {
+                throw new Error("PNGImageDecoder0");
+            }
 
-                    outBuff.writeInt32BE(dpm, outOffset);
-                    outBuff.writeInt32BE(dpm, outOffset + 4);
-                    outBuff.writeInt8(1, outOffset + 8);
-                    outOffset += 9;
-
-                    data = Buffer.allocUnsafe(9);
-                    data.writeInt32BE(dpm, 0);
-                    data.writeInt32BE(dpm, 4);
-                    data.writeInt8(1, 8);
-                } else {
-                    outBuff.write(key, outOffset);
-                    outOffset += key.length;
-                    outBuff.writeInt8(0, outOffset);
-                    outOffset++;
+            outBuff.writeUInt32BE(magic1, outOffset);
+            outOffset += 4;
+            outBuff.writeUInt32BE(magic2, outOffset);
+            outOffset += 4;
+        } catch (e) {
+            logger.error(e.message, {
+                stack: e.stack
+            });
+            throw new Error("PNGImageDecoder1");
+        }
 
-                    if (compressed) {
+        try {
+            while (inOffset < origBuff.length) {
+                var length = origBuff.readInt32BE(inOffset);
+                inOffset += 4;
+                var type = origBuff.readInt32BE(inOffset)
+                inOffset += 4;
+
+                if (type == PNG_CHUNK_IDAT) {
+                    // Insert zTXt chunk before IDAT chunk
+                    outBuff.writeInt32BE(dataLen, outOffset);
+                    outOffset += 4;
+
+                    var typeSignature = isDpi ? 'pHYs' : (compressed ? "zTXt" : "tEXt");
+                    outBuff.write(typeSignature, outOffset);
+
+                    outOffset += 4;
+
+                    if (isDpi) {
+                        var dpm = Math.round(parseInt(text) / 0.0254) || 3937; //One inch is equal to exactly 0.0254 meters. 3937 is 100dpi
+
+                        outBuff.writeInt32BE(dpm, outOffset);
+                        outBuff.writeInt32BE(dpm, outOffset + 4);
+                        outBuff.writeInt8(1, outOffset + 8);
+                        outOffset += 9;
+
+                        data = Buffer.allocUnsafe(9);
+                        data.writeInt32BE(dpm, 0);
+                        data.writeInt32BE(dpm, 4);
+                        data.writeInt8(1, 8);
+                    } else {
+                        outBuff.write(key, outOffset);
+                        outOffset += key.length;
                         outBuff.writeInt8(0, outOffset);
                         outOffset++;
-                        data.copy(outBuff, outOffset);
-                    } else {
-                        outBuff.write(data, outOffset);
+
+                        if (compressed) {
+                            outBuff.writeInt8(0, outOffset);
+                            outOffset++;
+                            data.copy(outBuff, outOffset);
+                        } else {
+                            outBuff.write(data, outOffset);
+                        }
+
+                        outOffset += data.length;
                     }
 
-                    outOffset += data.length;
-                }
+                    var crcVal = 0xffffffff;
+                    crcVal = crc.crcjam(typeSignature, crcVal);
+                    crcVal = crc.crcjam(data, crcVal);
 
-                var crcVal = 0xffffffff;
-                crcVal = crc.crcjam(typeSignature, crcVal);
-                crcVal = crc.crcjam(data, crcVal);
+                    // CRC
+                    outBuff.writeInt32BE(crcVal ^ 0xffffffff, outOffset);
+                    outOffset += 4;
 
-                // CRC
-                outBuff.writeInt32BE(crcVal ^ 0xffffffff, outOffset);
-                outOffset += 4;
+                    // Writes the IDAT chunk after the zTXt
+                    outBuff.writeInt32BE(length, outOffset);
+                    outOffset += 4;
+                    outBuff.writeInt32BE(type, outOffset);
+                    outOffset += 4;
+
+                    origBuff.copy(outBuff, outOffset, inOffset);
+
+                    // Encodes the buffer using base64 if requested
+                    return base64encoded ? outBuff.toString('base64') : outBuff;
+                }
 
-                // Writes the IDAT chunk after the zTXt
                 outBuff.writeInt32BE(length, outOffset);
                 outOffset += 4;
                 outBuff.writeInt32BE(type, outOffset);
                 outOffset += 4;
 
-                origBuff.copy(outBuff, outOffset, inOffset);
+                origBuff.copy(outBuff, outOffset, inOffset, inOffset + length + 4); // +4 to move past the crc
 
-                // Encodes the buffer using base64 if requested
-                return base64encoded ? outBuff.toString('base64') : outBuff;
+                inOffset += length + 4;
+                outOffset += length + 4;
             }
+        } catch (e) {
+            logger.error(e.message, {
+                stack: e.stack
+            });
+            throw e;
+        }
+    }
 
-            outBuff.writeInt32BE(length, outOffset);
-            outOffset += 4;
-            outBuff.writeInt32BE(type, outOffset);
-            outOffset += 4;
-
-            origBuff.copy(outBuff, outOffset, inOffset, inOffset + length + 4); // +4 to move past the crc
+    //From https://advancedweb.hu/secure-tempfiles-in-nodejs-without-dependencies/
+    const withTempFile = (fn) => withTempDir((dir) => fn(path.join(dir, "file")));
 
-            inOffset += length + 4;
-            outOffset += length + 4;
+    const withTempDir = async (fn) => {
+        const dir = await fs.mkdtemp(await fs.realpath(os.tmpdir()) + path.sep);
+        try {
+            return await fn(dir);
+        } finally {
+            //fs.rm is not available on old node versions
+            (fs.rm || fs.rmdir)(dir, {
+                recursive: true
+            });
         }
-    } catch (e) {
-        logger.error(e.message, {
-            stack: e.stack
-        });
-        throw e;
-    }
-}
+    };
 
-function padNumber(n, width, z) {
-    z = z || '0';
-    n = n + '';
+    function execFile(binPath, args) {
+        return new Promise(function(resolve, reject) {
+            childProcess.execFile(binPath, args, {
+                timeout: 25000 //25 sec
+            }, (error, stdout, stderr) => {
+                if (error) {
+                    reject(error);
+                } else {
+                    resolve(stdout);
+                }
+            });
+        });
+    };
 
-    return n.length >= width ? n : new Array(width - n.length + 1).join(z) + n;
-}
+    async function pdfToSvg(pdfFile, xml, transparent) {
+        return await withTempFile(async (tmpFile) => {
+            await fs.writeFile(tmpFile + '.pdf', pdfFile);
+
+            await execFile(process.env.INKSCAPE_PATH || 'inkscape',
+                [
+                    tmpFile + '.pdf',
+                    '--pdf-poppler',
+                    '--export-text-to-path',
+                    '--export-plain-svg',
+                    '--export-filename',
+                    tmpFile + '.svg'
+                ]);
+
+            let svg = await fs.readFile(tmpFile + '.svg', 'utf8');
+
+            if (xml) {
+                //TODO Is this string manubulation safe? DOM parsing is not easily done with JSDOM 
+                /*
+                const dom = new JSDOM(svg, {
+                	contentType: 'text/xml'
+                });
+				
+                doc.documentElement.setAttribute('content', xml);
+                svg = dom.serialize();*/
 
-async function mergePdfs(pdfFiles, xml) {
-    //Pass throgh single files
-    if (pdfFiles.length == 1 && xml == null) {
-        return pdfFiles[0];
-    }
+                svg = svg.replace(/<svg([^>]*)>/, '<svg $1 content="' + encodeURIComponent(xml.replace(/\n|\r/g, ' ')) + '">');
+            }
 
-    try {
-        const pdfDoc = await PDFDocument.create();
-        pdfDoc.setCreator('diagrams.net');
-
-        if (xml != null) {
-            //Embed diagram XML as file attachment
-            await pdfDoc.attach(Buffer.from(xml).toString('base64'), 'diagram.xml', {
-                mimeType: 'application/vnd.jgraph.mxfile',
-                description: 'Diagram Content'
-            });
-        }
+            if (transparent) {
+                //TODO Check that the first element is always the background, also, it has the same style
+                //Note: This depends on Inkscape's version
+                svg = svg.replace('style="fill:#ffffff;fill-opacity:1;fill-rule:nonzero;stroke:none"', 'style="fill:#ffffff;fill-opacity:0;fill-rule:nonzero;stroke:none"');
+            }
 
-        for (var i = 0; i < pdfFiles.length; i++) {
-            const pdfFile = await PDFDocument.load(pdfFiles[i].buffer);
-            const pages = await pdfDoc.copyPages(pdfFile, pdfFile.getPageIndices());
-            pages.forEach(p => pdfDoc.addPage(p));
-        }
+            return svg;
+        });
+    };
 
-        const pdfBytes = await pdfDoc.save();
-        return Buffer.from(pdfBytes);
-    } catch (e) {
-        //Sometimes embedding xml cause errors, so try again without embedding
-        if (xml != null) {
-            return mergePdfs(pdfFiles, null);
+    async function mergePdfs(pdfFiles, xml) {
+        //Pass throgh single files
+        if (pdfFiles.length == 1 && xml == null) {
+            return pdfFiles[0];
         }
 
-        let errMsg = 'Error during PDF combination: ' + e.message;
-        logger.error(errMsg);
-        throw new Error(errMsg);
-    }
-}
+        try {
+            const pdfDoc = await PDFDocument.create();
+            pdfDoc.setCreator('diagrams.net');
+
+            if (xml != null) {
+                //Embed diagram XML as file attachment
+                await pdfDoc.attach(Buffer.from(xml).toString('base64'), 'diagram.xml', {
+                    mimeType: 'application/vnd.jgraph.mxfile',
+                    description: 'Diagram Content'
+                });
+            }
 
-app.post('*', handleRequest);
-app.get('*', handleRequest);
+            for (var i = 0; i < pdfFiles.length; i++) {
+                const pdfFile = await PDFDocument.load(pdfFiles[i].buffer);
+                const pages = await pdfDoc.copyPages(pdfFile, pdfFile.getPageIndices());
+                pages.forEach(p => pdfDoc.addPage(p));
+            }
 
-async function handleRequest(req, res) {
-    try {
-        //Merge all parameters into body such that get and post works the same	
-        Object.assign(req.body, req.params, req.query);
-
-        // Checks for HTML export request
-        if (req.body.html) {
-            var html = req.body.html;
-
-            logger.info("HTML export referer: " + req.get("referer"));
-
-            var wp = req.body.w;
-            var w = (wp == null) ? 0 : parseInt(wp);
-
-            var hp = req.body.h;
-            var h = (hp == null) ? 0 : parseInt(hp);
-            var browser = null;
-
-            try {
-                //Handles buffer constructor deprecation
-                if (Buffer.from && Buffer.from !== Uint8Array.from) {
-                    html = decodeURIComponent(
-                        zlib.inflateRawSync(
-                            Buffer.from(decodeURIComponent(html), 'base64')).toString());
-                } else {
-                    html = decodeURIComponent(
-                        zlib.inflateRawSync(
-                            new Buffer(decodeURIComponent(html), 'base64')).toString());
-                }
+            const pdfBytes = await pdfDoc.save();
+            return Buffer.from(pdfBytes);
+        } catch (e) {
+            //Sometimes embedding xml cause errors, so try again without embedding
+            if (xml != null) {
+                return mergePdfs(pdfFiles, null);
+            }
 
-                browser = await puppeteer.launch({
-                    headless: true,
-                    args: ['--disable-gpu', '--no-sandbox', '--disable-setuid-sandbox', '--disable-dev-shm-usage']
-                });
+            let errMsg = 'Error during PDF combination: ' + e.message;
+            logger.error(errMsg);
+            throw new Error(errMsg);
+        }
+    }
 
-                // Workaround for timeouts/zombies is to kill after 30 secs
-                setTimeout(function() {
-                    browser.close();
-                }, 30000);
-
-                const page = await browser.newPage();
-                await page.setContent(html, {
-                    waitUntil: "networkidle0"
-                });
+    app.post('*', handleRequest);
+    app.get('*', handleRequest);
 
-                page.setViewport({
-                    width: w,
-                    height: h
-                });
+    async function handleRequest(req, res) {
+        try {
+            //Merge all parameters into body such that get and post works the same	
+            Object.assign(req.body, req.params, req.query);
+
+            // Checks for HTML export request
+            // Removed until we secure it
+            /*if (req.body.html)
+            {
+            	var html = req.body.html;
 
-                var data = await page.screenshot({
-                    type: 'png'
-                });
+            	logger.info("HTML export referer: " + req.get("referer"));
 
-                // Cross-origin access should be allowed to now
-                res.header("Access-Control-Allow-Origin", "*");
-                res.header('Content-disposition', 'attachment; filename="capture.png"');
-                res.header('Content-type', 'image/png');
-
-                res.end(data);
-
-                browser.close();
-            } catch (e) {
-                if (browser != null) {
-                    browser.close();
-                }
+            	var wp = req.body.w;
+            	var w = (wp == null) ? 0 : parseInt(wp);
 
-                logger.info("Inflate failed for HTML input: " + html);
-                throw e;
+            	var hp = req.body.h;
+            	var h = (hp == null) ? 0 : parseInt(hp);
+            	var browser = null;
+
+            	try
+            	{
+            		html = decodeURIComponent(
+            			zlib.inflateRawSync(
+            					Buffer.from(decodeURIComponent(html), 'base64')).toString());
+            		
+            		browser = await puppeteer.launch({
+            			headless: true,
+            			args: ['--disable-gpu', '--no-sandbox', '--disable-setuid-sandbox', '--disable-dev-shm-usage']
+            		});
+            		
+            		// Workaround for timeouts/zombies is to kill after 30 secs
+            		setTimeout(function()
+            		{
+            			browser.close();
+            		}, 30000);
+            		
+            		const page = await browser.newPage();
+            		await page.setContent(html, {waitUntil: "networkidle0"});
+
+            		page.setViewport({width: w, height: h});
+
+            		var data = await page.screenshot({
+            		type: 'png'
+            		});
+
+            		// Cross-origin access should be allowed to now
+            		res.header("Access-Control-Allow-Origin", "*");
+            		res.header('Content-disposition', 'attachment; filename="capture.png"');
+            		res.header('Content-type', 'image/png');
+            		
+            		res.end(data);
+
+            		browser.close();
+            	}
+            	catch (e)
+            	{
+            		if (browser != null)
+            		{
+            			browser.close();
+            		}
+            		
+            		logger.info("Inflate failed for HTML input: " + html);
+            		throw e;
+            	}
             }
-        } else {
-            var xml;
-            if (req.body.url) {
-                var urlRes = await fetch(req.body.url);
-                xml = await urlRes.text();
-
-                if (req.body.format == null)
-                    req.body.format = 'png';
-            } else if (req.body.xmldata) {
-                try {
-                    xml = zlib.inflateRawSync(
-                        new Buffer(decodeURIComponent(req.body.xmldata), 'base64')).toString();
-                } catch (e) {
-                    logger.info("Inflate failed for XML input: " + req.body.xmldata);
-                    throw e;
+            else*/
+            {
+                var xml;
+
+                // Removed until we secure it. Remember to add back the fetch import
+                /*if (req.body.url)
+                {
+                	var urlRes = await fetch(req.body.url);
+                	xml = await urlRes.text();
+                	
+                	if (req.body.format == null)
+                		req.body.format = 'png';
+                }
+                else*/
+                if (req.body.xmldata) {
+                    try {
+                        xml = zlib.inflateRawSync(
+                            Buffer.from(decodeURIComponent(req.body.xmldata), 'base64')).toString();
+                    } catch (e) {
+                        logger.info("Inflate failed for XML input: " + req.body.xmldata);
+                        throw e;
+                    }
+                } else {
+                    xml = req.body.xml;
                 }
-            } else {
-                xml = req.body.xml;
-            }
 
-            if (xml != null && xml.indexOf("%3C") == 0) {
-                xml = decodeURIComponent(xml);
-            }
+                if (xml != null && xml.indexOf("%3C") == 0) {
+                    xml = decodeURIComponent(xml);
+                }
 
-            // Extracts the compressed XML from the DIV in a HTML document
-            if (xml != null && (xml.indexOf("<!DOCTYPE html>") == 0 ||
-                    xml.indexOf("<!--[if IE]><meta http-equiv") == 0)) //TODO not tested!
-            {
-                try {
-                    var doc = new DOMParser().parseFromString(xml);
-                    var divs = doc.documentElement
-                        .getElementsByTagName("div");
-
-                    if (divs != null && divs.length > 0 &&
-                        "mxgraph" == (divs.item(0).attributes
-                            .getNamedItem("class").nodeValue)) {
-                        if (divs.item(0).nodeType == 1) {
-                            if (divs.item(0).hasAttribute("data-mxgraph")) {
-                                var jsonString = divs.item(0).getAttribute("data-mxgraph");
-
-                                if (jsonString != null) {
-                                    var obj = JSON.parse(jsonString);
-                                    xml = obj["xml"];
-                                }
-                            } else {
-                                divs = divs.item(0).getElementsByTagName("div");
+                // Extracts the compressed XML from the DIV in a HTML document
+                if (xml != null && (xml.indexOf("<!DOCTYPE html>") == 0 ||
+                        xml.indexOf("<!--[if IE]><meta http-equiv") == 0)) //TODO not tested!
+                {
+                    try {
+                        var doc = new JSDOM(xml).window.document;
+                        var divs = doc.documentElement
+                            .getElementsByTagName("div");
+
+                        if (divs != null && divs.length > 0 &&
+                            "mxgraph" == (divs.item(0).attributes
+                                .getNamedItem("class").nodeValue)) {
+                            if (divs.item(0).nodeType == 1) {
+                                if (divs.item(0).hasAttribute("data-mxgraph")) {
+                                    var jsonString = divs.item(0).getAttribute("data-mxgraph");
+
+                                    if (jsonString != null) {
+                                        var obj = JSON.parse(jsonString);
+                                        xml = obj["xml"];
+                                    }
+                                } else {
+                                    divs = divs.item(0).getElementsByTagName("div");
 
-                                if (divs != null && divs.length > 0) {
-                                    var tmp = divs.item(0).textContent;
+                                    if (divs != null && divs.length > 0) {
+                                        var tmp = divs.item(0).textContent;
 
-                                    if (tmp != null) {
-                                        tmp = zlib.inflateRawSync(new Buffer(tmp, 'base64')).toString();
+                                        if (tmp != null) {
+                                            tmp = zlib.inflateRawSync(Buffer.from(tmp, 'base64')).toString();
 
-                                        if (tmp != null && tmp.length > 0) {
-                                            xml = decodeURIComponent(tmp);
+                                            if (tmp != null && tmp.length > 0) {
+                                                xml = decodeURIComponent(tmp);
+                                            }
                                         }
                                     }
                                 }
                             }
                         }
+                    } catch (e) {
+                        // ignore
                     }
-                } catch (e) {
-                    // ignore
                 }
-            }
 
-            // Extracts the URL encoded XML from the content attribute of an SVG node
-            if (xml != null && (xml.indexOf(
-                    "<?xml version=\"1.0\" encoding=\"UTF-8\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\" \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">") == 0)) { //TODO not tested!
-                try {
-                    var doc = new DOMParser().parseFromString(xml);
-
-                    if (doc != null && doc.documentElement != null && doc
-                        .documentElement.nodeName == "svg") {
-                        var content = doc.documentElement.getAttribute("content");
+                // Extracts the URL encoded XML from the content attribute of an SVG node
+                if (xml != null && (xml.indexOf(
+                        "<?xml version=\"1.0\" encoding=\"UTF-8\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\" \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">") == 0)) { //TODO not tested!
+                    try {
+                        var doc = new JSDOM(xml).window.document;
+
+                        if (doc != null && doc.documentElement != null && doc
+                            .documentElement.nodeName == "svg") {
+                            var content = doc.documentElement.getAttribute("content");
 
-                        if (content != null) {
-                            xml = content;
+                            if (content != null) {
+                                xml = content;
 
-                            if (xml.charAt(0) == '%') {
-                                xml = decodeURIComponent(xml);
+                                if (xml.charAt(0) == '%') {
+                                    xml = decodeURIComponent(xml);
+                                }
                             }
                         }
+                    } catch (e) {
+                        // ignore
                     }
-                } catch (e) {
-                    // ignore
                 }
-            }
-
-            req.body.w = req.body.w || 0;
-            req.body.h = req.body.h || 0;
-
-            // Checks parameters
-            if (req.body.format && xml && req.body.w * req.body.h <= MAX_AREA) {
-                var browser = null;
-
-                try {
-                    var reqStr = ((xml != null) ? "xml=" + xml.length : "") +
-                        ((req.body.embedXml != null) ? " embed=" + req.body.embedXml : "") + " format=" +
-                        req.body.format;
-
-                    req.body.xml = xml;
-
-                    var t0 = Date.now();
-
-                    browser = await puppeteer.launch({
-                        headless: true,
-                        args: ['--disable-gpu', '--no-sandbox', '--disable-setuid-sandbox', '--disable-dev-shm-usage']
-                    });
-
-                    // Workaround for timeouts/zombies is to kill after 30 secs
-                    setTimeout(function() {
-                        browser.close();
-                    }, 30000);
-
-                    const page = await browser.newPage();
-                    await page.goto((process.env.DRAWIO_SERVER_URL || 'https://viewer.diagrams.net') + '/export3.html', {
-                        waitUntil: 'networkidle0'
-                    });
-
-                    async function rederPage(pageIndex) {
-                        await page.evaluate((body, pageIndex) => {
-                            return render({
-                                xml: body.xml,
-                                format: body.format,
-                                w: body.w,
-                                h: body.h,
-                                border: body.border || 0,
-                                bg: body.bg,
-                                from: pageIndex,
-                                to: pageIndex,
-                                pageId: body.pageId,
-                                scale: body.scale || 1,
-                                extras: body.extras
-                            });
-                        }, req.body, pageIndex);
-
-                        //default timeout is 30000 (30 sec)
-                        await page.waitForSelector('#LoadingComplete');
 
-                        var bounds = await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('bounds'));
-                        var pageId = await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('page-id'));
-                        var scale = await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('scale'));
-                        var pageCount = parseInt(await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('pageCount')));
-                        var pdfOptions = {
-                            format: 'A4'
-                        };
+                req.body.w = req.body.w || 0;
+                req.body.h = req.body.h || 0;
 
-                        if (bounds != null) {
-                            bounds = JSON.parse(bounds);
+                // Checks parameters
+                if (req.body.format && xml && req.body.w * req.body.h <= MAX_AREA) {
+                    var browser = null;
 
-                            var isPdf = req.body.format == 'pdf';
+                    try {
+                        var reqStr = ((xml != null) ? "xml=" + xml.length : "") +
+                            ((req.body.embedXml != null) ? " embed=" + req.body.embedXml : "") + " format=" +
+                            req.body.format;
 
-                            //Chrome generates Pdf files larger than requested pixels size and requires scaling
-                            //For images, the fixing scale shows scrollbars
-                            var fixingScale = isPdf ? 0.959 : 1;
+                        req.body.xml = xml;
 
-                            var w = Math.ceil(Math.ceil(bounds.width + bounds.x) * fixingScale);
+                        var t0 = Date.now();
 
-                            // +0.1 fixes cases where adding 1px below is not enough
-                            // Increase this if more cropped PDFs have extra empty pages
-                            var h = Math.ceil(Math.ceil(bounds.height + bounds.y) * fixingScale + (isPdf ? 0.1 : 0));
+                        browser = await puppeteer.launch({
+                            headless: true,
+                            args: ['--disable-gpu', '--no-sandbox', '--disable-setuid-sandbox', '--disable-dev-shm-usage']
+                        });
 
-                            page.setViewport({
-                                width: w,
-                                height: h
+                        // Workaround for timeouts/zombies is to kill after 30 secs
+                        setTimeout(function() {
+                            browser.close();
+                        }, 30000);
+
+                        const page = await browser.newPage();
+
+                        async function renderPage(pageIndex) {
+                            // LATER: Reuse same page (ie. reuse image- and font cache, reset state, viewport and remove LoadingComplete on each iteration)
+                            await page.goto((process.env.DRAWIO_SERVER_URL || 'https://viewer.diagrams.net') + '/export3.html', {
+                                waitUntil: 'networkidle0'
                             });
 
-                            pdfOptions = {
-                                printBackground: true,
-                                width: w + 'px',
-                                height: (h + 1) + 'px', //the extra pixel to prevent adding an extra empty page
-                                margin: {
-                                    top: '0px',
-                                    bottom: '0px',
-                                    left: '0px',
-                                    right: '0px'
+                            await page.evaluate((body, pageIndex) => {
+                                return render({
+                                    xml: body.xml,
+                                    format: body.format,
+                                    w: body.w,
+                                    h: body.h,
+                                    border: body.border || 0,
+                                    bg: body.bg,
+                                    from: pageIndex,
+                                    to: pageIndex,
+                                    pageId: body.pageId,
+                                    scale: body.scale || 1,
+                                    extras: body.extras
+                                });
+                            }, req.body, pageIndex);
+
+                            //default timeout is 30000 (30 sec)
+                            await page.waitForSelector('#LoadingComplete');
+
+                            var bounds = await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('bounds'));
+                            var pageId = await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('page-id'));
+                            var scale = await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('scale'));
+                            var pageCount = parseInt(await page.mainFrame().$eval('#LoadingComplete', div => div.getAttribute('pageCount')));
+                            var pdfOptions = {
+                                format: 'A4'
+                            };
+
+                            if (bounds != null) {
+                                bounds = JSON.parse(bounds);
+
+                                var isPdf = req.body.format == 'pdf';
+
+                                //Chrome generates Pdf files larger than requested pixels size and requires scaling
+                                //For images, the fixing scale shows scrollbars
+                                var fixingScale = isPdf ? 0.959 : 1;
+
+                                var w = Math.ceil(Math.ceil(bounds.width + bounds.x) * fixingScale);
+
+                                // +0.1 fixes cases where adding 1px below is not enough
+                                // Increase this if more cropped PDFs have extra empty pages
+                                var h = Math.ceil(Math.ceil(bounds.height + bounds.y) * fixingScale + (isPdf ? 0.1 : 0));
+
+                                page.setViewport({
+                                    width: w,
+                                    height: h
+                                });
+
+                                pdfOptions = {
+                                    printBackground: true,
+                                    omitBackground: true,
+                                    width: w + 'px',
+                                    height: (h + 2) + 'px', //the extra 2 pixels to prevent adding an extra empty page
+                                    margin: {
+                                        top: '0px',
+                                        bottom: '0px',
+                                        left: '0px',
+                                        right: '0px'
+                                    }
                                 }
                             }
-                        }
 
-                        return {
-                            pdfOptions: pdfOptions,
-                            pageId: pageId,
-                            scale: scale,
-                            pageCount: pageCount,
-                            w: w,
-                            h: h
-                        };
-                    }
+                            return {
+                                pdfOptions: pdfOptions,
+                                pageId: pageId,
+                                scale: scale,
+                                pageCount: pageCount,
+                                w: w,
+                                h: h
+                            };
+                        }
+
+                        // Cross-origin access should be allowed to now
+                        res.header("Access-Control-Allow-Origin", "*");
+
+                        var base64encoded = req.body.base64 == "1";
+
+                        if (req.body.format == 'png' || req.body.format == 'jpg' || req.body.format == 'jpeg') {
+                            var info = await renderPage(req.body.from || 0);
+                            var pageId = info.pageId,
+                                scale = info.scale,
+                                h = info.h,
+                                w = info.w;
+
+                            var data = await page.screenshot({
+                                omitBackground: req.body.format == 'png' && (req.body.bg == null || req.body.bg == 'none'),
+                                type: req.body.format == 'jpg' ? 'jpeg' : req.body.format,
+                                fullPage: true
+                            });
 
-                    // Cross-origin access should be allowed to now
-                    res.header("Access-Control-Allow-Origin", "*");
+                            if (req.body.dpi != null && req.body.format == 'png') {
+                                data = writePngWithText(data, 'dpi', req.body.dpi);
+                            }
 
-                    var base64encoded = req.body.base64 == "1";
+                            if (req.body.embedXml == "1" && req.body.format == 'png') {
+                                data = writePngWithText(data, "mxGraphModel", xml, true,
+                                    base64encoded);
+                            } else if (req.body.embedData == "1" && req.body.format == 'png') {
+                                data = writePngWithText(data, req.body.dataHeader, req.body.data, true,
+                                    base64encoded);
+                            } else {
+                                if (base64encoded) {
+                                    data = data.toString('base64');
+                                }
 
-                    if (req.body.format == 'png' || req.body.format == 'jpg' || req.body.format == 'jpeg') {
-                        var info = await rederPage(req.body.from || 0);
-                        var pageId = info.pageId,
-                            scale = info.scale,
-                            h = info.h,
-                            w = info.w;
-
-                        var data = await page.screenshot({
-                            omitBackground: req.body.format == 'png' && (req.body.bg == null || req.body.bg == 'none'),
-                            type: req.body.format == 'jpg' ? 'jpeg' : req.body.format,
-                            fullPage: true
-                        });
+                                if (data.length == 0) {
+                                    throw new Error("Invalid image");
+                                }
+                            }
 
-                        if (req.body.dpi != null && req.body.format == 'png') {
-                            data = writePngWithText(data, 'dpi', req.body.dpi);
-                        }
+                            if (req.body.filename != null) {
+                                logger.info("Filename in request " + req.body.filename);
 
-                        if (req.body.embedXml == "1" && req.body.format == 'png') {
-                            data = writePngWithText(data, "mxGraphModel", xml, true,
-                                base64encoded);
-                        } else if (req.body.embedData == "1" && req.body.format == 'png') {
-                            data = writePngWithText(data, req.body.dataHeader, req.body.data, true,
-                                base64encoded);
-                        } else {
-                            if (base64encoded) {
-                                data = data.toString('base64');
+                                res.header('Content-disposition', 'attachment; filename="' + req.body.filename +
+                                    '"; filename*=UTF-8\'\'' + req.body.filename);
                             }
 
-                            if (data.length == 0) {
-                                throw new Error("Invalid image");
-                            }
-                        }
+                            res.header('Content-type', base64encoded ? 'text/plain' : ('image/' + req.body.format));
+                            res.header("Content-Length", data.length);
 
-                        if (req.body.filename != null) {
-                            logger.info("Filename in request " + req.body.filename);
+                            // These two parameters are for Google Docs or other recipients to transfer the real image width x height information
+                            // (in case this information is inaccessible or lost)
+                            res.header("content-ex-width", w);
+                            res.header("content-ex-height", h);
 
-                            res.header('Content-disposition', 'attachment; filename="' + req.body.filename +
-                                '"; filename*=UTF-8\'\'' + req.body.filename);
-                        }
+                            if (pageId != null && pageId != 'undefined') {
+                                res.header("content-page-id", pageId);
+                            }
 
-                        res.header('Content-type', base64encoded ? 'text/plain' : ('image/' + req.body.format));
-                        res.header("Content-Length", data.length);
+                            if (scale != null && scale != 'undefined') {
+                                res.header("content-scale", scale);
+                            }
 
-                        // These two parameters are for Google Docs or other recipients to transfer the real image width x height information
-                        // (in case this information is inaccessible or lost)
-                        res.header("content-ex-width", w);
-                        res.header("content-ex-height", h);
+                            res.end(data);
 
-                        if (pageId != null && pageId != 'undefined') {
-                            res.header("content-page-id", pageId);
-                        }
+                            var dt = Date.now() - t0;
 
-                        if (scale != null && scale != 'undefined') {
-                            res.header("content-scale", scale);
-                        }
+                            logger.info("Success " + reqStr + " dt=" + dt);
+                        } else if (req.body.format == 'pdf' || req.body.format == 'svg') {
+                            var isSVG = req.body.format == 'svg';
+                            var from = req.body.allPages ? 0 : parseInt(req.body.from || 0);
+                            var to = isSVG ? from + 1 : //SVG is for one page only
+                                (req.body.allPages ? 1000 : parseInt(req.body.to || 1000) + 1); //The 'to' will be corrected later
+                            var pageId;
+                            var pdfs = [];
+
+                            for (var i = from; i < to; i++) {
+                                var info = await renderPage(i);
+                                pageId = info.pageId;
+                                to = to > info.pageCount ? info.pageCount : to;
+                                pdfs.push(await page.pdf(info.pdfOptions));
+                            }
 
-                        res.end(data);
+                            var data = isSVG ? await pdfToSvg(pdfs[0], req.body.embedXml == '1' ? xml : null,
+                                    req.body.bg == null || req.body.bg == 'none') :
+                                await mergePdfs(pdfs, req.body.embedXml == '1' ? xml : null);
+
+                            if (req.body.filename != null) {
+                                res.header('Content-disposition', 'attachment; filename="' + req.body.filename +
+                                    '"; filename*=UTF-8\'\'' + req.body.filename);
+                            }
 
-                        var dt = Date.now() - t0;
+                            if (base64encoded) {
+                                data = data.toString('base64');
+                            }
 
-                        logger.info("Success " + reqStr + " dt=" + dt);
-                    } else if (req.body.format == 'pdf') {
-                        var from = req.body.allPages ? 0 : parseInt(req.body.from || 0);
-                        var to = req.body.allPages ? 1000 : parseInt(req.body.to || 1000) + 1; //The 'to' will be corrected later
-                        var pageId;
-                        var pdfs = [];
+                            res.header('Content-type', isSVG ? 'image/svg+xml' : (base64encoded ? 'text/plain' : 'application/pdf'));
+                            res.header("Content-Length", data.length);
 
-                        for (var i = from; i < to; i++) {
-                            var info = await rederPage(i);
-                            pageId = info.pageId;
-                            to = to > info.pageCount ? info.pageCount : to;
-                            await page.emulateMedia('screen');
-                            await page._emulationManager._client.send(
-                                'Emulation.setDefaultBackgroundColorOverride', {
-                                    color: {
-                                        r: 0,
-                                        g: 0,
-                                        b: 0,
-                                        a: 0
-                                    }
-                                }
-                            );
-                            pdfs.push(await page.pdf(info.pdfOptions));
-                        }
+                            if (pageId != null && pageId != 'undefined') {
+                                res.header("content-page-id", pageId);
+                            }
 
-                        var data = await mergePdfs(pdfs, req.body.embedXml == '1' ? xml : null);
+                            res.end(data);
 
-                        if (req.body.filename != null) {
-                            res.header('Content-disposition', 'attachment; filename="' + req.body.filename +
-                                '"; filename*=UTF-8\'\'' + req.body.filename);
-                        }
+                            var dt = Date.now() - t0;
 
-                        if (base64encoded) {
-                            data = data.toString('base64');
+                            logger.info("Success " + reqStr + " dt=" + dt);
+                        } else {
+                            //BAD_REQUEST
+                            res.status(400).end("Unsupported Format!");
+                            logger.warn("Unsupported Format: " + req.body.format);
                         }
-
-                        res.header('Content-type', base64encoded ? 'text/plain' : 'application/pdf');
-                        res.header("Content-Length", data.length);
-
-                        if (pageId != null && pageId != 'undefined') {
-                            res.header("content-page-id", pageId);
+                        await browser.close();
+                    } catch (e) {
+                        if (browser != null) {
+                            browser.close();
                         }
 
-                        res.end(data);
+                        res.status(500).end("Error!");
 
-                        var dt = Date.now() - t0;
+                        var ip = (req.headers['x-forwarded-for'] ||
+                            req.connection.remoteAddress ||
+                            req.socket.remoteAddress ||
+                            req.connection.socket.remoteAddress).split(",")[0];
 
-                        logger.info("Success " + reqStr + " dt=" + dt);
-                    } else {
-                        //BAD_REQUEST
-                        res.status(400).end("Unsupported Format!");
-                        logger.warn("Unsupported Format: " + req.body.format);
-                    }
-                    await browser.close();
-                } catch (e) {
-                    if (browser != null) {
-                        browser.close();
-                    }
+                        var reqStr = "ip=" + ip + " ";
 
-                    res.status(500).end("Error!");
-
-                    var ip = (req.headers['x-forwarded-for'] ||
-                        req.connection.remoteAddress ||
-                        req.socket.remoteAddress ||
-                        req.connection.socket.remoteAddress).split(",")[0];
+                        if (req.body.format != null) {
+                            reqStr += ("format=" + req.body.format + " ");
+                        }
 
-                    var reqStr = "ip=" + ip + " ";
+                        if (req.body.w != null) {
+                            reqStr += ("w=" + req.body.w + " ");
+                        }
 
-                    if (req.body.format != null) {
-                        reqStr += ("format=" + req.body.format + " ");
-                    }
+                        if (req.body.h != null) {
+                            reqStr += ("h=" + req.body.h + " ");
+                        }
 
-                    if (req.body.w != null) {
-                        reqStr += ("w=" + req.body.w + " ");
-                    }
+                        if (req.body.scale != null) {
+                            reqStr += ("s=" + req.body.scale + " ");
+                        }
 
-                    if (req.body.h != null) {
-                        reqStr += ("h=" + req.body.h + " ");
-                    }
+                        if (req.body.bg != null) {
+                            reqStr += ("bg=" + req.body.bg + " ");
+                        }
 
-                    if (req.body.scale != null) {
-                        reqStr += ("s=" + req.body.scale + " ");
-                    }
+                        if (req.body.xmlData != null) {
+                            reqStr += ("xmlData=" + req.body.xmlData.length + " ");
+                        }
 
-                    if (req.body.bg != null) {
-                        reqStr += ("bg=" + req.body.bg + " ");
-                    }
+                        logger.warn("Handled exception: " + e.message +
+                            " req=" + reqStr, {
+                                stack: e.stack
+                            });
 
-                    if (req.body.xmlData != null) {
-                        reqStr += ("xmlData=" + req.body.xmlData.length + " ");
                     }
-
-                    logger.warn("Handled exception: " + e.message +
-                        " req=" + reqStr, {
-                            stack: e.stack
-                        });
-
+                } else {
+                    res.status(400).end("BAD REQUEST");
                 }
-            } else {
-                res.status(400).end("BAD REQUEST");
             }
+        } catch (e) {
+            logger.error(e.message, {
+                stack: e.stack
+            });
+            //INTERNAL_SERVER_ERROR
+            res.status(500).end("Unknown error");
         }
-    } catch (e) {
-        logger.error(e.message, {
-            stack: e.stack
-        });
-        //INTERNAL_SERVER_ERROR
-        res.status(500).end("Unknown error");
-    }
-};
+    };
 
-app.listen(PORT, function() {
-    console.log(`draw.io export server listening on port ${PORT}...`);
-});
+    app.listen(PORT, function() {
+        if (NO_CLUSTER) {
+            console.log(`draw.io export server listening on port ${PORT}...`);
+        } else {
+            console.log(`draw.io export server worker ${cluster.worker.id} listening on port ${PORT}...`);
+        }
+    });
+}
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/package.json` & `ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9419191919191918%*

 * *Differences: {"'dependencies'": "{'crc': '^4.3.1', 'express': '^4.18.2', 'node-fetch': '^3.3.0', 'pdf-lib': "*

 * *                   "'^1.17.1', 'puppeteer': '^19.5.2', 'winston': '^3.8.2', 'jsdom': '^21.0.0', "*

 * *                   "delete: ['body-parser', 'xmldom']}",*

 * * "'devDependencies'": "{'nodemon': '^2.0.20'}"}*

```diff
@@ -1,24 +1,23 @@
 {
     "author": "",
     "dependencies": {
-        "body-parser": "^1.19.0",
         "compression": "^1.7.4",
-        "crc": "^3.8.0",
-        "express": "^4.16.4",
+        "crc": "^4.3.1",
+        "express": "^4.18.2",
+        "jsdom": "^21.0.0",
         "morgan": "^1.9.1",
-        "node-fetch": "^2.6.1",
-        "pdf-lib": "^1.16.0",
-        "puppeteer": "^1.15.0",
-        "winston": "^3.2.1",
-        "xmldom": "^0.1.27"
+        "node-fetch": "^3.3.0",
+        "pdf-lib": "^1.17.1",
+        "puppeteer": "^19.5.2",
+        "winston": "^3.8.2"
     },
     "description": "",
     "devDependencies": {
-        "nodemon": "^2.0.7"
+        "nodemon": "^2.0.20"
     },
     "license": "ISC",
     "main": "export.js",
     "name": "drawio-export",
     "scripts": {
         "devstart": "nodemon export.js",
         "start": "node export.js",
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export/vendor/draw-image-export2/yarn.lock` & `ipydrawio-export-1.3.0/src/ipydrawio_export/vendor/draw-image-export2/yarn.lock`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # THIS IS AN AUTOGENERATED FILE. DO NOT EDIT THIS FILE DIRECTLY.
 # yarn lockfile v1
 
 
+"@babel/code-frame@^7.0.0":
+  version "7.21.4"
+  resolved "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.21.4.tgz#d0fa9e4413aca81f2b23b9442797bda1826edb39"
+  integrity sha512-LYvhNKfwWSPpocw8GI7gpK2nq3HSDuEPC/uSYaALSJu9xjsalaaYFOq0Pwt5KmVqwEbZlDu81aLXwBOmD/Fv9g==
+  dependencies:
+    "@babel/highlight" "^7.18.6"
+
+"@babel/helper-validator-identifier@^7.18.6":
+  version "7.19.1"
+  resolved "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.19.1.tgz#7eea834cf32901ffdc1a7ee555e2f9c27e249ca2"
+  integrity sha512-awrNfaMtnHUr653GgGEs++LlAvW6w+DcPrOliSMXWCKo597CwL5Acf/wWdNkf/tfEQE3mjkeD1YOVZOUV/od1w==
+
+"@babel/highlight@^7.18.6":
+  version "7.18.6"
+  resolved "https://registry.npmjs.org/@babel/highlight/-/highlight-7.18.6.tgz#81158601e93e2563795adcbfbdf5d64be3f2ecdf"
+  integrity sha512-u7stbOuYjaPezCuLj29hNW1v64M2Md2qupEKP1fHc7WdOA3DgLh37suiSrZYY7haUB7iBeQZ9P1uiRF359do3g==
+  dependencies:
+    "@babel/helper-validator-identifier" "^7.18.6"
+    chalk "^2.0.0"
+    js-tokens "^4.0.0"
+
 "@colors/colors@1.5.0":
   version "1.5.0"
   resolved "https://registry.npmjs.org/@colors/colors/-/colors-1.5.0.tgz#bb504579c1cae923e6576a4f5da43d25f97bdbd9"
   integrity sha512-ooWCrlZP11i8GImSjTHYHLkvFDP48nS4+204nGb1RiX/WXYHmJA2III9/e2DWVabCESdW7hBAEzHRqUn9OUVvQ==
 
 "@dabh/diagnostics@^2.0.2":
   version "2.0.3"
@@ -26,57 +47,140 @@
 "@pdf-lib/upng@^1.0.1":
   version "1.0.1"
   resolved "https://registry.npmjs.org/@pdf-lib/upng/-/upng-1.0.1.tgz#7dc9c636271aca007a9df4deaf2dd7e7960280cb"
   integrity sha512-dQK2FUMQtowVP00mtIksrlZhdFXQZPC+taih1q4CvPZ5vqdxR/LKBaFg0oAfzd1GlHZXXSPdQfzQnt+ViGvEIQ==
   dependencies:
     pako "^1.0.10"
 
+"@puppeteer/browsers@0.4.0":
+  version "0.4.0"
+  resolved "https://registry.npmjs.org/@puppeteer/browsers/-/browsers-0.4.0.tgz#abaae1eddc9902e1ea441e34171229bd7644ea62"
+  integrity sha512-3iB5pWn9Sr55PKKwqFWSWjLsTKCOEhKNI+uV3BZesgXuA3IhsX8I3hW0HI+3ksMIPkh2mVYzKSpvgq3oicjG2Q==
+  dependencies:
+    debug "4.3.4"
+    extract-zip "2.0.1"
+    https-proxy-agent "5.0.1"
+    progress "2.0.3"
+    proxy-from-env "1.1.0"
+    tar-fs "2.1.1"
+    unbzip2-stream "1.4.3"
+    yargs "17.7.1"
+
+"@tootallnate/once@2":
+  version "2.0.0"
+  resolved "https://registry.npmjs.org/@tootallnate/once/-/once-2.0.0.tgz#f544a148d3ab35801c1f633a7441fd87c2e484bf"
+  integrity sha512-XCuKFP5PS55gnMVu3dty8KPatLqUoy/ZYzDzAGCQ8JNFCkLXzmI7vNHCR+XpbZaMWQK/vQubr7PkYq8g470J/A==
+
+"@types/node@*":
+  version "18.15.11"
+  resolved "https://registry.npmjs.org/@types/node/-/node-18.15.11.tgz#b3b790f09cb1696cffcec605de025b088fa4225f"
+  integrity sha512-E5Kwq2n4SbMzQOn6wnmBjuK9ouqlURrcZDVfbo9ftDDTFt3nk7ZKK4GMOzoYgnpQJKcxwQw+lGaBvvlMo0qN/Q==
+
+"@types/triple-beam@^1.3.2":
+  version "1.3.2"
+  resolved "https://registry.npmjs.org/@types/triple-beam/-/triple-beam-1.3.2.tgz#38ecb64f01aa0d02b7c8f4222d7c38af6316fef8"
+  integrity sha512-txGIh+0eDFzKGC25zORnswy+br1Ha7hj5cMVwKIU7+s0U2AxxJru/jZSMU6OC9MJWP6+pc/hc6ZjyZShpsyY2g==
+
+"@types/yauzl@^2.9.1":
+  version "2.10.0"
+  resolved "https://registry.npmjs.org/@types/yauzl/-/yauzl-2.10.0.tgz#b3248295276cf8c6f153ebe6a9aba0c988cb2599"
+  integrity sha512-Cn6WYCm0tXv8p6k+A8PvbDG763EDpBoTzHdA+Q/MF6H3sapGjCm9NzoaJncJS9tUKSuCoDs9XHxYYsQDgxR6kw==
+  dependencies:
+    "@types/node" "*"
+
+abab@^2.0.6:
+  version "2.0.6"
+  resolved "https://registry.npmjs.org/abab/-/abab-2.0.6.tgz#41b80f2c871d19686216b82309231cfd3cb3d291"
+  integrity sha512-j2afSsaIENvHZN2B8GOpF566vZ5WVk5opAiMTvWgaQT8DkbOqsTfvNAvHoRGU2zzP8cPoqys+xHTRDWW8L+/BA==
+
 abbrev@1:
   version "1.1.1"
   resolved "https://registry.npmjs.org/abbrev/-/abbrev-1.1.1.tgz#f8f2c887ad10bf67f634f005b6987fed3179aac8"
   integrity sha512-nne9/IiQ/hzIhY6pdDnbBtz7DjPTKrY00P/zvPSm5pOFkl6xuGrGnXn/VtTNNfNtAfZ9/1RtehkszU9qcTii0Q==
 
 accepts@~1.3.5, accepts@~1.3.8:
   version "1.3.8"
   resolved "https://registry.npmjs.org/accepts/-/accepts-1.3.8.tgz#0bf0be125b67014adcb0b0921e62db7bffe16b2e"
   integrity sha512-PYAthTa2m2VKxuvSD3DPC/Gy+U+sOA1LAuT8mkmRuvw+NACSaeXEQ+NHcVF7rONl6qcaxV3Uuemwawk+7+SJLw==
   dependencies:
     mime-types "~2.1.34"
     negotiator "0.6.3"
 
-agent-base@^4.3.0:
+acorn-globals@^7.0.0:
+  version "7.0.1"
+  resolved "https://registry.npmjs.org/acorn-globals/-/acorn-globals-7.0.1.tgz#0dbf05c44fa7c94332914c02066d5beff62c40c3"
+  integrity sha512-umOSDSDrfHbTNPuNpC2NSnnA3LUrqpevPb4T9jRx4MagXNS0rs+gwiTcAvqCRmsD6utzsrzNt+ebm00SNWiC3Q==
+  dependencies:
+    acorn "^8.1.0"
+    acorn-walk "^8.0.2"
+
+acorn-walk@^8.0.2:
+  version "8.2.0"
+  resolved "https://registry.npmjs.org/acorn-walk/-/acorn-walk-8.2.0.tgz#741210f2e2426454508853a2f44d0ab83b7f69c1"
+  integrity sha512-k+iyHEuPgSw6SbuDpGQM+06HQUa04DZ3o+F6CSzXMvvI5KMvnaEqXe+YVe555R9nn6GPt404fos4wcgpw12SDA==
+
+acorn@^8.1.0, acorn@^8.8.2:
+  version "8.8.2"
+  resolved "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz#1b2f25db02af965399b9776b0c2c391276d37c4a"
+  integrity sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==
+
+agent-base@6:
+  version "6.0.2"
+  resolved "https://registry.npmjs.org/agent-base/-/agent-base-6.0.2.tgz#49fff58577cfee3f37176feab4c22e00f86d7f77"
+  integrity sha512-RZNwNclF7+MS/8bDg70amg32dyeZGZxiDuQmZxKLAlQjr3jGyLx+4Kkk58UO7D2QdgFIQCovuSuZESne6RG6XQ==
+  dependencies:
+    debug "4"
+
+ansi-regex@^5.0.1:
+  version "5.0.1"
+  resolved "https://registry.npmjs.org/ansi-regex/-/ansi-regex-5.0.1.tgz#082cb2c89c9fe8659a311a53bd6a4dc5301db304"
+  integrity sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==
+
+ansi-styles@^3.2.1:
+  version "3.2.1"
+  resolved "https://registry.npmjs.org/ansi-styles/-/ansi-styles-3.2.1.tgz#41fbb20243e50b12be0f04b8dedbf07520ce841d"
+  integrity sha512-VT0ZI6kZRdTh8YyJw3SMbYm/u+NqfsAxEpWO0Pf9sq8/e94WxxOpPKx9FR1FlyCtOVDNOQ+8ntlqFxiRc+r5qA==
+  dependencies:
+    color-convert "^1.9.0"
+
+ansi-styles@^4.0.0:
   version "4.3.0"
-  resolved "https://registry.npmjs.org/agent-base/-/agent-base-4.3.0.tgz#8165f01c436009bccad0b1d122f05ed770efc6ee"
-  integrity sha512-salcGninV0nPrwpGNn4VTXBb1SOuXQBiqbrNXoeizJsHrsL6ERFM2Ne3JUSBWRE6aeNJI2ROP/WEEIDUiDe3cg==
+  resolved "https://registry.npmjs.org/ansi-styles/-/ansi-styles-4.3.0.tgz#edd803628ae71c04c85ae7a0906edad34b648937"
+  integrity sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==
   dependencies:
-    es6-promisify "^5.0.0"
+    color-convert "^2.0.1"
 
 anymatch@~3.1.2:
-  version "3.1.2"
-  resolved "https://registry.npmjs.org/anymatch/-/anymatch-3.1.2.tgz#c0557c096af32f106198f4f4e2a383537e378716"
-  integrity sha512-P43ePfOAIupkguHUycrc4qJ9kz8ZiuOUijaETwX7THt0Y/GNK7v0aa8rY816xWjZ7rJdA5XdMcpVFTKMq+RvWg==
+  version "3.1.3"
+  resolved "https://registry.npmjs.org/anymatch/-/anymatch-3.1.3.tgz#790c58b19ba1720a84205b57c618d5ad8524973e"
+  integrity sha512-KMReFUr0B4t+D+OBkjR3KYqvocp2XaSzO55UcB6mgQMd3KbcE+mWTyvVV7D/zsdEbNnV6acZUutkiHQXvTr1Rw==
   dependencies:
     normalize-path "^3.0.0"
     picomatch "^2.0.4"
 
+argparse@^2.0.1:
+  version "2.0.1"
+  resolved "https://registry.npmjs.org/argparse/-/argparse-2.0.1.tgz#246f50f3ca78a3240f6c997e8a9bd1eac49e4b38"
+  integrity sha512-8+9WqebbFzpX9OR+Wa6O29asIogeRMzcGtAINdpMHHyAg10f05aSFVBbcEqGf/PXw1EjAZ+q2/bEBg3DvurK3Q==
+
 array-flatten@1.1.1:
   version "1.1.1"
   resolved "https://registry.npmjs.org/array-flatten/-/array-flatten-1.1.1.tgz#9a5f699051b1e7073328f2a008968b64ea2955d2"
   integrity sha512-PCVAQswWemu6UdxsDFFX/+gVeYqKAod3D3UVm91jHwynguOwAvYPhx8nNlM++NqRcK6CxxpUafjmhIdKiHibqg==
 
-async-limiter@~1.0.0:
-  version "1.0.1"
-  resolved "https://registry.npmjs.org/async-limiter/-/async-limiter-1.0.1.tgz#dd379e94f0db8310b08291f9d64c3209766617fd"
-  integrity sha512-csOlWGAcRFJaI6m+F2WKdnMKr4HhdhFVBk0H/QbJFMCr+uO2kwohwXQPxw/9OCxp05r5ghVBFSyioixx3gfkNQ==
-
 async@^3.2.3:
   version "3.2.4"
   resolved "https://registry.npmjs.org/async/-/async-3.2.4.tgz#2d22e00f8cddeb5fde5dd33522b56d1cf569a81c"
   integrity sha512-iAB+JbDEGXhyIUavoDl9WP/Jj106Kz9DEn1DPgYw5ruDn0e3Wgi3sKFm55sASdGBNOQB8F59d9qQ7deqrHA8wQ==
 
+asynckit@^0.4.0:
+  version "0.4.0"
+  resolved "https://registry.npmjs.org/asynckit/-/asynckit-0.4.0.tgz#c79ed97f7f34cb8f2ba1bc9790bcc366474b4b79"
+  integrity sha512-Oei9OH4tRh0YqU3GxhX79dM/mwVgvbZJaSNaRk+bshkj0S5cfHcgYakreBjrHwatXKbz+IoIdYLxrKim2MjW0Q==
+
 balanced-match@^1.0.0:
   version "1.0.2"
   resolved "https://registry.npmjs.org/balanced-match/-/balanced-match-1.0.2.tgz#e83e3a7e3f300b34cb9d87f615fa0cbf357690ee"
   integrity sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==
 
 base64-js@^1.3.1:
   version "1.5.1"
@@ -91,15 +195,24 @@
     safe-buffer "5.1.2"
 
 binary-extensions@^2.0.0:
   version "2.2.0"
   resolved "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.2.0.tgz#75f502eeaf9ffde42fc98829645be4ea76bd9e2d"
   integrity sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==
 
-body-parser@1.20.1, body-parser@^1.19.0:
+bl@^4.0.3:
+  version "4.1.0"
+  resolved "https://registry.npmjs.org/bl/-/bl-4.1.0.tgz#451535264182bec2fbbc83a62ab98cf11d9f7b3a"
+  integrity sha512-1W07cM9gS6DcLperZfFSj+bWLtaPGSOHWhPiGzXmvVJbRLdG82sH/Kn8EtW1VqWVA54AKf2h5k5BbnIbwF3h6w==
+  dependencies:
+    buffer "^5.5.0"
+    inherits "^2.0.4"
+    readable-stream "^3.4.0"
+
+body-parser@1.20.1:
   version "1.20.1"
   resolved "https://registry.npmjs.org/body-parser/-/body-parser-1.20.1.tgz#b1812a8912c195cd371a3ee5e66faa2338a5c668"
   integrity sha512-jWi7abTbYwajOytWCQc37VulmWiRae5RyTpaCyDcS5/lMdtwSz5lOpDE67srw/HYe35f1z3fDQw+3txg7gNtWw==
   dependencies:
     bytes "3.1.2"
     content-type "~1.0.4"
     debug "2.6.9"
@@ -129,20 +242,15 @@
     fill-range "^7.0.1"
 
 buffer-crc32@~0.2.3:
   version "0.2.13"
   resolved "https://registry.npmjs.org/buffer-crc32/-/buffer-crc32-0.2.13.tgz#0d333e3f00eac50aa1454abd30ef8c2a5d9a7242"
   integrity sha512-VO9Ht/+p3SN7SKWqcrgEzjGbRSJYTx+Q1pTQC0wrWqHx0vpJraQ6GtHx8tvcg1rlK1byhU5gccxgOgj7B0TDkQ==
 
-buffer-from@^1.0.0:
-  version "1.1.2"
-  resolved "https://registry.npmjs.org/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
-  integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
-
-buffer@^5.1.0:
+buffer@^5.2.1, buffer@^5.5.0:
   version "5.7.1"
   resolved "https://registry.npmjs.org/buffer/-/buffer-5.7.1.tgz#ba62e7c13133053582197160851a8f648e99eed0"
   integrity sha512-EHcyIPBQ4BSGlvjB16k5KgAJ27CIsHY/2JBmCRReo48y9rQ3MaUzWX3KVlBa4U7MyX02HdVj0K7C3WaB3ju7FQ==
   dependencies:
     base64-js "^1.3.1"
     ieee754 "^1.1.13"
 
@@ -160,14 +268,28 @@
   version "1.0.2"
   resolved "https://registry.npmjs.org/call-bind/-/call-bind-1.0.2.tgz#b1d4e89e688119c3c9a903ad30abb2f6a919be3c"
   integrity sha512-7O+FbCihrB5WGbFYesctwmTKae6rOiIzmz1icreWJ+0aA7LJfuqhEso2T9ncpcFtzMQtzXf2QGGueWJGTYsqrA==
   dependencies:
     function-bind "^1.1.1"
     get-intrinsic "^1.0.2"
 
+callsites@^3.0.0:
+  version "3.1.0"
+  resolved "https://registry.npmjs.org/callsites/-/callsites-3.1.0.tgz#b3630abd8943432f54b3f0519238e33cd7df2f73"
+  integrity sha512-P8BjAsXvZS+VIDUI11hHCQEv74YT67YUi5JJFNWIqL235sBmjX4+qx9Muvls5ivyNENctx46xQLQ3aTuE7ssaQ==
+
+chalk@^2.0.0:
+  version "2.4.2"
+  resolved "https://registry.npmjs.org/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
+  integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
+  dependencies:
+    ansi-styles "^3.2.1"
+    escape-string-regexp "^1.0.5"
+    supports-color "^5.3.0"
+
 chokidar@^3.5.2:
   version "3.5.3"
   resolved "https://registry.npmjs.org/chokidar/-/chokidar-3.5.3.tgz#1cf37c8707b932bd1af1ae22c0432e2acd1903bd"
   integrity sha512-Dr3sfKRP6oTcjf2JmUmFJfeVMvXBdegxB0iVQ5eb2V10uFJUCAS8OByZdVAyVb8xXNz3GjjTgj9kLWsZTqE6kw==
   dependencies:
     anymatch "~3.1.2"
     braces "~3.0.2"
@@ -175,27 +297,55 @@
     is-binary-path "~2.1.0"
     is-glob "~4.0.1"
     normalize-path "~3.0.0"
     readdirp "~3.6.0"
   optionalDependencies:
     fsevents "~2.3.2"
 
-color-convert@^1.9.3:
+chownr@^1.1.1:
+  version "1.1.4"
+  resolved "https://registry.npmjs.org/chownr/-/chownr-1.1.4.tgz#6fc9d7b42d32a583596337666e7d08084da2cc6b"
+  integrity sha512-jJ0bqzaylmJtVnNgzTeSOs8DPavpbYgEr/b0YL8/2GO3xJEhInFmhKMUnEJQjZumK7KXGFhUy89PrsJWlakBVg==
+
+chromium-bidi@0.4.6:
+  version "0.4.6"
+  resolved "https://registry.npmjs.org/chromium-bidi/-/chromium-bidi-0.4.6.tgz#a082151834083ed002624f12fa35e748817b2ee5"
+  integrity sha512-TQOkWRaLI/IWvoP8XC+7jO4uHTIiAUiklXU1T0qszlUFEai9LgKXIBXy3pOS3EnQZ3bQtMbKUPkug0fTAEHCSw==
+  dependencies:
+    mitt "3.0.0"
+
+cliui@^8.0.1:
+  version "8.0.1"
+  resolved "https://registry.npmjs.org/cliui/-/cliui-8.0.1.tgz#0c04b075db02cbfe60dc8e6cf2f5486b1a3608aa"
+  integrity sha512-BSeNnyus75C4//NQ9gQt1/csTXyo/8Sb+afLAkzAptFuMsod9HFokGNudZpi/oQV73hnVK+sR+5PVRMd+Dr7YQ==
+  dependencies:
+    string-width "^4.2.0"
+    strip-ansi "^6.0.1"
+    wrap-ansi "^7.0.0"
+
+color-convert@^1.9.0, color-convert@^1.9.3:
   version "1.9.3"
   resolved "https://registry.npmjs.org/color-convert/-/color-convert-1.9.3.tgz#bb71850690e1f136567de629d2d5471deda4c1e8"
   integrity sha512-QfAUtd+vFdAtFQcC8CCyYt1fYWxSqAiK2cSD6zDB8N3cpsEBAvRxp9zOGg6G/SHHJYAT88/az/IuDGALsNVbGg==
   dependencies:
     color-name "1.1.3"
 
+color-convert@^2.0.1:
+  version "2.0.1"
+  resolved "https://registry.npmjs.org/color-convert/-/color-convert-2.0.1.tgz#72d3a68d598c9bdb3af2ad1e84f21d896abd4de3"
+  integrity sha512-RRECPsj7iu/xb5oKYcsFHSppFNnsj/52OVTRKb4zP5onXwVF3zVmmToNcOfGC+CRDpfK/U584fMg38ZHCaElKQ==
+  dependencies:
+    color-name "~1.1.4"
+
 color-name@1.1.3:
   version "1.1.3"
   resolved "https://registry.npmjs.org/color-name/-/color-name-1.1.3.tgz#a7d0558bd89c42f795dd42328f740831ca53bc25"
   integrity sha512-72fSenhMw2HZMTVHeCA9KCmpEIbzWiQsjN+BHcBbS9vr1mtt+vJjPdksIBNUmKAW8TFUDPJK5SUU3QhE9NEXDw==
 
-color-name@^1.0.0:
+color-name@^1.0.0, color-name@~1.1.4:
   version "1.1.4"
   resolved "https://registry.npmjs.org/color-name/-/color-name-1.1.4.tgz#c2a09a87acbde69543de6f63fa3995c826c536a2"
   integrity sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==
 
 color-string@^1.6.0:
   version "1.9.1"
   resolved "https://registry.npmjs.org/color-string/-/color-string-1.9.1.tgz#4467f9146f036f855b764dfb5bf8582bf342c7a4"
@@ -216,14 +366,21 @@
   version "1.1.4"
   resolved "https://registry.npmjs.org/colorspace/-/colorspace-1.1.4.tgz#8d442d1186152f60453bf8070cd66eb364e59243"
   integrity sha512-BgvKJiuVu1igBUF2kEjRCZXol6wiiGbY5ipL/oVPwm0BL9sIpMIzM8IK7vwuxIIzOXMV3Ey5w+vxhm0rR/TN8w==
   dependencies:
     color "^3.1.3"
     text-hex "1.0.x"
 
+combined-stream@^1.0.8:
+  version "1.0.8"
+  resolved "https://registry.npmjs.org/combined-stream/-/combined-stream-1.0.8.tgz#c3d45a8b34fd730631a110a8a2520682b31d5a7f"
+  integrity sha512-FQN4MRfuJeHf7cBbBMJFXhKSDq+2kAArBlmRBvcvFE5BB1HZKXtSFASDhdlz9zOYwxh8lDdnvmMOe/+5cdoEdg==
+  dependencies:
+    delayed-stream "~1.0.0"
+
 compressible@~2.0.16:
   version "2.0.18"
   resolved "https://registry.npmjs.org/compressible/-/compressible-2.0.18.tgz#af53cca6b070d4c3c0750fbd77286a6d7cc46fba"
   integrity sha512-AF3r7P5dWxL8MxyITRMlORQNaOA2IkAFaTr4k7BUumjPtRpGDTZpl0Pb1XCO6JeDCBdp126Cgs9sMxqSjgYyRg==
   dependencies:
     mime-db ">= 1.43.0 < 2"
 
@@ -241,127 +398,224 @@
     vary "~1.1.2"
 
 concat-map@0.0.1:
   version "0.0.1"
   resolved "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz#d8a96bd77fd68df7793a73036a3ba0d5405d477b"
   integrity sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==
 
-concat-stream@^1.6.2:
-  version "1.6.2"
-  resolved "https://registry.npmjs.org/concat-stream/-/concat-stream-1.6.2.tgz#904bdf194cd3122fc675c77fc4ac3d4ff0fd1a34"
-  integrity sha512-27HBghJxjiZtIk3Ycvn/4kbJk/1uZuJFfuPEns6LaEvpvG1f0hTea8lilrouyo9mVc2GWdcEZ8OLoGmSADlrCw==
-  dependencies:
-    buffer-from "^1.0.0"
-    inherits "^2.0.3"
-    readable-stream "^2.2.2"
-    typedarray "^0.0.6"
-
 content-disposition@0.5.4:
   version "0.5.4"
   resolved "https://registry.npmjs.org/content-disposition/-/content-disposition-0.5.4.tgz#8b82b4efac82512a02bb0b1dcec9d2c5e8eb5bfe"
   integrity sha512-FveZTNuGw04cxlAiWbzi6zTAL/lhehaWbTtgluJh4/E95DqMwTmha3KZN1aAWA8cFIhHzMZUvLevkw5Rqk+tSQ==
   dependencies:
     safe-buffer "5.2.1"
 
 content-type@~1.0.4:
-  version "1.0.4"
-  resolved "https://registry.npmjs.org/content-type/-/content-type-1.0.4.tgz#e138cc75e040c727b1966fe5e5f8c9aee256fe3b"
-  integrity sha512-hIP3EEPs8tB9AT1L+NUqtwOAps4mk2Zob89MWXMHjHWg9milF/j4osnnQLXBCBFBk/tvIG/tUc9mOUJiPBhPXA==
+  version "1.0.5"
+  resolved "https://registry.npmjs.org/content-type/-/content-type-1.0.5.tgz#8b773162656d1d1086784c8f23a54ce6d73d7918"
+  integrity sha512-nTjqfcBFEipKdXCv4YDQWCfmcLZKm81ldF0pAopTvyrFGVbcR6P/VAAd5G7N+0tTr8QqiU0tFadD6FK4NtJwOA==
 
 cookie-signature@1.0.6:
   version "1.0.6"
   resolved "https://registry.npmjs.org/cookie-signature/-/cookie-signature-1.0.6.tgz#e303a882b342cc3ee8ca513a79999734dab3ae2c"
   integrity sha512-QADzlaHc8icV8I7vbaJXJwod9HWYp8uCqf1xa4OfNu1T7JVxQIrUgOWtHdNDtPiywmFbiS12VjotIXLrKM3orQ==
 
 cookie@0.5.0:
   version "0.5.0"
   resolved "https://registry.npmjs.org/cookie/-/cookie-0.5.0.tgz#d1f5d71adec6558c58f389987c366aa47e994f8b"
   integrity sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==
 
-core-util-is@~1.0.0:
-  version "1.0.3"
-  resolved "https://registry.npmjs.org/core-util-is/-/core-util-is-1.0.3.tgz#a6042d3634c2b27e9328f837b965fac83808db85"
-  integrity sha512-ZQBvi1DcpJ4GDqanjucZ2Hj3wEO5pZDS89BWbkcrvdxksJorwUDDZamX9ldFkp9aw2lmBDLgkObEA4DWNJ9FYQ==
+cosmiconfig@8.1.3:
+  version "8.1.3"
+  resolved "https://registry.npmjs.org/cosmiconfig/-/cosmiconfig-8.1.3.tgz#0e614a118fcc2d9e5afc2f87d53cd09931015689"
+  integrity sha512-/UkO2JKI18b5jVMJUp0lvKFMpa/Gye+ZgZjKD+DGEN9y7NRcf/nK1A0sp67ONmKtnDCNMS44E6jrk0Yc3bDuUw==
+  dependencies:
+    import-fresh "^3.2.1"
+    js-yaml "^4.1.0"
+    parse-json "^5.0.0"
+    path-type "^4.0.0"
+
+crc@^4.3.1:
+  version "4.3.2"
+  resolved "https://registry.npmjs.org/crc/-/crc-4.3.2.tgz#49b7821cbf2cf61dfd079ed93863bbebd5469b9a"
+  integrity sha512-uGDHf4KLLh2zsHa8D8hIQ1H/HtFQhyHrc0uhHBcoKGol/Xnb+MPYfUMw7cvON6ze/GUESTudKayDcJC5HnJv1A==
+
+cross-fetch@3.1.5:
+  version "3.1.5"
+  resolved "https://registry.npmjs.org/cross-fetch/-/cross-fetch-3.1.5.tgz#e1389f44d9e7ba767907f7af8454787952ab534f"
+  integrity sha512-lvb1SBsI0Z7GDwmuid+mU3kWVBwTVUbe7S0H52yaaAdQOXq2YktTCZdlAcNKFzE6QtRz0snpw9bNiPeOIkkQvw==
+  dependencies:
+    node-fetch "2.6.7"
 
-crc@^3.8.0:
-  version "3.8.0"
-  resolved "https://registry.npmjs.org/crc/-/crc-3.8.0.tgz#ad60269c2c856f8c299e2c4cc0de4556914056c6"
-  integrity sha512-iX3mfgcTMIq3ZKLIsVFAbv7+Mc10kxabAGQb8HvjA1o3T1PIYprbakQ65d3I+2HGHt6nSKkM9PYjgoJO2KcFBQ==
+cssstyle@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.npmjs.org/cssstyle/-/cssstyle-3.0.0.tgz#17ca9c87d26eac764bb8cfd00583cff21ce0277a"
+  integrity sha512-N4u2ABATi3Qplzf0hWbVCdjenim8F3ojEXpBDF5hBpjzW182MjNGLqfmQ0SkSPeQ+V86ZXgeH8aXj6kayd4jgg==
   dependencies:
-    buffer "^5.1.0"
+    rrweb-cssom "^0.6.0"
+
+data-uri-to-buffer@^4.0.0:
+  version "4.0.1"
+  resolved "https://registry.npmjs.org/data-uri-to-buffer/-/data-uri-to-buffer-4.0.1.tgz#d8feb2b2881e6a4f58c2e08acfd0e2834e26222e"
+  integrity sha512-0R9ikRb668HB7QDxT1vkpuUBtqc53YyAwMwGeUFKRojY/NWKvdZ+9UYtRfGmhqNbRkTSVpMbmyhXipFFv2cb/A==
+
+data-urls@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/data-urls/-/data-urls-4.0.0.tgz#333a454eca6f9a5b7b0f1013ff89074c3f522dd4"
+  integrity sha512-/mMTei/JXPqvFqQtfyTowxmJVwr2PVAeCcDxyFf6LhoOu/09TX2OX3kb2wzi4DMXcfj4OItwDOnhl5oziPnT6g==
+  dependencies:
+    abab "^2.0.6"
+    whatwg-mimetype "^3.0.0"
+    whatwg-url "^12.0.0"
 
-debug@2.6.9, debug@^2.6.9:
+debug@2.6.9:
   version "2.6.9"
   resolved "https://registry.npmjs.org/debug/-/debug-2.6.9.tgz#5d128515df134ff327e90a4c93f4e077a536341f"
   integrity sha512-bC7ElrdJaJnPbAP+1EotYvqZsb3ecl5wi6Bfi6BJTUcNowp6cvspg0jXznRTKDjm/E7AdgFBVeAPVMNcKGsHMA==
   dependencies:
     ms "2.0.0"
 
-debug@^3.1.0, debug@^3.2.7:
+debug@4, debug@4.3.4, debug@^4.1.1:
+  version "4.3.4"
+  resolved "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz#1319f6579357f2338d3337d2cdd4914bb5dcc865"
+  integrity sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==
+  dependencies:
+    ms "2.1.2"
+
+debug@^3.2.7:
   version "3.2.7"
   resolved "https://registry.npmjs.org/debug/-/debug-3.2.7.tgz#72580b7e9145fb39b6676f9c5e5fb100b934179a"
   integrity sha512-CFjzYYAi4ThfiQvizrFQevTTXHtnCqWfe7x1AhgEscTz6ZbLbfoLRLPugTQyBth6f8ZERVUSyWHFD/7Wu4t1XQ==
   dependencies:
     ms "^2.1.1"
 
-debug@^4.1.0:
-  version "4.3.4"
-  resolved "https://registry.npmjs.org/debug/-/debug-4.3.4.tgz#1319f6579357f2338d3337d2cdd4914bb5dcc865"
-  integrity sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==
-  dependencies:
-    ms "2.1.2"
+decimal.js@^10.4.3:
+  version "10.4.3"
+  resolved "https://registry.npmjs.org/decimal.js/-/decimal.js-10.4.3.tgz#1044092884d245d1b7f65725fa4ad4c6f781cc23"
+  integrity sha512-VBBaLc1MgL5XpzgIP7ny5Z6Nx3UrRkIViUkPUdtl9aya5amy3De1gsUUSB1g3+3sExYNjCAsAznmukyxCb1GRA==
+
+deep-is@~0.1.3:
+  version "0.1.4"
+  resolved "https://registry.npmjs.org/deep-is/-/deep-is-0.1.4.tgz#a6f2dce612fadd2ef1f519b73551f17e85199831"
+  integrity sha512-oIPzksmTg4/MriiaYGO+okXDT7ztn/w3Eptv/+gSIdMdKsJo0u4CfYNFJPy+4SKMuCqGw2wxnA+URMg3t8a/bQ==
+
+delayed-stream@~1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmjs.org/delayed-stream/-/delayed-stream-1.0.0.tgz#df3ae199acadfb7d440aaae0b29e2272b24ec619"
+  integrity sha512-ZySD7Nf91aLB0RxL4KGrKHBXl7Eds1DAmEdcoVawXnLD7SDhpNgtuII2aAkg7a7QS41jxPSZ17p4VdGnMHk3MQ==
 
 depd@2.0.0, depd@~2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/depd/-/depd-2.0.0.tgz#b696163cc757560d09cf22cc8fad1571b79e76df"
   integrity sha512-g7nH6P6dyDioJogAAGprGpCtVImJhpPk/roCzdb3fIh61/s/nPsfR6onyMwkCAR/OlC3yBC0lESvUoQEAssIrw==
 
 destroy@1.2.0:
   version "1.2.0"
   resolved "https://registry.npmjs.org/destroy/-/destroy-1.2.0.tgz#4803735509ad8be552934c67df614f94e66fa015"
   integrity sha512-2sJGJTaXIIaR1w4iJSNoN0hnMY7Gpc/n8D4qSCJw8QqFWXf7cuAgnEHxBpweaVcPevC2l3KpjYCx3NypQQgaJg==
 
+devtools-protocol@0.0.1107588:
+  version "0.0.1107588"
+  resolved "https://registry.npmjs.org/devtools-protocol/-/devtools-protocol-0.0.1107588.tgz#f8cac707840b97cc30b029359341bcbbb0ad8ffa"
+  integrity sha512-yIR+pG9x65Xko7bErCUSQaDLrO/P1p3JUzEk7JCU4DowPcGHkTGUGQapcfcLc4qj0UaALwZ+cr0riFgiqpixcg==
+
+domexception@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/domexception/-/domexception-4.0.0.tgz#4ad1be56ccadc86fc76d033353999a8037d03673"
+  integrity sha512-A2is4PLG+eeSfoTMA95/s4pvAoSo2mKtiM5jlHkAVewmiO8ISFTFKZjH7UAM1Atli/OT/7JHOrJRJiMKUZKYBw==
+  dependencies:
+    webidl-conversions "^7.0.0"
+
 ee-first@1.1.1:
   version "1.1.1"
   resolved "https://registry.npmjs.org/ee-first/-/ee-first-1.1.1.tgz#590c61156b0ae2f4f0255732a158b266bc56b21d"
   integrity sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==
 
+emoji-regex@^8.0.0:
+  version "8.0.0"
+  resolved "https://registry.npmjs.org/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
+  integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
+
 enabled@2.0.x:
   version "2.0.0"
   resolved "https://registry.npmjs.org/enabled/-/enabled-2.0.0.tgz#f9dd92ec2d6f4bbc0d5d1e64e21d61cd4665e7c2"
   integrity sha512-AKrN98kuwOzMIdAizXGI86UFBoo26CL21UM763y1h/GMSJ4/OHU9k2YlsmBpyScFo/wbLzWQJBMCW4+IO3/+OQ==
 
 encodeurl@~1.0.2:
   version "1.0.2"
   resolved "https://registry.npmjs.org/encodeurl/-/encodeurl-1.0.2.tgz#ad3ff4c86ec2d029322f5a02c3a9a606c95b3f59"
   integrity sha512-TPJXq8JqFaVYm2CWmPvnP2Iyo4ZSM7/QKcSmuMLDObfpH5fi7RUGmd/rTDf+rut/saiDiQEeVTNgAmJEdAOx0w==
 
-es6-promise@^4.0.3:
-  version "4.2.8"
-  resolved "https://registry.npmjs.org/es6-promise/-/es6-promise-4.2.8.tgz#4eb21594c972bc40553d276e510539143db53e0a"
-  integrity sha512-HJDGx5daxeIvxdBxvG2cb9g4tEvwIk3i8+nhX0yGrYmZUzbkdg8QbDevheDB8gd0//uPj4c1EQua8Q+MViT0/w==
-
-es6-promisify@^5.0.0:
-  version "5.0.0"
-  resolved "https://registry.npmjs.org/es6-promisify/-/es6-promisify-5.0.0.tgz#5109d62f3e56ea967c4b63505aef08291c8a5203"
-  integrity sha512-C+d6UdsYDk0lMebHNR4S2NybQMMngAOnOwYBQjTOiv0MkoJMP0Myw2mgpDLBcpfCmRLxyFqYhS/CfOENq4SJhQ==
-  dependencies:
-    es6-promise "^4.0.3"
+end-of-stream@^1.1.0, end-of-stream@^1.4.1:
+  version "1.4.4"
+  resolved "https://registry.npmjs.org/end-of-stream/-/end-of-stream-1.4.4.tgz#5ae64a5f45057baf3626ec14da0ca5e4b2431eb0"
+  integrity sha512-+uw1inIHVPQoaVuHzRyXd21icM+cnt4CzD5rW+NC1wjOUSTOs+Te7FOv7AhN7vS9x/oIyhLP5PR1H+phQAHu5Q==
+  dependencies:
+    once "^1.4.0"
+
+entities@^4.4.0:
+  version "4.4.0"
+  resolved "https://registry.npmjs.org/entities/-/entities-4.4.0.tgz#97bdaba170339446495e653cfd2db78962900174"
+  integrity sha512-oYp7156SP8LkeGD0GF85ad1X9Ai79WtRsZ2gxJqtBuzH+98YUV6jkHEKlZkMbcrjJjIVJNIDP/3WL9wQkoPbWA==
+
+error-ex@^1.3.1:
+  version "1.3.2"
+  resolved "https://registry.npmjs.org/error-ex/-/error-ex-1.3.2.tgz#b4ac40648107fdcdcfae242f428bea8a14d4f1bf"
+  integrity sha512-7dFHNmqeFSEt2ZBsCriorKnn3Z2pj+fd9kmI6QoWw4//DL+icEBfc0U7qJCisqrTsKTjw4fNFy2pW9OqStD84g==
+  dependencies:
+    is-arrayish "^0.2.1"
+
+escalade@^3.1.1:
+  version "3.1.1"
+  resolved "https://registry.npmjs.org/escalade/-/escalade-3.1.1.tgz#d8cfdc7000965c5a0174b4a82eaa5c0552742e40"
+  integrity sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==
 
 escape-html@~1.0.3:
   version "1.0.3"
   resolved "https://registry.npmjs.org/escape-html/-/escape-html-1.0.3.tgz#0258eae4d3d0c0974de1c169188ef0051d1d1988"
   integrity sha512-NiSupZ4OeuGwr68lGIeym/ksIZMJodUGOSCZ/FSnTxcrekbvqrgdUxlJOMpijaKZVjAJrWrGs/6Jy8OMuyj9ow==
 
+escape-string-regexp@^1.0.5:
+  version "1.0.5"
+  resolved "https://registry.npmjs.org/escape-string-regexp/-/escape-string-regexp-1.0.5.tgz#1b61c0562190a8dff6ae3bb2cf0200ca130b86d4"
+  integrity sha512-vbRorB5FUQWvla16U8R/qgaFIya2qGzwDrNmCZuYKrbdSUMG6I1ZCGQRefkRVhuOkIGVne7BQ35DSfo1qvJqFg==
+
+escodegen@^2.0.0:
+  version "2.0.0"
+  resolved "https://registry.npmjs.org/escodegen/-/escodegen-2.0.0.tgz#5e32b12833e8aa8fa35e1bf0befa89380484c7dd"
+  integrity sha512-mmHKys/C8BFUGI+MAWNcSYoORYLMdPzjrknd2Vc+bUsjN5bXcr8EhrNB+UTqfL1y3I9c4fw2ihgtMPQLBRiQxw==
+  dependencies:
+    esprima "^4.0.1"
+    estraverse "^5.2.0"
+    esutils "^2.0.2"
+    optionator "^0.8.1"
+  optionalDependencies:
+    source-map "~0.6.1"
+
+esprima@^4.0.1:
+  version "4.0.1"
+  resolved "https://registry.npmjs.org/esprima/-/esprima-4.0.1.tgz#13b04cdb3e6c5d19df91ab6987a8695619b0aa71"
+  integrity sha512-eGuFFw7Upda+g4p+QHvnW0RyTX/SVeJBDM/gCtMARO0cLuT2HcEKnTPvhjV6aGeqrCB/sbNop0Kszm0jsaWU4A==
+
+estraverse@^5.2.0:
+  version "5.3.0"
+  resolved "https://registry.npmjs.org/estraverse/-/estraverse-5.3.0.tgz#2eea5290702f26ab8fe5370370ff86c965d21123"
+  integrity sha512-MMdARuVEQziNTeJD8DgMqmhwR11BRQ/cBP+pLtYdSTnf3MIO8fFeiINEbX36ZdNlfU/7A9f3gUw49B3oQsvwBA==
+
+esutils@^2.0.2:
+  version "2.0.3"
+  resolved "https://registry.npmjs.org/esutils/-/esutils-2.0.3.tgz#74d2eb4de0b8da1293711910d50775b9b710ef64"
+  integrity sha512-kVscqXk4OCp68SZ0dkgEKVi6/8ij300KBWTJq32P/dYeWTSwK41WyTxalN1eRmA5Z9UU/LX9D7FWSmV9SAYx6g==
+
 etag@~1.8.1:
   version "1.8.1"
   resolved "https://registry.npmjs.org/etag/-/etag-1.8.1.tgz#41ae2eeb65efa62268aebfea83ac7d79299b0887"
   integrity sha512-aIL5Fx7mawVa300al2BnEE4iNvo1qETxLrPI/o05L7z6go7fCw1J6EQmbK4FmJ2AS7kgVF/KEZWufBfdClMcPg==
 
-express@^4.16.4:
+express@^4.18.2:
   version "4.18.2"
   resolved "https://registry.npmjs.org/express/-/express-4.18.2.tgz#3fabe08296e930c796c19e3c516979386ba9fd59"
   integrity sha512-5/PsL6iGPdfQ/lKM1UuielYgv3BUoJfz1aUwU9vHZ+J7gyvwdQXFEBIEIaxeGf0GIcreATNyBExtalisDbuMqQ==
   dependencies:
     accepts "~1.3.8"
     array-flatten "1.1.1"
     body-parser "1.20.1"
@@ -390,36 +644,50 @@
     serve-static "1.15.0"
     setprototypeof "1.2.0"
     statuses "2.0.1"
     type-is "~1.6.18"
     utils-merge "1.0.1"
     vary "~1.1.2"
 
-extract-zip@^1.6.6:
-  version "1.7.0"
-  resolved "https://registry.npmjs.org/extract-zip/-/extract-zip-1.7.0.tgz#556cc3ae9df7f452c493a0cfb51cc30277940927"
-  integrity sha512-xoh5G1W/PB0/27lXgMQyIhP5DSY/LhoCsOyZgb+6iMmRtCwVBo55uKaMoEYrDCKQhWvqEip5ZPKAc6eFNyf/MA==
-  dependencies:
-    concat-stream "^1.6.2"
-    debug "^2.6.9"
-    mkdirp "^0.5.4"
+extract-zip@2.0.1:
+  version "2.0.1"
+  resolved "https://registry.npmjs.org/extract-zip/-/extract-zip-2.0.1.tgz#663dca56fe46df890d5f131ef4a06d22bb8ba13a"
+  integrity sha512-GDhU9ntwuKyGXdZBUgTIe+vXnWj0fppUEtMDL0+idd5Sta8TGpHssn/eusA9mrPr9qNDym6SxAYZjNvCn/9RBg==
+  dependencies:
+    debug "^4.1.1"
+    get-stream "^5.1.0"
     yauzl "^2.10.0"
+  optionalDependencies:
+    "@types/yauzl" "^2.9.1"
+
+fast-levenshtein@~2.0.6:
+  version "2.0.6"
+  resolved "https://registry.npmjs.org/fast-levenshtein/-/fast-levenshtein-2.0.6.tgz#3d8a5c66883a16a30ca8643e851f19baa7797917"
+  integrity sha512-DCXu6Ifhqcks7TZKY3Hxp3y6qphY5SJZmrWMDrKcERSOXWQdMhU9Ig/PYrzyw/ul9jOIyh0N4M0tbC5hodg8dw==
 
 fd-slicer@~1.1.0:
   version "1.1.0"
   resolved "https://registry.npmjs.org/fd-slicer/-/fd-slicer-1.1.0.tgz#25c7c89cb1f9077f8891bbe61d8f390eae256f1e"
   integrity sha512-cE1qsB/VwyQozZ+q1dGxR8LBYNZeofhEdUNGSMbQD3Gw2lAzX9Zb3uIU6Ebc/Fmyjo9AWWfnn0AUCHqtevs/8g==
   dependencies:
     pend "~1.2.0"
 
 fecha@^4.2.0:
   version "4.2.3"
   resolved "https://registry.npmjs.org/fecha/-/fecha-4.2.3.tgz#4d9ccdbc61e8629b259fdca67e65891448d569fd"
   integrity sha512-OP2IUU6HeYKJi3i0z4A19kHMQoLVs4Hc+DPqqxI2h/DPZHTm/vjsfC6P0b4jCMy14XizLBqvndQ+UilD7707Jw==
 
+fetch-blob@^3.1.2, fetch-blob@^3.1.4:
+  version "3.2.0"
+  resolved "https://registry.npmjs.org/fetch-blob/-/fetch-blob-3.2.0.tgz#f09b8d4bbd45adc6f0c20b7e787e793e309dcce9"
+  integrity sha512-7yAQpD2UMJzLi1Dqv7qFYnPbaPx7ZfFK6PiIxQ4PfkGPyNyl2Ugx+a/umUonmKqjhM4DnfbMvdX6otXq83soQQ==
+  dependencies:
+    node-domexception "^1.0.0"
+    web-streams-polyfill "^3.0.3"
+
 fill-range@^7.0.1:
   version "7.0.1"
   resolved "https://registry.npmjs.org/fill-range/-/fill-range-7.0.1.tgz#1919a6a7c75fe38b2c7c77e5198535da9acdda40"
   integrity sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==
   dependencies:
     to-regex-range "^5.0.1"
 
@@ -437,67 +705,83 @@
     unpipe "~1.0.0"
 
 fn.name@1.x.x:
   version "1.1.0"
   resolved "https://registry.npmjs.org/fn.name/-/fn.name-1.1.0.tgz#26cad8017967aea8731bc42961d04a3d5988accc"
   integrity sha512-GRnmB5gPyJpAhTQdSZTSp9uaPSvl09KoYcMQtsB9rQoOmzs9dH6ffeccH+Z+cv6P68Hu5bC6JjRh4Ah/mHSNRw==
 
+form-data@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/form-data/-/form-data-4.0.0.tgz#93919daeaf361ee529584b9b31664dc12c9fa452"
+  integrity sha512-ETEklSGi5t0QMZuiXoA/Q6vcnxcLQP5vdugSpuAyi6SVGi2clPPp+xgEhuMaHC+zGgn31Kd235W35f7Hykkaww==
+  dependencies:
+    asynckit "^0.4.0"
+    combined-stream "^1.0.8"
+    mime-types "^2.1.12"
+
+formdata-polyfill@^4.0.10:
+  version "4.0.10"
+  resolved "https://registry.npmjs.org/formdata-polyfill/-/formdata-polyfill-4.0.10.tgz#24807c31c9d402e002ab3d8c720144ceb8848423"
+  integrity sha512-buewHzMvYL29jdeQTVILecSaZKnt/RJWjoZCF5OW60Z67/GmSLBkOFM7qh1PI3zFNtJbaZL5eQu1vLfazOwj4g==
+  dependencies:
+    fetch-blob "^3.1.2"
+
 forwarded@0.2.0:
   version "0.2.0"
   resolved "https://registry.npmjs.org/forwarded/-/forwarded-0.2.0.tgz#2269936428aad4c15c7ebe9779a84bf0b2a81811"
   integrity sha512-buRG0fpBtRHSTCOASe6hD258tEubFoRLb4ZNA6NxMVHNw2gOcwHo9wyablzMzOA5z9xA9L1KNjk/Nt6MT9aYow==
 
 fresh@0.5.2:
   version "0.5.2"
   resolved "https://registry.npmjs.org/fresh/-/fresh-0.5.2.tgz#3d8cadd90d976569fa835ab1f8e4b23a105605a7"
   integrity sha512-zJ2mQYM18rEFOudeV4GShTGIQ7RbzA7ozbU9I/XBpm7kqgMywgmylMwXHxZJmkVoYkna9d2pVXVXPdYTP9ej8Q==
 
-fs.realpath@^1.0.0:
+fs-constants@^1.0.0:
   version "1.0.0"
-  resolved "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz#1504ad2523158caa40db4a2787cb01411994ea4f"
-  integrity sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==
+  resolved "https://registry.npmjs.org/fs-constants/-/fs-constants-1.0.0.tgz#6be0de9be998ce16af8afc24497b9ee9b7ccd9ad"
+  integrity sha512-y6OAwoSIf7FyjMIv94u+b5rdheZEjzR63GTyZJm5qh4Bi+2YgwLCcI/fPFZkL5PSixOt6ZNKm+w+Hfp/Bciwow==
 
 fsevents@~2.3.2:
   version "2.3.2"
   resolved "https://registry.npmjs.org/fsevents/-/fsevents-2.3.2.tgz#8a526f78b8fdf4623b709e0b975c52c24c02fd1a"
   integrity sha512-xiqMQR4xAeHTuB9uWm+fFRcIOgKBMiOBP+eXiyT7jsgVCq1bkVygt00oASowB7EdtpOHaaPgKt812P9ab+DDKA==
 
 function-bind@^1.1.1:
   version "1.1.1"
   resolved "https://registry.npmjs.org/function-bind/-/function-bind-1.1.1.tgz#a56899d3ea3c9bab874bb9773b7c5ede92f4895d"
   integrity sha512-yIovAzMX49sF8Yl58fSCWJ5svSLuaibPxXQJFLmBObTuCr0Mf1KiPopGM9NiFjiYBCbfaa2Fh6breQ6ANVTI0A==
 
+get-caller-file@^2.0.5:
+  version "2.0.5"
+  resolved "https://registry.npmjs.org/get-caller-file/-/get-caller-file-2.0.5.tgz#4f94412a82db32f36e3b0b9741f8a97feb031f7e"
+  integrity sha512-DyFP3BM/3YHTQOCUL/w0OZHR0lpKeGrxotcHWcqNEdnltqFwXVfhEBQ94eIo34AfQpo0rGki4cyIiftY06h2Fg==
+
 get-intrinsic@^1.0.2:
-  version "1.1.3"
-  resolved "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.1.3.tgz#063c84329ad93e83893c7f4f243ef63ffa351385"
-  integrity sha512-QJVz1Tj7MS099PevUG5jvnt9tSkXN8K14dxQlikJuPt4uD9hHAHjLyLBiLR5zELelBdD9QNRAXZzsJx0WaDL9A==
+  version "1.2.0"
+  resolved "https://registry.npmjs.org/get-intrinsic/-/get-intrinsic-1.2.0.tgz#7ad1dc0535f3a2904bba075772763e5051f6d05f"
+  integrity sha512-L049y6nFOuom5wGyRc3/gdTLO94dySVKRACj1RmJZBQXlbTMhtNIgkWkUHq+jYmZvKf14EW1EoJnnjbmoHij0Q==
   dependencies:
     function-bind "^1.1.1"
     has "^1.0.3"
     has-symbols "^1.0.3"
 
+get-stream@^5.1.0:
+  version "5.2.0"
+  resolved "https://registry.npmjs.org/get-stream/-/get-stream-5.2.0.tgz#4966a1795ee5ace65e706c4b7beb71257d6e22d3"
+  integrity sha512-nBF+F1rAZVCu/p7rjzgA+Yb4lfYXrpl7a6VmJrU8wF9I1CKvP/QwPNZHnOlwbTkY6dvtFIzFMSyQXbLoTQPRpA==
+  dependencies:
+    pump "^3.0.0"
+
 glob-parent@~5.1.2:
   version "5.1.2"
   resolved "https://registry.npmjs.org/glob-parent/-/glob-parent-5.1.2.tgz#869832c58034fe68a4093c17dc15e8340d8401c4"
   integrity sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==
   dependencies:
     is-glob "^4.0.1"
 
-glob@^7.1.3:
-  version "7.2.3"
-  resolved "https://registry.npmjs.org/glob/-/glob-7.2.3.tgz#b8df0fb802bbfa8e89bd1d938b4e16578ed44f2b"
-  integrity sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==
-  dependencies:
-    fs.realpath "^1.0.0"
-    inflight "^1.0.4"
-    inherits "2"
-    minimatch "^3.1.1"
-    once "^1.3.0"
-    path-is-absolute "^1.0.0"
-
 has-flag@^3.0.0:
   version "3.0.0"
   resolved "https://registry.npmjs.org/has-flag/-/has-flag-3.0.0.tgz#b5d454dc2199ae225699f3467e5a07f3b955bafd"
   integrity sha512-sKJf1+ceQBr4SMkvQnBDNDtf4TXpVhVGateu0t918bl30FnbE2m4vNLX+VWe/dpjlb+HugGYzW7uQXH98HPEYw==
 
 has-symbols@^1.0.3:
   version "1.0.3"
@@ -507,68 +791,96 @@
 has@^1.0.3:
   version "1.0.3"
   resolved "https://registry.npmjs.org/has/-/has-1.0.3.tgz#722d7cbfc1f6aa8241f16dd814e011e1f41e8796"
   integrity sha512-f2dvO0VU6Oej7RkWJGrehjbzMAjFp5/VKPp5tTpWIV4JHHZK1/BxbFRtf/siA2SWTe09caDmVtYYzWEIbBS4zw==
   dependencies:
     function-bind "^1.1.1"
 
+html-encoding-sniffer@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.npmjs.org/html-encoding-sniffer/-/html-encoding-sniffer-3.0.0.tgz#2cb1a8cf0db52414776e5b2a7a04d5dd98158de9"
+  integrity sha512-oWv4T4yJ52iKrufjnyZPkrN0CH3QnrUqdB6In1g5Fe1mia8GmF36gnfNySxoZtxD5+NmYw1EElVXiBk93UeskA==
+  dependencies:
+    whatwg-encoding "^2.0.0"
+
 http-errors@2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/http-errors/-/http-errors-2.0.0.tgz#b7774a1486ef73cf7667ac9ae0858c012c57b9d3"
   integrity sha512-FtwrG/euBzaEjYeRqOgly7G0qviiXoJWnvEH2Z1plBdXgbyjv34pHTSb9zoeHMyDy33+DWy5Wt9Wo+TURtOYSQ==
   dependencies:
     depd "2.0.0"
     inherits "2.0.4"
     setprototypeof "1.2.0"
     statuses "2.0.1"
     toidentifier "1.0.1"
 
-https-proxy-agent@^2.2.1:
-  version "2.2.4"
-  resolved "https://registry.npmjs.org/https-proxy-agent/-/https-proxy-agent-2.2.4.tgz#4ee7a737abd92678a293d9b34a1af4d0d08c787b"
-  integrity sha512-OmvfoQ53WLjtA9HeYP9RNrWMJzzAz1JGaSFr1nijg0PVR1JaD/xbJq1mdEIIlxGpXp9eSe/O2LgU9DJmTPd0Eg==
+http-proxy-agent@^5.0.0:
+  version "5.0.0"
+  resolved "https://registry.npmjs.org/http-proxy-agent/-/http-proxy-agent-5.0.0.tgz#5129800203520d434f142bc78ff3c170800f2b43"
+  integrity sha512-n2hY8YdoRE1i7r6M0w9DIw5GgZN0G25P8zLCRQ8rjXtTU3vsNFBI/vWK/UIeE6g5MUUz6avwAPXmL6Fy9D/90w==
+  dependencies:
+    "@tootallnate/once" "2"
+    agent-base "6"
+    debug "4"
+
+https-proxy-agent@5.0.1, https-proxy-agent@^5.0.1:
+  version "5.0.1"
+  resolved "https://registry.npmjs.org/https-proxy-agent/-/https-proxy-agent-5.0.1.tgz#c59ef224a04fe8b754f3db0063a25ea30d0005d6"
+  integrity sha512-dFcAjpTQFgoLMzC2VwU+C/CbS7uRL0lWmxDITmqm7C+7F0Odmj6s9l6alZc6AELXhrnggM2CeWSXHGOdX2YtwA==
   dependencies:
-    agent-base "^4.3.0"
-    debug "^3.1.0"
+    agent-base "6"
+    debug "4"
 
 iconv-lite@0.4.24:
   version "0.4.24"
   resolved "https://registry.npmjs.org/iconv-lite/-/iconv-lite-0.4.24.tgz#2022b4b25fbddc21d2f524974a474aafe733908b"
   integrity sha512-v3MXnZAcvnywkTUEZomIActle7RXXeedOR31wwl7VlyoXO4Qi9arvSenNQWne1TcRwhCL1HwLI21bEqdpj8/rA==
   dependencies:
     safer-buffer ">= 2.1.2 < 3"
 
+iconv-lite@0.6.3:
+  version "0.6.3"
+  resolved "https://registry.npmjs.org/iconv-lite/-/iconv-lite-0.6.3.tgz#a52f80bf38da1952eb5c681790719871a1a72501"
+  integrity sha512-4fCk79wshMdzMp2rH06qWrJE4iolqLhCUH+OiuIgU++RB0+94NlDL81atO7GX55uUKueo0txHNtvEyI6D7WdMw==
+  dependencies:
+    safer-buffer ">= 2.1.2 < 3.0.0"
+
 ieee754@^1.1.13:
   version "1.2.1"
   resolved "https://registry.npmjs.org/ieee754/-/ieee754-1.2.1.tgz#8eb7a10a63fff25d15a57b001586d177d1b0d352"
   integrity sha512-dcyqhDvX1C46lXZcVqCpK+FtMRQVdIMN6/Df5js2zouUsqG7I6sFxitIC+7KYK29KdXOLHdu9zL4sFnoVQnqaA==
 
 ignore-by-default@^1.0.1:
   version "1.0.1"
   resolved "https://registry.npmjs.org/ignore-by-default/-/ignore-by-default-1.0.1.tgz#48ca6d72f6c6a3af00a9ad4ae6876be3889e2b09"
   integrity sha512-Ius2VYcGNk7T90CppJqcIkS5ooHUZyIQK+ClZfMfMNFEF9VSE73Fq+906u/CWu92x4gzZMWOwfFYckPObzdEbA==
 
-inflight@^1.0.4:
-  version "1.0.6"
-  resolved "https://registry.npmjs.org/inflight/-/inflight-1.0.6.tgz#49bd6331d7d02d0c09bc910a1075ba8165b56df9"
-  integrity sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==
+import-fresh@^3.2.1:
+  version "3.3.0"
+  resolved "https://registry.npmjs.org/import-fresh/-/import-fresh-3.3.0.tgz#37162c25fcb9ebaa2e6e53d5b4d88ce17d9e0c2b"
+  integrity sha512-veYYhQa+D1QBKznvhUHxb8faxlrwUnxseDAbAp457E0wLNio2bOSKnjYDhMj+YiAq61xrMGhQk9iXVk5FzgQMw==
   dependencies:
-    once "^1.3.0"
-    wrappy "1"
+    parent-module "^1.0.0"
+    resolve-from "^4.0.0"
 
-inherits@2, inherits@2.0.4, inherits@^2.0.3, inherits@~2.0.3:
+inherits@2.0.4, inherits@^2.0.3, inherits@^2.0.4:
   version "2.0.4"
   resolved "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz#0fa2c64f932917c3433a0ded55363aae37416b7c"
   integrity sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==
 
 ipaddr.js@1.9.1:
   version "1.9.1"
   resolved "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-1.9.1.tgz#bff38543eeb8984825079ff3a2a8e6cbd46781b3"
   integrity sha512-0KI/607xoxSToH7GjN1FfSbLoU0+btTicjsQSWQlh/hZykN8KpmMf7uYwPW3R+akZ6R/w18ZlXSHBYXiYUPO3g==
 
+is-arrayish@^0.2.1:
+  version "0.2.1"
+  resolved "https://registry.npmjs.org/is-arrayish/-/is-arrayish-0.2.1.tgz#77c99840527aa8ecb1a8ba697b80645a7a926a9d"
+  integrity sha512-zz06S8t0ozoDXMG+ube26zeCTNXcKIPJZJi8hBrF4idCLms4CG9QtK7qBl1boi5ODzFpjswb5JPmHCbMpjaYzg==
+
 is-arrayish@^0.3.1:
   version "0.3.2"
   resolved "https://registry.npmjs.org/is-arrayish/-/is-arrayish-0.3.2.tgz#4574a2ae56f7ab206896fb431eaeed066fdf8f03"
   integrity sha512-eVRqCvVlZbuw3GrM63ovNSNAeA1K16kaR/LRY/92w0zxQ5/1YzwblUX652i4Xs9RwAGjW9d9y6X88t8OaAJfWQ==
 
 is-binary-path@~2.1.0:
   version "2.1.0"
@@ -578,47 +890,115 @@
     binary-extensions "^2.0.0"
 
 is-extglob@^2.1.1:
   version "2.1.1"
   resolved "https://registry.npmjs.org/is-extglob/-/is-extglob-2.1.1.tgz#a88c02535791f02ed37c76a1b9ea9773c833f8c2"
   integrity sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==
 
+is-fullwidth-code-point@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-3.0.0.tgz#f116f8064fe90b3f7844a38997c0b75051269f1d"
+  integrity sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==
+
 is-glob@^4.0.1, is-glob@~4.0.1:
   version "4.0.3"
   resolved "https://registry.npmjs.org/is-glob/-/is-glob-4.0.3.tgz#64f61e42cbbb2eec2071a9dac0b28ba1e65d5084"
   integrity sha512-xelSayHH36ZgE7ZWhli7pW34hNbNl8Ojv5KVmkJD4hBdD3th8Tfk9vYasLM+mXWOZhFkgZfxhLSnrwRr4elSSg==
   dependencies:
     is-extglob "^2.1.1"
 
 is-number@^7.0.0:
   version "7.0.0"
   resolved "https://registry.npmjs.org/is-number/-/is-number-7.0.0.tgz#7535345b896734d5f80c4d06c50955527a14f12b"
   integrity sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==
 
+is-potential-custom-element-name@^1.0.1:
+  version "1.0.1"
+  resolved "https://registry.npmjs.org/is-potential-custom-element-name/-/is-potential-custom-element-name-1.0.1.tgz#171ed6f19e3ac554394edf78caa05784a45bebb5"
+  integrity sha512-bCYeRA2rVibKZd+s2625gGnGF/t7DSqDs4dP7CrLA1m7jKWz6pps0LpYLJN8Q64HtmPKJ1hrN3nzPNKFEKOUiQ==
+
 is-stream@^2.0.0:
   version "2.0.1"
   resolved "https://registry.npmjs.org/is-stream/-/is-stream-2.0.1.tgz#fac1e3d53b97ad5a9d0ae9cef2389f5810a5c077"
   integrity sha512-hFoiJiTl63nn+kstHGBtewWSKnQLpyb155KHheA1l39uvtO9nWIop1p3udqPcUd/xbF1VLMO4n7OI6p7RbngDg==
 
-isarray@~1.0.0:
-  version "1.0.0"
-  resolved "https://registry.npmjs.org/isarray/-/isarray-1.0.0.tgz#bb935d48582cba168c06834957a54a3e07124f11"
-  integrity sha512-VLghIWNM6ELQzo7zwmcg0NmTVyWKYjvIeM83yjp0wRDTmUnrM678fQbcKBo6n2CJEF0szoG//ytg+TKla89ALQ==
+js-tokens@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz#19203fb59991df98e3a287050d4647cdeaf32499"
+  integrity sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==
+
+js-yaml@^4.1.0:
+  version "4.1.0"
+  resolved "https://registry.npmjs.org/js-yaml/-/js-yaml-4.1.0.tgz#c1fb65f8f5017901cdd2c951864ba18458a10602"
+  integrity sha512-wpxZs9NoxZaJESJGIZTyDEaYpl0FKSA+FB9aJiyemKhMwkxQg63h4T1KJgUGHpTqPDNRcmmYLugrRjJlBtWvRA==
+  dependencies:
+    argparse "^2.0.1"
+
+jsdom@^21.0.0:
+  version "21.1.1"
+  resolved "https://registry.npmjs.org/jsdom/-/jsdom-21.1.1.tgz#ab796361e3f6c01bcfaeda1fea3c06197ac9d8ae"
+  integrity sha512-Jjgdmw48RKcdAIQyUD1UdBh2ecH7VqwaXPN3ehoZN6MqgVbMn+lRm1aAT1AsdJRAJpwfa4IpwgzySn61h2qu3w==
+  dependencies:
+    abab "^2.0.6"
+    acorn "^8.8.2"
+    acorn-globals "^7.0.0"
+    cssstyle "^3.0.0"
+    data-urls "^4.0.0"
+    decimal.js "^10.4.3"
+    domexception "^4.0.0"
+    escodegen "^2.0.0"
+    form-data "^4.0.0"
+    html-encoding-sniffer "^3.0.0"
+    http-proxy-agent "^5.0.0"
+    https-proxy-agent "^5.0.1"
+    is-potential-custom-element-name "^1.0.1"
+    nwsapi "^2.2.2"
+    parse5 "^7.1.2"
+    rrweb-cssom "^0.6.0"
+    saxes "^6.0.0"
+    symbol-tree "^3.2.4"
+    tough-cookie "^4.1.2"
+    w3c-xmlserializer "^4.0.0"
+    webidl-conversions "^7.0.0"
+    whatwg-encoding "^2.0.0"
+    whatwg-mimetype "^3.0.0"
+    whatwg-url "^12.0.1"
+    ws "^8.13.0"
+    xml-name-validator "^4.0.0"
+
+json-parse-even-better-errors@^2.3.0:
+  version "2.3.1"
+  resolved "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz#7c47805a94319928e05777405dc12e1f7a4ee02d"
+  integrity sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==
 
 kuler@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/kuler/-/kuler-2.0.0.tgz#e2c570a3800388fb44407e851531c1d670b061b3"
   integrity sha512-Xq9nH7KlWZmXAtodXDDRE7vs6DU1gTU8zYDHDiWLSip45Egwq3plLHzPn27NgvzL2r1LMPC1vdqh98sQxtqj4A==
 
+levn@~0.3.0:
+  version "0.3.0"
+  resolved "https://registry.npmjs.org/levn/-/levn-0.3.0.tgz#3b09924edf9f083c0490fdd4c0bc4421e04764ee"
+  integrity sha512-0OO4y2iOHix2W6ujICbKIaEQXvFQHue65vUG3pb5EUomzPI90z9hsA1VsO/dbIIpC53J8gxM9Q4Oho0jrCM/yA==
+  dependencies:
+    prelude-ls "~1.1.2"
+    type-check "~0.3.2"
+
+lines-and-columns@^1.1.6:
+  version "1.2.4"
+  resolved "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz#eca284f75d2965079309dc0ad9255abb2ebc1632"
+  integrity sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==
+
 logform@^2.3.2, logform@^2.4.0:
-  version "2.4.2"
-  resolved "https://registry.npmjs.org/logform/-/logform-2.4.2.tgz#a617983ac0334d0c3b942c34945380062795b47c"
-  integrity sha512-W4c9himeAwXEdZ05dQNerhFz2XG80P9Oj0loPUMV23VC2it0orMHQhJm4hdnnor3rd1HsGf6a2lPwBM1zeXHGw==
+  version "2.5.1"
+  resolved "https://registry.npmjs.org/logform/-/logform-2.5.1.tgz#44c77c34becd71b3a42a3970c77929e52c6ed48b"
+  integrity sha512-9FyqAm9o9NKKfiAKfZoYo9bGXXuwMkxQiQttkT4YjjVtQVIQtK6LmVtlxmCaFswo6N4AfEkHqZTV0taDtPotNg==
   dependencies:
     "@colors/colors" "1.5.0"
+    "@types/triple-beam" "^1.3.2"
     fecha "^4.2.0"
     ms "^2.1.1"
     safe-stable-stringify "^2.3.1"
     triple-beam "^1.3.0"
 
 media-typer@0.3.0:
   version "0.3.0"
@@ -636,49 +1016,42 @@
   integrity sha512-iclAHeNqNm68zFtnZ0e+1L2yUIdvzNoauKU4WBA3VvH/vPFieF7qfRlwUZU+DA9P9bPXIS90ulxoUoCH23sV2w==
 
 mime-db@1.52.0, "mime-db@>= 1.43.0 < 2":
   version "1.52.0"
   resolved "https://registry.npmjs.org/mime-db/-/mime-db-1.52.0.tgz#bbabcdc02859f4987301c856e3387ce5ec43bf70"
   integrity sha512-sPU4uV7dYlvtWJxwwxHD0PuihVNiE7TyAbQ5SWxDCB9mUYvOgroQOwYQQOKPJ8CIbE+1ETVlOoK1UC2nU3gYvg==
 
-mime-types@~2.1.24, mime-types@~2.1.34:
+mime-types@^2.1.12, mime-types@~2.1.24, mime-types@~2.1.34:
   version "2.1.35"
   resolved "https://registry.npmjs.org/mime-types/-/mime-types-2.1.35.tgz#381a871b62a734450660ae3deee44813f70d959a"
   integrity sha512-ZDY+bPm5zTTF+YpCrAU9nK0UgICYPT0QtT1NZWFv4s++TNkcgVaT0g6+4R2uI4MjQjzysHB1zxuWL50hzaeXiw==
   dependencies:
     mime-db "1.52.0"
 
 mime@1.6.0:
   version "1.6.0"
   resolved "https://registry.npmjs.org/mime/-/mime-1.6.0.tgz#32cd9e5c64553bd58d19a568af452acff04981b1"
   integrity sha512-x0Vn8spI+wuJ1O6S7gnbaQg8Pxh4NNHb7KSINmEWKiPE4RKOplvijn+NkmYmmRgP68mc70j2EbeTFRsrswaQeg==
 
-mime@^2.0.3:
-  version "2.6.0"
-  resolved "https://registry.npmjs.org/mime/-/mime-2.6.0.tgz#a2a682a95cd4d0cb1d6257e28f83da7e35800367"
-  integrity sha512-USPkMeET31rOMiarsBNIHZKLGgvKc/LrjofAnBlOttf5ajRvqiRA8QsenbcooctK6d6Ts6aqZXBA+XbkKthiQg==
-
-minimatch@^3.1.1, minimatch@^3.1.2:
+minimatch@^3.1.2:
   version "3.1.2"
   resolved "https://registry.npmjs.org/minimatch/-/minimatch-3.1.2.tgz#19cd194bfd3e428f049a70817c038d89ab4be35b"
   integrity sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==
   dependencies:
     brace-expansion "^1.1.7"
 
-minimist@^1.2.6:
-  version "1.2.7"
-  resolved "https://registry.npmjs.org/minimist/-/minimist-1.2.7.tgz#daa1c4d91f507390437c6a8bc01078e7000c4d18"
-  integrity sha512-bzfL1YUZsP41gmu/qjrEk0Q6i2ix/cVeAhbCbqH9u3zYutS1cLg00qhrD0M2MVdCcx4Sc0UpP2eBWo9rotpq6g==
-
-mkdirp@^0.5.4:
-  version "0.5.6"
-  resolved "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.6.tgz#7def03d2432dcae4ba1d611445c48396062255f6"
-  integrity sha512-FP+p8RB8OWpF3YZBCrP5gtADmtXApB5AMLn+vdyA+PyxCjrCs00mjyUozssO33cwDeT3wNGdLxJ5M//YqtHAJw==
-  dependencies:
-    minimist "^1.2.6"
+mitt@3.0.0:
+  version "3.0.0"
+  resolved "https://registry.npmjs.org/mitt/-/mitt-3.0.0.tgz#69ef9bd5c80ff6f57473e8d89326d01c414be0bd"
+  integrity sha512-7dX2/10ITVyqh4aOSVI9gdape+t9l2/8QxHrFmUXu4EEUpdlxl6RudZUPZoc+zuY2hk1j7XxVroIVIan/pD/SQ==
+
+mkdirp-classic@^0.5.2:
+  version "0.5.3"
+  resolved "https://registry.npmjs.org/mkdirp-classic/-/mkdirp-classic-0.5.3.tgz#fa10c9115cc6d8865be221ba47ee9bed78601113"
+  integrity sha512-gKLcREMhtuZRwRAfqP3RFW+TK4JqApVBtOIftVgjuABpAtpxhPGaDcfvbhNvD0B8iD1oUr/txX35NjcaY6Ns/A==
 
 morgan@^1.9.1:
   version "1.10.0"
   resolved "https://registry.npmjs.org/morgan/-/morgan-1.10.0.tgz#091778abc1fc47cd3509824653dae1faab6b17d7"
   integrity sha512-AbegBVI4sh6El+1gNwvD5YIck7nSA36weD7xvIxG4in80j/UoK8AEGaWnnz8v1GxonMCltmlNs5ZKbGvl9b1XQ==
   dependencies:
     basic-auth "~2.0.1"
@@ -688,40 +1061,54 @@
     on-headers "~1.0.2"
 
 ms@2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/ms/-/ms-2.0.0.tgz#5608aeadfc00be6c2901df5f9861788de0d597c8"
   integrity sha512-Tpp60P6IUJDTuOq/5Z8cdskzJujfwqfOTkrwIwj7IRISpnkJnT6SyJ4PCPnGMoFjC9ddhal5KVIYtAt97ix05A==
 
-ms@2.1.2:
+ms@2.1.2, ms@^2.1.1:
   version "2.1.2"
   resolved "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz#d09d1f357b443f493382a8eb3ccd183872ae6009"
   integrity sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==
 
-ms@2.1.3, ms@^2.1.1:
+ms@2.1.3:
   version "2.1.3"
   resolved "https://registry.npmjs.org/ms/-/ms-2.1.3.tgz#574c8138ce1d2b5861f0b44579dbadd60c6615b2"
   integrity sha512-6FlzubTLZG3J2a/NVCAleEhjzq5oxgHyaCU9yYXvcLsvoVaHJq/s5xXI6/XXP6tz7R9xAOtHnSO/tXtF3WRTlA==
 
 negotiator@0.6.3:
   version "0.6.3"
   resolved "https://registry.npmjs.org/negotiator/-/negotiator-0.6.3.tgz#58e323a72fedc0d6f9cd4d31fe49f51479590ccd"
   integrity sha512-+EUsqGPLsM+j/zdChZjsnX51g4XrHFOIXwfnCVPGlQk/k5giakcKsuxCObBRu6DSm9opw/O6slWbJdghQM4bBg==
 
-node-fetch@^2.6.1:
+node-domexception@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmjs.org/node-domexception/-/node-domexception-1.0.0.tgz#6888db46a1f71c0b76b3f7555016b63fe64766e5"
+  integrity sha512-/jKZoMpw0F8GRwl4/eLROPA3cfcXtLApP0QzLmUT/HuPCZWyB7IY9ZrMeKw2O/nFIqPQB3PVM9aYm0F312AXDQ==
+
+node-fetch@2.6.7:
   version "2.6.7"
   resolved "https://registry.npmjs.org/node-fetch/-/node-fetch-2.6.7.tgz#24de9fba827e3b4ae44dc8b20256a379160052ad"
   integrity sha512-ZjMPFEfVx5j+y2yF35Kzx5sF7kDzxuDj6ziH4FFbOp87zKDZNx8yExJIb05OGF4Nlt9IHFIMBkRl41VdvcNdbQ==
   dependencies:
     whatwg-url "^5.0.0"
 
-nodemon@^2.0.7:
-  version "2.0.20"
-  resolved "https://registry.npmjs.org/nodemon/-/nodemon-2.0.20.tgz#e3537de768a492e8d74da5c5813cb0c7486fc701"
-  integrity sha512-Km2mWHKKY5GzRg6i1j5OxOHQtuvVsgskLfigG25yTtbyfRGn/GNvIbRyOf1PSCKJ2aT/58TiuUsuOU5UToVViw==
+node-fetch@^3.3.0:
+  version "3.3.1"
+  resolved "https://registry.npmjs.org/node-fetch/-/node-fetch-3.3.1.tgz#b3eea7b54b3a48020e46f4f88b9c5a7430d20b2e"
+  integrity sha512-cRVc/kyto/7E5shrWca1Wsea4y6tL9iYJE5FBCius3JQfb/4P4I295PfhgbJQBLTx6lATE4z+wK0rPM4VS2uow==
+  dependencies:
+    data-uri-to-buffer "^4.0.0"
+    fetch-blob "^3.1.4"
+    formdata-polyfill "^4.0.10"
+
+nodemon@^2.0.20:
+  version "2.0.22"
+  resolved "https://registry.npmjs.org/nodemon/-/nodemon-2.0.22.tgz#182c45c3a78da486f673d6c1702e00728daf5258"
+  integrity sha512-B8YqaKMmyuCO7BowF1Z1/mkPqLk6cs/l63Ojtd6otKjMx47Dq1utxfRxcavH1I7VSaL8n5BUaoutadnsX3AAVQ==
   dependencies:
     chokidar "^3.5.2"
     debug "^3.2.7"
     ignore-by-default "^1.0.1"
     minimatch "^3.1.2"
     pstree.remy "^1.1.8"
     semver "^5.7.1"
@@ -738,18 +1125,23 @@
     abbrev "1"
 
 normalize-path@^3.0.0, normalize-path@~3.0.0:
   version "3.0.0"
   resolved "https://registry.npmjs.org/normalize-path/-/normalize-path-3.0.0.tgz#0dcd69ff23a1c9b11fd0978316644a0388216a65"
   integrity sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==
 
+nwsapi@^2.2.2:
+  version "2.2.3"
+  resolved "https://registry.npmjs.org/nwsapi/-/nwsapi-2.2.3.tgz#00e04dfd5a4a751e5ec2fecdc75dfd2f0db820fa"
+  integrity sha512-jscxIO4/VKScHlbmFBdV1Z6LXnLO+ZR4VMtypudUdfwtKxUN3TQcNFIHLwKtrUbDyHN4/GycY9+oRGZ2XMXYPw==
+
 object-inspect@^1.9.0:
-  version "1.12.2"
-  resolved "https://registry.npmjs.org/object-inspect/-/object-inspect-1.12.2.tgz#c0641f26394532f28ab8d796ab954e43c009a8ea"
-  integrity sha512-z+cPxW0QGUp0mcqcsgQyLVRDoXFQbXOwBaqyF7VIgI4TWNQsDHrBpUQslRmIfAoYWdYzs6UlKJtB2XJpTaNSpQ==
+  version "1.12.3"
+  resolved "https://registry.npmjs.org/object-inspect/-/object-inspect-1.12.3.tgz#ba62dffd67ee256c8c086dfae69e016cd1f198b9"
+  integrity sha512-geUvdk7c+eizMNUDkRpW1wJwgfOiOeHbxBR/hLXK1aT6zmVSO0jsQcs7fj6MGw89jC/cjGfLcNOrtMYtGqm81g==
 
 on-finished@2.4.1:
   version "2.4.1"
   resolved "https://registry.npmjs.org/on-finished/-/on-finished-2.4.1.tgz#58c8c44116e54845ad57f14ab10b03533184ac3f"
   integrity sha512-oVlzkg3ENAhCk2zdv7IJwd/QUD4z2RxRwpkcGY8psCVcCYZNq4wYnVWALHM+brtuJjePWiYF/ClmuDr8Ch5+kg==
   dependencies:
     ee-first "1.1.1"
@@ -762,49 +1154,85 @@
     ee-first "1.1.1"
 
 on-headers@~1.0.2:
   version "1.0.2"
   resolved "https://registry.npmjs.org/on-headers/-/on-headers-1.0.2.tgz#772b0ae6aaa525c399e489adfad90c403eb3c28f"
   integrity sha512-pZAE+FJLoyITytdqK0U5s+FIpjN0JP3OzFi/u8Rx+EV5/W+JTWGXG8xFzevE7AjBfDqHv/8vL8qQsIhHnqRkrA==
 
-once@^1.3.0:
+once@^1.3.1, once@^1.4.0:
   version "1.4.0"
   resolved "https://registry.npmjs.org/once/-/once-1.4.0.tgz#583b1aa775961d4b113ac17d9c50baef9dd76bd1"
   integrity sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==
   dependencies:
     wrappy "1"
 
 one-time@^1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/one-time/-/one-time-1.0.0.tgz#e06bc174aed214ed58edede573b433bbf827cb45"
   integrity sha512-5DXOiRKwuSEcQ/l0kGCF6Q3jcADFv5tSmRaJck/OqkVFcOzutB134KRSfF0xDrL39MNnqxbHBbUUcjZIhTgb2g==
   dependencies:
     fn.name "1.x.x"
 
+optionator@^0.8.1:
+  version "0.8.3"
+  resolved "https://registry.npmjs.org/optionator/-/optionator-0.8.3.tgz#84fa1d036fe9d3c7e21d99884b601167ec8fb495"
+  integrity sha512-+IW9pACdk3XWmmTXG8m3upGUJst5XRGzxMRjXzAuJ1XnIFNvfhjjIuYkDvysnPQ7qzqVzLt78BCruntqRhWQbA==
+  dependencies:
+    deep-is "~0.1.3"
+    fast-levenshtein "~2.0.6"
+    levn "~0.3.0"
+    prelude-ls "~1.1.2"
+    type-check "~0.3.2"
+    word-wrap "~1.2.3"
+
 pako@^1.0.10, pako@^1.0.11, pako@^1.0.6:
   version "1.0.11"
   resolved "https://registry.npmjs.org/pako/-/pako-1.0.11.tgz#6c9599d340d54dfd3946380252a35705a6b992bf"
   integrity sha512-4hLB8Py4zZce5s4yd9XzopqwVv/yGNhV1Bl8NTmCq1763HeK2+EwVTv+leGeL13Dnh2wfbqowVPXCIO0z4taYw==
 
+parent-module@^1.0.0:
+  version "1.0.1"
+  resolved "https://registry.npmjs.org/parent-module/-/parent-module-1.0.1.tgz#691d2709e78c79fae3a156622452d00762caaaa2"
+  integrity sha512-GQ2EWRpQV8/o+Aw8YqtfZZPfNRWZYkbidE9k5rpl/hC3vtHHBfGm2Ifi6qWV+coDGkrUKZAxE3Lot5kcsRlh+g==
+  dependencies:
+    callsites "^3.0.0"
+
+parse-json@^5.0.0:
+  version "5.2.0"
+  resolved "https://registry.npmjs.org/parse-json/-/parse-json-5.2.0.tgz#c76fc66dee54231c962b22bcc8a72cf2f99753cd"
+  integrity sha512-ayCKvm/phCGxOkYRSCM82iDwct8/EonSEgCSxWxD7ve6jHggsFl4fZVQBPRNgQoKiuV/odhFrGzQXZwbifC8Rg==
+  dependencies:
+    "@babel/code-frame" "^7.0.0"
+    error-ex "^1.3.1"
+    json-parse-even-better-errors "^2.3.0"
+    lines-and-columns "^1.1.6"
+
+parse5@^7.1.2:
+  version "7.1.2"
+  resolved "https://registry.npmjs.org/parse5/-/parse5-7.1.2.tgz#0736bebbfd77793823240a23b7fc5e010b7f8e32"
+  integrity sha512-Czj1WaSVpaoj0wbhMzLmWD69anp2WH7FXMB9n1Sy8/ZFF9jolSQVMu1Ij5WIyGmcBmhk7EOndpO4mIpihVqAXw==
+  dependencies:
+    entities "^4.4.0"
+
 parseurl@~1.3.3:
   version "1.3.3"
   resolved "https://registry.npmjs.org/parseurl/-/parseurl-1.3.3.tgz#9da19e7bee8d12dff0513ed5b76957793bc2e8d4"
   integrity sha512-CiyeOxFT/JZyN5m0z9PfXw4SCBJ6Sygz1Dpl0wqjlhDEGGBP1GnsUVEL0p63hoG1fcj3fHynXi9NYO4nWOL+qQ==
 
-path-is-absolute@^1.0.0:
-  version "1.0.1"
-  resolved "https://registry.npmjs.org/path-is-absolute/-/path-is-absolute-1.0.1.tgz#174b9268735534ffbc7ace6bf53a5a9e1b5c5f5f"
-  integrity sha512-AVbw3UJ2e9bq64vSaS9Am0fje1Pa8pbGqTTsmXfaIiMpnr5DlDhfJOuLj9Sf95ZPVDAUerDfEk88MPmPe7UCQg==
-
 path-to-regexp@0.1.7:
   version "0.1.7"
   resolved "https://registry.npmjs.org/path-to-regexp/-/path-to-regexp-0.1.7.tgz#df604178005f522f15eb4490e7247a1bfaa67f8c"
   integrity sha512-5DFkuoqlv1uYQKxy8omFBeJPQcdoE07Kv2sferDCrAq1ohOU+MSDswDIbnx3YAM60qIOnYa53wBhXW0EbMonrQ==
 
-pdf-lib@^1.16.0:
+path-type@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/path-type/-/path-type-4.0.0.tgz#84ed01c0a7ba380afe09d90a8c180dcd9d03043b"
+  integrity sha512-gDKb8aZMDeD/tZWs9P6+q0J9Mwkdl6xMV8TjnGP3qJVJ06bdMgkbBlLU8IdfOsIsFz2BW1rNVT3XuNEl8zPAvw==
+
+pdf-lib@^1.17.1:
   version "1.17.1"
   resolved "https://registry.npmjs.org/pdf-lib/-/pdf-lib-1.17.1.tgz#9e7dd21261a0c1fb17992580885b39e7d08f451f"
   integrity sha512-V/mpyJAoTsN4cnP31vc0wfNA1+p20evqqnap0KLoRUN0Yk/p3wN52DOEsL4oBFcLdb76hlpKPtzJIgo67j/XLw==
   dependencies:
     "@pdf-lib/standard-fonts" "^1.0.0"
     "@pdf-lib/upng" "^1.0.1"
     pako "^1.0.11"
@@ -816,63 +1244,101 @@
   integrity sha512-F3asv42UuXchdzt+xXqfW1OGlVBe+mxa2mqI0pg5yAHZPvFmY3Y6drSf/GQ1A86WgWEN9Kzh/WrgKa6iGcHXLg==
 
 picomatch@^2.0.4, picomatch@^2.2.1:
   version "2.3.1"
   resolved "https://registry.npmjs.org/picomatch/-/picomatch-2.3.1.tgz#3ba3833733646d9d3e4995946c1365a67fb07a42"
   integrity sha512-JU3teHTNjmE2VCGFzuY8EXzCDVwEqB2a8fsIvwaStHhAWJEeVd1o1QD80CU6+ZdEXXSLbSsuLwJjkCBWqRQUVA==
 
-process-nextick-args@~2.0.0:
-  version "2.0.1"
-  resolved "https://registry.npmjs.org/process-nextick-args/-/process-nextick-args-2.0.1.tgz#7820d9b16120cc55ca9ae7792680ae7dba6d7fe2"
-  integrity sha512-3ouUOpQhtgrbOa17J7+uxOTpITYWaGP7/AhoR3+A+/1e9skrzelGi/dXzEYyvbxubEF6Wn2ypscTKiKJFFn1ag==
+prelude-ls@~1.1.2:
+  version "1.1.2"
+  resolved "https://registry.npmjs.org/prelude-ls/-/prelude-ls-1.1.2.tgz#21932a549f5e52ffd9a827f570e04be62a97da54"
+  integrity sha512-ESF23V4SKG6lVSGZgYNpbsiaAkdab6ZgOxe52p7+Kid3W3u3bxR4Vfd/o21dmN7jSt0IwgZ4v5MUd26FEtXE9w==
 
-progress@^2.0.1:
+progress@2.0.3:
   version "2.0.3"
   resolved "https://registry.npmjs.org/progress/-/progress-2.0.3.tgz#7e8cf8d8f5b8f239c1bc68beb4eb78567d572ef8"
   integrity sha512-7PiHtLll5LdnKIMw100I+8xJXR5gW2QwWYkT6iJva0bXitZKa/XMrSbdmg3r2Xnaidz9Qumd0VPaMrZlF9V9sA==
 
 proxy-addr@~2.0.7:
   version "2.0.7"
   resolved "https://registry.npmjs.org/proxy-addr/-/proxy-addr-2.0.7.tgz#f19fe69ceab311eeb94b42e70e8c2070f9ba1025"
   integrity sha512-llQsMLSUDUPT44jdrU/O37qlnifitDP+ZwrmmZcoSKyLKvtZxpyV0n2/bD/N4tBAAZ/gJEdZU7KMraoK1+XYAg==
   dependencies:
     forwarded "0.2.0"
     ipaddr.js "1.9.1"
 
-proxy-from-env@^1.0.0:
+proxy-from-env@1.1.0:
   version "1.1.0"
   resolved "https://registry.npmjs.org/proxy-from-env/-/proxy-from-env-1.1.0.tgz#e102f16ca355424865755d2c9e8ea4f24d58c3e2"
   integrity sha512-D+zkORCbA9f1tdWRK0RaCR3GPv50cMxcrz4X8k5LTSUD1Dkw47mKJEZQNunItRTkWwgtaUSo1RVFRIG9ZXiFYg==
 
+psl@^1.1.33:
+  version "1.9.0"
+  resolved "https://registry.npmjs.org/psl/-/psl-1.9.0.tgz#d0df2a137f00794565fcaf3b2c00cd09f8d5a5a7"
+  integrity sha512-E/ZsdU4HLs/68gYzgGTkMicWTLPdAftJLfJFlLUAAKZGkStNU72sZjT66SnMDVOfOWY/YAoiD7Jxa9iHvngcag==
+
 pstree.remy@^1.1.8:
   version "1.1.8"
   resolved "https://registry.npmjs.org/pstree.remy/-/pstree.remy-1.1.8.tgz#c242224f4a67c21f686839bbdb4ac282b8373d3a"
   integrity sha512-77DZwxQmxKnu3aR542U+X8FypNzbfJ+C5XQDk3uWjWxn6151aIMGthWYRXTqT1E5oJvg+ljaa2OJi+VfvCOQ8w==
 
-puppeteer@^1.15.0:
-  version "1.20.0"
-  resolved "https://registry.npmjs.org/puppeteer/-/puppeteer-1.20.0.tgz#e3d267786f74e1d87cf2d15acc59177f471bbe38"
-  integrity sha512-bt48RDBy2eIwZPrkgbcwHtb51mj2nKvHOPMaSH2IsWiv7lOG9k9zhaRzpDZafrk05ajMc3cu+lSQYYOfH2DkVQ==
-  dependencies:
-    debug "^4.1.0"
-    extract-zip "^1.6.6"
-    https-proxy-agent "^2.2.1"
-    mime "^2.0.3"
-    progress "^2.0.1"
-    proxy-from-env "^1.0.0"
-    rimraf "^2.6.1"
-    ws "^6.1.0"
+pump@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.npmjs.org/pump/-/pump-3.0.0.tgz#b4a2116815bde2f4e1ea602354e8c75565107a64"
+  integrity sha512-LwZy+p3SFs1Pytd/jYct4wpv49HiYCqd9Rlc5ZVdk0V+8Yzv6jR5Blk3TRmPL1ft69TxP0IMZGJ+WPFU2BFhww==
+  dependencies:
+    end-of-stream "^1.1.0"
+    once "^1.3.1"
+
+punycode@^2.1.1, punycode@^2.3.0:
+  version "2.3.0"
+  resolved "https://registry.npmjs.org/punycode/-/punycode-2.3.0.tgz#f67fa67c94da8f4d0cfff981aee4118064199b8f"
+  integrity sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==
+
+puppeteer-core@19.8.5:
+  version "19.8.5"
+  resolved "https://registry.npmjs.org/puppeteer-core/-/puppeteer-core-19.8.5.tgz#ba02fbe5bc2f82a9270aa1b983cf29cc1d4f1573"
+  integrity sha512-zoGhim/oBQbkND6h4Xz4X7l5DkWVH9wH7z0mVty5qa/c0P1Yad47t/npVtt2xS10BiQwzztWKx7Pa2nJ5yykdw==
+  dependencies:
+    "@puppeteer/browsers" "0.4.0"
+    chromium-bidi "0.4.6"
+    cross-fetch "3.1.5"
+    debug "4.3.4"
+    devtools-protocol "0.0.1107588"
+    extract-zip "2.0.1"
+    https-proxy-agent "5.0.1"
+    proxy-from-env "1.1.0"
+    tar-fs "2.1.1"
+    unbzip2-stream "1.4.3"
+    ws "8.13.0"
+
+puppeteer@^19.5.2:
+  version "19.8.5"
+  resolved "https://registry.npmjs.org/puppeteer/-/puppeteer-19.8.5.tgz#18e701ff3122c46c3ce3e292191f3e439ee1e081"
+  integrity sha512-WSjouU7eux6cwBMEz4A7mDRVZWTQQTDXrb1R6AhKDdeEgpiBBkAzcAusPhILxiJOKj60rULZpWuCZ7HZIO6GTA==
+  dependencies:
+    "@puppeteer/browsers" "0.4.0"
+    cosmiconfig "8.1.3"
+    https-proxy-agent "5.0.1"
+    progress "2.0.3"
+    proxy-from-env "1.1.0"
+    puppeteer-core "19.8.5"
 
 qs@6.11.0:
   version "6.11.0"
   resolved "https://registry.npmjs.org/qs/-/qs-6.11.0.tgz#fd0d963446f7a65e1367e01abd85429453f0c37a"
   integrity sha512-MvjoMCJwEarSbUYk5O+nmoSzSutSsTwF85zcHPQ9OrlFoZOYIjaqBAJIqIXjptyD5vThxGq52Xu/MaJzRkIk4Q==
   dependencies:
     side-channel "^1.0.4"
 
+querystringify@^2.1.1:
+  version "2.2.0"
+  resolved "https://registry.npmjs.org/querystringify/-/querystringify-2.2.0.tgz#3345941b4153cb9d082d8eee4cda2016a9aef7f6"
+  integrity sha512-FIqgj2EUvTa7R50u0rGsyTftzjYmv/a3hO345bZNrqabNqjtgiDMgmo4mkUjd+nzU5oF3dClKqFIPUKybUyqoQ==
+
 range-parser@~1.2.1:
   version "1.2.1"
   resolved "https://registry.npmjs.org/range-parser/-/range-parser-1.2.1.tgz#3cf37023d199e1c24d1a55b84800c2f3e6468031"
   integrity sha512-Hrgsx+orqoygnmhFbKaHE6c296J+HTAQXoxEF6gNupROmmGJRoyzfG3ccAveqCBrwr/2yxQ5BVd/GTl5agOwSg==
 
 raw-body@2.5.1:
   version "2.5.1"
@@ -880,70 +1346,77 @@
   integrity sha512-qqJBtEyVgS0ZmPGdCFPWJ3FreoqvG4MVQln/kCgF7Olq95IbOp0/BWyMwbdtn4VTvkM8Y7khCQ2Xgk/tcrCXig==
   dependencies:
     bytes "3.1.2"
     http-errors "2.0.0"
     iconv-lite "0.4.24"
     unpipe "1.0.0"
 
-readable-stream@^2.2.2:
-  version "2.3.7"
-  resolved "https://registry.npmjs.org/readable-stream/-/readable-stream-2.3.7.tgz#1eca1cf711aef814c04f62252a36a62f6cb23b57"
-  integrity sha512-Ebho8K4jIbHAxnuxi7o42OrZgF/ZTNcsZj6nRKyUmkhLFq8CHItp/fy6hQZuZmP/n3yZ9VBUbp4zz/mX8hmYPw==
-  dependencies:
-    core-util-is "~1.0.0"
-    inherits "~2.0.3"
-    isarray "~1.0.0"
-    process-nextick-args "~2.0.0"
-    safe-buffer "~5.1.1"
-    string_decoder "~1.1.1"
-    util-deprecate "~1.0.1"
-
-readable-stream@^3.4.0, readable-stream@^3.6.0:
-  version "3.6.0"
-  resolved "https://registry.npmjs.org/readable-stream/-/readable-stream-3.6.0.tgz#337bbda3adc0706bd3e024426a286d4b4b2c9198"
-  integrity sha512-BViHy7LKeTz4oNnkcLJ+lVSL6vpiFeX6/d3oSH8zCW7UxP2onchk+vTGB143xuFjHS3deTgkKoXXymXqymiIdA==
+readable-stream@^3.1.1, readable-stream@^3.4.0, readable-stream@^3.6.0:
+  version "3.6.2"
+  resolved "https://registry.npmjs.org/readable-stream/-/readable-stream-3.6.2.tgz#56a9b36ea965c00c5a93ef31eb111a0f11056967"
+  integrity sha512-9u/sniCrY3D5WdsERHzHE4G2YCXqoG5FTHUiCC4SIbr6XcLZBY05ya9EKjYek9O5xOAwjGq+1JdGBAS7Q9ScoA==
   dependencies:
     inherits "^2.0.3"
     string_decoder "^1.1.1"
     util-deprecate "^1.0.1"
 
 readdirp@~3.6.0:
   version "3.6.0"
   resolved "https://registry.npmjs.org/readdirp/-/readdirp-3.6.0.tgz#74a370bd857116e245b29cc97340cd431a02a6c7"
   integrity sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==
   dependencies:
     picomatch "^2.2.1"
 
-rimraf@^2.6.1:
-  version "2.7.1"
-  resolved "https://registry.npmjs.org/rimraf/-/rimraf-2.7.1.tgz#35797f13a7fdadc566142c29d4f07ccad483e3ec"
-  integrity sha512-uWjbaKIK3T1OSVptzX7Nl6PvQ3qAGtKEtVRjRuazjfL3Bx5eI409VZSqgND+4UNnmzLVdPj9FqFJNPqBZFve4w==
-  dependencies:
-    glob "^7.1.3"
+require-directory@^2.1.1:
+  version "2.1.1"
+  resolved "https://registry.npmjs.org/require-directory/-/require-directory-2.1.1.tgz#8c64ad5fd30dab1c976e2344ffe7f792a6a6df42"
+  integrity sha512-fGxEI7+wsG9xrvdjsrlmL22OMTTiHRwAMroiEeMgq8gzoLC/PQr7RsRDSTLUg/bZAZtF+TVIkHc6/4RIKrui+Q==
+
+requires-port@^1.0.0:
+  version "1.0.0"
+  resolved "https://registry.npmjs.org/requires-port/-/requires-port-1.0.0.tgz#925d2601d39ac485e091cf0da5c6e694dc3dcaff"
+  integrity sha512-KigOCHcocU3XODJxsu8i/j8T9tzT4adHiecwORRQ0ZZFcp7ahwXuRU1m+yuO90C5ZUyGeGfocHDI14M3L3yDAQ==
 
-safe-buffer@5.1.2, safe-buffer@~5.1.0, safe-buffer@~5.1.1:
+resolve-from@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/resolve-from/-/resolve-from-4.0.0.tgz#4abcd852ad32dd7baabfe9b40e00a36db5f392e6"
+  integrity sha512-pb/MYmXstAkysRFx8piNI1tGFNQIFA3vkE3Gq4EuA1dF6gHp/+vgZqsCGJapvy8N3Q+4o7FwvquPJcnZ7RYy4g==
+
+rrweb-cssom@^0.6.0:
+  version "0.6.0"
+  resolved "https://registry.npmjs.org/rrweb-cssom/-/rrweb-cssom-0.6.0.tgz#ed298055b97cbddcdeb278f904857629dec5e0e1"
+  integrity sha512-APM0Gt1KoXBz0iIkkdB/kfvGOwC4UuJFeG/c+yV7wSc7q96cG/kJ0HiYCnzivD9SB53cLV1MlHFNfOuPaadYSw==
+
+safe-buffer@5.1.2:
   version "5.1.2"
   resolved "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.1.2.tgz#991ec69d296e0313747d59bdfd2b745c35f8828d"
   integrity sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==
 
 safe-buffer@5.2.1, safe-buffer@~5.2.0:
   version "5.2.1"
   resolved "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.2.1.tgz#1eaf9fa9bdb1fdd4ec75f58f9cdb4e6b7827eec6"
   integrity sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==
 
 safe-stable-stringify@^2.3.1:
-  version "2.4.1"
-  resolved "https://registry.npmjs.org/safe-stable-stringify/-/safe-stable-stringify-2.4.1.tgz#34694bd8a30575b7f94792aa51527551bd733d61"
-  integrity sha512-dVHE6bMtS/bnL2mwualjc6IxEv1F+OCUpA46pKUj6F8uDbUM0jCCulPqRNPSnWwGNKx5etqMjZYdXtrm5KJZGA==
+  version "2.4.3"
+  resolved "https://registry.npmjs.org/safe-stable-stringify/-/safe-stable-stringify-2.4.3.tgz#138c84b6f6edb3db5f8ef3ef7115b8f55ccbf886"
+  integrity sha512-e2bDA2WJT0wxseVd4lsDP4+3ONX6HpMXQa1ZhFQ7SU+GjvORCmShbCMltrtIDfkYhVHrOcPtj+KhmDBdPdZD1g==
 
-"safer-buffer@>= 2.1.2 < 3":
+"safer-buffer@>= 2.1.2 < 3", "safer-buffer@>= 2.1.2 < 3.0.0":
   version "2.1.2"
   resolved "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz#44fa161b0187b9549dd84bb91802f9bd8385cd6a"
   integrity sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==
 
+saxes@^6.0.0:
+  version "6.0.0"
+  resolved "https://registry.npmjs.org/saxes/-/saxes-6.0.0.tgz#fe5b4a4768df4f14a201b1ba6a65c1f3d9988cc5"
+  integrity sha512-xAg7SOnEhrm5zI3puOOKyy1OMcMlIJZYNJY7xLBwSze0UjhPLnWfj2GF2EpT0jmzaJKIWKHLsaSSajf35bcYnA==
+  dependencies:
+    xmlchars "^2.2.0"
+
 semver@^5.7.1:
   version "5.7.1"
   resolved "https://registry.npmjs.org/semver/-/semver-5.7.1.tgz#a954f931aeba508d307bbf069eff0c01c96116f7"
   integrity sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==
 
 semver@~7.0.0:
   version "7.0.0"
@@ -997,56 +1470,101 @@
   version "0.2.2"
   resolved "https://registry.npmjs.org/simple-swizzle/-/simple-swizzle-0.2.2.tgz#a4da6b635ffcccca33f70d17cb92592de95e557a"
   integrity sha512-JA//kQgZtbuY83m+xT+tXJkmJncGMTFT+C+g2h2R9uxkYIrE2yy9sgmcLhCnw57/WSD+Eh3J97FPEDFnbXnDUg==
   dependencies:
     is-arrayish "^0.3.1"
 
 simple-update-notifier@^1.0.7:
-  version "1.0.7"
-  resolved "https://registry.npmjs.org/simple-update-notifier/-/simple-update-notifier-1.0.7.tgz#7edf75c5bdd04f88828d632f762b2bc32996a9cc"
-  integrity sha512-BBKgR84BJQJm6WjWFMHgLVuo61FBDSj1z/xSFUIozqO6wO7ii0JxCqlIud7Enr/+LhlbNI0whErq96P2qHNWew==
+  version "1.1.0"
+  resolved "https://registry.npmjs.org/simple-update-notifier/-/simple-update-notifier-1.1.0.tgz#67694c121de354af592b347cdba798463ed49c82"
+  integrity sha512-VpsrsJSUcJEseSbMHkrsrAVSdvVS5I96Qo1QAQ4FxQ9wXFcB+pjj7FB7/us9+GcgfW4ziHtYMc1J0PLczb55mg==
   dependencies:
     semver "~7.0.0"
 
+source-map@~0.6.1:
+  version "0.6.1"
+  resolved "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz#74722af32e9614e9c287a8d0bbde48b5e2f1a263"
+  integrity sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==
+
 stack-trace@0.0.x:
   version "0.0.10"
   resolved "https://registry.npmjs.org/stack-trace/-/stack-trace-0.0.10.tgz#547c70b347e8d32b4e108ea1a2a159e5fdde19c0"
   integrity sha512-KGzahc7puUKkzyMt+IqAep+TVNbKP+k2Lmwhub39m1AsTSkaDutx56aDCo+HLDzf/D26BIHTJWNiTG1KAJiQCg==
 
 statuses@2.0.1:
   version "2.0.1"
   resolved "https://registry.npmjs.org/statuses/-/statuses-2.0.1.tgz#55cb000ccf1d48728bd23c685a063998cf1a1b63"
   integrity sha512-RwNA9Z/7PrK06rYLIzFMlaF+l73iwpzsqRIFgbMLbTcLD6cOao82TaWefPXQvB2fOC4AjuYSEndS7N/mTCbkdQ==
 
+string-width@^4.1.0, string-width@^4.2.0, string-width@^4.2.3:
+  version "4.2.3"
+  resolved "https://registry.npmjs.org/string-width/-/string-width-4.2.3.tgz#269c7117d27b05ad2e536830a8ec895ef9c6d010"
+  integrity sha512-wKyQRQpjJ0sIp62ErSZdGsjMJWsap5oRNihHhu6G7JVO/9jIB6UyevL+tXuOqrng8j/cxKTWyWUwvSTriiZz/g==
+  dependencies:
+    emoji-regex "^8.0.0"
+    is-fullwidth-code-point "^3.0.0"
+    strip-ansi "^6.0.1"
+
 string_decoder@^1.1.1:
   version "1.3.0"
   resolved "https://registry.npmjs.org/string_decoder/-/string_decoder-1.3.0.tgz#42f114594a46cf1a8e30b0a84f56c78c3edac21e"
   integrity sha512-hkRX8U1WjJFd8LsDJ2yQ/wWWxaopEsABU1XfkM8A+j0+85JAGppt16cr1Whg6KIbb4okU6Mql6BOj+uup/wKeA==
   dependencies:
     safe-buffer "~5.2.0"
 
-string_decoder@~1.1.1:
-  version "1.1.1"
-  resolved "https://registry.npmjs.org/string_decoder/-/string_decoder-1.1.1.tgz#9cf1611ba62685d7030ae9e4ba34149c3af03fc8"
-  integrity sha512-n/ShnvDi6FHbbVfviro+WojiFzv+s8MPMHBczVePfUpDJLwoLT0ht1l4YwBCbi8pJAveEEdnkHyPyTP/mzRfwg==
+strip-ansi@^6.0.0, strip-ansi@^6.0.1:
+  version "6.0.1"
+  resolved "https://registry.npmjs.org/strip-ansi/-/strip-ansi-6.0.1.tgz#9e26c63d30f53443e9489495b2105d37b67a85d9"
+  integrity sha512-Y38VPSHcqkFrCpFnQ9vuSXmquuv5oXOKpGeT6aGrr3o3Gc9AlVa6JBfUSOCnbxGGZF+/0ooI7KrPuUSztUdU5A==
   dependencies:
-    safe-buffer "~5.1.0"
+    ansi-regex "^5.0.1"
 
-supports-color@^5.5.0:
+supports-color@^5.3.0, supports-color@^5.5.0:
   version "5.5.0"
   resolved "https://registry.npmjs.org/supports-color/-/supports-color-5.5.0.tgz#e2e69a44ac8772f78a1ec0b35b689df6530efc8f"
   integrity sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==
   dependencies:
     has-flag "^3.0.0"
 
+symbol-tree@^3.2.4:
+  version "3.2.4"
+  resolved "https://registry.npmjs.org/symbol-tree/-/symbol-tree-3.2.4.tgz#430637d248ba77e078883951fb9aa0eed7c63fa2"
+  integrity sha512-9QNk5KwDF+Bvz+PyObkmSYjI5ksVUYtjW7AU22r2NKcfLJcXp96hkDWU3+XndOsUb+AQ9QhfzfCT2O+CNWT5Tw==
+
+tar-fs@2.1.1:
+  version "2.1.1"
+  resolved "https://registry.npmjs.org/tar-fs/-/tar-fs-2.1.1.tgz#489a15ab85f1f0befabb370b7de4f9eb5cbe8784"
+  integrity sha512-V0r2Y9scmbDRLCNex/+hYzvp/zyYjvFbHPNgVTKfQvVrb6guiE/fxP+XblDNR011utopbkex2nM4dHNV6GDsng==
+  dependencies:
+    chownr "^1.1.1"
+    mkdirp-classic "^0.5.2"
+    pump "^3.0.0"
+    tar-stream "^2.1.4"
+
+tar-stream@^2.1.4:
+  version "2.2.0"
+  resolved "https://registry.npmjs.org/tar-stream/-/tar-stream-2.2.0.tgz#acad84c284136b060dc3faa64474aa9aebd77287"
+  integrity sha512-ujeqbceABgwMZxEJnk2HDY2DlnUZ+9oEcb1KzTVfYHio0UE6dG71n60d8D2I4qNvleWrrXpmjpt7vZeF1LnMZQ==
+  dependencies:
+    bl "^4.0.3"
+    end-of-stream "^1.4.1"
+    fs-constants "^1.0.0"
+    inherits "^2.0.3"
+    readable-stream "^3.1.1"
+
 text-hex@1.0.x:
   version "1.0.0"
   resolved "https://registry.npmjs.org/text-hex/-/text-hex-1.0.0.tgz#69dc9c1b17446ee79a92bf5b884bb4b9127506f5"
   integrity sha512-uuVGNWzgJ4yhRaNSiubPY7OjISw4sw4E5Uv0wbjp+OzcbmVU/rsT8ujgcXJhn9ypzsgr5vlzpPqP+MBBKcGvbg==
 
+through@^2.3.8:
+  version "2.3.8"
+  resolved "https://registry.npmjs.org/through/-/through-2.3.8.tgz#0dd4c9ffaabc357960b1b724115d7e0e86a2e1f5"
+  integrity sha512-w89qg7PI8wAdvX60bMDP+bFoD5Dvhm9oLheFp5O4a2QF0cSBGsBX4qZmadPMvVqlLJBBci+WqGGOAPvcDeNSVg==
+
 to-regex-range@^5.0.1:
   version "5.0.1"
   resolved "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz#1648c44aae7c8d988a326018ed72f5b4dd0392e4"
   integrity sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==
   dependencies:
     is-number "^7.0.0"
 
@@ -1058,14 +1576,31 @@
 touch@^3.1.0:
   version "3.1.0"
   resolved "https://registry.npmjs.org/touch/-/touch-3.1.0.tgz#fe365f5f75ec9ed4e56825e0bb76d24ab74af83b"
   integrity sha512-WBx8Uy5TLtOSRtIq+M03/sKDrXCLHxwDcquSP2c43Le03/9serjQBIztjRz6FkJez9D/hleyAXTBGLwwZUw9lA==
   dependencies:
     nopt "~1.0.10"
 
+tough-cookie@^4.1.2:
+  version "4.1.2"
+  resolved "https://registry.npmjs.org/tough-cookie/-/tough-cookie-4.1.2.tgz#e53e84b85f24e0b65dd526f46628db6c85f6b874"
+  integrity sha512-G9fqXWoYFZgTc2z8Q5zaHy/vJMjm+WV0AkAeHxVCQiEB1b+dGvWzFW6QV07cY5jQ5gRkeid2qIkzkxUnmoQZUQ==
+  dependencies:
+    psl "^1.1.33"
+    punycode "^2.1.1"
+    universalify "^0.2.0"
+    url-parse "^1.5.3"
+
+tr46@^4.1.1:
+  version "4.1.1"
+  resolved "https://registry.npmjs.org/tr46/-/tr46-4.1.1.tgz#281a758dcc82aeb4fe38c7dfe4d11a395aac8469"
+  integrity sha512-2lv/66T7e5yNyhAAC4NaKe5nVavzuGJQVVtRYLyQ2OI8tsJ61PMLlelehb0wi2Hx6+hT/OJUWZcw8MjlSRnxvw==
+  dependencies:
+    punycode "^2.3.0"
+
 tr46@~0.0.3:
   version "0.0.3"
   resolved "https://registry.npmjs.org/tr46/-/tr46-0.0.3.tgz#8184fd347dac9cdc185992f3a6622e14b9d9ab6a"
   integrity sha512-N3WMsuqV66lT30CrXNbEjx4GEwlow3v6rr4mCcv6prnfwhS01rkgyFdjPNBYd9br7LpXV1+Emh01fHnq2Gdgrw==
 
 triple-beam@^1.3.0:
   version "1.3.0"
@@ -1073,57 +1608,117 @@
   integrity sha512-XrHUvV5HpdLmIj4uVMxHggLbFSZYIn7HEWsqePZcI50pco+MPqJ50wMGY794X7AOOhxOBAjbkqfAbEe/QMp2Lw==
 
 tslib@^1.11.1:
   version "1.14.1"
   resolved "https://registry.npmjs.org/tslib/-/tslib-1.14.1.tgz#cf2d38bdc34a134bcaf1091c41f6619e2f672d00"
   integrity sha512-Xni35NKzjgMrwevysHTCArtLDpPvye8zV/0E4EyYn43P7/7qvQwPh9BGkHewbMulVntbigmcT7rdX3BNo9wRJg==
 
+type-check@~0.3.2:
+  version "0.3.2"
+  resolved "https://registry.npmjs.org/type-check/-/type-check-0.3.2.tgz#5884cab512cf1d355e3fb784f30804b2b520db72"
+  integrity sha512-ZCmOJdvOWDBYJlzAoFkC+Q0+bUyEOS1ltgp1MGU03fqHG+dbi9tBFU2Rd9QKiDZFAYrhPh2JUf7rZRIuHRKtOg==
+  dependencies:
+    prelude-ls "~1.1.2"
+
 type-is@~1.6.18:
   version "1.6.18"
   resolved "https://registry.npmjs.org/type-is/-/type-is-1.6.18.tgz#4e552cd05df09467dcbc4ef739de89f2cf37c131"
   integrity sha512-TkRKr9sUTxEH8MdfuCSP7VizJyzRNMjj2J2do2Jr3Kym598JVdEksuzPQCnlFPW4ky9Q+iA+ma9BGm06XQBy8g==
   dependencies:
     media-typer "0.3.0"
     mime-types "~2.1.24"
 
-typedarray@^0.0.6:
-  version "0.0.6"
-  resolved "https://registry.npmjs.org/typedarray/-/typedarray-0.0.6.tgz#867ac74e3864187b1d3d47d996a78ec5c8830777"
-  integrity sha512-/aCDEGatGvZ2BIk+HmLf4ifCJFwvKFNb9/JeZPMulfgFracn9QFcAf5GO8B/mweUjSoblS5In0cWhqpfs/5PQA==
+unbzip2-stream@1.4.3:
+  version "1.4.3"
+  resolved "https://registry.npmjs.org/unbzip2-stream/-/unbzip2-stream-1.4.3.tgz#b0da04c4371311df771cdc215e87f2130991ace7"
+  integrity sha512-mlExGW4w71ebDJviH16lQLtZS32VKqsSfk80GCfUlwT/4/hNRFsoscrF/c++9xinkMzECL1uL9DDwXqFWkruPg==
+  dependencies:
+    buffer "^5.2.1"
+    through "^2.3.8"
 
 undefsafe@^2.0.5:
   version "2.0.5"
   resolved "https://registry.npmjs.org/undefsafe/-/undefsafe-2.0.5.tgz#38733b9327bdcd226db889fb723a6efd162e6e2c"
   integrity sha512-WxONCrssBM8TSPRqN5EmsjVrsv4A8X12J4ArBiiayv3DyyG3ZlIg6yysuuSYdZsVz3TKcTg2fd//Ujd4CHV1iA==
 
+universalify@^0.2.0:
+  version "0.2.0"
+  resolved "https://registry.npmjs.org/universalify/-/universalify-0.2.0.tgz#6451760566fa857534745ab1dde952d1b1761be0"
+  integrity sha512-CJ1QgKmNg3CwvAv/kOFmtnEN05f0D/cn9QntgNOQlQF9dgvVTHj3t+8JPdjqawCHk7V/KA+fbUqzZ9XWhcqPUg==
+
 unpipe@1.0.0, unpipe@~1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz#b2bf4ee8514aae6165b4817829d21b2ef49904ec"
   integrity sha512-pjy2bYhSsufwWlKwPc+l3cN7+wuJlK6uz0YdJEOlQDbl6jo/YlPi4mb8agUkVC8BF7V8NuzeyPNqRksA3hztKQ==
 
-util-deprecate@^1.0.1, util-deprecate@~1.0.1:
+url-parse@^1.5.3:
+  version "1.5.10"
+  resolved "https://registry.npmjs.org/url-parse/-/url-parse-1.5.10.tgz#9d3c2f736c1d75dd3bd2be507dcc111f1e2ea9c1"
+  integrity sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==
+  dependencies:
+    querystringify "^2.1.1"
+    requires-port "^1.0.0"
+
+util-deprecate@^1.0.1:
   version "1.0.2"
   resolved "https://registry.npmjs.org/util-deprecate/-/util-deprecate-1.0.2.tgz#450d4dc9fa70de732762fbd2d4a28981419a0ccf"
   integrity sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==
 
 utils-merge@1.0.1:
   version "1.0.1"
   resolved "https://registry.npmjs.org/utils-merge/-/utils-merge-1.0.1.tgz#9f95710f50a267947b2ccc124741c1028427e713"
   integrity sha512-pMZTvIkT1d+TFGvDOqodOclx0QWkkgi6Tdoa8gC8ffGAAqz9pzPTZWAybbsHHoED/ztMtkv/VoYTYyShUn81hA==
 
 vary@~1.1.2:
   version "1.1.2"
   resolved "https://registry.npmjs.org/vary/-/vary-1.1.2.tgz#2299f02c6ded30d4a5961b0b9f74524a18f634fc"
   integrity sha512-BNGbWLfd0eUPabhkXUVm0j8uuvREyTh5ovRa/dyow/BqAbZJyC+5fU+IzQOzmAKzYqYRAISoRhdQr3eIZ/PXqg==
 
+w3c-xmlserializer@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/w3c-xmlserializer/-/w3c-xmlserializer-4.0.0.tgz#aebdc84920d806222936e3cdce408e32488a3073"
+  integrity sha512-d+BFHzbiCx6zGfz0HyQ6Rg69w9k19nviJspaj4yNscGjrHu94sVP+aRm75yEbCh+r2/yR+7q6hux9LVtbuTGBw==
+  dependencies:
+    xml-name-validator "^4.0.0"
+
+web-streams-polyfill@^3.0.3:
+  version "3.2.1"
+  resolved "https://registry.npmjs.org/web-streams-polyfill/-/web-streams-polyfill-3.2.1.tgz#71c2718c52b45fd49dbeee88634b3a60ceab42a6"
+  integrity sha512-e0MO3wdXWKrLbL0DgGnUV7WHVuw9OUvL4hjgnPkIeEvESk74gAITi5G606JtZPp39cd8HA9VQzCIvA49LpPN5Q==
+
 webidl-conversions@^3.0.0:
   version "3.0.1"
   resolved "https://registry.npmjs.org/webidl-conversions/-/webidl-conversions-3.0.1.tgz#24534275e2a7bc6be7bc86611cc16ae0a5654871"
   integrity sha512-2JAn3z8AR6rjK8Sm8orRC0h/bcl/DqL7tRPdGZ4I1CjdF+EaMLmYxBHyXuKL849eucPFhvBoxMsflfOb8kxaeQ==
 
+webidl-conversions@^7.0.0:
+  version "7.0.0"
+  resolved "https://registry.npmjs.org/webidl-conversions/-/webidl-conversions-7.0.0.tgz#256b4e1882be7debbf01d05f0aa2039778ea080a"
+  integrity sha512-VwddBukDzu71offAQR975unBIGqfKZpM+8ZX6ySk8nYhVoo5CYaZyzt3YBvYtRtO+aoGlqxPg/B87NGVZ/fu6g==
+
+whatwg-encoding@^2.0.0:
+  version "2.0.0"
+  resolved "https://registry.npmjs.org/whatwg-encoding/-/whatwg-encoding-2.0.0.tgz#e7635f597fd87020858626805a2729fa7698ac53"
+  integrity sha512-p41ogyeMUrw3jWclHWTQg1k05DSVXPLcVxRTYsXUk+ZooOCZLcoYgPZ/HL/D/N+uQPOtcp1me1WhBEaX02mhWg==
+  dependencies:
+    iconv-lite "0.6.3"
+
+whatwg-mimetype@^3.0.0:
+  version "3.0.0"
+  resolved "https://registry.npmjs.org/whatwg-mimetype/-/whatwg-mimetype-3.0.0.tgz#5fa1a7623867ff1af6ca3dc72ad6b8a4208beba7"
+  integrity sha512-nt+N2dzIutVRxARx1nghPKGv1xHikU7HKdfafKkLNLindmPU/ch3U31NOCGGA/dmPcmb1VlofO0vnKAcsm0o/Q==
+
+whatwg-url@^12.0.0, whatwg-url@^12.0.1:
+  version "12.0.1"
+  resolved "https://registry.npmjs.org/whatwg-url/-/whatwg-url-12.0.1.tgz#fd7bcc71192e7c3a2a97b9a8d6b094853ed8773c"
+  integrity sha512-Ed/LrqB8EPlGxjS+TrsXcpUond1mhccS3pchLhzSgPCnTimUCKj3IZE75pAs5m6heB2U2TMerKFUXheyHY+VDQ==
+  dependencies:
+    tr46 "^4.1.1"
+    webidl-conversions "^7.0.0"
+
 whatwg-url@^5.0.0:
   version "5.0.0"
   resolved "https://registry.npmjs.org/whatwg-url/-/whatwg-url-5.0.0.tgz#966454e8765462e37644d3626f6742ce8b70965d"
   integrity sha512-saE57nupxk6v3HY35+jzBwYa0rKSy0XR8JSxZPwgLr7ys0IBzhGviA1/TUGJLmSVqs8pb9AnvICXEuOHLprYTw==
   dependencies:
     tr46 "~0.0.3"
     webidl-conversions "^3.0.0"
@@ -1133,15 +1728,15 @@
   resolved "https://registry.npmjs.org/winston-transport/-/winston-transport-4.5.0.tgz#6e7b0dd04d393171ed5e4e4905db265f7ab384fa"
   integrity sha512-YpZzcUzBedhlTAfJg6vJDlyEai/IFMIVcaEZZyl3UXIl4gmqRpU7AE89AHLkbzLUsv0NVmw7ts+iztqKxxPW1Q==
   dependencies:
     logform "^2.3.2"
     readable-stream "^3.6.0"
     triple-beam "^1.3.0"
 
-winston@^3.2.1:
+winston@^3.8.2:
   version "3.8.2"
   resolved "https://registry.npmjs.org/winston/-/winston-3.8.2.tgz#56e16b34022eb4cff2638196d9646d7430fdad50"
   integrity sha512-MsE1gRx1m5jdTTO9Ld/vND4krP2To+lgDoMEHGGa4HIlAUyXJtfc7CxQcGXVyz2IBpw5hbFkj2b/AtUdQwyRew==
   dependencies:
     "@colors/colors" "1.5.0"
     "@dabh/diagnostics" "^2.0.2"
     async "^3.2.3"
@@ -1150,30 +1745,70 @@
     one-time "^1.0.0"
     readable-stream "^3.4.0"
     safe-stable-stringify "^2.3.1"
     stack-trace "0.0.x"
     triple-beam "^1.3.0"
     winston-transport "^4.5.0"
 
+word-wrap@~1.2.3:
+  version "1.2.3"
+  resolved "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.3.tgz#610636f6b1f703891bd34771ccb17fb93b47079c"
+  integrity sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==
+
+wrap-ansi@^7.0.0:
+  version "7.0.0"
+  resolved "https://registry.npmjs.org/wrap-ansi/-/wrap-ansi-7.0.0.tgz#67e145cff510a6a6984bdf1152911d69d2eb9e43"
+  integrity sha512-YVGIj2kamLSTxw6NsZjoBxfSwsn0ycdesmc4p+Q21c5zPuZ1pl+NfxVdxPtdHvmNVOQ6XSYG4AUtyt/Fi7D16Q==
+  dependencies:
+    ansi-styles "^4.0.0"
+    string-width "^4.1.0"
+    strip-ansi "^6.0.0"
+
 wrappy@1:
   version "1.0.2"
   resolved "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz#b5243d8f3ec1aa35f1364605bc0d1036e30ab69f"
   integrity sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==
 
-ws@^6.1.0:
-  version "6.2.2"
-  resolved "https://registry.npmjs.org/ws/-/ws-6.2.2.tgz#dd5cdbd57a9979916097652d78f1cc5faea0c32e"
-  integrity sha512-zmhltoSR8u1cnDsD43TX59mzoMZsLKqUweyYBAIvTngR3shc0W6aOZylZmq/7hqyVxPdi+5Ud2QInblgyE72fw==
-  dependencies:
-    async-limiter "~1.0.0"
-
-xmldom@^0.1.27:
-  version "0.1.31"
-  resolved "https://registry.npmjs.org/xmldom/-/xmldom-0.1.31.tgz#b76c9a1bd9f0a9737e5a72dc37231cf38375e2ff"
-  integrity sha512-yS2uJflVQs6n+CyjHoaBmVSqIDevTAWrzMmjG1Gc7h1qQ7uVozNhEPJAwZXWyGQ/Gafo3fCwrcaokezLPupVyQ==
+ws@8.13.0, ws@^8.13.0:
+  version "8.13.0"
+  resolved "https://registry.npmjs.org/ws/-/ws-8.13.0.tgz#9a9fb92f93cf41512a0735c8f4dd09b8a1211cd0"
+  integrity sha512-x9vcZYTrFPC7aSIbj7sRCYo7L/Xb8Iy+pW0ng0wt2vCJv7M9HOMy0UoN3rr+IFC7hb7vXoqS+P9ktyLLLhO+LA==
+
+xml-name-validator@^4.0.0:
+  version "4.0.0"
+  resolved "https://registry.npmjs.org/xml-name-validator/-/xml-name-validator-4.0.0.tgz#79a006e2e63149a8600f15430f0a4725d1524835"
+  integrity sha512-ICP2e+jsHvAj2E2lIHxa5tjXRlKDJo4IdvPvCXbXQGdzSfmSpNVyIKMvoZHjDY9DP0zV17iI85o90vRFXNccRw==
+
+xmlchars@^2.2.0:
+  version "2.2.0"
+  resolved "https://registry.npmjs.org/xmlchars/-/xmlchars-2.2.0.tgz#060fe1bcb7f9c76fe2a17db86a9bc3ab894210cb"
+  integrity sha512-JZnDKK8B0RCDw84FNdDAIpZK+JuJw+s7Lz8nksI7SIuU3UXJJslUthsi+uWBUYOwPFwW7W7PRLRfUKpxjtjFCw==
+
+y18n@^5.0.5:
+  version "5.0.8"
+  resolved "https://registry.npmjs.org/y18n/-/y18n-5.0.8.tgz#7f4934d0f7ca8c56f95314939ddcd2dd91ce1d55"
+  integrity sha512-0pfFzegeDWJHJIAmTLRP2DwHjdF5s7jo9tuztdQxAhINCdvS+3nGINqPd00AphqJR/0LhANUS6/+7SCb98YOfA==
+
+yargs-parser@^21.1.1:
+  version "21.1.1"
+  resolved "https://registry.npmjs.org/yargs-parser/-/yargs-parser-21.1.1.tgz#9096bceebf990d21bb31fa9516e0ede294a77d35"
+  integrity sha512-tVpsJW7DdjecAiFpbIB1e3qxIQsE6NoPc5/eTdrbbIC4h0LVsWhnoa3g+m2HclBIujHzsxZ4VJVA+GUuc2/LBw==
+
+yargs@17.7.1:
+  version "17.7.1"
+  resolved "https://registry.npmjs.org/yargs/-/yargs-17.7.1.tgz#34a77645201d1a8fc5213ace787c220eabbd0967"
+  integrity sha512-cwiTb08Xuv5fqF4AovYacTFNxk62th7LKJ6BL9IGUpTJrWoU7/7WdQGTP2SjKf1dUNBGzDd28p/Yfs/GI6JrLw==
+  dependencies:
+    cliui "^8.0.1"
+    escalade "^3.1.1"
+    get-caller-file "^2.0.5"
+    require-directory "^2.1.1"
+    string-width "^4.2.3"
+    y18n "^5.0.5"
+    yargs-parser "^21.1.1"
 
 yauzl@^2.10.0:
   version "2.10.0"
   resolved "https://registry.npmjs.org/yauzl/-/yauzl-2.10.0.tgz#c7eb17c93e112cb1086fa6d8e51fb0667b79a5f9"
   integrity sha512-p4a9I6X6nu6IhoGmBqAcbJy1mlC4j27vEPZX9F4L4/vZT3Lyq1VkFHw/V/PUcB9Buo+DG3iHkT0x3Qya58zc3g==
   dependencies:
     buffer-crc32 "~0.2.3"
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/PKG-INFO` & `ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ipydrawio-export
-Version: 1.2.2
+Version: 1.3.0
 Summary: PDF export for Drawio diagrams in JupyterLab
 Home-page: https://ipydrawio.rtfd.io
 Author: ipydrawio Contributors
 Author-email: ripxl@example.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/deathbeds/ipydrawio/issues
-Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://app.codecov.io/gh/deathbeds/ipydrawio
 Project-URL: Documentation, https://ipydrawio.rtfd.io
 Project-URL: Source Code, https://github.com/deathbeds/ipydrawio
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # IPyDrawio Export
 
 [![docs][docs-badge]][docs] [![binder-badge][]][binder]
@@ -125,15 +124,15 @@
 
 This work is licensed under the [Apache-2.0] License.
 
 The vendored code from [@jgraph/draw-image-export2][] is also licensed under the
 [Apache-2.0][draw2-license] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -142,28 +141,28 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [@jgraph/draw-image-export2]: https://github.com/jgraph/draw-image-export2
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-export/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-export/LICENSE.txt
 [draw2-license]:
   https://github.com/jgraph/draw-image-export2/blob/master/LICENSE
 [serverext]:
   https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Distributing%20Jupyter%20Extensions%20as%20Python%20Packages.html
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-export
 [pypi]: https://pypi.org/project/ipydrawio-export
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-export
 [conda]: https://anaconda.org/conda-forge/ipydrawio-export
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-export-1.2.2/src/ipydrawio_export.egg-info/SOURCES.txt` & `ipydrawio-export-1.3.0/src/ipydrawio_export.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+./README.md
 _/ipydrawio-pdf/package.json
-_/ipydrawio-pdf/static/385.92b16e78cc4802eb266f.js
-_/ipydrawio-pdf/static/568.3ea8d02d5f8c77cec1bd.js
-_/ipydrawio-pdf/static/remoteEntry.aaae5653dd69b7dedcd0.js
+_/ipydrawio-pdf/static/385.1639e823caa9b50aada5.js
+_/ipydrawio-pdf/static/568.c1c4c11fee97c25006f5.js
+_/ipydrawio-pdf/static/remoteEntry.a38839e484daf1046bb6.js
 _/ipydrawio-pdf/static/style.js
 _/ipydrawio-pdf/static/third-party-licenses.json
 src/ipydrawio_export/__init__.py
 src/ipydrawio_export/_version.py
 src/ipydrawio_export/app.py
 src/ipydrawio_export/constants.py
 src/ipydrawio_export/handlers.py
```

### Comparing `ipydrawio-export-1.2.2/tests/__init__.py` & `ipydrawio-export-1.3.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """tests of ipydrawio-export"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-export-1.2.2/tests/conftest.py` & `ipydrawio-export-1.3.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ipydrawio-export test environment"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-export-1.2.2/tests/fixtures/a.svg` & `ipydrawio-export-1.3.0/tests/fixtures/a.svg`

 * *Files identical despite different names*

### Comparing `ipydrawio-export-1.2.2/tests/fixtures/b.png` & `ipydrawio-export-1.3.0/tests/fixtures/b.png`

 * *Files identical despite different names*

### Comparing `ipydrawio-export-1.2.2/tests/fixtures/empty.dio` & `ipydrawio-export-1.3.0/tests/fixtures/empty.dio`

 * *Files identical despite different names*

### Comparing `ipydrawio-export-1.2.2/tests/fixtures/empty.ipynb` & `ipydrawio-export-1.3.0/tests/fixtures/empty.ipynb`

 * *Files identical despite different names*

### Comparing `ipydrawio-export-1.2.2/tests/test_app.py` & `ipydrawio-export-1.3.0/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """test basic app functionality"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-export-1.2.2/tests/test_cli.py` & `ipydrawio-export-1.3.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """test basic CLI functionality"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-export-1.2.2/tests/test_meta.py` & `ipydrawio-export-1.3.0/tests/test_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ipydrawio-export metadata tests"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `ipydrawio-export-1.2.2/tests/test_pdf.py` & `ipydrawio-export-1.3.0/tests/test_pdf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """ipydrawio-export pdf tests"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-from PyPDF2 import PdfFileReader
+from pypdf import PdfReader
 
 
 @pytest.mark.parametrize("attach_xml", [0, 1])
 def test_export_empty(tmp_path, export_app, any_diagram, attach_xml):
     manager = export_app.drawio_manager
     manager.attach_xml = bool(attach_xml)
 
     export_app.dio_files = [any_diagram]
     export_app.start()
 
     out = tmp_path / f"{any_diagram.stem}.pdf"
-    reader = PdfFileReader(str(out), "rb")
-    assert reader.getNumPages() == 1
+    assert out.exists(), f"{out} was not created"
+    reader = PdfReader(str(out), "rb")
+    assert len(reader.pages) == 1
 
     attachments = sorted(manager.attachments(out))
     assert len(attachments) == attach_xml
 
 
 @pytest.mark.parametrize("attach_xml", [0, 1])
 def test_export_merged(tmp_path, export_app, empty_dio, svg, png, ipynb, attach_xml):
@@ -41,12 +42,12 @@
 
     export_app.dio_files = [empty_dio, svg, png, ipynb]
     export_app.start()
 
     out = tmp_path / f"{empty_dio.stem}.pdf"
     assert out.exists(), f"{out} was not created"
 
-    reader = PdfFileReader(str(out), "rb")
-    assert reader.getNumPages() == 4, "unexpected number of pages"
+    reader = PdfReader(str(out), "rb")
+    assert len(reader.pages) == 4, "unexpected number of pages"
 
     attachments = sorted(manager.attachments(out))
     assert len(attachments) == attach_xml, "unexpected attachment status"
```

### Comparing `ipydrawio-export-1.2.2/tests/test_serverextension.py` & `ipydrawio-export-1.3.0/tests/test_serverextension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ipydrawio-export serverextension tests"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

