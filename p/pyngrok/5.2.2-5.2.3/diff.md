# Comparing `tmp/pyngrok-5.2.2.tar.gz` & `tmp/pyngrok-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyngrok-5.2.2.tar", last modified: Tue Apr 11 15:56:04 2023, max compression
+gzip compressed data, was "pyngrok-5.2.3.tar", last modified: Wed Apr 12 13:51:42 2023, max compression
```

## Comparing `pyngrok-5.2.2.tar` & `pyngrok-5.2.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.438800 pyngrok-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    24140 2023-04-11 15:54:15.000000 pyngrok-5.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-11 15:54:15.000000 pyngrok-5.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 15:54:15.000000 pyngrok-5.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-04-11 15:56:04.438800 pyngrok-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-11 15:54:15.000000 pyngrok-5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.410799 pyngrok-5.2.2/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.418799 pyngrok-5.2.2/_build/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/coverage.xml
--rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48___init___py.html
--rw-r--r--   0 runner    (1001) docker     (123)    32143 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_conf_py.html
--rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_exception_py.html
--rw-r--r--   0 runner    (1001) docker     (123)    88135 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_installer_py.html
--rw-r--r--   0 runner    (1001) docker     (123)   141997 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_ngrok_py.html
--rw-r--r--   0 runner    (1001) docker     (123)   127602 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_process_py.html
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/status.json
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-11 15:55:50.000000 pyngrok-5.2.2/_build/coverage/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.410799 pyngrok-5.2.2/_build/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.426800 pyngrok-5.2.2/_build/docs/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)   278765 2023-04-11 15:56:00.000000 pyngrok-5.2.2/_build/docs/doctrees/api.doctree
--rw-r--r--   0 runner    (1001) docker     (123)  2670977 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    74732 2023-04-11 15:56:00.000000 pyngrok-5.2.2/_build/docs/doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    53406 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/doctrees/integrations.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    32389 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/doctrees/troubleshooting.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.430800 pyngrok-5.2.2/_build/docs/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.430800 pyngrok-5.2.2/_build/docs/html/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    35534 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/_images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.430800 pyngrok-5.2.2/_build/docs/html/_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_modules/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.430800 pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/
--rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/conf.html
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/exception.html
--rw-r--r--   0 runner    (1001) docker     (123)    50746 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/installer.html
--rw-r--r--   0 runner    (1001) docker     (123)    76233 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/ngrok.html
--rw-r--r--   0 runner    (1001) docker     (123)    69413 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/process.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.434800 pyngrok-5.2.2/_build/docs/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/_sources/api.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/_sources/integrations.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/_sources/troubleshooting.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.438800 pyngrok-5.2.2/_build/docs/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-11 15:55:57.000000 pyngrok-5.2.2/_build/docs/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-11 15:55:57.000000 pyngrok-5.2.2/_build/docs/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 15:55:57.000000 pyngrok-5.2.2/_build/docs/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 15:55:57.000000 pyngrok-5.2.2/_build/docs/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-04-11 15:55:57.000000 pyngrok-5.2.2/_build/docs/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-11 15:55:57.000000 pyngrok-5.2.2/_build/docs/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)   128681 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/api.html
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)    51323 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    63553 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/integrations.html
--rw-r--r--   0 runner    (1001) docker     (123)    35534 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-11 15:54:15.000000 pyngrok-5.2.2/_build/docs/html/sitemap-index.xml
--rw-r--r--   0 runner    (1001) docker     (123)    40994 2023-04-11 15:56:01.000000 pyngrok-5.2.2/_build/docs/html/troubleshooting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.438800 pyngrok-5.2.2/pyngrok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:54:15.000000 pyngrok-5.2.2/pyngrok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-11 15:54:15.000000 pyngrok-5.2.2/pyngrok/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-11 15:54:15.000000 pyngrok-5.2.2/pyngrok/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-11 15:54:15.000000 pyngrok-5.2.2/pyngrok/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-04-11 15:54:15.000000 pyngrok-5.2.2/pyngrok/ngrok.py
--rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-04-11 15:54:15.000000 pyngrok-5.2.2/pyngrok/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:56:04.438800 pyngrok-5.2.2/pyngrok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-04-11 15:56:04.000000 pyngrok-5.2.2/pyngrok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-11 15:56:04.000000 pyngrok-5.2.2/pyngrok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:56:04.000000 pyngrok-5.2.2/pyngrok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-11 15:56:04.000000 pyngrok-5.2.2/pyngrok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 15:56:04.000000 pyngrok-5.2.2/pyngrok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 15:56:04.000000 pyngrok-5.2.2/pyngrok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 15:56:04.442800 pyngrok-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-11 15:54:15.000000 pyngrok-5.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.810422 pyngrok-5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    24339 2023-04-12 13:50:16.000000 pyngrok-5.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 13:50:16.000000 pyngrok-5.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 13:50:16.000000 pyngrok-5.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-04-12 13:51:42.810422 pyngrok-5.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-12 13:50:16.000000 pyngrok-5.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.786422 pyngrok-5.2.3/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.790422 pyngrok-5.2.3/_build/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)    22933 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/coverage.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48___init___py.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32143 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_conf_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_exception_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)    88135 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_installer_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)   144682 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_ngrok_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127602 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_process_py.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/keybd_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/status.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-12 13:51:32.000000 pyngrok-5.2.3/_build/coverage/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.786422 pyngrok-5.2.3/_build/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.794422 pyngrok-5.2.3/_build/docs/doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)   278765 2023-04-12 13:51:40.000000 pyngrok-5.2.3/_build/docs/doctrees/api.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)  2672383 2023-04-12 13:51:40.000000 pyngrok-5.2.3/_build/docs/doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    75146 2023-04-12 13:51:40.000000 pyngrok-5.2.3/_build/docs/doctrees/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    53406 2023-04-12 13:51:40.000000 pyngrok-5.2.3/_build/docs/doctrees/integrations.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    32389 2023-04-12 13:51:40.000000 pyngrok-5.2.3/_build/docs/doctrees/troubleshooting.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.798422 pyngrok-5.2.3/_build/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.802422 pyngrok-5.2.3/_build/docs/html/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    35534 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/_images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.802422 pyngrok-5.2.3/_build/docs/html/_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_modules/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.802422 pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/
+-rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/conf.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/exception.html
+-rw-r--r--   0 runner    (1001) docker     (123)    50746 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/installer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77567 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/ngrok.html
+-rw-r--r--   0 runner    (1001) docker     (123)    69413 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/process.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.802422 pyngrok-5.2.3/_build/docs/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/_sources/api.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/_sources/integrations.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/_sources/troubleshooting.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.806422 pyngrok-5.2.3/_build/docs/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-12 13:51:38.000000 pyngrok-5.2.3/_build/docs/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 13:51:38.000000 pyngrok-5.2.3/_build/docs/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 13:51:38.000000 pyngrok-5.2.3/_build/docs/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 13:51:38.000000 pyngrok-5.2.3/_build/docs/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-04-12 13:51:38.000000 pyngrok-5.2.3/_build/docs/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-12 13:51:38.000000 pyngrok-5.2.3/_build/docs/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)   128681 2023-04-12 13:51:40.000000 pyngrok-5.2.3/_build/docs/html/api.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)    51587 2023-04-12 13:51:40.000000 pyngrok-5.2.3/_build/docs/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    63553 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/integrations.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35534 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 13:50:16.000000 pyngrok-5.2.3/_build/docs/html/sitemap-index.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    40994 2023-04-12 13:51:41.000000 pyngrok-5.2.3/_build/docs/html/troubleshooting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.810422 pyngrok-5.2.3/pyngrok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:16.000000 pyngrok-5.2.3/pyngrok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-12 13:50:16.000000 pyngrok-5.2.3/pyngrok/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-12 13:50:16.000000 pyngrok-5.2.3/pyngrok/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-12 13:50:16.000000 pyngrok-5.2.3/pyngrok/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20876 2023-04-12 13:50:16.000000 pyngrok-5.2.3/pyngrok/ngrok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-04-12 13:50:16.000000 pyngrok-5.2.3/pyngrok/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:51:42.810422 pyngrok-5.2.3/pyngrok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-04-12 13:51:42.000000 pyngrok-5.2.3/pyngrok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-12 13:51:42.000000 pyngrok-5.2.3/pyngrok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:51:42.000000 pyngrok-5.2.3/pyngrok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 13:51:42.000000 pyngrok-5.2.3/pyngrok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 13:51:42.000000 pyngrok-5.2.3/pyngrok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 13:51:42.000000 pyngrok-5.2.3/pyngrok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 13:51:42.810422 pyngrok-5.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-12 13:50:16.000000 pyngrok-5.2.3/setup.py
```

### Comparing `pyngrok-5.2.2/CHANGELOG.md` & `pyngrok-5.2.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased](https://github.com/alexdlaird/pyngrok/compare/5.2.2...HEAD)
+## [Unreleased](https://github.com/alexdlaird/pyngrok/compare/5.2.3...HEAD)
+
+## [5.2.3](https://github.com/alexdlaird/pyngrok/compare/5.2.2...5.2.3) - 2023-04-12
+### Added
+- Support for `basic_auth` parameter in `ngrok` v3.
+- Documentation improvements.
+- Test improvements.
 
 ## [5.2.2](https://github.com/alexdlaird/pyngrok/compare/5.2.1...5.2.2) - 2023-04-11
 ### Fixed
 - Documentation improvements.
 - Test improvements.
 
 ## [5.2.1](https://github.com/alexdlaird/pyngrok/compare/5.2.0...5.2.1) - 2022-11-29
```

### Comparing `pyngrok-5.2.2/LICENSE` & `pyngrok-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/PKG-INFO` & `pyngrok-5.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyngrok
-Version: 5.2.2
+Version: 5.2.3
 Summary: A Python wrapper for ngrok.
 Home-page: https://github.com/alexdlaird/pyngrok
-Download-URL: https://github.com/alexdlaird/pyngrok/archive/5.2.2.tar.gz
+Download-URL: https://github.com/alexdlaird/pyngrok/archive/5.2.3.tar.gz
 Author: Alex Laird
 Author-email: contact@alexlaird.com
 License: MIT
 Project-URL: Documentation, https://pyngrok.readthedocs.io
 Project-URL: Changelog, https://github.com/alexdlaird/pyngrok/blob/main/CHANGELOG.md
 Project-URL: Sponsor, https://www.paypal.me/alexdlaird
 Keywords: ngrok,tunnel,tunneling,webhook,localhost,reverse-proxy,localtunnel
```

### Comparing `pyngrok-5.2.2/README.md` & `pyngrok-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/coverage/coverage.xml` & `pyngrok-5.2.3/_build/coverage/coverage.xml`

 * *Files 1% similar despite different names*

#### Comparing `pyngrok-5.2.2/_build/coverage/coverage.xml` & `pyngrok-5.2.3/_build/coverage/coverage.xml`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.3" timestamp="1681228550317" lines-valid="592" lines-covered="553" line-rate="0.9341" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
+<coverage version="7.2.3" timestamp="1681307492212" lines-valid="599" lines-covered="559" line-rate="0.9332" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.3 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/pyngrok/pyngrok</source>
   </sources>
   <packages>
-    <package name="pyngrok" line-rate="0.9341" branch-rate="0" complexity="0">
+    <package name="pyngrok" line-rate="0.9332" branch-rate="0" complexity="0">
       <classes>
         <class name="__init__.py" filename="pyngrok/__init__.py" complexity="0" line-rate="1" branch-rate="0">
           <methods/>
           <lines/>
         </class>
         <class name="conf.py" filename="pyngrok/conf.py" complexity="0" line-rate="0.9655" branch-rate="0">
           <methods/>
@@ -226,15 +226,15 @@
             <line number="309" hits="1"/>
             <line number="312" hits="1"/>
             <line number="313" hits="1"/>
             <line number="314" hits="1"/>
             <line number="315" hits="1"/>
           </lines>
         </class>
-        <class name="ngrok.py" filename="pyngrok/ngrok.py" complexity="0" line-rate="0.8778" branch-rate="0">
+        <class name="ngrok.py" filename="pyngrok/ngrok.py" complexity="0" line-rate="0.877" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
             <line number="3" hits="1"/>
             <line number="4" hits="1"/>
             <line number="5" hits="1"/>
@@ -317,106 +317,113 @@
             <line number="243" hits="1"/>
             <line number="245" hits="1"/>
             <line number="247" hits="1"/>
             <line number="249" hits="1"/>
             <line number="254" hits="1"/>
             <line number="257" hits="1"/>
             <line number="258" hits="1"/>
-            <line number="259" hits="0"/>
-            <line number="260" hits="1"/>
-            <line number="261" hits="0"/>
-            <line number="263" hits="1"/>
-            <line number="265" hits="1"/>
-            <line number="267" hits="1"/>
+            <line number="259" hits="1"/>
+            <line number="260" hits="0"/>
+            <line number="261" hits="1"/>
+            <line number="262" hits="0"/>
+            <line number="264" hits="1"/>
+            <line number="266" hits="1"/>
+            <line number="268" hits="1"/>
             <line number="269" hits="1"/>
-            <line number="271" hits="1"/>
+            <line number="270" hits="1"/>
+            <line number="271" hits="0"/>
+            <line number="273" hits="1"/>
             <line number="275" hits="1"/>
-            <line number="276" hits="1"/>
-            <line number="280" hits="1"/>
-            <line number="282" hits="1"/>
+            <line number="277" hits="1"/>
+            <line number="279" hits="1"/>
+            <line number="281" hits="1"/>
             <line number="285" hits="1"/>
+            <line number="286" hits="1"/>
+            <line number="290" hits="1"/>
+            <line number="292" hits="1"/>
             <line number="295" hits="1"/>
-            <line number="296" hits="0"/>
-            <line number="299" hits="1"/>
-            <line number="300" hits="0"/>
-            <line number="302" hits="1"/>
-            <line number="304" hits="1"/>
-            <line number="305" hits="0"/>
-            <line number="308" hits="0"/>
-            <line number="309" hits="0"/>
-            <line number="311" hits="1"/>
-            <line number="313" hits="1"/>
-            <line number="315" hits="1"/>
-            <line number="318" hits="1"/>
+            <line number="305" hits="1"/>
+            <line number="306" hits="0"/>
+            <line number="309" hits="1"/>
+            <line number="310" hits="0"/>
+            <line number="312" hits="1"/>
+            <line number="314" hits="1"/>
+            <line number="315" hits="0"/>
+            <line number="318" hits="0"/>
+            <line number="319" hits="0"/>
             <line number="321" hits="1"/>
-            <line number="337" hits="1"/>
-            <line number="338" hits="0"/>
-            <line number="340" hits="1"/>
-            <line number="342" hits="1"/>
-            <line number="343" hits="1"/>
-            <line number="345" hits="1"/>
-            <line number="346" hits="1"/>
-            <line number="348" hits="1"/>
-            <line number="351" hits="1"/>
-            <line number="360" hits="1"/>
-            <line number="361" hits="0"/>
-            <line number="363" hits="1"/>
-            <line number="365" hits="1"/>
-            <line number="368" hits="1"/>
+            <line number="323" hits="1"/>
+            <line number="325" hits="1"/>
+            <line number="328" hits="1"/>
+            <line number="331" hits="1"/>
+            <line number="347" hits="1"/>
+            <line number="348" hits="0"/>
+            <line number="350" hits="1"/>
+            <line number="352" hits="1"/>
+            <line number="353" hits="1"/>
+            <line number="355" hits="1"/>
+            <line number="356" hits="1"/>
+            <line number="358" hits="1"/>
+            <line number="361" hits="1"/>
+            <line number="370" hits="1"/>
+            <line number="371" hits="0"/>
+            <line number="373" hits="1"/>
+            <line number="375" hits="1"/>
             <line number="378" hits="1"/>
-            <line number="379" hits="0"/>
-            <line number="381" hits="1"/>
-            <line number="383" hits="1"/>
-            <line number="386" hits="1"/>
+            <line number="388" hits="1"/>
+            <line number="389" hits="0"/>
+            <line number="391" hits="1"/>
+            <line number="393" hits="1"/>
             <line number="396" hits="1"/>
-            <line number="397" hits="0"/>
-            <line number="399" hits="1"/>
-            <line number="402" hits="1"/>
-            <line number="439" hits="1"/>
-            <line number="440" hits="1"/>
-            <line number="442" hits="1"/>
-            <line number="443" hits="1"/>
-            <line number="445" hits="1"/>
-            <line number="447" hits="1"/>
-            <line number="448" hits="1"/>
+            <line number="406" hits="1"/>
+            <line number="407" hits="0"/>
+            <line number="409" hits="1"/>
+            <line number="412" hits="1"/>
+            <line number="449" hits="1"/>
             <line number="450" hits="1"/>
-            <line number="451" hits="1"/>
+            <line number="452" hits="1"/>
             <line number="453" hits="1"/>
             <line number="455" hits="1"/>
-            <line number="456" hits="1"/>
             <line number="457" hits="1"/>
-            <line number="459" hits="1"/>
+            <line number="458" hits="1"/>
             <line number="460" hits="1"/>
-            <line number="462" hits="1"/>
-            <line number="463" hits="0"/>
+            <line number="461" hits="1"/>
+            <line number="463" hits="1"/>
             <line number="465" hits="1"/>
             <line number="466" hits="1"/>
-            <line number="468" hits="1"/>
+            <line number="467" hits="1"/>
             <line number="469" hits="1"/>
             <line number="470" hits="1"/>
-            <line number="471" hits="1"/>
             <line number="472" hits="1"/>
-            <line number="474" hits="1"/>
+            <line number="473" hits="0"/>
             <line number="475" hits="1"/>
-            <line number="477" hits="1"/>
-            <line number="480" hits="0"/>
-            <line number="481" hits="0"/>
+            <line number="476" hits="1"/>
+            <line number="478" hits="1"/>
+            <line number="479" hits="1"/>
+            <line number="480" hits="1"/>
+            <line number="481" hits="1"/>
+            <line number="482" hits="1"/>
             <line number="484" hits="1"/>
-            <line number="498" hits="1"/>
-            <line number="499" hits="1"/>
-            <line number="500" hits="1"/>
-            <line number="501" hits="1"/>
-            <line number="503" hits="1"/>
-            <line number="505" hits="1"/>
+            <line number="485" hits="1"/>
+            <line number="487" hits="1"/>
+            <line number="490" hits="0"/>
+            <line number="491" hits="0"/>
+            <line number="494" hits="1"/>
             <line number="508" hits="1"/>
-            <line number="517" hits="1"/>
-            <line number="519" hits="1"/>
-            <line number="520" hits="0"/>
-            <line number="521" hits="1"/>
-            <line number="522" hits="0"/>
+            <line number="509" hits="1"/>
+            <line number="510" hits="1"/>
+            <line number="511" hits="1"/>
+            <line number="513" hits="1"/>
+            <line number="515" hits="1"/>
+            <line number="518" hits="1"/>
+            <line number="527" hits="1"/>
+            <line number="529" hits="1"/>
+            <line number="530" hits="0"/>
+            <line number="531" hits="1"/>
+            <line number="532" hits="0"/>
           </lines>
         </class>
         <class name="process.py" filename="pyngrok/process.py" complexity="0" line-rate="0.9617" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
```

### Comparing `pyngrok-5.2.2/_build/coverage/coverage_html.js` & `pyngrok-5.2.3/_build/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48___init___py.html` & `pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_conf_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_conf_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,12 +7,12 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 0 statements   0 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
```

### Comparing `pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_conf_py.html` & `pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_conf_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_exception_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -204,13 +204,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_exception_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 29 statements   28 run 1 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
 
 
 1import os 
 2 
 3from pyngrok.installer import get_ngrok_bin 
 4 
 5__author__ = "Alex Laird" 
@@ -151,8 +151,8 @@
 115 :type pyngrok_config: PyngrokConfig 
 116 """ 
 117 global _default_pyngrok_config 
 118 
 119 _default_pyngrok_config = pyngrok_config 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
```

### Comparing `pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_exception_py.html` & `pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_exception_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_conf_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_installer_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -176,13 +176,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_conf_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_installer_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 28 statements   28 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
 
 
 1__author__ = "Alex Laird" 
 2__copyright__ = "Copyright 2023, Alex Laird" 
 3__version__ = "5.2.2" 
 4 
 5 
@@ -106,8 +106,8 @@
 87 
 88 def __init__(self, error, reason): 
 89 super(PyngrokNgrokURLError, self).__init__(error) 
 90 
 91 self.reason = reason 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
```

### Comparing `pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_installer_py.html` & `pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_installer_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_exception_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_ngrok_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -400,13 +400,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_exception_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_ngrok_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 146 statements   138 run 8 missing 4 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
 
 
 1import copy 
 2import logging 
 3import os 
 4import platform 
 5import socket 
@@ -349,8 +349,8 @@
 311 
 312def _clear_progress(spaces=100): 
 313 if _print_progress_enabled: 
 314 sys.stdout.write((" " * spaces) + "\r") 
 315 sys.stdout.flush() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
```

### Comparing `pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_ngrok_py.html` & `pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_ngrok_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for pyngrok/ngrok.py: 87.78%</title>
+    <title>Coverage for pyngrok/ngrok.py: 87.70%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>pyngrok/ngrok.py</b>:
-            <span class="pc_cov">87.78%</span>
+            <span class="pc_cov">87.70%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">180 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">158<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">22<span class="text"> missing</span></button>
+            <span class="text">187 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">164<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">23<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">6<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_installer_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_process_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -92,15 +92,15 @@
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">urllib</span><span class="op">.</span><span class="nam">request</span> <span class="key">import</span> <span class="nam">urlopen</span><span class="op">,</span> <span class="nam">Request</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">pyngrok</span> <span class="key">import</span> <span class="nam">process</span><span class="op">,</span> <span class="nam">conf</span><span class="op">,</span> <span class="nam">installer</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">pyngrok</span><span class="op">.</span><span class="nam">exception</span> <span class="key">import</span> <span class="nam">PyngrokNgrokHTTPError</span><span class="op">,</span> <span class="nam">PyngrokNgrokURLError</span><span class="op">,</span> <span class="nam">PyngrokSecurityError</span><span class="op">,</span> <span class="nam">PyngrokError</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">__author__</span> <span class="op">=</span> <span class="str">"Alex Laird"</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">__copyright__</span> <span class="op">=</span> <span class="str">"Copyright 2023, Alex Laird"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"5.2.2"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"5.2.3"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">from</span> <span class="nam">pyngrok</span><span class="op">.</span><span class="nam">installer</span> <span class="key">import</span> <span class="nam">get_default_config</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="nam">logger</span> <span class="op">=</span> <span class="nam">logging</span><span class="op">.</span><span class="nam">getLogger</span><span class="op">(</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="nam">_current_tunnels</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -332,292 +332,302 @@
     <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">        <span class="str">"name"</span><span class="op">:</span> <span class="nam">name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="str">"addr"</span><span class="op">:</span> <span class="nam">addr</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="str">"proto"</span><span class="op">:</span> <span class="nam">proto</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">    <span class="nam">options</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">config</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="com"># Upgrade legacy parameters, if present</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_version</span> <span class="op">==</span> <span class="str">"v3"</span> <span class="key">and</span> <span class="str">"bind_tls"</span> <span class="key">in</span> <span class="nam">options</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span> <span class="key">or</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"true"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="nam">options</span><span class="op">[</span><span class="str">"schemes"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="str">"https"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="key">elif</span> <span class="key">not</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">False</span> <span class="key">or</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"false"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="nam">options</span><span class="op">[</span><span class="str">"schemes"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="str">"http"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">            <span class="nam">options</span><span class="op">[</span><span class="str">"schemes"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="str">"http"</span><span class="op">,</span> <span class="str">"https"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">        <span class="nam">options</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="nam">api_url</span> <span class="op">=</span> <span class="nam">get_ngrok_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span><span class="op">.</span><span class="nam">api_url</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Creating tunnel with options: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">options</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">    <span class="nam">tunnel</span> <span class="op">=</span> <span class="nam">NgrokTunnel</span><span class="op">(</span><span class="nam">api_request</span><span class="op">(</span><span class="str">"{}/api/tunnels"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"POST"</span><span class="op">,</span> <span class="nam">data</span><span class="op">=</span><span class="nam">options</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">                                     <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                         <span class="nam">pyngrok_config</span><span class="op">,</span> <span class="nam">api_url</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_version</span> <span class="op">==</span> <span class="str">"v3"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">        <span class="key">if</span> <span class="str">"bind_tls"</span> <span class="key">in</span> <span class="nam">options</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">            <span class="key">if</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="key">is</span> <span class="key">True</span> <span class="key">or</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"true"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                <span class="nam">options</span><span class="op">[</span><span class="str">"schemes"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="str">"https"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="key">elif</span> <span class="key">not</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="key">is</span> <span class="key">not</span> <span class="key">False</span> <span class="key">or</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"false"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                <span class="nam">options</span><span class="op">[</span><span class="str">"schemes"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="str">"http"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">                <span class="nam">options</span><span class="op">[</span><span class="str">"schemes"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="str">"http"</span><span class="op">,</span> <span class="str">"https"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="key">if</span> <span class="str">"auth"</span> <span class="key">in</span> <span class="nam">options</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">            <span class="nam">auth</span> <span class="op">=</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"auth"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">auth</span><span class="op">,</span> <span class="nam">list</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">                <span class="nam">options</span><span class="op">[</span><span class="str">"basic_auth"</span><span class="op">]</span> <span class="op">=</span> <span class="nam">auth</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">                <span class="nam">options</span><span class="op">[</span><span class="str">"basic_auth"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span><span class="nam">auth</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_version</span> <span class="op">==</span> <span class="str">"v2"</span> <span class="key">and</span> <span class="nam">proto</span> <span class="op">==</span> <span class="str">"http"</span> <span class="key">and</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">,</span> <span class="str">"both"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"both"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="nam">tunnel</span> <span class="op">=</span> <span class="nam">NgrokTunnel</span><span class="op">(</span><span class="nam">api_request</span><span class="op">(</span><span class="str">"{}{}%20%28http%29"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">,</span> <span class="nam">tunnel</span><span class="op">.</span><span class="nam">uri</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"GET"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">                                         <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">                             <span class="nam">pyngrok_config</span><span class="op">,</span> <span class="nam">api_url</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">[</span><span class="nam">tunnel</span><span class="op">.</span><span class="nam">public_url</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tunnel</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">    <span class="key">return</span> <span class="nam">tunnel</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">            <span class="nam">options</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"auth"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="nam">api_url</span> <span class="op">=</span> <span class="nam">get_ngrok_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span><span class="op">.</span><span class="nam">api_url</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Creating tunnel with options: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">options</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">    <span class="nam">tunnel</span> <span class="op">=</span> <span class="nam">NgrokTunnel</span><span class="op">(</span><span class="nam">api_request</span><span class="op">(</span><span class="str">"{}/api/tunnels"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"POST"</span><span class="op">,</span> <span class="nam">data</span><span class="op">=</span><span class="nam">options</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">                                     <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">                         <span class="nam">pyngrok_config</span><span class="op">,</span> <span class="nam">api_url</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t"><span class="key">def</span> <span class="nam">disconnect</span><span class="op">(</span><span class="nam">public_url</span><span class="op">,</span> <span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t"><span class="str">    Disconnect the ``ngrok`` tunnel for the given URL, if open.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t"><span class="str">    :param public_url: The public URL of the tunnel to disconnect.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t"><span class="str">    :type public_url: str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">    <span class="com"># If ngrok is not running, there are no tunnels to disconnect</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">process</span><span class="op">.</span><span class="nam">is_process_running</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">    <span class="nam">api_url</span> <span class="op">=</span> <span class="nam">get_ngrok_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span><span class="op">.</span><span class="nam">api_url</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">    <span class="key">if</span> <span class="nam">public_url</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_current_tunnels</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">        <span class="nam">get_tunnels</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="com"># One more check, if the given URL is still not in the list of tunnels, it is not active</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">        <span class="key">if</span> <span class="nam">public_url</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_current_tunnels</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">    <span class="nam">tunnel</span> <span class="op">=</span> <span class="nam">_current_tunnels</span><span class="op">[</span><span class="nam">public_url</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Disconnecting tunnel: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">tunnel</span><span class="op">.</span><span class="nam">public_url</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">    <span class="nam">api_request</span><span class="op">(</span><span class="str">"{}{}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">,</span> <span class="nam">tunnel</span><span class="op">.</span><span class="nam">uri</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"DELETE"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">                <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="nam">public_url</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_version</span> <span class="op">==</span> <span class="str">"v2"</span> <span class="key">and</span> <span class="nam">proto</span> <span class="op">==</span> <span class="str">"http"</span> <span class="key">and</span> <span class="nam">options</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"bind_tls"</span><span class="op">,</span> <span class="str">"both"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"both"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">        <span class="nam">tunnel</span> <span class="op">=</span> <span class="nam">NgrokTunnel</span><span class="op">(</span><span class="nam">api_request</span><span class="op">(</span><span class="str">"{}{}%20%28http%29"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">,</span> <span class="nam">tunnel</span><span class="op">.</span><span class="nam">uri</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"GET"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">                                         <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">                             <span class="nam">pyngrok_config</span><span class="op">,</span> <span class="nam">api_url</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">[</span><span class="nam">tunnel</span><span class="op">.</span><span class="nam">public_url</span><span class="op">]</span> <span class="op">=</span> <span class="nam">tunnel</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">    <span class="key">return</span> <span class="nam">tunnel</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t"><span class="key">def</span> <span class="nam">disconnect</span><span class="op">(</span><span class="nam">public_url</span><span class="op">,</span> <span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t"><span class="str">    Disconnect the ``ngrok`` tunnel for the given URL, if open.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t"><span class="str">    :param public_url: The public URL of the tunnel to disconnect.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t"><span class="str">    :type public_url: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">    <span class="com"># If ngrok is not running, there are no tunnels to disconnect</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">process</span><span class="op">.</span><span class="nam">is_process_running</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">        <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">    <span class="nam">api_url</span> <span class="op">=</span> <span class="nam">get_ngrok_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span><span class="op">.</span><span class="nam">api_url</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">    <span class="key">if</span> <span class="nam">public_url</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_current_tunnels</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="nam">get_tunnels</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">        <span class="com"># One more check, if the given URL is still not in the list of tunnels, it is not active</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">        <span class="key">if</span> <span class="nam">public_url</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_current_tunnels</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="key">def</span> <span class="nam">get_tunnels</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="str">    Get a list of active ``ngrok`` tunnels for the given config's ``ngrok_path``.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">    <span class="nam">tunnel</span> <span class="op">=</span> <span class="nam">_current_tunnels</span><span class="op">[</span><span class="nam">public_url</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">    <span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Disconnecting tunnel: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">tunnel</span><span class="op">.</span><span class="nam">public_url</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="str">    If ``ngrok`` is not installed at :class:`~pyngrok.conf.PyngrokConfig`'s ``ngrok_path``, calling this method</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">    will first download and install ``ngrok``.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">    <span class="nam">api_request</span><span class="op">(</span><span class="str">"{}{}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">,</span> <span class="nam">tunnel</span><span class="op">.</span><span class="nam">uri</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"DELETE"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">                <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">    If ``ngrok`` is not running, calling this method will first start a process with</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t"><span class="str">    :class:`~pyngrok.conf.PyngrokConfig`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="nam">public_url</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="str">    :return: The active ``ngrok`` tunnels.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t"><span class="str">    :rtype: list[NgrokTunnel]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">    <span class="nam">api_url</span> <span class="op">=</span> <span class="nam">get_ngrok_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span><span class="op">.</span><span class="nam">api_url</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">    <span class="key">for</span> <span class="nam">tunnel</span> <span class="key">in</span> <span class="nam">api_request</span><span class="op">(</span><span class="str">"{}/api/tunnels"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"GET"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">                              <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span><span class="op">[</span><span class="str">"tunnels"</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">        <span class="nam">ngrok_tunnel</span> <span class="op">=</span> <span class="nam">NgrokTunnel</span><span class="op">(</span><span class="nam">tunnel</span><span class="op">,</span> <span class="nam">pyngrok_config</span><span class="op">,</span> <span class="nam">api_url</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">        <span class="nam">_current_tunnels</span><span class="op">[</span><span class="nam">ngrok_tunnel</span><span class="op">.</span><span class="nam">public_url</span><span class="op">]</span> <span class="op">=</span> <span class="nam">ngrok_tunnel</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="key">return</span> <span class="nam">list</span><span class="op">(</span><span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t"><span class="key">def</span> <span class="nam">get_tunnels</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t"><span class="str">    Get a list of active ``ngrok`` tunnels for the given config's ``ngrok_path``.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t"><span class="str">    If ``ngrok`` is not installed at :class:`~pyngrok.conf.PyngrokConfig`'s ``ngrok_path``, calling this method</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t"><span class="str">    will first download and install ``ngrok``.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="str">    If ``ngrok`` is not running, calling this method will first start a process with</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t"><span class="str">    :class:`~pyngrok.conf.PyngrokConfig`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t"><span class="str">    :return: The active ``ngrok`` tunnels.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">    :rtype: list[NgrokTunnel]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="key">def</span> <span class="nam">kill</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t"><span class="str">    Terminate the ``ngrok`` processes, if running, for the given config's ``ngrok_path``. This method will not</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">    block, it will just issue a kill request.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">    <span class="nam">process</span><span class="op">.</span><span class="nam">kill_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t"><span class="key">def</span> <span class="nam">get_version</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t"><span class="str">    Get a tuple with the ``ngrok`` and ``pyngrok`` versions.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t"><span class="str">    :return: A tuple of ``(ngrok_version, pyngrok_version)``.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t"><span class="str">    :rtype: tuple</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">    <span class="nam">ngrok_version</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">capture_run_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">,</span> <span class="op">[</span><span class="str">"--version"</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"version "</span><span class="op">)</span><span class="op">[</span><span class="num">1</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">    <span class="key">return</span> <span class="nam">ngrok_version</span><span class="op">,</span> <span class="nam">__version__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t"><span class="str">    Update ``ngrok`` for the given config's ``ngrok_path``, if an update is available.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t"><span class="str">    :return: The result from the ``ngrok`` update.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t"><span class="str">    :rtype: str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">    <span class="key">return</span> <span class="nam">process</span><span class="op">.</span><span class="nam">capture_run_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">,</span> <span class="op">[</span><span class="str">"update"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t"><span class="key">def</span> <span class="nam">api_request</span><span class="op">(</span><span class="nam">url</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"GET"</span><span class="op">,</span> <span class="nam">data</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">params</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="num">4</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t"><span class="str">    Invoke an API request to the given URL, returning JSON data from the response.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t"><span class="str">    One use for this method is making requests to ``ngrok`` tunnels:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t"><span class="str">    .. code-block:: python</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t"><span class="str">        from pyngrok import ngrok</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">    <span class="nam">api_url</span> <span class="op">=</span> <span class="nam">get_ngrok_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span><span class="op">.</span><span class="nam">api_url</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="key">for</span> <span class="nam">tunnel</span> <span class="key">in</span> <span class="nam">api_request</span><span class="op">(</span><span class="str">"{}/api/tunnels"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">api_url</span><span class="op">)</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"GET"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">                              <span class="nam">timeout</span><span class="op">=</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">request_timeout</span><span class="op">)</span><span class="op">[</span><span class="str">"tunnels"</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">        <span class="nam">ngrok_tunnel</span> <span class="op">=</span> <span class="nam">NgrokTunnel</span><span class="op">(</span><span class="nam">tunnel</span><span class="op">,</span> <span class="nam">pyngrok_config</span><span class="op">,</span> <span class="nam">api_url</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">        <span class="nam">_current_tunnels</span><span class="op">[</span><span class="nam">ngrok_tunnel</span><span class="op">.</span><span class="nam">public_url</span><span class="op">]</span> <span class="op">=</span> <span class="nam">ngrok_tunnel</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">    <span class="key">return</span> <span class="nam">list</span><span class="op">(</span><span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="key">def</span> <span class="nam">kill</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">    Terminate the ``ngrok`` processes, if running, for the given config's ``ngrok_path``. This method will not</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t"><span class="str">    block, it will just issue a kill request.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="nam">process</span><span class="op">.</span><span class="nam">kill_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="nam">_current_tunnels</span><span class="op">.</span><span class="nam">clear</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t"><span class="key">def</span> <span class="nam">get_version</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t"><span class="str">    Get a tuple with the ``ngrok`` and ``pyngrok`` versions.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="str">    :return: A tuple of ``(ngrok_version, pyngrok_version)``.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="str">    :rtype: tuple</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">    <span class="nam">ngrok_version</span> <span class="op">=</span> <span class="nam">process</span><span class="op">.</span><span class="nam">capture_run_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">,</span> <span class="op">[</span><span class="str">"--version"</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">split</span><span class="op">(</span><span class="str">"version "</span><span class="op">)</span><span class="op">[</span><span class="num">1</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">    <span class="key">return</span> <span class="nam">ngrok_version</span><span class="op">,</span> <span class="nam">__version__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t"><span class="key">def</span> <span class="nam">update</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t"><span class="str">    Update ``ngrok`` for the given config's ``ngrok_path``, if an update is available.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t"><span class="str">    :return: The result from the ``ngrok`` update.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t"><span class="str">    :rtype: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="key">return</span> <span class="nam">process</span><span class="op">.</span><span class="nam">capture_run_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">,</span> <span class="op">[</span><span class="str">"update"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t"><span class="str">        public_url = ngrok.connect()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t"><span class="str">        response = ngrok.api_request("{}/some-route".format(public_url),</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t"><span class="str">                                     method="POST", data={"foo": "bar"})</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t"><span class="key">def</span> <span class="nam">api_request</span><span class="op">(</span><span class="nam">url</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="str">"GET"</span><span class="op">,</span> <span class="nam">data</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">params</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">=</span><span class="num">4</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t"><span class="str">    Invoke an API request to the given URL, returning JSON data from the response.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t"><span class="str">    Another is making requests to the ``ngrok`` API itself:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t"><span class="str">    One use for this method is making requests to ``ngrok`` tunnels:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t"><span class="str">    .. code-block:: python</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t"><span class="str">        from pyngrok import ngrok</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t"><span class="str">        api_url = ngrok.get_ngrok_process().api_url</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t"><span class="str">        response = ngrok.api_request("{}/api/requests/http".format(api_url),</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t"><span class="str">                                     params={"tunnel_name": "foo"})</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t"><span class="str">        public_url = ngrok.connect()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t"><span class="str">        response = ngrok.api_request("{}/some-route".format(public_url),</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t"><span class="str">                                     method="POST", data={"foo": "bar"})</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t"><span class="str">    :param url: The request URL.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t"><span class="str">    :type url: str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t"><span class="str">    :param method: The HTTP method.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t"><span class="str">    :type method: str, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="str">    :param data: The request body.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t"><span class="str">    :type data: dict, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="str">    :param params: The URL parameters.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t"><span class="str">    :type params: dict, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">    :param timeout: The request timeout, in seconds.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t"><span class="str">    :type timeout: float, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t"><span class="str">    :return: The response from the request.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="str">    :rtype: dict</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">    <span class="key">if</span> <span class="nam">params</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">        <span class="nam">params</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">url</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"http"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokSecurityError</span><span class="op">(</span><span class="str">"URL must start with \"http\": {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">url</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">if</span> <span class="nam">data</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">    <span class="key">if</span> <span class="nam">params</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">        <span class="nam">url</span> <span class="op">+=</span> <span class="str">"?{}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">urlencode</span><span class="op">(</span><span class="op">[</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">params</span><span class="op">[</span><span class="nam">x</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">params</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">    <span class="nam">request</span> <span class="op">=</span> <span class="nam">Request</span><span class="op">(</span><span class="nam">url</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="nam">method</span><span class="op">.</span><span class="nam">upper</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">    <span class="nam">request</span><span class="op">.</span><span class="nam">add_header</span><span class="op">(</span><span class="str">"Content-Type"</span><span class="op">,</span> <span class="str">"application/json"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">    <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Making {} request to {} with data: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">method</span><span class="op">,</span> <span class="nam">url</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t"><span class="str">    Another is making requests to the ``ngrok`` API itself:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t"><span class="str">    .. code-block:: python</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="str">        from pyngrok import ngrok</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="str">        api_url = ngrok.get_ngrok_process().api_url</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t"><span class="str">        response = ngrok.api_request("{}/api/requests/http".format(api_url),</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">                                     params={"tunnel_name": "foo"})</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t"><span class="str">    :param url: The request URL.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="str">    :type url: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t"><span class="str">    :param method: The HTTP method.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t"><span class="str">    :type method: str, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="str">    :param data: The request body.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t"><span class="str">    :type data: dict, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t"><span class="str">    :param params: The URL parameters.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t"><span class="str">    :type params: dict, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t"><span class="str">    :param timeout: The request timeout, in seconds.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t"><span class="str">    :type timeout: float, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t"><span class="str">    :return: The response from the request.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t"><span class="str">    :rtype: dict</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">    <span class="key">if</span> <span class="nam">params</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">        <span class="nam">params</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">    <span class="key">if</span> <span class="key">not</span> <span class="nam">url</span><span class="op">.</span><span class="nam">lower</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"http"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokSecurityError</span><span class="op">(</span><span class="str">"URL must start with \"http\": {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">url</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="nam">urlopen</span><span class="op">(</span><span class="nam">request</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">        <span class="nam">response_data</span> <span class="op">=</span> <span class="nam">response</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="str">"utf-8"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">        <span class="nam">status_code</span> <span class="op">=</span> <span class="nam">response</span><span class="op">.</span><span class="nam">getcode</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">        <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Response {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">        <span class="key">if</span> <span class="nam">str</span><span class="op">(</span><span class="nam">status_code</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"2"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">            <span class="key">raise</span> <span class="nam">PyngrokNgrokHTTPError</span><span class="op">(</span><span class="str">"ngrok client API returned {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span><span class="op">,</span> <span class="nam">url</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">                                        <span class="nam">status_code</span><span class="op">,</span> <span class="key">None</span><span class="op">,</span> <span class="nam">request</span><span class="op">.</span><span class="nam">headers</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">        <span class="key">elif</span> <span class="nam">status_code</span> <span class="op">==</span> <span class="nam">HTTPStatus</span><span class="op">.</span><span class="nam">NO_CONTENT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">        <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">response_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">    <span class="key">except</span> <span class="nam">socket</span><span class="op">.</span><span class="nam">timeout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokNgrokURLError</span><span class="op">(</span><span class="str">"ngrok client exception, URLError: timed out"</span><span class="op">,</span> <span class="str">"timed out"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">    <span class="key">except</span> <span class="nam">HTTPError</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t">        <span class="nam">response_data</span> <span class="op">=</span> <span class="nam">e</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="str">"utf-8"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t">        <span class="nam">status_code</span> <span class="op">=</span> <span class="nam">e</span><span class="op">.</span><span class="nam">getcode</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t">        <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Response {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokNgrokHTTPError</span><span class="op">(</span><span class="str">"ngrok client exception, API returned {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t">                                    <span class="nam">e</span><span class="op">.</span><span class="nam">url</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t">                                    <span class="nam">status_code</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">msg</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">hdrs</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t">    <span class="key">except</span> <span class="nam">URLError</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokNgrokURLError</span><span class="op">(</span><span class="str">"ngrok client exception, URLError: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">e</span><span class="op">.</span><span class="nam">reason</span><span class="op">)</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">reason</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">    <span class="nam">data</span> <span class="op">=</span> <span class="nam">json</span><span class="op">.</span><span class="nam">dumps</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="str">"utf-8"</span><span class="op">)</span> <span class="key">if</span> <span class="nam">data</span> <span class="key">else</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">    <span class="key">if</span> <span class="nam">params</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">        <span class="nam">url</span> <span class="op">+=</span> <span class="str">"?{}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">urlencode</span><span class="op">(</span><span class="op">[</span><span class="op">(</span><span class="nam">x</span><span class="op">,</span> <span class="nam">params</span><span class="op">[</span><span class="nam">x</span><span class="op">]</span><span class="op">)</span> <span class="key">for</span> <span class="nam">x</span> <span class="key">in</span> <span class="nam">params</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">    <span class="nam">request</span> <span class="op">=</span> <span class="nam">Request</span><span class="op">(</span><span class="nam">url</span><span class="op">,</span> <span class="nam">method</span><span class="op">=</span><span class="nam">method</span><span class="op">.</span><span class="nam">upper</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">    <span class="nam">request</span><span class="op">.</span><span class="nam">add_header</span><span class="op">(</span><span class="str">"Content-Type"</span><span class="op">,</span> <span class="str">"application/json"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">    <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Making {} request to {} with data: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">method</span><span class="op">,</span> <span class="nam">url</span><span class="op">,</span> <span class="nam">data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="nam">urlopen</span><span class="op">(</span><span class="nam">request</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">timeout</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">        <span class="nam">response_data</span> <span class="op">=</span> <span class="nam">response</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="str">"utf-8"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">        <span class="nam">status_code</span> <span class="op">=</span> <span class="nam">response</span><span class="op">.</span><span class="nam">getcode</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">        <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Response {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t">        <span class="key">if</span> <span class="nam">str</span><span class="op">(</span><span class="nam">status_code</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"2"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t">            <span class="key">raise</span> <span class="nam">PyngrokNgrokHTTPError</span><span class="op">(</span><span class="str">"ngrok client API returned {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span><span class="op">,</span> <span class="nam">url</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t">                                        <span class="nam">status_code</span><span class="op">,</span> <span class="key">None</span><span class="op">,</span> <span class="nam">request</span><span class="op">.</span><span class="nam">headers</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t">        <span class="key">elif</span> <span class="nam">status_code</span> <span class="op">==</span> <span class="nam">HTTPStatus</span><span class="op">.</span><span class="nam">NO_CONTENT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t">        <span class="key">return</span> <span class="nam">json</span><span class="op">.</span><span class="nam">loads</span><span class="op">(</span><span class="nam">response_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t">    <span class="key">except</span> <span class="nam">socket</span><span class="op">.</span><span class="nam">timeout</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokNgrokURLError</span><span class="op">(</span><span class="str">"ngrok client exception, URLError: timed out"</span><span class="op">,</span> <span class="str">"timed out"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t">    <span class="key">except</span> <span class="nam">HTTPError</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t">        <span class="nam">response_data</span> <span class="op">=</span> <span class="nam">e</span><span class="op">.</span><span class="nam">read</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="str">"utf-8"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t"><span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">args</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t"><span class="str">    Ensure ``ngrok`` is installed at the default path, then call :func:`~pyngrok.process.run_process`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t"><span class="str">    This method is meant for interacting with ``ngrok`` from the command line and is not necessarily</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t489" href="#t489">489</a></span><span class="t"><span class="str">    compatible with non-blocking API methods. For that, use :mod:`~pyngrok.ngrok`'s interface methods (like</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t490" href="#t490">490</a></span><span class="t"><span class="str">    :func:`~pyngrok.ngrok.connect`), or use :func:`~pyngrok.process.get_process`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t491" href="#t491">491</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t492" href="#t492">492</a></span><span class="t"><span class="str">    :param args: Arguments to be passed to the ``ngrok`` process.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t493" href="#t493">493</a></span><span class="t"><span class="str">    :type args: list[str], optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t494" href="#t494">494</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t495" href="#t495">495</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t496" href="#t496">496</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t497" href="#t497">497</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t498" href="#t498">498</a></span><span class="t">    <span class="key">if</span> <span class="nam">args</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t499" href="#t499">499</a></span><span class="t">        <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t500" href="#t500">500</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t501" href="#t501">501</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t502" href="#t502">502</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t503" href="#t503">503</a></span><span class="t">    <span class="nam">install_ngrok</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t504" href="#t504">504</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t505" href="#t505">505</a></span><span class="t">    <span class="nam">process</span><span class="op">.</span><span class="nam">run_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">,</span> <span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t506" href="#t506">506</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t507" href="#t507">507</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t508" href="#t508">508</a></span><span class="t"><span class="key">def</span> <span class="nam">main</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t509" href="#t509">509</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t510" href="#t510">510</a></span><span class="t"><span class="str">    Entry point for the package's ``console_scripts``. This initializes a call from the command</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t511" href="#t511">511</a></span><span class="t"><span class="str">    line and invokes :func:`~pyngrok.ngrok.run`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">        <span class="nam">status_code</span> <span class="op">=</span> <span class="nam">e</span><span class="op">.</span><span class="nam">getcode</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">        <span class="nam">logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Response {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">.</span><span class="nam">strip</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokNgrokHTTPError</span><span class="op">(</span><span class="str">"ngrok client exception, API returned {}: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">status_code</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t">                                    <span class="nam">e</span><span class="op">.</span><span class="nam">url</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t489" href="#t489">489</a></span><span class="t">                                    <span class="nam">status_code</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">msg</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">hdrs</span><span class="op">,</span> <span class="nam">response_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t490" href="#t490">490</a></span><span class="t">    <span class="key">except</span> <span class="nam">URLError</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t491" href="#t491">491</a></span><span class="t">        <span class="key">raise</span> <span class="nam">PyngrokNgrokURLError</span><span class="op">(</span><span class="str">"ngrok client exception, URLError: {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">e</span><span class="op">.</span><span class="nam">reason</span><span class="op">)</span><span class="op">,</span> <span class="nam">e</span><span class="op">.</span><span class="nam">reason</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t492" href="#t492">492</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t493" href="#t493">493</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t494" href="#t494">494</a></span><span class="t"><span class="key">def</span> <span class="nam">run</span><span class="op">(</span><span class="nam">args</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">pyngrok_config</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t495" href="#t495">495</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t496" href="#t496">496</a></span><span class="t"><span class="str">    Ensure ``ngrok`` is installed at the default path, then call :func:`~pyngrok.process.run_process`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t497" href="#t497">497</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t498" href="#t498">498</a></span><span class="t"><span class="str">    This method is meant for interacting with ``ngrok`` from the command line and is not necessarily</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t499" href="#t499">499</a></span><span class="t"><span class="str">    compatible with non-blocking API methods. For that, use :mod:`~pyngrok.ngrok`'s interface methods (like</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t500" href="#t500">500</a></span><span class="t"><span class="str">    :func:`~pyngrok.ngrok.connect`), or use :func:`~pyngrok.process.get_process`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t501" href="#t501">501</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t502" href="#t502">502</a></span><span class="t"><span class="str">    :param args: Arguments to be passed to the ``ngrok`` process.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t503" href="#t503">503</a></span><span class="t"><span class="str">    :type args: list[str], optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t504" href="#t504">504</a></span><span class="t"><span class="str">    :param pyngrok_config: A ``pyngrok`` configuration to use when interacting with the ``ngrok`` binary,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t505" href="#t505">505</a></span><span class="t"><span class="str">        overriding :func:`~pyngrok.conf.get_default()`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t506" href="#t506">506</a></span><span class="t"><span class="str">    :type pyngrok_config: PyngrokConfig, optional</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t507" href="#t507">507</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t508" href="#t508">508</a></span><span class="t">    <span class="key">if</span> <span class="nam">args</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t509" href="#t509">509</a></span><span class="t">        <span class="nam">args</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t510" href="#t510">510</a></span><span class="t">    <span class="key">if</span> <span class="nam">pyngrok_config</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t511" href="#t511">511</a></span><span class="t">        <span class="nam">pyngrok_config</span> <span class="op">=</span> <span class="nam">conf</span><span class="op">.</span><span class="nam">get_default</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t512" href="#t512">512</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t513" href="#t513">513</a></span><span class="t"><span class="str">    This method is meant for interacting with ``ngrok`` from the command line and is not necessarily</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t514" href="#t514">514</a></span><span class="t"><span class="str">    compatible with non-blocking API methods. For that, use :mod:`~pyngrok.ngrok`'s interface methods (like</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t515" href="#t515">515</a></span><span class="t"><span class="str">    :func:`~pyngrok.ngrok.connect`), or use :func:`~pyngrok.process.get_process`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t516" href="#t516">516</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t517" href="#t517">517</a></span><span class="t">    <span class="nam">run</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t518" href="#t518">518</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t519" href="#t519">519</a></span><span class="t">    <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span> <span class="key">or</span> <span class="nam">len</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">)</span> <span class="op">==</span> <span class="num">2</span> <span class="key">and</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"help"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t520" href="#t520">520</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">"\nPYNGROK VERSION:\n   {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">__version__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t521" href="#t521">521</a></span><span class="t">    <span class="key">elif</span> <span class="nam">len</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">)</span> <span class="op">==</span> <span class="num">2</span> <span class="key">and</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span> <span class="key">in</span> <span class="op">[</span><span class="str">"v"</span><span class="op">,</span> <span class="str">"version"</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t522" href="#t522">522</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">"pyngrok version {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">__version__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t523" href="#t523">523</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t524" href="#t524">524</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t525" href="#t525">525</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t526" href="#t526">526</a></span><span class="t">    <span class="nam">main</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t513" href="#t513">513</a></span><span class="t">    <span class="nam">install_ngrok</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t514" href="#t514">514</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t515" href="#t515">515</a></span><span class="t">    <span class="nam">process</span><span class="op">.</span><span class="nam">run_process</span><span class="op">(</span><span class="nam">pyngrok_config</span><span class="op">.</span><span class="nam">ngrok_path</span><span class="op">,</span> <span class="nam">args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t516" href="#t516">516</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t517" href="#t517">517</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t518" href="#t518">518</a></span><span class="t"><span class="key">def</span> <span class="nam">main</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t519" href="#t519">519</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t520" href="#t520">520</a></span><span class="t"><span class="str">    Entry point for the package's ``console_scripts``. This initializes a call from the command</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t521" href="#t521">521</a></span><span class="t"><span class="str">    line and invokes :func:`~pyngrok.ngrok.run`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t522" href="#t522">522</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t523" href="#t523">523</a></span><span class="t"><span class="str">    This method is meant for interacting with ``ngrok`` from the command line and is not necessarily</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t524" href="#t524">524</a></span><span class="t"><span class="str">    compatible with non-blocking API methods. For that, use :mod:`~pyngrok.ngrok`'s interface methods (like</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t525" href="#t525">525</a></span><span class="t"><span class="str">    :func:`~pyngrok.ngrok.connect`), or use :func:`~pyngrok.process.get_process`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t526" href="#t526">526</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t527" href="#t527">527</a></span><span class="t">    <span class="nam">run</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">[</span><span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t528" href="#t528">528</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t529" href="#t529">529</a></span><span class="t">    <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span> <span class="key">or</span> <span class="nam">len</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">)</span> <span class="op">==</span> <span class="num">2</span> <span class="key">and</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"help"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t530" href="#t530">530</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">"\nPYNGROK VERSION:\n   {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">__version__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t531" href="#t531">531</a></span><span class="t">    <span class="key">elif</span> <span class="nam">len</span><span class="op">(</span><span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">)</span> <span class="op">==</span> <span class="num">2</span> <span class="key">and</span> <span class="nam">sys</span><span class="op">.</span><span class="nam">argv</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"-"</span><span class="op">)</span> <span class="key">in</span> <span class="op">[</span><span class="str">"v"</span><span class="op">,</span> <span class="str">"version"</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t532" href="#t532">532</a></span><span class="t">        <span class="nam">print</span><span class="op">(</span><span class="str">"pyngrok version {}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">__version__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t533" href="#t533">533</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t534" href="#t534">534</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t535" href="#t535">535</a></span><span class="t"><span class="key">if</span> <span class="nam">__name__</span> <span class="op">==</span> <span class="str">"__main__"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t536" href="#t536">536</a></span><span class="t">    <span class="nam">main</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_installer_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48_process_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for pyngrok/ngrok.py: 87.78% ******
+****** Coverage for pyngrok/ngrok.py: 87.70% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 180 statements   158 run 22 missing 6 excluded *****
+***** 187 statements   164 run 23 missing 6 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
 
 
 1import json 
 2import logging 
 3import os 
 4import socket 
 5import sys 
@@ -27,15 +27,15 @@
 11 
 12from pyngrok import process, conf, installer 
 13from pyngrok.exception import PyngrokNgrokHTTPError, PyngrokNgrokURLError,
 PyngrokSecurityError, PyngrokError 
 14 
 15__author__ = "Alex Laird" 
 16__copyright__ = "Copyright 2023, Alex Laird" 
-17__version__ = "5.2.2" 
+17__version__ = "5.2.3" 
 18 
 19from pyngrok.installer import get_default_config 
 20 
 21logger = logging.getLogger(__name__) 
 22 
 23_current_tunnels = {} 
 24 
@@ -304,313 +304,323 @@
 250 "name": name, 
 251 "addr": addr, 
 252 "proto": proto 
 253 } 
 254 options.update(config) 
 255 
 256 # Upgrade legacy parameters, if present 
-257 if pyngrok_config.ngrok_version == "v3" and "bind_tls" in options: 
-258 if options.get("bind_tls") is True or options.get("bind_tls") == "true": 
-259 options["schemes"] = ["https"] 
-260 elif not options.get("bind_tls") is not False or options.get("bind_tls") ==
+257 if pyngrok_config.ngrok_version == "v3": 
+258 if "bind_tls" in options: 
+259 if options.get("bind_tls") is True or options.get("bind_tls") == "true": 
+260 options["schemes"] = ["https"] 
+261 elif not options.get("bind_tls") is not False or options.get("bind_tls") ==
 "false": 
-261 options["schemes"] = ["http"] 
-262 else: 
-263 options["schemes"] = ["http", "https"] 
-264 
-265 options.pop("bind_tls") 
-266 
-267 api_url = get_ngrok_process(pyngrok_config).api_url 
-268 
-269 logger.debug("Creating tunnel with options: {}".format(options)) 
-270 
-271 tunnel = NgrokTunnel(api_request("{}/api/tunnels".format(api_url),
-method="POST", data=options, 
-272 timeout=pyngrok_config.request_timeout), 
-273 pyngrok_config, api_url) 
+262 options["schemes"] = ["http"] 
+263 else: 
+264 options["schemes"] = ["http", "https"] 
+265 
+266 options.pop("bind_tls") 
+267 
+268 if "auth" in options: 
+269 auth = options.get("auth") 
+270 if isinstance(auth, list): 
+271 options["basic_auth"] = auth 
+272 else: 
+273 options["basic_auth"] = [auth] 
 274 
-275 if pyngrok_config.ngrok_version == "v2" and proto == "http" and options.get
+275 options.pop("auth") 
+276 
+277 api_url = get_ngrok_process(pyngrok_config).api_url 
+278 
+279 logger.debug("Creating tunnel with options: {}".format(options)) 
+280 
+281 tunnel = NgrokTunnel(api_request("{}/api/tunnels".format(api_url),
+method="POST", data=options, 
+282 timeout=pyngrok_config.request_timeout), 
+283 pyngrok_config, api_url) 
+284 
+285 if pyngrok_config.ngrok_version == "v2" and proto == "http" and options.get
 ("bind_tls", "both") == "both": 
-276 tunnel = NgrokTunnel(api_request("{}{}%20%28http%29".format(api_url,
+286 tunnel = NgrokTunnel(api_request("{}{}%20%28http%29".format(api_url,
 tunnel.uri), method="GET", 
-277 timeout=pyngrok_config.request_timeout), 
-278 pyngrok_config, api_url) 
-279 
-280 _current_tunnels[tunnel.public_url] = tunnel 
-281 
-282 return tunnel 
-283 
-284 
-285def disconnect(public_url, pyngrok_config=None): 
-286 """ 
-287 Disconnect the ``ngrok`` tunnel for the given URL, if open. 
-288 
-289 :param public_url: The public URL of the tunnel to disconnect. 
-290 :type public_url: str 
-291 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
+287 timeout=pyngrok_config.request_timeout), 
+288 pyngrok_config, api_url) 
+289 
+290 _current_tunnels[tunnel.public_url] = tunnel 
+291 
+292 return tunnel 
+293 
+294 
+295def disconnect(public_url, pyngrok_config=None): 
+296 """ 
+297 Disconnect the ``ngrok`` tunnel for the given URL, if open. 
+298 
+299 :param public_url: The public URL of the tunnel to disconnect. 
+300 :type public_url: str 
+301 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
 with the ``ngrok`` binary, 
-292 overriding :func:`~pyngrok.conf.get_default()`. 
-293 :type pyngrok_config: PyngrokConfig, optional 
-294 """ 
-295 if pyngrok_config is None: 
-296 pyngrok_config = conf.get_default() 
-297 
-298 # If ngrok is not running, there are no tunnels to disconnect 
-299 if not process.is_process_running(pyngrok_config.ngrok_path): 
-300 return 
-301 
-302 api_url = get_ngrok_process(pyngrok_config).api_url 
-303 
-304 if public_url not in _current_tunnels: 
-305 get_tunnels(pyngrok_config) 
-306 
-307 # One more check, if the given URL is still not in the list of tunnels, it
+302 overriding :func:`~pyngrok.conf.get_default()`. 
+303 :type pyngrok_config: PyngrokConfig, optional 
+304 """ 
+305 if pyngrok_config is None: 
+306 pyngrok_config = conf.get_default() 
+307 
+308 # If ngrok is not running, there are no tunnels to disconnect 
+309 if not process.is_process_running(pyngrok_config.ngrok_path): 
+310 return 
+311 
+312 api_url = get_ngrok_process(pyngrok_config).api_url 
+313 
+314 if public_url not in _current_tunnels: 
+315 get_tunnels(pyngrok_config) 
+316 
+317 # One more check, if the given URL is still not in the list of tunnels, it
 is not active 
-308 if public_url not in _current_tunnels: 
-309 return 
-310 
-311 tunnel = _current_tunnels[public_url] 
-312 
-313 logger.info("Disconnecting tunnel: {}".format(tunnel.public_url)) 
-314 
-315 api_request("{}{}".format(api_url, tunnel.uri), method="DELETE", 
-316 timeout=pyngrok_config.request_timeout) 
-317 
-318 _current_tunnels.pop(public_url, None) 
-319 
+318 if public_url not in _current_tunnels: 
+319 return 
 320 
-321def get_tunnels(pyngrok_config=None): 
-322 """ 
-323 Get a list of active ``ngrok`` tunnels for the given config's
-``ngrok_path``. 
+321 tunnel = _current_tunnels[public_url] 
+322 
+323 logger.info("Disconnecting tunnel: {}".format(tunnel.public_url)) 
 324 
-325 If ``ngrok`` is not installed at :class:`~pyngrok.conf.PyngrokConfig`'s
-``ngrok_path``, calling this method 
-326 will first download and install ``ngrok``. 
+325 api_request("{}{}".format(api_url, tunnel.uri), method="DELETE", 
+326 timeout=pyngrok_config.request_timeout) 
 327 
-328 If ``ngrok`` is not running, calling this method will first start a process
-with 
-329 :class:`~pyngrok.conf.PyngrokConfig`. 
+328 _current_tunnels.pop(public_url, None) 
+329 
 330 
-331 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
+331def get_tunnels(pyngrok_config=None): 
+332 """ 
+333 Get a list of active ``ngrok`` tunnels for the given config's
+``ngrok_path``. 
+334 
+335 If ``ngrok`` is not installed at :class:`~pyngrok.conf.PyngrokConfig`'s
+``ngrok_path``, calling this method 
+336 will first download and install ``ngrok``. 
+337 
+338 If ``ngrok`` is not running, calling this method will first start a process
+with 
+339 :class:`~pyngrok.conf.PyngrokConfig`. 
+340 
+341 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
 with the ``ngrok`` binary, 
-332 overriding :func:`~pyngrok.conf.get_default()`. 
-333 :type pyngrok_config: PyngrokConfig, optional 
-334 :return: The active ``ngrok`` tunnels. 
-335 :rtype: list[NgrokTunnel] 
-336 """ 
-337 if pyngrok_config is None: 
-338 pyngrok_config = conf.get_default() 
-339 
-340 api_url = get_ngrok_process(pyngrok_config).api_url 
-341 
-342 _current_tunnels.clear() 
-343 for tunnel in api_request("{}/api/tunnels".format(api_url), method="GET", 
-344 timeout=pyngrok_config.request_timeout)["tunnels"]: 
-345 ngrok_tunnel = NgrokTunnel(tunnel, pyngrok_config, api_url) 
-346 _current_tunnels[ngrok_tunnel.public_url] = ngrok_tunnel 
-347 
-348 return list(_current_tunnels.values()) 
+342 overriding :func:`~pyngrok.conf.get_default()`. 
+343 :type pyngrok_config: PyngrokConfig, optional 
+344 :return: The active ``ngrok`` tunnels. 
+345 :rtype: list[NgrokTunnel] 
+346 """ 
+347 if pyngrok_config is None: 
+348 pyngrok_config = conf.get_default() 
 349 
-350 
-351def kill(pyngrok_config=None): 
-352 """ 
-353 Terminate the ``ngrok`` processes, if running, for the given config's
+350 api_url = get_ngrok_process(pyngrok_config).api_url 
+351 
+352 _current_tunnels.clear() 
+353 for tunnel in api_request("{}/api/tunnels".format(api_url), method="GET", 
+354 timeout=pyngrok_config.request_timeout)["tunnels"]: 
+355 ngrok_tunnel = NgrokTunnel(tunnel, pyngrok_config, api_url) 
+356 _current_tunnels[ngrok_tunnel.public_url] = ngrok_tunnel 
+357 
+358 return list(_current_tunnels.values()) 
+359 
+360 
+361def kill(pyngrok_config=None): 
+362 """ 
+363 Terminate the ``ngrok`` processes, if running, for the given config's
 ``ngrok_path``. This method will not 
-354 block, it will just issue a kill request. 
-355 
-356 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
+364 block, it will just issue a kill request. 
+365 
+366 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
 with the ``ngrok`` binary, 
-357 overriding :func:`~pyngrok.conf.get_default()`. 
-358 :type pyngrok_config: PyngrokConfig, optional 
-359 """ 
-360 if pyngrok_config is None: 
-361 pyngrok_config = conf.get_default() 
-362 
-363 process.kill_process(pyngrok_config.ngrok_path) 
-364 
-365 _current_tunnels.clear() 
-366 
-367 
-368def get_version(pyngrok_config=None): 
+367 overriding :func:`~pyngrok.conf.get_default()`. 
+368 :type pyngrok_config: PyngrokConfig, optional 
 369 """ 
-370 Get a tuple with the ``ngrok`` and ``pyngrok`` versions. 
-371 
-372 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
+370 if pyngrok_config is None: 
+371 pyngrok_config = conf.get_default() 
+372 
+373 process.kill_process(pyngrok_config.ngrok_path) 
+374 
+375 _current_tunnels.clear() 
+376 
+377 
+378def get_version(pyngrok_config=None): 
+379 """ 
+380 Get a tuple with the ``ngrok`` and ``pyngrok`` versions. 
+381 
+382 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
 with the ``ngrok`` binary, 
-373 overriding :func:`~pyngrok.conf.get_default()`. 
-374 :type pyngrok_config: PyngrokConfig, optional 
-375 :return: A tuple of ``(ngrok_version, pyngrok_version)``. 
-376 :rtype: tuple 
-377 """ 
-378 if pyngrok_config is None: 
-379 pyngrok_config = conf.get_default() 
-380 
-381 ngrok_version = process.capture_run_process(pyngrok_config.ngrok_path, ["--
-version"]).split("version ")[1] 
-382 
-383 return ngrok_version, __version__ 
-384 
-385 
-386def update(pyngrok_config=None): 
+383 overriding :func:`~pyngrok.conf.get_default()`. 
+384 :type pyngrok_config: PyngrokConfig, optional 
+385 :return: A tuple of ``(ngrok_version, pyngrok_version)``. 
+386 :rtype: tuple 
 387 """ 
-388 Update ``ngrok`` for the given config's ``ngrok_path``, if an update is
+388 if pyngrok_config is None: 
+389 pyngrok_config = conf.get_default() 
+390 
+391 ngrok_version = process.capture_run_process(pyngrok_config.ngrok_path, ["--
+version"]).split("version ")[1] 
+392 
+393 return ngrok_version, __version__ 
+394 
+395 
+396def update(pyngrok_config=None): 
+397 """ 
+398 Update ``ngrok`` for the given config's ``ngrok_path``, if an update is
 available. 
-389 
-390 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
+399 
+400 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
 with the ``ngrok`` binary, 
-391 overriding :func:`~pyngrok.conf.get_default()`. 
-392 :type pyngrok_config: PyngrokConfig, optional 
-393 :return: The result from the ``ngrok`` update. 
-394 :rtype: str 
-395 """ 
-396 if pyngrok_config is None: 
-397 pyngrok_config = conf.get_default() 
-398 
-399 return process.capture_run_process(pyngrok_config.ngrok_path, ["update"]) 
-400 
-401 
-402def api_request(url, method="GET", data=None, params=None, timeout=4): 
-403 """ 
-404 Invoke an API request to the given URL, returning JSON data from the
-response. 
-405 
-406 One use for this method is making requests to ``ngrok`` tunnels: 
-407 
-408 .. code-block:: python 
-409 
-410 from pyngrok import ngrok 
+401 overriding :func:`~pyngrok.conf.get_default()`. 
+402 :type pyngrok_config: PyngrokConfig, optional 
+403 :return: The result from the ``ngrok`` update. 
+404 :rtype: str 
+405 """ 
+406 if pyngrok_config is None: 
+407 pyngrok_config = conf.get_default() 
+408 
+409 return process.capture_run_process(pyngrok_config.ngrok_path, ["update"]) 
+410 
 411 
-412 public_url = ngrok.connect() 
-413 response = ngrok.api_request("{}/some-route".format(public_url), 
-414 method="POST", data={"foo": "bar"}) 
+412def api_request(url, method="GET", data=None, params=None, timeout=4): 
+413 """ 
+414 Invoke an API request to the given URL, returning JSON data from the
+response. 
 415 
-416 Another is making requests to the ``ngrok`` API itself: 
+416 One use for this method is making requests to ``ngrok`` tunnels: 
 417 
 418 .. code-block:: python 
 419 
 420 from pyngrok import ngrok 
 421 
-422 api_url = ngrok.get_ngrok_process().api_url 
-423 response = ngrok.api_request("{}/api/requests/http".format(api_url), 
-424 params={"tunnel_name": "foo"}) 
+422 public_url = ngrok.connect() 
+423 response = ngrok.api_request("{}/some-route".format(public_url), 
+424 method="POST", data={"foo": "bar"}) 
 425 
-426 :param url: The request URL. 
-427 :type url: str 
-428 :param method: The HTTP method. 
-429 :type method: str, optional 
-430 :param data: The request body. 
-431 :type data: dict, optional 
-432 :param params: The URL parameters. 
-433 :type params: dict, optional 
-434 :param timeout: The request timeout, in seconds. 
-435 :type timeout: float, optional 
-436 :return: The response from the request. 
-437 :rtype: dict 
-438 """ 
-439 if params is None: 
-440 params = [] 
-441 
-442 if not url.lower().startswith("http"): 
-443 raise PyngrokSecurityError("URL must start with \"http\": {}".format(url)) 
-444 
-445 data = json.dumps(data).encode("utf-8") if data else None 
-446 
-447 if params: 
-448 url += "?{}".format(urlencode([(x, params[x]) for x in params])) 
-449 
-450 request = Request(url, method=method.upper()) 
-451 request.add_header("Content-Type", "application/json") 
-452 
-453 logger.debug("Making {} request to {} with data: {}".format(method, url,
-data)) 
+426 Another is making requests to the ``ngrok`` API itself: 
+427 
+428 .. code-block:: python 
+429 
+430 from pyngrok import ngrok 
+431 
+432 api_url = ngrok.get_ngrok_process().api_url 
+433 response = ngrok.api_request("{}/api/requests/http".format(api_url), 
+434 params={"tunnel_name": "foo"}) 
+435 
+436 :param url: The request URL. 
+437 :type url: str 
+438 :param method: The HTTP method. 
+439 :type method: str, optional 
+440 :param data: The request body. 
+441 :type data: dict, optional 
+442 :param params: The URL parameters. 
+443 :type params: dict, optional 
+444 :param timeout: The request timeout, in seconds. 
+445 :type timeout: float, optional 
+446 :return: The response from the request. 
+447 :rtype: dict 
+448 """ 
+449 if params is None: 
+450 params = [] 
+451 
+452 if not url.lower().startswith("http"): 
+453 raise PyngrokSecurityError("URL must start with \"http\": {}".format(url)) 
 454 
-455 try: 
-456 response = urlopen(request, data, timeout) 
-457 response_data = response.read().decode("utf-8") 
-458 
-459 status_code = response.getcode() 
-460 logger.debug("Response {}: {}".format(status_code, response_data.strip())) 
-461 
-462 if str(status_code)[0] != "2": 
-463 raise PyngrokNgrokHTTPError("ngrok client API returned {}: {}".format
+455 data = json.dumps(data).encode("utf-8") if data else None 
+456 
+457 if params: 
+458 url += "?{}".format(urlencode([(x, params[x]) for x in params])) 
+459 
+460 request = Request(url, method=method.upper()) 
+461 request.add_header("Content-Type", "application/json") 
+462 
+463 logger.debug("Making {} request to {} with data: {}".format(method, url,
+data)) 
+464 
+465 try: 
+466 response = urlopen(request, data, timeout) 
+467 response_data = response.read().decode("utf-8") 
+468 
+469 status_code = response.getcode() 
+470 logger.debug("Response {}: {}".format(status_code, response_data.strip())) 
+471 
+472 if str(status_code)[0] != "2": 
+473 raise PyngrokNgrokHTTPError("ngrok client API returned {}: {}".format
 (status_code, response_data), url, 
-464 status_code, None, request.headers, response_data) 
-465 elif status_code == HTTPStatus.NO_CONTENT: 
-466 return None 
-467 
-468 return json.loads(response_data) 
-469 except socket.timeout: 
-470 raise PyngrokNgrokURLError("ngrok client exception, URLError: timed out",
+474 status_code, None, request.headers, response_data) 
+475 elif status_code == HTTPStatus.NO_CONTENT: 
+476 return None 
+477 
+478 return json.loads(response_data) 
+479 except socket.timeout: 
+480 raise PyngrokNgrokURLError("ngrok client exception, URLError: timed out",
 "timed out") 
-471 except HTTPError as e: 
-472 response_data = e.read().decode("utf-8") 
-473 
-474 status_code = e.getcode() 
-475 logger.debug("Response {}: {}".format(status_code, response_data.strip())) 
-476 
-477 raise PyngrokNgrokHTTPError("ngrok client exception, API returned {}:
+481 except HTTPError as e: 
+482 response_data = e.read().decode("utf-8") 
+483 
+484 status_code = e.getcode() 
+485 logger.debug("Response {}: {}".format(status_code, response_data.strip())) 
+486 
+487 raise PyngrokNgrokHTTPError("ngrok client exception, API returned {}:
 {}".format(status_code, response_data), 
-478 e.url, 
-479 status_code, e.msg, e.hdrs, response_data) 
-480 except URLError as e: 
-481 raise PyngrokNgrokURLError("ngrok client exception, URLError: {}".format
+488 e.url, 
+489 status_code, e.msg, e.hdrs, response_data) 
+490 except URLError as e: 
+491 raise PyngrokNgrokURLError("ngrok client exception, URLError: {}".format
 (e.reason), e.reason) 
-482 
-483 
-484def run(args=None, pyngrok_config=None): 
-485 """ 
-486 Ensure ``ngrok`` is installed at the default path, then call :func:
+492 
+493 
+494def run(args=None, pyngrok_config=None): 
+495 """ 
+496 Ensure ``ngrok`` is installed at the default path, then call :func:
 `~pyngrok.process.run_process`. 
-487 
-488 This method is meant for interacting with ``ngrok`` from the command line
+497 
+498 This method is meant for interacting with ``ngrok`` from the command line
 and is not necessarily 
-489 compatible with non-blocking API methods. For that, use :mod:
+499 compatible with non-blocking API methods. For that, use :mod:
 `~pyngrok.ngrok`'s interface methods (like 
-490 :func:`~pyngrok.ngrok.connect`), or use :func:
+500 :func:`~pyngrok.ngrok.connect`), or use :func:
 `~pyngrok.process.get_process`. 
-491 
-492 :param args: Arguments to be passed to the ``ngrok`` process. 
-493 :type args: list[str], optional 
-494 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
+501 
+502 :param args: Arguments to be passed to the ``ngrok`` process. 
+503 :type args: list[str], optional 
+504 :param pyngrok_config: A ``pyngrok`` configuration to use when interacting
 with the ``ngrok`` binary, 
-495 overriding :func:`~pyngrok.conf.get_default()`. 
-496 :type pyngrok_config: PyngrokConfig, optional 
-497 """ 
-498 if args is None: 
-499 args = [] 
-500 if pyngrok_config is None: 
-501 pyngrok_config = conf.get_default() 
-502 
-503 install_ngrok(pyngrok_config) 
-504 
-505 process.run_process(pyngrok_config.ngrok_path, args) 
-506 
-507 
-508def main(): 
-509 """ 
-510 Entry point for the package's ``console_scripts``. This initializes a call
-from the command 
-511 line and invokes :func:`~pyngrok.ngrok.run`. 
+505 overriding :func:`~pyngrok.conf.get_default()`. 
+506 :type pyngrok_config: PyngrokConfig, optional 
+507 """ 
+508 if args is None: 
+509 args = [] 
+510 if pyngrok_config is None: 
+511 pyngrok_config = conf.get_default() 
 512 
-513 This method is meant for interacting with ``ngrok`` from the command line
+513 install_ngrok(pyngrok_config) 
+514 
+515 process.run_process(pyngrok_config.ngrok_path, args) 
+516 
+517 
+518def main(): 
+519 """ 
+520 Entry point for the package's ``console_scripts``. This initializes a call
+from the command 
+521 line and invokes :func:`~pyngrok.ngrok.run`. 
+522 
+523 This method is meant for interacting with ``ngrok`` from the command line
 and is not necessarily 
-514 compatible with non-blocking API methods. For that, use :mod:
+524 compatible with non-blocking API methods. For that, use :mod:
 `~pyngrok.ngrok`'s interface methods (like 
-515 :func:`~pyngrok.ngrok.connect`), or use :func:
+525 :func:`~pyngrok.ngrok.connect`), or use :func:
 `~pyngrok.process.get_process`. 
-516 """ 
-517 run(sys.argv[1:]) 
-518 
-519 if len(sys.argv) == 1 or len(sys.argv) == 2 and sys.argv[1].lstrip("-
+526 """ 
+527 run(sys.argv[1:]) 
+528 
+529 if len(sys.argv) == 1 or len(sys.argv) == 2 and sys.argv[1].lstrip("-
 ").lstrip("-") == "help": 
-520 print("\nPYNGROK VERSION:\n {}".format(__version__)) 
-521 elif len(sys.argv) == 2 and sys.argv[1].lstrip("-").lstrip("-") in ["v",
+530 print("\nPYNGROK VERSION:\n {}".format(__version__)) 
+531 elif len(sys.argv) == 2 and sys.argv[1].lstrip("-").lstrip("-") in ["v",
 "version"]: 
-522 print("pyngrok version {}".format(__version__)) 
-523 
-524 
-525if __name__ == "__main__": 
-526 main() 
+532 print("pyngrok version {}".format(__version__)) 
+533 
+534 
+535if __name__ == "__main__": 
+536 main() 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
```

### Comparing `pyngrok-5.2.2/_build/coverage/d_a54c45401daf5a48_process_py.html` & `pyngrok-5.2.3/_build/coverage/d_a54c45401daf5a48_process_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_ngrok_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -563,13 +563,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_ngrok_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 209 statements   201 run 8 missing 15 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
 
 
 1import atexit 
 2import logging 
 3import os 
 4import shlex 
 5import subprocess 
@@ -534,8 +534,8 @@
 475 else: 
 476 raise PyngrokNgrokError("The ngrok process was unable to start.",
 ngrok_process.logs) 
 477 
 478 return ngrok_process 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.3, created
-at 2023-04-11 15:55 +0000
+at 2023-04-12 13:51 +0000
```

### Comparing `pyngrok-5.2.2/_build/coverage/favicon_32.png` & `pyngrok-5.2.3/_build/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/coverage/index.html` & `pyngrok-5.2.3/_build/coverage/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>pyngrok Coverage Report:
-            <span class="pc_cov">93.41%</span>
+            <span class="pc_cov">93.32%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -87,46 +87,46 @@
                 <td>146</td>
                 <td>8</td>
                 <td>4</td>
                 <td class="right" data-ratio="138 146">94.52%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_a54c45401daf5a48_ngrok_py.html">pyngrok/ngrok.py</a></td>
-                <td>180</td>
-                <td>22</td>
+                <td>187</td>
+                <td>23</td>
                 <td>6</td>
-                <td class="right" data-ratio="158 180">87.78%</td>
+                <td class="right" data-ratio="164 187">87.70%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_a54c45401daf5a48_process_py.html">pyngrok/process.py</a></td>
                 <td>209</td>
                 <td>8</td>
                 <td>15</td>
                 <td class="right" data-ratio="201 209">96.17%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>592</td>
-                <td>39</td>
+                <td>599</td>
+                <td>40</td>
                 <td>25</td>
-                <td class="right" data-ratio="553 592">93.41%</td>
+                <td class="right" data-ratio="559 599">93.32%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.3">coverage.py v7.2.3</a>,
-            created at 2023-04-11 15:55 +0000
+            created at 2023-04-12 13:51 +0000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_a54c45401daf5a48_process_py.html"/>
         <a id="nextFileLink" class="nav" href="d_a54c45401daf5a48___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 
-****** pyngrok Coverage Report: 93.41% ******
+****** pyngrok Coverage Report: 93.32% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.3, created at 2023-04-11 15:55 +0000
+coverage.py_v7.2.3, created at 2023-04-12 13:51 +0000
 
 Module               statements missing excluded coverage
 pyngrok/__init__.py  0          0       0        100.00%
 pyngrok/conf.py      29         1       0        96.55%
 pyngrok/exception.py 28         0       0        100.00%
 pyngrok/installer.py 146        8       4        94.52%
-pyngrok/ngrok.py     180        22      6        87.78%
+pyngrok/ngrok.py     187        23      6        87.70%
 pyngrok/process.py   209        8       15       96.17%
-Total                592        39      25       93.41%
+Total                599        40      25       93.32%
 No items found using the specified filter.
 
-coverage.py_v7.2.3, created at 2023-04-11 15:55 +0000
+coverage.py_v7.2.3, created at 2023-04-12 13:51 +0000
  ____
```

### Comparing `pyngrok-5.2.2/_build/coverage/keybd_closed.png` & `pyngrok-5.2.3/_build/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/coverage/keybd_open.png` & `pyngrok-5.2.3/_build/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/coverage/status.json` & `pyngrok-5.2.3/_build/coverage/status.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972222222222222%*

 * *Differences: {"'files'": "{'d_a54c45401daf5a48_ngrok_py': {'hash': '6ce040c6a85e1deebe319fdb4e7a963a', 'index': "*

 * *            "{'nums': {insert: [(2, 187), (4, 23)], delete: [4, 2]}}}}"}*

```diff
@@ -65,23 +65,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "pyngrok/installer.py"
             }
         },
         "d_a54c45401daf5a48_ngrok_py": {
-            "hash": "ac3621925a541498b02e19aaa05ff088",
+            "hash": "6ce040c6a85e1deebe319fdb4e7a963a",
             "index": {
                 "html_filename": "d_a54c45401daf5a48_ngrok_py.html",
                 "nums": [
                     2,
                     1,
-                    180,
+                    187,
                     6,
-                    22,
+                    23,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "pyngrok/ngrok.py"
             }
         },
```

### Comparing `pyngrok-5.2.2/_build/coverage/style.css` & `pyngrok-5.2.3/_build/coverage/style.css`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/doctrees/api.doctree` & `pyngrok-5.2.3/_build/docs/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/doctrees/index.doctree` & `pyngrok-5.2.3/_build/docs/doctrees/index.doctree`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 952b 0001 0000 0000 008c 0f73 7068  ...+.........sph
+00000000: 8005 9501 0001 0000 0000 008c 0f73 7068  .............sph
 00000010: 696e 782e 6164 646e 6f64 6573 948c 0864  inx.addnodes...d
 00000020: 6f63 756d 656e 7494 9394 2981 947d 9428  ocument...)..}.(
 00000030: 8c09 7261 7773 6f75 7263 6594 8c00 948c  ..rawsource.....
 00000040: 0863 6869 6c64 7265 6e94 5d94 8c0e 646f  .children.]...do
 00000050: 6375 7469 6c73 2e6e 6f64 6573 948c 0773  cutils.nodes...s
 00000060: 6563 7469 6f6e 9493 9429 8194 7d94 2868  ection...)..}.(h
 00000070: 0568 0668 075d 9428 6809 8c05 7469 746c  .h.h.].(h...titl
@@ -2506,2166 +2506,2192 @@
 00009c90: 7468 7994 7568 2b6a b202 0000 681d 682c  thy.uh+j....h.h,
 00009ca0: 681e 4bed 681b 6a7c 0a00 0075 6268 168c  h.K.h.j|...ubh..
 00009cb0: 0820 6d65 7468 6f64 2e94 8594 8194 7d94  . method......}.
 00009cc0: 2868 1b6a 7c0a 0000 681c 6803 681d 4e68  (h.j|...h.h.h.Nh
 00009cd0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
 00009ce0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
 00009cf0: 2b68 ed68 1d68 2c68 1e4b ed68 1b6a 8609  +h.h.h,h.K.h.j..
-00009d00: 0000 681c 6803 7562 68ee 2981 947d 9428  ..h.h.ubh.)..}.(
-00009d10: 6805 8cac 6060 7079 6e67 726f 6b60 6020  h...``pyngrok`` 
-00009d20: 6973 2063 6f6d 7061 7469 626c 6520 7769  is compatible wi
-00009d30: 7468 2060 606e 6772 6f6b 6060 2076 3220  th ``ngrok`` v2 
-00009d40: 616e 6420 7633 2c20 6275 7420 6279 2064  and v3, but by d
-00009d50: 6566 6175 6c74 2069 7420 7769 6c6c 2069  efault it will i
-00009d60: 6e73 7461 6c6c 2076 322e 2054 6f20 696e  nstall v2. To in
-00009d70: 7374 616c 6c20 7633 2069 6e73 7465 6164  stall v3 instead
-00009d80: 2c0a 7365 7420 6060 6e67 726f 6b5f 7665  ,.set ``ngrok_ve
-00009d90: 7273 696f 6e60 6020 696e 203a 636c 6173  rsion`` in :clas
-00009da0: 733a 607e 7079 6e67 726f 6b2e 636f 6e66  s:`~pyngrok.conf
-00009db0: 2e50 796e 6772 6f6b 436f 6e66 6967 603a  .PyngrokConfig`:
-00009dc0: 9468 075d 9428 68f4 2981 947d 9428 6805  .h.].(h.)..}.(h.
-00009dd0: 8c0b 6060 7079 6e67 726f 6b60 6094 6807  ..``pyngrok``.h.
-00009de0: 5d94 6816 8c07 7079 6e67 726f 6b94 8594  ].h...pyngrok...
-00009df0: 8194 7d94 2868 1b6a fa0a 0000 681c 6803  ..}.(h.j....h.h.
-00009e00: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-00009e10: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00009e20: 5d94 7568 2b68 f368 1b6a f60a 0000 7562  ].uh+h.h.j....ub
-00009e30: 6816 8c14 2069 7320 636f 6d70 6174 6962  h... is compatib
-00009e40: 6c65 2077 6974 6820 9485 9481 947d 9428  le with .....}.(
-00009e50: 681b 6af6 0a00 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-00009e60: 4e75 6268 f429 8194 7d94 2868 058c 0960  Nubh.)..}.(h...`
-00009e70: 606e 6772 6f6b 6060 9468 075d 9468 168c  `ngrok``.h.].h..
-00009e80: 056e 6772 6f6b 9485 9481 947d 9428 681b  .ngrok.....}.(h.
-00009e90: 6a0c 0b00 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-00009ea0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00009eb0: 255d 9468 275d 9468 295d 9475 682b 68f3  %].h'].h)].uh+h.
-00009ec0: 681b 6af6 0a00 0075 6268 168c 4a20 7632  h.j....ubh..J v2
-00009ed0: 2061 6e64 2076 332c 2062 7574 2062 7920   and v3, but by 
-00009ee0: 6465 6661 756c 7420 6974 2077 696c 6c20  default it will 
-00009ef0: 696e 7374 616c 6c20 7632 2e20 546f 2069  install v2. To i
-00009f00: 6e73 7461 6c6c 2076 3320 696e 7374 6561  nstall v3 instea
-00009f10: 642c 0a73 6574 2094 8594 8194 7d94 2868  d,.set .....}.(h
-00009f20: 1b6a f60a 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-00009f30: 7562 68f4 2981 947d 9428 6805 8c11 6060  ubh.)..}.(h...``
-00009f40: 6e67 726f 6b5f 7665 7273 696f 6e60 6094  ngrok_version``.
-00009f50: 6807 5d94 6816 8c0d 6e67 726f 6b5f 7665  h.].h...ngrok_ve
-00009f60: 7273 696f 6e94 8594 8194 7d94 2868 1b6a  rsion.....}.(h.j
-00009f70: 1e0b 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-00009f80: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00009f90: 5d94 6827 5d94 6829 5d94 7568 2b68 f368  ].h'].h)].uh+h.h
-00009fa0: 1b6a f60a 0000 7562 6816 8c04 2069 6e20  .j....ubh... in 
-00009fb0: 9485 9481 947d 9428 681b 6af6 0a00 0068  .....}.(h.j....h
-00009fc0: 1c68 0368 1d4e 681e 4e75 626a b302 0000  .h.h.Nh.Nubj....
-00009fd0: 2981 947d 9428 6805 8c24 3a63 6c61 7373  )..}.(h..$:class
-00009fe0: 3a60 7e70 796e 6772 6f6b 2e63 6f6e 662e  :`~pyngrok.conf.
-00009ff0: 5079 6e67 726f 6b43 6f6e 6669 6760 9468  PyngrokConfig`.h
-0000a000: 075d 9468 f429 8194 7d94 2868 056a 320b  .].h.)..}.(h.j2.
-0000a010: 0000 6807 5d94 6816 8c0d 5079 6e67 726f  ..h.].h...Pyngro
-0000a020: 6b43 6f6e 6669 6794 8594 8194 7d94 2868  kConfig.....}.(h
-0000a030: 1b6a 340b 0000 681c 6803 681d 4e68 1e4e  .j4...h.h.h.Nh.N
-0000a040: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-0000a050: 286a c202 0000 8c02 7079 948c 0870 792d  (j......py...py-
-0000a060: 636c 6173 7394 6568 255d 9468 275d 9468  class.eh%].h'].h
-0000a070: 295d 9475 682b 68f3 681b 6a30 0b00 0075  )].uh+h.h.j0...u
-0000a080: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-0000a090: 255d 9468 275d 9468 295d 948c 0672 6566  %].h'].h)]...ref
-0000a0a0: 646f 6394 6acf 0200 008c 0972 6566 646f  doc.j......refdo
-0000a0b0: 6d61 696e 946a 3e0b 0000 8c07 7265 6674  main.j>.....reft
-0000a0c0: 7970 6594 8c05 636c 6173 7394 8c0b 7265  ype...class...re
-0000a0d0: 6665 7870 6c69 6369 7494 898c 0772 6566  fexplicit....ref
-0000a0e0: 7761 726e 9489 6ad5 0200 004e 6ad6 0200  warn..j....Nj...
-0000a0f0: 004e 6ad7 0200 008c 1a70 796e 6772 6f6b  .Nj......pyngrok
-0000a100: 2e63 6f6e 662e 5079 6e67 726f 6b43 6f6e  .conf.PyngrokCon
-0000a110: 6669 6794 7568 2b6a b202 0000 681d 682c  fig.uh+j....h.h,
-0000a120: 681e 4bf1 681b 6af6 0a00 0075 6268 168c  h.K.h.j....ubh..
-0000a130: 013a 9485 9481 947d 9428 681b 6af6 0a00  .:.....}.(h.j...
-0000a140: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-0000a150: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-0000a160: 275d 9468 295d 9475 682b 68ed 681d 682c  '].h)].uh+h.h.h,
-0000a170: 681e 4bf1 681b 6a86 0900 0068 1c68 0375  h.K.h.j....h.h.u
-0000a180: 626a d501 0000 2981 947d 9428 6805 8c48  bj....)..}.(h..H
-0000a190: 6672 6f6d 2070 796e 6772 6f6b 2069 6d70  from pyngrok imp
-0000a1a0: 6f72 7420 636f 6e66 2c20 6e67 726f 6b0a  ort conf, ngrok.
-0000a1b0: 0a63 6f6e 662e 6765 745f 6465 6661 756c  .conf.get_defaul
-0000a1c0: 7428 292e 6e67 726f 6b5f 7665 7273 696f  t().ngrok_versio
-0000a1d0: 6e20 3d20 2276 3322 9468 075d 9468 168c  n = "v3".h.].h..
-0000a1e0: 4866 726f 6d20 7079 6e67 726f 6b20 696d  Hfrom pyngrok im
-0000a1f0: 706f 7274 2063 6f6e 662c 206e 6772 6f6b  port conf, ngrok
-0000a200: 0a0a 636f 6e66 2e67 6574 5f64 6566 6175  ..conf.get_defau
-0000a210: 6c74 2829 2e6e 6772 6f6b 5f76 6572 7369  lt().ngrok_versi
-0000a220: 6f6e 203d 2022 7633 2294 8594 8194 7d94  on = "v3".....}.
-0000a230: 681b 6a5a 0b00 0073 6261 681f 7d94 2868  h.jZ...sbah.}.(h
-0000a240: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-0000a250: 295d 946a e401 0000 6ae5 0100 006a e601  )].j....j....j..
-0000a260: 0000 896a e701 0000 8c06 7079 7468 6f6e  ...j......python
-0000a270: 946a e901 0000 7d94 7568 2b6a d401 0000  .j....}.uh+j....
-0000a280: 681d 682c 681e 4bf4 681b 6a86 0900 0068  h.h,h.K.h.j....h
-0000a290: 1c68 0375 626a b703 0000 2981 947d 9428  .h.ubj....)..}.(
-0000a2a0: 6805 58a7 0200 0049 6620 6060 6e67 726f  h.X....If ``ngro
-0000a2b0: 6b60 6020 6973 206e 6f74 2061 6c72 6561  k`` is not alrea
-0000a2c0: 6479 2069 6e73 7461 6c6c 6564 2061 7420  dy installed at 
-0000a2d0: 7468 6520 6060 6e67 726f 6b5f 7061 7468  the ``ngrok_path
-0000a2e0: 6060 2069 6e20 3a63 6c61 7373 3a60 7e70  `` in :class:`~p
-0000a2f0: 796e 6772 6f6b 2e63 6f6e 662e 5079 6e67  yngrok.conf.Pyng
-0000a300: 726f 6b43 6f6e 6669 6760 2c20 6974 0a77  rokConfig`, it.w
-0000a310: 696c 6c20 6265 2069 6e73 7461 6c6c 6564  ill be installed
-0000a320: 2074 6865 2066 6972 7374 2074 696d 6520   the first time 
-0000a330: 6d6f 7374 206d 6574 686f 6473 2069 6e20  most methods in 
-0000a340: 7468 6520 3a6d 6f64 3a60 7e70 796e 6772  the :mod:`~pyngr
-0000a350: 6f6b 2e6e 6772 6f6b 6020 6d6f 6475 6c65  ok.ngrok` module
-0000a360: 2061 7265 2063 616c 6c65 642e 0a0a 4966   are called...If
-0000a370: 2077 6520 6e65 6564 2074 6f20 6375 7374   we need to cust
-0000a380: 6f6d 697a 6520 7468 6520 696e 7374 616c  omize the instal
-0000a390: 6c61 7469 6f6e 206f 6620 6060 6e67 726f  lation of ``ngro
-0000a3a0: 6b60 602c 2070 6572 6861 7073 2073 7065  k``, perhaps spe
-0000a3b0: 6369 6679 696e 6720 6120 7469 6d65 6f75  cifying a timeou
-0000a3c0: 742c 2070 726f 7879 2c20 7573 6520 6120  t, proxy, use a 
-0000a3d0: 6375 7374 6f6d 206d 6972 726f 720a 666f  custom mirror.fo
-0000a3e0: 7220 7468 6520 646f 776e 6c6f 6164 2c20  r the download, 
-0000a3f0: 6574 632e 2077 6520 6361 6e20 646f 2073  etc. we can do s
-0000a400: 6f20 6279 206c 6576 6572 6167 696e 6720  o by leveraging 
-0000a410: 7468 6520 3a6d 6f64 3a60 7e70 796e 6772  the :mod:`~pyngr
-0000a420: 6f6b 2e69 6e73 7461 6c6c 6572 6020 6d6f  ok.installer` mo
-0000a430: 6475 6c65 2e20 4b65 7977 6f72 6420 6172  dule. Keyword ar
-0000a440: 6775 6d65 6e74 7320 696e 2074 6869 730a  guments in this.
-0000a450: 6d6f 6475 6c65 2061 7265 2075 6c74 696d  module are ultim
-0000a460: 6174 656c 7920 7061 7373 6564 2064 6f77  ately passed dow
-0000a470: 6e20 746f 203a 7079 3a66 756e 633a 6075  n to :py:func:`u
-0000a480: 726c 6c69 622e 7265 7175 6573 742e 7572  rllib.request.ur
-0000a490: 6c6f 7065 6e60 2c20 736f 2061 7320 6c6f  lopen`, so as lo
-0000a4a0: 6e67 2061 7320 7765 2075 7365 2074 6865  ng as we use the
-0000a4b0: 0a3a 6d6f 643a 607e 7079 6e67 726f 6b2e  .:mod:`~pyngrok.
-0000a4c0: 696e 7374 616c 6c65 7260 206d 6f64 756c  installer` modul
-0000a4d0: 6520 6f75 7273 656c 7665 7320 7072 696f  e ourselves prio
-0000a4e0: 7220 746f 2069 6e76 6f6b 696e 6720 616e  r to invoking an
-0000a4f0: 7920 3a6d 6f64 3a60 7e70 796e 6772 6f6b  y :mod:`~pyngrok
-0000a500: 2e6e 6772 6f6b 6020 6d65 7468 6f64 732c  .ngrok` methods,
-0000a510: 2077 6520 6361 6e20 6361 6e20 636f 6e74   we can can cont
-0000a520: 726f 6c0a 686f 7720 6060 6e67 726f 6b60  rol.how ``ngrok`
-0000a530: 6020 6973 2069 6e73 7461 6c6c 6564 2061  ` is installed a
-0000a540: 6e64 2066 726f 6d20 7768 6572 652e 9468  nd from where..h
-0000a550: 075d 9428 68ee 2981 947d 9428 6805 8cc5  .].(h.)..}.(h...
-0000a560: 4966 2060 606e 6772 6f6b 6060 2069 7320  If ``ngrok`` is 
-0000a570: 6e6f 7420 616c 7265 6164 7920 696e 7374  not already inst
-0000a580: 616c 6c65 6420 6174 2074 6865 2060 606e  alled at the ``n
-0000a590: 6772 6f6b 5f70 6174 6860 6020 696e 203a  grok_path`` in :
-0000a5a0: 636c 6173 733a 607e 7079 6e67 726f 6b2e  class:`~pyngrok.
-0000a5b0: 636f 6e66 2e50 796e 6772 6f6b 436f 6e66  conf.PyngrokConf
-0000a5c0: 6967 602c 2069 740a 7769 6c6c 2062 6520  ig`, it.will be 
-0000a5d0: 696e 7374 616c 6c65 6420 7468 6520 6669  installed the fi
-0000a5e0: 7273 7420 7469 6d65 206d 6f73 7420 6d65  rst time most me
-0000a5f0: 7468 6f64 7320 696e 2074 6865 203a 6d6f  thods in the :mo
-0000a600: 643a 607e 7079 6e67 726f 6b2e 6e67 726f  d:`~pyngrok.ngro
-0000a610: 6b60 206d 6f64 756c 6520 6172 6520 6361  k` module are ca
-0000a620: 6c6c 6564 2e94 6807 5d94 2868 168c 0349  lled..h.].(h...I
-0000a630: 6620 9485 9481 947d 9428 681b 6a6e 0b00  f .....}.(h.jn..
-0000a640: 0068 1c68 0368 1d4e 681e 4e75 6268 f429  .h.h.h.Nh.Nubh.)
-0000a650: 8194 7d94 2868 058c 0960 606e 6772 6f6b  ..}.(h...``ngrok
-0000a660: 6060 9468 075d 9468 168c 056e 6772 6f6b  ``.h.].h...ngrok
-0000a670: 9485 9481 947d 9428 681b 6a76 0b00 0068  .....}.(h.jv...h
-0000a680: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-0000a690: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000a6a0: 9468 295d 9475 682b 68f3 681b 6a6e 0b00  .h)].uh+h.h.jn..
-0000a6b0: 0075 6268 168c 2120 6973 206e 6f74 2061  .ubh..! is not a
-0000a6c0: 6c72 6561 6479 2069 6e73 7461 6c6c 6564  lready installed
-0000a6d0: 2061 7420 7468 6520 9485 9481 947d 9428   at the .....}.(
-0000a6e0: 681b 6a6e 0b00 0068 1c68 0368 1d4e 681e  h.jn...h.h.h.Nh.
-0000a6f0: 4e75 6268 f429 8194 7d94 2868 058c 0e60  Nubh.)..}.(h...`
-0000a700: 606e 6772 6f6b 5f70 6174 6860 6094 6807  `ngrok_path``.h.
-0000a710: 5d94 6816 8c0a 6e67 726f 6b5f 7061 7468  ].h...ngrok_path
-0000a720: 9485 9481 947d 9428 681b 6a88 0b00 0068  .....}.(h.j....h
-0000a730: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-0000a740: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000a750: 9468 295d 9475 682b 68f3 681b 6a6e 0b00  .h)].uh+h.h.jn..
-0000a760: 0075 6268 168c 0420 696e 2094 8594 8194  .ubh... in .....
-0000a770: 7d94 2868 1b6a 6e0b 0000 681c 6803 681d  }.(h.jn...h.h.h.
-0000a780: 4e68 1e4e 7562 6ab3 0200 0029 8194 7d94  Nh.Nubj....)..}.
-0000a790: 2868 058c 243a 636c 6173 733a 607e 7079  (h..$:class:`~py
-0000a7a0: 6e67 726f 6b2e 636f 6e66 2e50 796e 6772  ngrok.conf.Pyngr
-0000a7b0: 6f6b 436f 6e66 6967 6094 6807 5d94 68f4  okConfig`.h.].h.
-0000a7c0: 2981 947d 9428 6805 6a9c 0b00 0068 075d  )..}.(h.j....h.]
-0000a7d0: 9468 168c 0d50 796e 6772 6f6b 436f 6e66  .h...PyngrokConf
-0000a7e0: 6967 9485 9481 947d 9428 681b 6a9e 0b00  ig.....}.(h.j...
-0000a7f0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-0000a800: 7d94 2868 215d 9468 235d 9428 6ac2 0200  }.(h!].h#].(j...
-0000a810: 008c 0270 7994 8c08 7079 2d63 6c61 7373  ...py...py-class
-0000a820: 9465 6825 5d94 6827 5d94 6829 5d94 7568  .eh%].h'].h)].uh
-0000a830: 2b68 f368 1b6a 9a0b 0000 7562 6168 1f7d  +h.h.j....ubah.}
-0000a840: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-0000a850: 5d94 6829 5d94 8c06 7265 6664 6f63 946a  ].h)]...refdoc.j
-0000a860: cf02 0000 8c09 7265 6664 6f6d 6169 6e94  ......refdomain.
-0000a870: 6aa8 0b00 008c 0772 6566 7479 7065 948c  j......reftype..
-0000a880: 0563 6c61 7373 948c 0b72 6566 6578 706c  .class...refexpl
-0000a890: 6963 6974 9489 8c07 7265 6677 6172 6e94  icit....refwarn.
-0000a8a0: 896a d502 0000 4e6a d602 0000 4e6a d702  .j....Nj....Nj..
-0000a8b0: 0000 8c1a 7079 6e67 726f 6b2e 636f 6e66  ....pyngrok.conf
-0000a8c0: 2e50 796e 6772 6f6b 436f 6e66 6967 9475  .PyngrokConfig.u
-0000a8d0: 682b 6ab2 0200 0068 1d68 2c68 1e4b fc68  h+j....h.h,h.K.h
-0000a8e0: 1b6a 6e0b 0000 7562 6816 8c3a 2c20 6974  .jn...ubh..:, it
-0000a8f0: 0a77 696c 6c20 6265 2069 6e73 7461 6c6c  .will be install
-0000a900: 6564 2074 6865 2066 6972 7374 2074 696d  ed the first tim
-0000a910: 6520 6d6f 7374 206d 6574 686f 6473 2069  e most methods i
-0000a920: 6e20 7468 6520 9485 9481 947d 9428 681b  n the .....}.(h.
-0000a930: 6a6e 0b00 0068 1c68 0368 1d4e 681e 4e75  jn...h.h.h.Nh.Nu
-0000a940: 626a b302 0000 2981 947d 9428 6805 8c15  bj....)..}.(h...
-0000a950: 3a6d 6f64 3a60 7e70 796e 6772 6f6b 2e6e  :mod:`~pyngrok.n
-0000a960: 6772 6f6b 6094 6807 5d94 68f4 2981 947d  grok`.h.].h.)..}
-0000a970: 9428 6805 6ac0 0b00 0068 075d 9468 168c  .(h.j....h.].h..
-0000a980: 056e 6772 6f6b 9485 9481 947d 9428 681b  .ngrok.....}.(h.
-0000a990: 6ac2 0b00 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-0000a9a0: 6261 681f 7d94 2868 215d 9468 235d 9428  bah.}.(h!].h#].(
-0000a9b0: 6ac2 0200 008c 0270 7994 8c06 7079 2d6d  j......py...py-m
-0000a9c0: 6f64 9465 6825 5d94 6827 5d94 6829 5d94  od.eh%].h'].h)].
-0000a9d0: 7568 2b68 f368 1b6a be0b 0000 7562 6168  uh+h.h.j....ubah
-0000a9e0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-0000a9f0: 6827 5d94 6829 5d94 8c06 7265 6664 6f63  h'].h)]...refdoc
-0000aa00: 946a cf02 0000 8c09 7265 6664 6f6d 6169  .j......refdomai
-0000aa10: 6e94 6acc 0b00 008c 0772 6566 7479 7065  n.j......reftype
-0000aa20: 948c 036d 6f64 948c 0b72 6566 6578 706c  ...mod...refexpl
-0000aa30: 6963 6974 9489 8c07 7265 6677 6172 6e94  icit....refwarn.
-0000aa40: 896a d502 0000 4e6a d602 0000 4e6a d702  .j....Nj....Nj..
-0000aa50: 0000 8c0d 7079 6e67 726f 6b2e 6e67 726f  ....pyngrok.ngro
-0000aa60: 6b94 7568 2b6a b202 0000 681d 682c 681e  k.uh+j....h.h,h.
-0000aa70: 4bfc 681b 6a6e 0b00 0075 6268 168c 1320  K.h.jn...ubh... 
-0000aa80: 6d6f 6475 6c65 2061 7265 2063 616c 6c65  module are calle
-0000aa90: 642e 9485 9481 947d 9428 681b 6a6e 0b00  d......}.(h.jn..
-0000aaa0: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-0000aab0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-0000aac0: 275d 9468 295d 9475 682b 68ed 681d 682c  '].h)].uh+h.h.h,
-0000aad0: 681e 4bfc 681b 6a6a 0b00 0075 6268 ee29  h.K.h.jj...ubh.)
-0000aae0: 8194 7d94 2868 0558 e001 0000 4966 2077  ..}.(h.X....If w
-0000aaf0: 6520 6e65 6564 2074 6f20 6375 7374 6f6d  e need to custom
-0000ab00: 697a 6520 7468 6520 696e 7374 616c 6c61  ize the installa
-0000ab10: 7469 6f6e 206f 6620 6060 6e67 726f 6b60  tion of ``ngrok`
-0000ab20: 602c 2070 6572 6861 7073 2073 7065 6369  `, perhaps speci
-0000ab30: 6679 696e 6720 6120 7469 6d65 6f75 742c  fying a timeout,
-0000ab40: 2070 726f 7879 2c20 7573 6520 6120 6375   proxy, use a cu
-0000ab50: 7374 6f6d 206d 6972 726f 720a 666f 7220  stom mirror.for 
-0000ab60: 7468 6520 646f 776e 6c6f 6164 2c20 6574  the download, et
-0000ab70: 632e 2077 6520 6361 6e20 646f 2073 6f20  c. we can do so 
-0000ab80: 6279 206c 6576 6572 6167 696e 6720 7468  by leveraging th
-0000ab90: 6520 3a6d 6f64 3a60 7e70 796e 6772 6f6b  e :mod:`~pyngrok
-0000aba0: 2e69 6e73 7461 6c6c 6572 6020 6d6f 6475  .installer` modu
-0000abb0: 6c65 2e20 4b65 7977 6f72 6420 6172 6775  le. Keyword argu
-0000abc0: 6d65 6e74 7320 696e 2074 6869 730a 6d6f  ments in this.mo
-0000abd0: 6475 6c65 2061 7265 2075 6c74 696d 6174  dule are ultimat
-0000abe0: 656c 7920 7061 7373 6564 2064 6f77 6e20  ely passed down 
-0000abf0: 746f 203a 7079 3a66 756e 633a 6075 726c  to :py:func:`url
-0000ac00: 6c69 622e 7265 7175 6573 742e 7572 6c6f  lib.request.urlo
-0000ac10: 7065 6e60 2c20 736f 2061 7320 6c6f 6e67  pen`, so as long
-0000ac20: 2061 7320 7765 2075 7365 2074 6865 0a3a   as we use the.:
-0000ac30: 6d6f 643a 607e 7079 6e67 726f 6b2e 696e  mod:`~pyngrok.in
-0000ac40: 7374 616c 6c65 7260 206d 6f64 756c 6520  staller` module 
-0000ac50: 6f75 7273 656c 7665 7320 7072 696f 7220  ourselves prior 
-0000ac60: 746f 2069 6e76 6f6b 696e 6720 616e 7920  to invoking any 
-0000ac70: 3a6d 6f64 3a60 7e70 796e 6772 6f6b 2e6e  :mod:`~pyngrok.n
-0000ac80: 6772 6f6b 6020 6d65 7468 6f64 732c 2077  grok` methods, w
-0000ac90: 6520 6361 6e20 6361 6e20 636f 6e74 726f  e can can contro
-0000aca0: 6c0a 686f 7720 6060 6e67 726f 6b60 6020  l.how ``ngrok`` 
-0000acb0: 6973 2069 6e73 7461 6c6c 6564 2061 6e64  is installed and
-0000acc0: 2066 726f 6d20 7768 6572 652e 9468 075d   from where..h.]
-0000acd0: 9428 6816 8c2c 4966 2077 6520 6e65 6564  .(h..,If we need
-0000ace0: 2074 6f20 6375 7374 6f6d 697a 6520 7468   to customize th
-0000acf0: 6520 696e 7374 616c 6c61 7469 6f6e 206f  e installation o
-0000ad00: 6620 9485 9481 947d 9428 681b 6ae8 0b00  f .....}.(h.j...
-0000ad10: 0068 1c68 0368 1d4e 681e 4e75 6268 f429  .h.h.h.Nh.Nubh.)
-0000ad20: 8194 7d94 2868 058c 0960 606e 6772 6f6b  ..}.(h...``ngrok
-0000ad30: 6060 9468 075d 9468 168c 056e 6772 6f6b  ``.h.].h...ngrok
-0000ad40: 9485 9481 947d 9428 681b 6af0 0b00 0068  .....}.(h.j....h
-0000ad50: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-0000ad60: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000ad70: 9468 295d 9475 682b 68f3 681b 6ae8 0b00  .h)].uh+h.h.j...
-0000ad80: 0075 6268 168c 712c 2070 6572 6861 7073  .ubh..q, perhaps
-0000ad90: 2073 7065 6369 6679 696e 6720 6120 7469   specifying a ti
-0000ada0: 6d65 6f75 742c 2070 726f 7879 2c20 7573  meout, proxy, us
-0000adb0: 6520 6120 6375 7374 6f6d 206d 6972 726f  e a custom mirro
-0000adc0: 720a 666f 7220 7468 6520 646f 776e 6c6f  r.for the downlo
-0000add0: 6164 2c20 6574 632e 2077 6520 6361 6e20  ad, etc. we can 
-0000ade0: 646f 2073 6f20 6279 206c 6576 6572 6167  do so by leverag
-0000adf0: 696e 6720 7468 6520 9485 9481 947d 9428  ing the .....}.(
-0000ae00: 681b 6ae8 0b00 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-0000ae10: 4e75 626a b302 0000 2981 947d 9428 6805  Nubj....)..}.(h.
-0000ae20: 8c19 3a6d 6f64 3a60 7e70 796e 6772 6f6b  ..:mod:`~pyngrok
-0000ae30: 2e69 6e73 7461 6c6c 6572 6094 6807 5d94  .installer`.h.].
-0000ae40: 68f4 2981 947d 9428 6805 6a04 0c00 0068  h.)..}.(h.j....h
-0000ae50: 075d 9468 168c 0969 6e73 7461 6c6c 6572  .].h...installer
-0000ae60: 9485 9481 947d 9428 681b 6a06 0c00 0068  .....}.(h.j....h
-0000ae70: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-0000ae80: 2868 215d 9468 235d 9428 6ac2 0200 008c  (h!].h#].(j.....
-0000ae90: 0270 7994 8c06 7079 2d6d 6f64 9465 6825  .py...py-mod.eh%
-0000aea0: 5d94 6827 5d94 6829 5d94 7568 2b68 f368  ].h'].h)].uh+h.h
-0000aeb0: 1b6a 020c 0000 7562 6168 1f7d 9428 6821  .j....ubah.}.(h!
-0000aec0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-0000aed0: 5d94 8c06 7265 6664 6f63 946a cf02 0000  ]...refdoc.j....
-0000aee0: 8c09 7265 6664 6f6d 6169 6e94 6a10 0c00  ..refdomain.j...
-0000aef0: 008c 0772 6566 7479 7065 948c 036d 6f64  ...reftype...mod
-0000af00: 948c 0b72 6566 6578 706c 6963 6974 9489  ...refexplicit..
-0000af10: 8c07 7265 6677 6172 6e94 896a d502 0000  ..refwarn..j....
-0000af20: 4e6a d602 0000 4e6a d702 0000 8c11 7079  Nj....Nj......py
-0000af30: 6e67 726f 6b2e 696e 7374 616c 6c65 7294  ngrok.installer.
-0000af40: 7568 2b6a b202 0000 681d 682c 681e 4bff  uh+j....h.h,h.K.
-0000af50: 681b 6ae8 0b00 0075 6268 168c 4820 6d6f  h.j....ubh..H mo
-0000af60: 6475 6c65 2e20 4b65 7977 6f72 6420 6172  dule. Keyword ar
-0000af70: 6775 6d65 6e74 7320 696e 2074 6869 730a  guments in this.
-0000af80: 6d6f 6475 6c65 2061 7265 2075 6c74 696d  module are ultim
-0000af90: 6174 656c 7920 7061 7373 6564 2064 6f77  ately passed dow
-0000afa0: 6e20 746f 2094 8594 8194 7d94 2868 1b6a  n to .....}.(h.j
-0000afb0: e80b 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-0000afc0: 6ab3 0200 0029 8194 7d94 2868 058c 213a  j....)..}.(h..!:
-0000afd0: 7079 3a66 756e 633a 6075 726c 6c69 622e  py:func:`urllib.
-0000afe0: 7265 7175 6573 742e 7572 6c6f 7065 6e60  request.urlopen`
-0000aff0: 9468 075d 9468 f429 8194 7d94 2868 056a  .h.].h.)..}.(h.j
-0000b000: 280c 0000 6807 5d94 6816 8c16 7572 6c6c  (...h.].h...urll
-0000b010: 6962 2e72 6571 7565 7374 2e75 726c 6f70  ib.request.urlop
-0000b020: 656e 9485 9481 947d 9428 681b 6a2a 0c00  en.....}.(h.j*..
-0000b030: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-0000b040: 7d94 2868 215d 9468 235d 9428 6ac2 0200  }.(h!].h#].(j...
-0000b050: 008c 0270 7994 8c07 7079 2d66 756e 6394  ...py...py-func.
-0000b060: 6568 255d 9468 275d 9468 295d 9475 682b  eh%].h'].h)].uh+
-0000b070: 68f3 681b 6a26 0c00 0075 6261 681f 7d94  h.h.j&...ubah.}.
-0000b080: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000b090: 9468 295d 948c 0672 6566 646f 6394 6acf  .h)]...refdoc.j.
-0000b0a0: 0200 008c 0972 6566 646f 6d61 696e 946a  .....refdomain.j
-0000b0b0: 340c 0000 8c07 7265 6674 7970 6594 8c04  4.....reftype...
-0000b0c0: 6675 6e63 948c 0b72 6566 6578 706c 6963  func...refexplic
-0000b0d0: 6974 9489 8c07 7265 6677 6172 6e94 896a  it....refwarn..j
-0000b0e0: d502 0000 4e6a d602 0000 4e6a d702 0000  ....Nj....Nj....
-0000b0f0: 8c16 7572 6c6c 6962 2e72 6571 7565 7374  ..urllib.request
-0000b100: 2e75 726c 6f70 656e 9475 682b 6ab2 0200  .urlopen.uh+j...
-0000b110: 0068 1d68 2c68 1e4b ff68 1b6a e80b 0000  .h.h,h.K.h.j....
-0000b120: 7562 6816 8c1b 2c20 736f 2061 7320 6c6f  ubh..., so as lo
-0000b130: 6e67 2061 7320 7765 2075 7365 2074 6865  ng as we use the
-0000b140: 0a94 8594 8194 7d94 2868 1b6a e80b 0000  ......}.(h.j....
-0000b150: 681c 6803 681d 4e68 1e4e 7562 6ab3 0200  h.h.h.Nh.Nubj...
-0000b160: 0029 8194 7d94 2868 058c 193a 6d6f 643a  .)..}.(h...:mod:
-0000b170: 607e 7079 6e67 726f 6b2e 696e 7374 616c  `~pyngrok.instal
-0000b180: 6c65 7260 9468 075d 9468 f429 8194 7d94  ler`.h.].h.)..}.
-0000b190: 2868 056a 4c0c 0000 6807 5d94 6816 8c09  (h.jL...h.].h...
-0000b1a0: 696e 7374 616c 6c65 7294 8594 8194 7d94  installer.....}.
-0000b1b0: 2868 1b6a 4e0c 0000 681c 6803 681d 4e68  (h.jN...h.h.h.Nh
-0000b1c0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-0000b1d0: 5d94 286a c202 0000 8c02 7079 948c 0670  ].(j......py...p
-0000b1e0: 792d 6d6f 6494 6568 255d 9468 275d 9468  y-mod.eh%].h'].h
-0000b1f0: 295d 9475 682b 68f3 681b 6a4a 0c00 0075  )].uh+h.h.jJ...u
-0000b200: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-0000b210: 255d 9468 275d 9468 295d 948c 0672 6566  %].h'].h)]...ref
-0000b220: 646f 6394 6acf 0200 008c 0972 6566 646f  doc.j......refdo
-0000b230: 6d61 696e 946a 580c 0000 8c07 7265 6674  main.jX.....reft
-0000b240: 7970 6594 8c03 6d6f 6494 8c0b 7265 6665  ype...mod...refe
-0000b250: 7870 6c69 6369 7494 898c 0772 6566 7761  xplicit....refwa
-0000b260: 726e 9489 6ad5 0200 004e 6ad6 0200 004e  rn..j....Nj....N
-0000b270: 6ad7 0200 008c 1170 796e 6772 6f6b 2e69  j......pyngrok.i
-0000b280: 6e73 7461 6c6c 6572 9475 682b 6ab2 0200  nstaller.uh+j...
-0000b290: 0068 1d68 2c68 1e4b ff68 1b6a e80b 0000  .h.h,h.K.h.j....
-0000b2a0: 7562 6816 8c28 206d 6f64 756c 6520 6f75  ubh..( module ou
-0000b2b0: 7273 656c 7665 7320 7072 696f 7220 746f  rselves prior to
-0000b2c0: 2069 6e76 6f6b 696e 6720 616e 7920 9485   invoking any ..
-0000b2d0: 9481 947d 9428 681b 6ae8 0b00 0068 1c68  ...}.(h.j....h.h
-0000b2e0: 0368 1d4e 681e 4e75 626a b302 0000 2981  .h.Nh.Nubj....).
-0000b2f0: 947d 9428 6805 8c15 3a6d 6f64 3a60 7e70  .}.(h...:mod:`~p
-0000b300: 796e 6772 6f6b 2e6e 6772 6f6b 6094 6807  yngrok.ngrok`.h.
-0000b310: 5d94 68f4 2981 947d 9428 6805 6a70 0c00  ].h.)..}.(h.jp..
-0000b320: 0068 075d 9468 168c 056e 6772 6f6b 9485  .h.].h...ngrok..
-0000b330: 9481 947d 9428 681b 6a72 0c00 0068 1c68  ...}.(h.jr...h.h
-0000b340: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-0000b350: 215d 9468 235d 9428 6ac2 0200 008c 0270  !].h#].(j......p
-0000b360: 7994 8c06 7079 2d6d 6f64 9465 6825 5d94  y...py-mod.eh%].
-0000b370: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
-0000b380: 6e0c 0000 7562 6168 1f7d 9428 6821 5d94  n...ubah.}.(h!].
-0000b390: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-0000b3a0: 8c06 7265 6664 6f63 946a cf02 0000 8c09  ..refdoc.j......
-0000b3b0: 7265 6664 6f6d 6169 6e94 6a7c 0c00 008c  refdomain.j|....
-0000b3c0: 0772 6566 7479 7065 948c 036d 6f64 948c  .reftype...mod..
-0000b3d0: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
-0000b3e0: 7265 6677 6172 6e94 896a d502 0000 4e6a  refwarn..j....Nj
-0000b3f0: d602 0000 4e6a d702 0000 8c0d 7079 6e67  ....Nj......pyng
-0000b400: 726f 6b2e 6e67 726f 6b94 7568 2b6a b202  rok.ngrok.uh+j..
-0000b410: 0000 681d 682c 681e 4bff 681b 6ae8 0b00  ..h.h,h.K.h.j...
-0000b420: 0075 6268 168c 2120 6d65 7468 6f64 732c  .ubh..! methods,
-0000b430: 2077 6520 6361 6e20 6361 6e20 636f 6e74   we can can cont
-0000b440: 726f 6c0a 686f 7720 9485 9481 947d 9428  rol.how .....}.(
-0000b450: 681b 6ae8 0b00 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-0000b460: 4e75 6268 f429 8194 7d94 2868 058c 0960  Nubh.)..}.(h...`
-0000b470: 606e 6772 6f6b 6060 9468 075d 9468 168c  `ngrok``.h.].h..
-0000b480: 056e 6772 6f6b 9485 9481 947d 9428 681b  .ngrok.....}.(h.
-0000b490: 6a92 0c00 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-0000b4a0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-0000b4b0: 255d 9468 275d 9468 295d 9475 682b 68f3  %].h'].h)].uh+h.
-0000b4c0: 681b 6ae8 0b00 0075 6268 168c 1d20 6973  h.j....ubh... is
-0000b4d0: 2069 6e73 7461 6c6c 6564 2061 6e64 2066   installed and f
-0000b4e0: 726f 6d20 7768 6572 652e 9485 9481 947d  rom where......}
-0000b4f0: 9428 681b 6ae8 0b00 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-0000b500: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
-0000b510: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-0000b520: 682b 68ed 681d 682c 681e 4bff 681b 6a6a  h+h.h.h,h.K.h.jj
-0000b530: 0b00 0075 6265 681f 7d94 2868 215d 9468  ...ubeh.}.(h!].h
-0000b540: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-0000b550: 682b 6ab6 0300 0068 1b6a 8609 0000 681c  h+j....h.j....h.
-0000b560: 6803 681d 682c 681e 4e75 6265 681f 7d94  h.h.h,h.Nubeh.}.
-0000b570: 2868 215d 948c 0d70 796e 6772 6f6b 636f  (h!]...pyngrokco
-0000b580: 6e66 6967 9461 6823 5d94 6825 5d94 8c0d  nfig.ah#].h%]...
-0000b590: 7079 6e67 726f 6b63 6f6e 6669 6794 6168  pyngrokconfig.ah
-0000b5a0: 275d 9468 295d 9475 682b 680a 681b 6a75  '].h)].uh+h.h.ju
-0000b5b0: 0900 0068 1c68 0368 1d68 2c68 1e4b db75  ...h.h.h.h,h.K.u
-0000b5c0: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
-0000b5d0: 9428 6810 2981 947d 9428 6805 8c19 5365  .(h.)..}.(h...Se
-0000b5e0: 7474 696e 6720 7468 6520 6060 6175 7468  tting the ``auth
-0000b5f0: 746f 6b65 6e60 6094 6807 5d94 2868 168c  token``.h.].(h..
-0000b600: 0c53 6574 7469 6e67 2074 6865 2094 8594  .Setting the ...
-0000b610: 8194 7d94 2868 1b6a bb0c 0000 681c 6803  ..}.(h.j....h.h.
-0000b620: 681d 4e68 1e4e 7562 68f4 2981 947d 9428  h.Nh.Nubh.)..}.(
-0000b630: 6805 8c0d 6060 6175 7468 746f 6b65 6e60  h...``authtoken`
-0000b640: 6094 6807 5d94 6816 8c09 6175 7468 746f  `.h.].h...authto
-0000b650: 6b65 6e94 8594 8194 7d94 2868 1b6a c30c  ken.....}.(h.j..
-0000b660: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-0000b670: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-0000b680: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
-0000b690: bb0c 0000 7562 6568 1f7d 9428 6821 5d94  ....ubeh.}.(h!].
-0000b6a0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-0000b6b0: 7568 2b68 0f68 1b6a b80c 0000 681c 6803  uh+h.h.j....h.h.
-0000b6c0: 681d 682c 681e 4d06 0175 6268 ee29 8194  h.h,h.M..ubh.)..
-0000b6d0: 7d94 2868 0558 2801 0000 5275 6e6e 696e  }.(h.X(...Runnin
-0000b6e0: 6720 6060 6e67 726f 6b60 6020 7769 7468  g ``ngrok`` with
-0000b6f0: 2061 6e20 6175 7468 2074 6f6b 656e 2065   an auth token e
-0000b700: 6e61 626c 6573 2061 6464 6974 696f 6e61  nables additiona
-0000b710: 6c20 6665 6174 7572 6573 2061 7661 696c  l features avail
-0000b720: 6162 6c65 206f 6e20 6f75 7220 6163 636f  able on our acco
-0000b730: 756e 7420 2866 6f72 0a69 6e73 7461 6e63  unt (for.instanc
-0000b740: 652c 2074 6865 2061 6269 6c69 7479 2074  e, the ability t
-0000b750: 6f20 6f70 656e 206d 756c 7469 706c 6520  o open multiple 
-0000b760: 7475 6e6e 656c 7320 636f 6e63 7572 7265  tunnels concurre
-0000b770: 6e74 6c79 292e 2057 6520 6361 6e20 6f62  ntly). We can ob
-0000b780: 7461 696e 206f 7572 2061 7574 6820 746f  tain our auth to
-0000b790: 6b65 6e20 6672 6f6d 0a74 6865 2060 6e67  ken from.the `ng
-0000b7a0: 726f 6b20 6461 7368 626f 6172 6420 3c68  rok dashboard <h
-0000b7b0: 7474 7073 3a2f 2f64 6173 6862 6f61 7264  ttps://dashboard
-0000b7c0: 2e6e 6772 6f6b 2e63 6f6d 3e60 5f20 616e  .ngrok.com>`_ an
-0000b7d0: 6420 696e 7374 616c 6c20 6974 2074 6f20  d install it to 
-0000b7e0: 6060 6e67 726f 6b60 6027 7320 636f 6e66  ``ngrok``'s conf
-0000b7f0: 6967 2066 696c 6520 6c69 6b65 2074 6869  ig file like thi
-0000b800: 733a 9468 075d 9428 6816 8c08 5275 6e6e  s:.h.].(h...Runn
-0000b810: 696e 6720 9485 9481 947d 9428 681b 6ad7  ing .....}.(h.j.
-0000b820: 0c00 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-0000b830: f429 8194 7d94 2868 058c 0960 606e 6772  .)..}.(h...``ngr
-0000b840: 6f6b 6060 9468 075d 9468 168c 056e 6772  ok``.h.].h...ngr
-0000b850: 6f6b 9485 9481 947d 9428 681b 6adf 0c00  ok.....}.(h.j...
-0000b860: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-0000b870: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-0000b880: 275d 9468 295d 9475 682b 68f3 681b 6ad7  '].h)].uh+h.h.j.
-0000b890: 0c00 0075 6268 168c b220 7769 7468 2061  ...ubh... with a
-0000b8a0: 6e20 6175 7468 2074 6f6b 656e 2065 6e61  n auth token ena
-0000b8b0: 626c 6573 2061 6464 6974 696f 6e61 6c20  bles additional 
-0000b8c0: 6665 6174 7572 6573 2061 7661 696c 6162  features availab
-0000b8d0: 6c65 206f 6e20 6f75 7220 6163 636f 756e  le on our accoun
-0000b8e0: 7420 2866 6f72 0a69 6e73 7461 6e63 652c  t (for.instance,
-0000b8f0: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
-0000b900: 6f70 656e 206d 756c 7469 706c 6520 7475  open multiple tu
-0000b910: 6e6e 656c 7320 636f 6e63 7572 7265 6e74  nnels concurrent
-0000b920: 6c79 292e 2057 6520 6361 6e20 6f62 7461  ly). We can obta
-0000b930: 696e 206f 7572 2061 7574 6820 746f 6b65  in our auth toke
-0000b940: 6e20 6672 6f6d 0a74 6865 2094 8594 8194  n from.the .....
-0000b950: 7d94 2868 1b6a d70c 0000 681c 6803 681d  }.(h.j....h.h.h.
-0000b960: 4e68 1e4e 7562 6843 2981 947d 9428 6805  Nh.NubhC)..}.(h.
-0000b970: 8c30 606e 6772 6f6b 2064 6173 6862 6f61  .0`ngrok dashboa
-0000b980: 7264 203c 6874 7470 733a 2f2f 6461 7368  rd <https://dash
-0000b990: 626f 6172 642e 6e67 726f 6b2e 636f 6d3e  board.ngrok.com>
-0000b9a0: 605f 9468 075d 9468 168c 0f6e 6772 6f6b  `_.h.].h...ngrok
-0000b9b0: 2064 6173 6862 6f61 7264 9485 9481 947d   dashboard.....}
-0000b9c0: 9428 681b 6af1 0c00 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-0000b9d0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-0000b9e0: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
-0000b9f0: 046e 616d 6594 8c0f 6e67 726f 6b20 6461  .name...ngrok da
-0000ba00: 7368 626f 6172 6494 6a45 0100 008c 1b68  shboard.jE.....h
-0000ba10: 7474 7073 3a2f 2f64 6173 6862 6f61 7264  ttps://dashboard
-0000ba20: 2e6e 6772 6f6b 2e63 6f6d 9475 682b 6842  .ngrok.com.uh+hB
-0000ba30: 681b 6ad7 0c00 0075 626a 4801 0000 2981  h.j....ubjH...).
-0000ba40: 947d 9428 6805 8c1e 203c 6874 7470 733a  .}.(h... <https:
-0000ba50: 2f2f 6461 7368 626f 6172 642e 6e67 726f  //dashboard.ngro
-0000ba60: 6b2e 636f 6d3e 9468 075d 9468 1f7d 9428  k.com>.h.].h.}.(
-0000ba70: 6821 5d94 8c0f 6e67 726f 6b2d 6461 7368  h!]...ngrok-dash
-0000ba80: 626f 6172 6494 6168 235d 9468 255d 948c  board.ah#].h%]..
-0000ba90: 0f6e 6772 6f6b 2064 6173 6862 6f61 7264  .ngrok dashboard
-0000baa0: 9461 6827 5d94 6829 5d94 8c06 7265 6675  .ah'].h)]...refu
-0000bab0: 7269 946a 010d 0000 7568 2b6a 4701 0000  ri.j....uh+jG...
-0000bac0: 6a56 0100 004b 0168 1b6a d70c 0000 7562  jV...K.h.j....ub
-0000bad0: 6816 8c13 2061 6e64 2069 6e73 7461 6c6c  h... and install
-0000bae0: 2069 7420 746f 2094 8594 8194 7d94 2868   it to .....}.(h
-0000baf0: 1b6a d70c 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-0000bb00: 7562 68f4 2981 947d 9428 6805 8c09 6060  ubh.)..}.(h...``
-0000bb10: 6e67 726f 6b60 6094 6807 5d94 6816 8c05  ngrok``.h.].h...
-0000bb20: 6e67 726f 6b94 8594 8194 7d94 2868 1b6a  ngrok.....}.(h.j
-0000bb30: 130d 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-0000bb40: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-0000bb50: 5d94 6827 5d94 6829 5d94 7568 2b68 f368  ].h'].h)].uh+h.h
-0000bb60: 1b6a d70c 0000 7562 6816 8c1b e280 9973  .j....ubh......s
-0000bb70: 2063 6f6e 6669 6720 6669 6c65 206c 696b   config file lik
-0000bb80: 6520 7468 6973 3a94 8594 8194 7d94 2868  e this:.....}.(h
-0000bb90: 1b6a d70c 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-0000bba0: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-0000bbb0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-0000bbc0: ed68 1d68 2c68 1e4d 0801 681b 6ab8 0c00  .h.h,h.M..h.j...
-0000bbd0: 0068 1c68 0375 626a d501 0000 2981 947d  .h.h.ubj....)..}
-0000bbe0: 9428 6805 586e 0100 0066 726f 6d20 7079  .(h.Xn...from py
-0000bbf0: 6e67 726f 6b20 696d 706f 7274 206e 6772  ngrok import ngr
-0000bc00: 6f6b 0a0a 2320 5365 7474 696e 6720 616e  ok..# Setting an
-0000bc10: 2061 7574 6820 746f 6b65 6e20 616c 6c6f   auth token allo
-0000bc20: 7773 2075 7320 746f 206f 7065 6e20 6d75  ws us to open mu
-0000bc30: 6c74 6970 6c65 0a23 2074 756e 6e65 6c73  ltiple.# tunnels
-0000bc40: 2061 7420 7468 6520 7361 6d65 2074 696d   at the same tim
-0000bc50: 650a 6e67 726f 6b2e 7365 745f 6175 7468  e.ngrok.set_auth
-0000bc60: 5f74 6f6b 656e 2822 3c4e 4752 4f4b 5f41  _token("<NGROK_A
-0000bc70: 5554 485f 544f 4b45 4e3e 2229 0a0a 2320  UTH_TOKEN>")..# 
-0000bc80: 3c4e 6772 6f6b 5475 6e6e 656c 3a20 2268  <NgrokTunnel: "h
-0000bc90: 7474 703a 2f2f 3c70 7562 6c69 635f 7375  ttp://<public_su
-0000bca0: 6231 3e2e 6e67 726f 6b2e 696f 2220 2d3e  b1>.ngrok.io" ->
-0000bcb0: 2022 6874 7470 3a2f 2f6c 6f63 616c 686f   "http://localho
-0000bcc0: 7374 3a38 3022 3e0a 6e67 726f 6b5f 7475  st:80">.ngrok_tu
-0000bcd0: 6e6e 656c 3120 3d20 6e67 726f 6b2e 636f  nnel1 = ngrok.co
-0000bce0: 6e6e 6563 7428 290a 2320 3c4e 6772 6f6b  nnect().# <Ngrok
-0000bcf0: 5475 6e6e 656c 3a20 2268 7474 703a 2f2f  Tunnel: "http://
-0000bd00: 3c70 7562 6c69 635f 7375 6232 3e2e 6e67  <public_sub2>.ng
-0000bd10: 726f 6b2e 696f 2220 2d3e 2022 6874 7470  rok.io" -> "http
-0000bd20: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3030  ://localhost:800
-0000bd30: 3022 3e0a 6e67 726f 6b5f 7475 6e6e 656c  0">.ngrok_tunnel
-0000bd40: 3220 3d20 6e67 726f 6b2e 636f 6e6e 6563  2 = ngrok.connec
-0000bd50: 7428 3830 3030 2994 6807 5d94 6816 586e  t(8000).h.].h.Xn
-0000bd60: 0100 0066 726f 6d20 7079 6e67 726f 6b20  ...from pyngrok 
-0000bd70: 696d 706f 7274 206e 6772 6f6b 0a0a 2320  import ngrok..# 
-0000bd80: 5365 7474 696e 6720 616e 2061 7574 6820  Setting an auth 
-0000bd90: 746f 6b65 6e20 616c 6c6f 7773 2075 7320  token allows us 
-0000bda0: 746f 206f 7065 6e20 6d75 6c74 6970 6c65  to open multiple
-0000bdb0: 0a23 2074 756e 6e65 6c73 2061 7420 7468  .# tunnels at th
-0000bdc0: 6520 7361 6d65 2074 696d 650a 6e67 726f  e same time.ngro
-0000bdd0: 6b2e 7365 745f 6175 7468 5f74 6f6b 656e  k.set_auth_token
-0000bde0: 2822 3c4e 4752 4f4b 5f41 5554 485f 544f  ("<NGROK_AUTH_TO
-0000bdf0: 4b45 4e3e 2229 0a0a 2320 3c4e 6772 6f6b  KEN>")..# <Ngrok
-0000be00: 5475 6e6e 656c 3a20 2268 7474 703a 2f2f  Tunnel: "http://
-0000be10: 3c70 7562 6c69 635f 7375 6231 3e2e 6e67  <public_sub1>.ng
-0000be20: 726f 6b2e 696f 2220 2d3e 2022 6874 7470  rok.io" -> "http
-0000be30: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3022  ://localhost:80"
-0000be40: 3e0a 6e67 726f 6b5f 7475 6e6e 656c 3120  >.ngrok_tunnel1 
-0000be50: 3d20 6e67 726f 6b2e 636f 6e6e 6563 7428  = ngrok.connect(
-0000be60: 290a 2320 3c4e 6772 6f6b 5475 6e6e 656c  ).# <NgrokTunnel
-0000be70: 3a20 2268 7474 703a 2f2f 3c70 7562 6c69  : "http://<publi
-0000be80: 635f 7375 6232 3e2e 6e67 726f 6b2e 696f  c_sub2>.ngrok.io
-0000be90: 2220 2d3e 2022 6874 7470 3a2f 2f6c 6f63  " -> "http://loc
-0000bea0: 616c 686f 7374 3a38 3030 3022 3e0a 6e67  alhost:8000">.ng
-0000beb0: 726f 6b5f 7475 6e6e 656c 3220 3d20 6e67  rok_tunnel2 = ng
-0000bec0: 726f 6b2e 636f 6e6e 6563 7428 3830 3030  rok.connect(8000
-0000bed0: 2994 8594 8194 7d94 681b 6a2b 0d00 0073  ).....}.h.j+...s
-0000bee0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-0000bef0: 255d 9468 275d 9468 295d 946a e401 0000  %].h'].h)].j....
-0000bf00: 6ae5 0100 006a e601 0000 896a e701 0000  j....j.....j....
-0000bf10: 8c06 7079 7468 6f6e 946a e901 0000 7d94  ..python.j....}.
-0000bf20: 7568 2b6a d401 0000 681d 682c 681e 4d0c  uh+j....h.h,h.M.
-0000bf30: 0168 1b6a b80c 0000 681c 6803 7562 68ee  .h.j....h.h.ubh.
-0000bf40: 2981 947d 9428 6805 8c61 5765 2063 616e  )..}.(h..aWe can
-0000bf50: 2061 6c73 6f20 6f76 6572 7269 6465 2060   also override `
-0000bf60: 606e 6772 6f6b 6060 2773 2069 6e73 7461  `ngrok``'s insta
-0000bf70: 6c6c 6564 2061 7574 6820 746f 6b65 6e20  lled auth token 
-0000bf80: 7573 696e 6720 3a63 6c61 7373 3a60 7e70  using :class:`~p
-0000bf90: 796e 6772 6f6b 2e63 6f6e 662e 5079 6e67  yngrok.conf.Pyng
-0000bfa0: 726f 6b43 6f6e 6669 6760 3a94 6807 5d94  rokConfig`:.h.].
-0000bfb0: 2868 168c 1557 6520 6361 6e20 616c 736f  (h...We can also
-0000bfc0: 206f 7665 7272 6964 6520 9485 9481 947d   override .....}
-0000bfd0: 9428 681b 6a3b 0d00 0068 1c68 0368 1d4e  .(h.j;...h.h.h.N
-0000bfe0: 681e 4e75 6268 f429 8194 7d94 2868 058c  h.Nubh.)..}.(h..
-0000bff0: 0960 606e 6772 6f6b 6060 9468 075d 9468  .``ngrok``.h.].h
-0000c000: 168c 056e 6772 6f6b 9485 9481 947d 9428  ...ngrok.....}.(
-0000c010: 681b 6a43 0d00 0068 1c68 0368 1d4e 681e  h.jC...h.h.h.Nh.
-0000c020: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-0000c030: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-0000c040: 68f3 681b 6a3b 0d00 0075 6268 168c 20e2  h.h.j;...ubh.. .
-0000c050: 8099 7320 696e 7374 616c 6c65 6420 6175  ..s installed au
-0000c060: 7468 2074 6f6b 656e 2075 7369 6e67 2094  th token using .
-0000c070: 8594 8194 7d94 2868 1b6a 3b0d 0000 681c  ....}.(h.j;...h.
-0000c080: 6803 681d 4e68 1e4e 7562 6ab3 0200 0029  h.h.Nh.Nubj....)
-0000c090: 8194 7d94 2868 058c 243a 636c 6173 733a  ..}.(h..$:class:
-0000c0a0: 607e 7079 6e67 726f 6b2e 636f 6e66 2e50  `~pyngrok.conf.P
-0000c0b0: 796e 6772 6f6b 436f 6e66 6967 6094 6807  yngrokConfig`.h.
-0000c0c0: 5d94 68f4 2981 947d 9428 6805 6a57 0d00  ].h.)..}.(h.jW..
-0000c0d0: 0068 075d 9468 168c 0d50 796e 6772 6f6b  .h.].h...Pyngrok
-0000c0e0: 436f 6e66 6967 9485 9481 947d 9428 681b  Config.....}.(h.
-0000c0f0: 6a59 0d00 0068 1c68 0368 1d4e 681e 4e75  jY...h.h.h.Nh.Nu
-0000c100: 6261 681f 7d94 2868 215d 9468 235d 9428  bah.}.(h!].h#].(
-0000c110: 6ac2 0200 008c 0270 7994 8c08 7079 2d63  j......py...py-c
-0000c120: 6c61 7373 9465 6825 5d94 6827 5d94 6829  lass.eh%].h'].h)
-0000c130: 5d94 7568 2b68 f368 1b6a 550d 0000 7562  ].uh+h.h.jU...ub
-0000c140: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-0000c150: 5d94 6827 5d94 6829 5d94 8c06 7265 6664  ].h'].h)]...refd
-0000c160: 6f63 946a cf02 0000 8c09 7265 6664 6f6d  oc.j......refdom
-0000c170: 6169 6e94 6a63 0d00 008c 0772 6566 7479  ain.jc.....refty
-0000c180: 7065 948c 0563 6c61 7373 948c 0b72 6566  pe...class...ref
-0000c190: 6578 706c 6963 6974 9489 8c07 7265 6677  explicit....refw
-0000c1a0: 6172 6e94 896a d502 0000 4e6a d602 0000  arn..j....Nj....
-0000c1b0: 4e6a d702 0000 8c1a 7079 6e67 726f 6b2e  Nj......pyngrok.
-0000c1c0: 636f 6e66 2e50 796e 6772 6f6b 436f 6e66  conf.PyngrokConf
-0000c1d0: 6967 9475 682b 6ab2 0200 0068 1d68 2c68  ig.uh+j....h.h,h
-0000c1e0: 1e4d 1901 681b 6a3b 0d00 0075 6268 168c  .M..h.j;...ubh..
-0000c1f0: 013a 9485 9481 947d 9428 681b 6a3b 0d00  .:.....}.(h.j;..
-0000c200: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-0000c210: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-0000c220: 275d 9468 295d 9475 682b 68ed 681d 682c  '].h)].uh+h.h.h,
-0000c230: 681e 4d19 0168 1b6a b80c 0000 681c 6803  h.M..h.j....h.h.
-0000c240: 7562 6ad5 0100 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-0000c250: be66 726f 6d20 7079 6e67 726f 6b20 696d  .from pyngrok im
-0000c260: 706f 7274 2063 6f6e 662c 206e 6772 6f6b  port conf, ngrok
-0000c270: 0a0a 636f 6e66 2e67 6574 5f64 6566 6175  ..conf.get_defau
-0000c280: 6c74 2829 2e61 7574 685f 746f 6b65 6e20  lt().auth_token 
-0000c290: 3d20 223c 4e47 524f 4b5f 4155 5448 5f54  = "<NGROK_AUTH_T
-0000c2a0: 4f4b 454e 3e22 0a0a 2320 3c4e 6772 6f6b  OKEN>"..# <Ngrok
-0000c2b0: 5475 6e6e 656c 3a20 2268 7474 703a 2f2f  Tunnel: "http://
-0000c2c0: 3c70 7562 6c69 635f 7375 623e 2e6e 6772  <public_sub>.ngr
-0000c2d0: 6f6b 2e69 6f22 202d 3e20 2268 7474 703a  ok.io" -> "http:
-0000c2e0: 2f2f 6c6f 6361 6c68 6f73 743a 3830 223e  //localhost:80">
-0000c2f0: 0a6e 6772 6f6b 5f74 756e 6e65 6c20 3d20  .ngrok_tunnel = 
-0000c300: 6e67 726f 6b2e 636f 6e6e 6563 7428 2994  ngrok.connect().
-0000c310: 6807 5d94 6816 8cbe 6672 6f6d 2070 796e  h.].h...from pyn
-0000c320: 6772 6f6b 2069 6d70 6f72 7420 636f 6e66  grok import conf
-0000c330: 2c20 6e67 726f 6b0a 0a63 6f6e 662e 6765  , ngrok..conf.ge
-0000c340: 745f 6465 6661 756c 7428 292e 6175 7468  t_default().auth
-0000c350: 5f74 6f6b 656e 203d 2022 3c4e 4752 4f4b  _token = "<NGROK
-0000c360: 5f41 5554 485f 544f 4b45 4e3e 220a 0a23  _AUTH_TOKEN>"..#
-0000c370: 203c 4e67 726f 6b54 756e 6e65 6c3a 2022   <NgrokTunnel: "
-0000c380: 6874 7470 3a2f 2f3c 7075 626c 6963 5f73  http://<public_s
-0000c390: 7562 3e2e 6e67 726f 6b2e 696f 2220 2d3e  ub>.ngrok.io" ->
-0000c3a0: 2022 6874 7470 3a2f 2f6c 6f63 616c 686f   "http://localho
-0000c3b0: 7374 3a38 3022 3e0a 6e67 726f 6b5f 7475  st:80">.ngrok_tu
-0000c3c0: 6e6e 656c 203d 206e 6772 6f6b 2e63 6f6e  nnel = ngrok.con
-0000c3d0: 6e65 6374 2829 9485 9481 947d 9468 1b6a  nect().....}.h.j
-0000c3e0: 7f0d 0000 7362 6168 1f7d 9428 6821 5d94  ....sbah.}.(h!].
-0000c3f0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-0000c400: 6ae4 0100 006a e501 0000 6ae6 0100 0089  j....j....j.....
-0000c410: 6ae7 0100 008c 0670 7974 686f 6e94 6ae9  j......python.j.
-0000c420: 0100 007d 9475 682b 6ad4 0100 0068 1d68  ...}.uh+j....h.h
-0000c430: 2c68 1e4d 1b01 681b 6ab8 0c00 0068 1c68  ,h.M..h.j....h.h
-0000c440: 0375 6265 681f 7d94 2868 215d 948c 1573  .ubeh.}.(h!]...s
-0000c450: 6574 7469 6e67 2d74 6865 2d61 7574 6874  etting-the-autht
-0000c460: 6f6b 656e 9461 6823 5d94 6825 5d94 8c15  oken.ah#].h%]...
-0000c470: 7365 7474 696e 6720 7468 6520 6175 7468  setting the auth
-0000c480: 746f 6b65 6e94 6168 275d 9468 295d 9475  token.ah'].h)].u
-0000c490: 682b 680a 681b 6a75 0900 0068 1c68 0368  h+h.h.ju...h.h.h
-0000c4a0: 1d68 2c68 1e4d 0601 7562 680b 2981 947d  .h,h.M..ubh.)..}
-0000c4b0: 9428 6805 6806 6807 5d94 2868 1029 8194  .(h.h.h.].(h.)..
-0000c4c0: 7d94 2868 058c 1653 6574 7469 6e67 2074  }.(h...Setting t
-0000c4d0: 6865 2060 6072 6567 696f 6e60 6094 6807  he ``region``.h.
-0000c4e0: 5d94 2868 168c 0c53 6574 7469 6e67 2074  ].(h...Setting t
-0000c4f0: 6865 2094 8594 8194 7d94 2868 1b6a 9a0d  he .....}.(h.j..
-0000c500: 0000 681c 6803 681d 4e68 1e4e 7562 68f4  ..h.h.h.Nh.Nubh.
-0000c510: 2981 947d 9428 6805 8c0a 6060 7265 6769  )..}.(h...``regi
-0000c520: 6f6e 6060 9468 075d 9468 168c 0672 6567  on``.h.].h...reg
-0000c530: 696f 6e94 8594 8194 7d94 2868 1b6a a20d  ion.....}.(h.j..
-0000c540: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-0000c550: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-0000c560: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
-0000c570: 9a0d 0000 7562 6568 1f7d 9428 6821 5d94  ....ubeh.}.(h!].
-0000c580: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-0000c590: 7568 2b68 0f68 1b6a 970d 0000 681c 6803  uh+h.h.j....h.h.
-0000c5a0: 681d 682c 681e 4d25 0175 6268 ee29 8194  h.h,h.M%.ubh.)..
-0000c5b0: 7d94 2868 058c 9642 7920 6465 6661 756c  }.(h...By defaul
-0000c5c0: 742c 2060 606e 6772 6f6b 6060 2077 696c  t, ``ngrok`` wil
-0000c5d0: 6c20 6f70 656e 2061 2074 756e 6e65 6c20  l open a tunnel 
-0000c5e0: 696e 2074 6865 2060 6075 7360 6020 7265  in the ``us`` re
-0000c5f0: 6769 6f6e 2e20 546f 206f 7665 7272 6964  gion. To overrid
-0000c600: 6520 7468 6973 2c20 7573 650a 7468 6520  e this, use.the 
-0000c610: 6060 7265 6769 6f6e 6060 2070 6172 616d  ``region`` param
-0000c620: 6574 6572 2069 6e20 3a63 6c61 7373 3a60  eter in :class:`
-0000c630: 7e70 796e 6772 6f6b 2e63 6f6e 662e 5079  ~pyngrok.conf.Py
-0000c640: 6e67 726f 6b43 6f6e 6669 6760 3a94 6807  ngrokConfig`:.h.
-0000c650: 5d94 2868 168c 0c42 7920 6465 6661 756c  ].(h...By defaul
-0000c660: 742c 2094 8594 8194 7d94 2868 1b6a b60d  t, .....}.(h.j..
-0000c670: 0000 681c 6803 681d 4e68 1e4e 7562 68f4  ..h.h.h.Nh.Nubh.
-0000c680: 2981 947d 9428 6805 8c09 6060 6e67 726f  )..}.(h...``ngro
-0000c690: 6b60 6094 6807 5d94 6816 8c05 6e67 726f  k``.h.].h...ngro
-0000c6a0: 6b94 8594 8194 7d94 2868 1b6a be0d 0000  k.....}.(h.j....
-0000c6b0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-0000c6c0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-0000c6d0: 5d94 6829 5d94 7568 2b68 f368 1b6a b60d  ].h)].uh+h.h.j..
-0000c6e0: 0000 7562 6816 8c1b 2077 696c 6c20 6f70  ..ubh... will op
-0000c6f0: 656e 2061 2074 756e 6e65 6c20 696e 2074  en a tunnel in t
-0000c700: 6865 2094 8594 8194 7d94 2868 1b6a b60d  he .....}.(h.j..
-0000c710: 0000 681c 6803 681d 4e68 1e4e 7562 68f4  ..h.h.h.Nh.Nubh.
-0000c720: 2981 947d 9428 6805 8c06 6060 7573 6060  )..}.(h...``us``
-0000c730: 9468 075d 9468 168c 0275 7394 8594 8194  .h.].h...us.....
-0000c740: 7d94 2868 1b6a d00d 0000 681c 6803 681d  }.(h.j....h.h.h.
-0000c750: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-0000c760: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-0000c770: 7568 2b68 f368 1b6a b60d 0000 7562 6816  uh+h.h.j....ubh.
-0000c780: 8c23 2072 6567 696f 6e2e 2054 6f20 6f76  .# region. To ov
-0000c790: 6572 7269 6465 2074 6869 732c 2075 7365  erride this, use
-0000c7a0: 0a74 6865 2094 8594 8194 7d94 2868 1b6a  .the .....}.(h.j
-0000c7b0: b60d 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-0000c7c0: 68f4 2981 947d 9428 6805 8c0a 6060 7265  h.)..}.(h...``re
-0000c7d0: 6769 6f6e 6060 9468 075d 9468 168c 0672  gion``.h.].h...r
-0000c7e0: 6567 696f 6e94 8594 8194 7d94 2868 1b6a  egion.....}.(h.j
-0000c7f0: e20d 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-0000c800: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-0000c810: 5d94 6827 5d94 6829 5d94 7568 2b68 f368  ].h'].h)].uh+h.h
-0000c820: 1b6a b60d 0000 7562 6816 8c0e 2070 6172  .j....ubh... par
-0000c830: 616d 6574 6572 2069 6e20 9485 9481 947d  ameter in .....}
-0000c840: 9428 681b 6ab6 0d00 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-0000c850: 681e 4e75 626a b302 0000 2981 947d 9428  h.Nubj....)..}.(
-0000c860: 6805 8c24 3a63 6c61 7373 3a60 7e70 796e  h..$:class:`~pyn
-0000c870: 6772 6f6b 2e63 6f6e 662e 5079 6e67 726f  grok.conf.Pyngro
-0000c880: 6b43 6f6e 6669 6760 9468 075d 9468 f429  kConfig`.h.].h.)
-0000c890: 8194 7d94 2868 056a f60d 0000 6807 5d94  ..}.(h.j....h.].
-0000c8a0: 6816 8c0d 5079 6e67 726f 6b43 6f6e 6669  h...PyngrokConfi
-0000c8b0: 6794 8594 8194 7d94 2868 1b6a f80d 0000  g.....}.(h.j....
-0000c8c0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-0000c8d0: 9428 6821 5d94 6823 5d94 286a c202 0000  .(h!].h#].(j....
-0000c8e0: 8c02 7079 948c 0870 792d 636c 6173 7394  ..py...py-class.
-0000c8f0: 6568 255d 9468 275d 9468 295d 9475 682b  eh%].h'].h)].uh+
-0000c900: 68f3 681b 6af4 0d00 0075 6261 681f 7d94  h.h.j....ubah.}.
-0000c910: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000c920: 9468 295d 948c 0672 6566 646f 6394 6acf  .h)]...refdoc.j.
-0000c930: 0200 008c 0972 6566 646f 6d61 696e 946a  .....refdomain.j
-0000c940: 020e 0000 8c07 7265 6674 7970 6594 8c05  ......reftype...
-0000c950: 636c 6173 7394 8c0b 7265 6665 7870 6c69  class...refexpli
-0000c960: 6369 7494 898c 0772 6566 7761 726e 9489  cit....refwarn..
-0000c970: 6ad5 0200 004e 6ad6 0200 004e 6ad7 0200  j....Nj....Nj...
-0000c980: 008c 1a70 796e 6772 6f6b 2e63 6f6e 662e  ...pyngrok.conf.
-0000c990: 5079 6e67 726f 6b43 6f6e 6669 6794 7568  PyngrokConfig.uh
-0000c9a0: 2b6a b202 0000 681d 682c 681e 4d27 0168  +j....h.h,h.M'.h
-0000c9b0: 1b6a b60d 0000 7562 6816 8c01 3a94 8594  .j....ubh...:...
-0000c9c0: 8194 7d94 2868 1b6a b60d 0000 681c 6803  ..}.(h.j....h.h.
-0000c9d0: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
-0000c9e0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-0000c9f0: 5d94 7568 2b68 ed68 1d68 2c68 1e4d 2701  ].uh+h.h.h,h.M'.
-0000ca00: 681b 6a97 0d00 0068 1c68 0375 626a d501  h.j....h.h.ubj..
-0000ca10: 0000 2981 947d 9428 6805 8cad 6672 6f6d  ..)..}.(h...from
-0000ca20: 2070 796e 6772 6f6b 2069 6d70 6f72 7420   pyngrok import 
-0000ca30: 636f 6e66 2c20 6e67 726f 6b0a 0a63 6f6e  conf, ngrok..con
-0000ca40: 662e 6765 745f 6465 6661 756c 7428 292e  f.get_default().
-0000ca50: 7265 6769 6f6e 203d 2022 6175 220a 0a23  region = "au"..#
-0000ca60: 203c 4e67 726f 6b54 756e 6e65 6c3a 2022   <NgrokTunnel: "
-0000ca70: 6874 7470 3a2f 2f3c 7075 626c 6963 5f73  http://<public_s
-0000ca80: 7562 3e2e 6175 2e6e 6772 6f6b 2e69 6f22  ub>.au.ngrok.io"
-0000ca90: 202d 3e20 2268 7474 703a 2f2f 6c6f 6361   -> "http://loca
-0000caa0: 6c68 6f73 743a 3830 223e 0a6e 6772 6f6b  lhost:80">.ngrok
-0000cab0: 5f74 756e 6e65 6c20 3d20 6e67 726f 6b2e  _tunnel = ngrok.
-0000cac0: 636f 6e6e 6563 7428 2994 6807 5d94 6816  connect().h.].h.
-0000cad0: 8cad 6672 6f6d 2070 796e 6772 6f6b 2069  ..from pyngrok i
-0000cae0: 6d70 6f72 7420 636f 6e66 2c20 6e67 726f  mport conf, ngro
-0000caf0: 6b0a 0a63 6f6e 662e 6765 745f 6465 6661  k..conf.get_defa
-0000cb00: 756c 7428 292e 7265 6769 6f6e 203d 2022  ult().region = "
-0000cb10: 6175 220a 0a23 203c 4e67 726f 6b54 756e  au"..# <NgrokTun
-0000cb20: 6e65 6c3a 2022 6874 7470 3a2f 2f3c 7075  nel: "http://<pu
-0000cb30: 626c 6963 5f73 7562 3e2e 6175 2e6e 6772  blic_sub>.au.ngr
-0000cb40: 6f6b 2e69 6f22 202d 3e20 2268 7474 703a  ok.io" -> "http:
-0000cb50: 2f2f 6c6f 6361 6c68 6f73 743a 3830 223e  //localhost:80">
-0000cb60: 0a6e 6772 6f6b 5f74 756e 6e65 6c20 3d20  .ngrok_tunnel = 
-0000cb70: 6e67 726f 6b2e 636f 6e6e 6563 7428 2994  ngrok.connect().
-0000cb80: 8594 8194 7d94 681b 6a1e 0e00 0073 6261  ....}.h.j....sba
-0000cb90: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-0000cba0: 9468 275d 9468 295d 946a e401 0000 6ae5  .h'].h)].j....j.
-0000cbb0: 0100 006a e601 0000 896a e701 0000 8c06  ...j.....j......
-0000cbc0: 7079 7468 6f6e 946a e901 0000 7d94 7568  python.j....}.uh
-0000cbd0: 2b6a d401 0000 681d 682c 681e 4d2a 0168  +j....h.h,h.M*.h
-0000cbe0: 1b6a 970d 0000 681c 6803 7562 6568 1f7d  .j....h.h.ubeh.}
-0000cbf0: 9428 6821 5d94 8c12 7365 7474 696e 672d  .(h!]...setting-
-0000cc00: 7468 652d 7265 6769 6f6e 9461 6823 5d94  the-region.ah#].
-0000cc10: 6825 5d94 8c12 7365 7474 696e 6720 7468  h%]...setting th
-0000cc20: 6520 7265 6769 6f6e 9461 6827 5d94 6829  e region.ah'].h)
-0000cc30: 5d94 7568 2b68 0a68 1b6a 7509 0000 681c  ].uh+h.h.ju...h.
-0000cc40: 6803 681d 682c 681e 4d25 0175 6268 0b29  h.h.h,h.M%.ubh.)
-0000cc50: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
-0000cc60: 2981 947d 9428 6805 8c21 5061 7373 696e  )..}.(h..!Passin
-0000cc70: 6720 6060 6f70 7469 6f6e 7360 6020 6173  g ``options`` as
-0000cc80: 2060 606b 7761 7267 7360 6094 6807 5d94   ``kwargs``.h.].
-0000cc90: 2868 168c 0850 6173 7369 6e67 2094 8594  (h...Passing ...
-0000cca0: 8194 7d94 2868 1b6a 390e 0000 681c 6803  ..}.(h.j9...h.h.
-0000ccb0: 681d 4e68 1e4e 7562 68f4 2981 947d 9428  h.Nh.Nubh.)..}.(
-0000ccc0: 6805 8c0b 6060 6f70 7469 6f6e 7360 6094  h...``options``.
-0000ccd0: 6807 5d94 6816 8c07 6f70 7469 6f6e 7394  h.].h...options.
-0000cce0: 8594 8194 7d94 2868 1b6a 410e 0000 681c  ....}.(h.jA...h.
-0000ccf0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-0000cd00: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-0000cd10: 6829 5d94 7568 2b68 f368 1b6a 390e 0000  h)].uh+h.h.j9...
-0000cd20: 7562 6816 8c04 2061 7320 9485 9481 947d  ubh... as .....}
-0000cd30: 9428 681b 6a39 0e00 0068 1c68 0368 1d4e  .(h.j9...h.h.h.N
-0000cd40: 681e 4e75 6268 f429 8194 7d94 2868 058c  h.Nubh.)..}.(h..
-0000cd50: 0a60 606b 7761 7267 7360 6094 6807 5d94  .``kwargs``.h.].
-0000cd60: 6816 8c06 6b77 6172 6773 9485 9481 947d  h...kwargs.....}
-0000cd70: 9428 681b 6a53 0e00 0068 1c68 0368 1d4e  .(h.jS...h.h.h.N
-0000cd80: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-0000cd90: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-0000cda0: 682b 68f3 681b 6a39 0e00 0075 6265 681f  h+h.h.j9...ubeh.
-0000cdb0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-0000cdc0: 275d 9468 295d 9475 682b 680f 681b 6a36  '].h)].uh+h.h.j6
-0000cdd0: 0e00 0068 1c68 0368 1d68 2c68 1e4d 3401  ...h.h.h.h,h.M4.
-0000cde0: 7562 68ee 2981 947d 9428 6805 5889 0100  ubh.)..}.(h.X...
-0000cdf0: 0049 7420 6973 2070 6f73 7369 626c 6520  .It is possible 
-0000ce00: 746f 2063 6f6e 6669 6775 7265 2074 6865  to configure the
-0000ce10: 2074 756e 6e65 6c20 7768 656e 2069 7420   tunnel when it 
-0000ce20: 6973 2063 7265 6174 6564 2c20 666f 7220  is created, for 
-0000ce30: 696e 7374 616e 6365 2061 6464 696e 6720  instance adding 
-0000ce40: 6175 7468 656e 7469 6361 7469 6f6e 2c0a  authentication,.
-0000ce50: 6120 7375 6264 6f6d 6169 6e2c 206f 7220  a subdomain, or 
-0000ce60: 6f74 6865 7220 7475 6e6e 656c 2070 726f  other tunnel pro
-0000ce70: 7065 7274 6965 7320 6073 7570 706f 7274  perties `support
-0000ce80: 6564 2062 7920 6e67 726f 6b20 3c68 7474  ed by ngrok <htt
-0000ce90: 7073 3a2f 2f6e 6772 6f6b 2e63 6f6d 2f64  ps://ngrok.com/d
-0000cea0: 6f63 732f 6e67 726f 6b2d 6167 656e 742f  ocs/ngrok-agent/
-0000ceb0: 6170 6923 7374 6172 742d 7475 6e6e 656c  api#start-tunnel
-0000cec0: 3e60 5f2e 0a54 6869 7320 6973 2061 6363  >`_..This is acc
-0000ced0: 6f6d 706c 6973 6865 6420 6279 2070 6173  omplished by pas
-0000cee0: 7369 6e67 2074 6865 7365 2060 606f 7074  sing these ``opt
-0000cef0: 696f 6e73 6060 2061 7320 6164 6469 7469  ions`` as additi
-0000cf00: 6f6e 616c 2060 606b 7761 7267 7360 6020  onal ``kwargs`` 
-0000cf10: 746f 203a 6675 6e63 3a60 7e70 796e 6772  to :func:`~pyngr
-0000cf20: 6f6b 2e6e 6772 6f6b 2e63 6f6e 6e65 6374  ok.ngrok.connect
-0000cf30: 602c 0a74 6865 6e20 7468 6579 2077 696c  `,.then they wil
-0000cf40: 6c20 6265 2075 7365 6420 6173 2070 726f  l be used as pro
-0000cf50: 7065 7274 6965 7320 666f 7220 7468 6520  perties for the 
-0000cf60: 7475 6e6e 656c 2077 6865 6e20 6974 2069  tunnel when it i
-0000cf70: 7320 6372 6561 7465 642e 9468 075d 9428  s created..h.].(
-0000cf80: 6816 8c87 4974 2069 7320 706f 7373 6962  h...It is possib
-0000cf90: 6c65 2074 6f20 636f 6e66 6967 7572 6520  le to configure 
-0000cfa0: 7468 6520 7475 6e6e 656c 2077 6865 6e20  the tunnel when 
-0000cfb0: 6974 2069 7320 6372 6561 7465 642c 2066  it is created, f
-0000cfc0: 6f72 2069 6e73 7461 6e63 6520 6164 6469  or instance addi
-0000cfd0: 6e67 2061 7574 6865 6e74 6963 6174 696f  ng authenticatio
-0000cfe0: 6e2c 0a61 2073 7562 646f 6d61 696e 2c20  n,.a subdomain, 
-0000cff0: 6f72 206f 7468 6572 2074 756e 6e65 6c20  or other tunnel 
-0000d000: 7072 6f70 6572 7469 6573 2094 8594 8194  properties .....
-0000d010: 7d94 2868 1b6a 670e 0000 681c 6803 681d  }.(h.jg...h.h.h.
-0000d020: 4e68 1e4e 7562 6843 2981 947d 9428 6805  Nh.NubhC)..}.(h.
-0000d030: 8c4b 6073 7570 706f 7274 6564 2062 7920  .K`supported by 
-0000d040: 6e67 726f 6b20 3c68 7474 7073 3a2f 2f6e  ngrok <https://n
-0000d050: 6772 6f6b 2e63 6f6d 2f64 6f63 732f 6e67  grok.com/docs/ng
-0000d060: 726f 6b2d 6167 656e 742f 6170 6923 7374  rok-agent/api#st
-0000d070: 6172 742d 7475 6e6e 656c 3e60 5f94 6807  art-tunnel>`_.h.
-0000d080: 5d94 6816 8c12 7375 7070 6f72 7465 6420  ].h...supported 
-0000d090: 6279 206e 6772 6f6b 9485 9481 947d 9428  by ngrok.....}.(
-0000d0a0: 681b 6a6f 0e00 0068 1c68 0368 1d4e 681e  h.jo...h.h.h.Nh.
-0000d0b0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-0000d0c0: 9468 255d 9468 275d 9468 295d 948c 046e  .h%].h'].h)]...n
-0000d0d0: 616d 6594 8c12 7375 7070 6f72 7465 6420  ame...supported 
-0000d0e0: 6279 206e 6772 6f6b 946a 4501 0000 8c33  by ngrok.jE....3
-0000d0f0: 6874 7470 733a 2f2f 6e67 726f 6b2e 636f  https://ngrok.co
-0000d100: 6d2f 646f 6373 2f6e 6772 6f6b 2d61 6765  m/docs/ngrok-age
-0000d110: 6e74 2f61 7069 2373 7461 7274 2d74 756e  nt/api#start-tun
-0000d120: 6e65 6c94 7568 2b68 4268 1b6a 670e 0000  nel.uh+hBh.jg...
-0000d130: 7562 6a48 0100 0029 8194 7d94 2868 058c  ubjH...)..}.(h..
-0000d140: 3620 3c68 7474 7073 3a2f 2f6e 6772 6f6b  6 <https://ngrok
-0000d150: 2e63 6f6d 2f64 6f63 732f 6e67 726f 6b2d  .com/docs/ngrok-
-0000d160: 6167 656e 742f 6170 6923 7374 6172 742d  agent/api#start-
-0000d170: 7475 6e6e 656c 3e94 6807 5d94 681f 7d94  tunnel>.h.].h.}.
-0000d180: 2868 215d 948c 0369 6431 9461 6823 5d94  (h!]...id1.ah#].
-0000d190: 6825 5d94 6827 5d94 8c12 7375 7070 6f72  h%].h']...suppor
-0000d1a0: 7465 6420 6279 206e 6772 6f6b 9461 6829  ted by ngrok.ah)
-0000d1b0: 5d94 8c06 7265 6675 7269 946a 7f0e 0000  ]...refuri.j....
-0000d1c0: 7568 2b6a 4701 0000 6a56 0100 004b 0168  uh+jG...jV...K.h
-0000d1d0: 1b6a 670e 0000 7562 6816 8c28 2e0a 5468  .jg...ubh..(..Th
-0000d1e0: 6973 2069 7320 6163 636f 6d70 6c69 7368  is is accomplish
-0000d1f0: 6564 2062 7920 7061 7373 696e 6720 7468  ed by passing th
-0000d200: 6573 6520 9485 9481 947d 9428 681b 6a67  ese .....}.(h.jg
-0000d210: 0e00 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
-0000d220: f429 8194 7d94 2868 058c 0b60 606f 7074  .)..}.(h...``opt
-0000d230: 696f 6e73 6060 9468 075d 9468 168c 076f  ions``.h.].h...o
-0000d240: 7074 696f 6e73 9485 9481 947d 9428 681b  ptions.....}.(h.
-0000d250: 6a91 0e00 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-0000d260: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-0000d270: 255d 9468 275d 9468 295d 9475 682b 68f3  %].h'].h)].uh+h.
-0000d280: 681b 6a67 0e00 0075 6268 168c 0f20 6173  h.jg...ubh... as
-0000d290: 2061 6464 6974 696f 6e61 6c20 9485 9481   additional ....
-0000d2a0: 947d 9428 681b 6a67 0e00 0068 1c68 0368  .}.(h.jg...h.h.h
-0000d2b0: 1d4e 681e 4e75 6268 f429 8194 7d94 2868  .Nh.Nubh.)..}.(h
-0000d2c0: 058c 0a60 606b 7761 7267 7360 6094 6807  ...``kwargs``.h.
-0000d2d0: 5d94 6816 8c06 6b77 6172 6773 9485 9481  ].h...kwargs....
-0000d2e0: 947d 9428 681b 6aa3 0e00 0068 1c68 0368  .}.(h.j....h.h.h
-0000d2f0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-0000d300: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-0000d310: 9475 682b 68f3 681b 6a67 0e00 0075 6268  .uh+h.h.jg...ubh
-0000d320: 168c 0420 746f 2094 8594 8194 7d94 2868  ... to .....}.(h
-0000d330: 1b6a 670e 0000 681c 6803 681d 4e68 1e4e  .jg...h.h.h.Nh.N
-0000d340: 7562 6ab3 0200 0029 8194 7d94 2868 058c  ubj....)..}.(h..
-0000d350: 1e3a 6675 6e63 3a60 7e70 796e 6772 6f6b  .:func:`~pyngrok
-0000d360: 2e6e 6772 6f6b 2e63 6f6e 6e65 6374 6094  .ngrok.connect`.
-0000d370: 6807 5d94 68f4 2981 947d 9428 6805 6ab7  h.].h.)..}.(h.j.
-0000d380: 0e00 0068 075d 9468 168c 0763 6f6e 6e65  ...h.].h...conne
-0000d390: 6374 9485 9481 947d 9428 681b 6ab9 0e00  ct.....}.(h.j...
-0000d3a0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-0000d3b0: 7d94 2868 215d 9468 235d 9428 6ac2 0200  }.(h!].h#].(j...
-0000d3c0: 008c 0270 7994 8c07 7079 2d66 756e 6394  ...py...py-func.
-0000d3d0: 6568 255d 9468 275d 9468 295d 9475 682b  eh%].h'].h)].uh+
-0000d3e0: 68f3 681b 6ab5 0e00 0075 6261 681f 7d94  h.h.j....ubah.}.
-0000d3f0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000d400: 9468 295d 948c 0672 6566 646f 6394 6acf  .h)]...refdoc.j.
-0000d410: 0200 008c 0972 6566 646f 6d61 696e 946a  .....refdomain.j
-0000d420: c30e 0000 8c07 7265 6674 7970 6594 8c04  ......reftype...
-0000d430: 6675 6e63 948c 0b72 6566 6578 706c 6963  func...refexplic
-0000d440: 6974 9489 8c07 7265 6677 6172 6e94 896a  it....refwarn..j
-0000d450: d502 0000 4e6a d602 0000 4e6a d702 0000  ....Nj....Nj....
-0000d460: 8c15 7079 6e67 726f 6b2e 6e67 726f 6b2e  ..pyngrok.ngrok.
-0000d470: 636f 6e6e 6563 7494 7568 2b6a b202 0000  connect.uh+j....
-0000d480: 681d 682c 681e 4d36 0168 1b6a 670e 0000  h.h,h.M6.h.jg...
-0000d490: 7562 6816 8c49 2c0a 7468 656e 2074 6865  ubh..I,.then the
-0000d4a0: 7920 7769 6c6c 2062 6520 7573 6564 2061  y will be used a
-0000d4b0: 7320 7072 6f70 6572 7469 6573 2066 6f72  s properties for
-0000d4c0: 2074 6865 2074 756e 6e65 6c20 7768 656e   the tunnel when
-0000d4d0: 2069 7420 6973 2063 7265 6174 6564 2e94   it is created..
-0000d4e0: 8594 8194 7d94 2868 1b6a 670e 0000 681c  ....}.(h.jg...h.
-0000d4f0: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
-0000d500: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-0000d510: 6829 5d94 7568 2b68 ed68 1d68 2c68 1e4d  h)].uh+h.h.h,h.M
-0000d520: 3601 681b 6a36 0e00 0068 1c68 0375 6268  6.h.j6...h.h.ubh
-0000d530: ee29 8194 7d94 2868 058c 9148 6572 6520  .)..}.(h...Here 
-0000d540: 6973 2061 6e20 6578 616d 706c 6520 7374  is an example st
-0000d550: 6172 7469 6e67 2060 606e 6772 6f6b 6060  arting ``ngrok``
-0000d560: 2069 6e20 4175 7374 7261 6c69 612c 2074   in Australia, t
-0000d570: 6865 6e20 6f70 656e 696e 6720 6120 7475  hen opening a tu
-0000d580: 6e6e 656c 2077 6974 6820 7375 6264 6f6d  nnel with subdom
-0000d590: 6169 6e0a 6060 666f 6f60 6020 7468 6174  ain.``foo`` that
-0000d5a0: 2072 6571 7569 7265 7320 6261 7369 6320   requires basic 
-0000d5b0: 6175 7468 656e 7469 6361 7469 6f6e 2066  authentication f
-0000d5c0: 6f72 2072 6571 7565 7374 732e 9468 075d  or requests..h.]
-0000d5d0: 9428 6816 8c1c 4865 7265 2069 7320 616e  .(h...Here is an
-0000d5e0: 2065 7861 6d70 6c65 2073 7461 7274 696e   example startin
-0000d5f0: 6720 9485 9481 947d 9428 681b 6adf 0e00  g .....}.(h.j...
-0000d600: 0068 1c68 0368 1d4e 681e 4e75 6268 f429  .h.h.h.Nh.Nubh.)
-0000d610: 8194 7d94 2868 058c 0960 606e 6772 6f6b  ..}.(h...``ngrok
-0000d620: 6060 9468 075d 9468 168c 056e 6772 6f6b  ``.h.].h...ngrok
-0000d630: 9485 9481 947d 9428 681b 6ae7 0e00 0068  .....}.(h.j....h
-0000d640: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-0000d650: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000d660: 9468 295d 9475 682b 68f3 681b 6adf 0e00  .h)].uh+h.h.j...
-0000d670: 0075 6268 168c 3420 696e 2041 7573 7472  .ubh..4 in Austr
-0000d680: 616c 6961 2c20 7468 656e 206f 7065 6e69  alia, then openi
-0000d690: 6e67 2061 2074 756e 6e65 6c20 7769 7468  ng a tunnel with
-0000d6a0: 2073 7562 646f 6d61 696e 0a94 8594 8194   subdomain......
-0000d6b0: 7d94 2868 1b6a df0e 0000 681c 6803 681d  }.(h.j....h.h.h.
-0000d6c0: 4e68 1e4e 7562 68f4 2981 947d 9428 6805  Nh.Nubh.)..}.(h.
-0000d6d0: 8c07 6060 666f 6f60 6094 6807 5d94 6816  ..``foo``.h.].h.
-0000d6e0: 8c03 666f 6f94 8594 8194 7d94 2868 1b6a  ..foo.....}.(h.j
-0000d6f0: f90e 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-0000d700: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-0000d710: 5d94 6827 5d94 6829 5d94 7568 2b68 f368  ].h'].h)].uh+h.h
-0000d720: 1b6a df0e 0000 7562 6816 8c31 2074 6861  .j....ubh..1 tha
-0000d730: 7420 7265 7175 6972 6573 2062 6173 6963  t requires basic
-0000d740: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
-0000d750: 666f 7220 7265 7175 6573 7473 2e94 8594  for requests....
-0000d760: 8194 7d94 2868 1b6a df0e 0000 681c 6803  ..}.(h.j....h.h.
-0000d770: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
-0000d780: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-0000d790: 5d94 7568 2b68 ed68 1d68 2c68 1e4d 3b01  ].uh+h.h.h,h.M;.
-0000d7a0: 681b 6a36 0e00 0068 1c68 0375 626a d501  h.j6...h.h.ubj..
-0000d7b0: 0000 2981 947d 9428 6805 8cea 6672 6f6d  ..)..}.(h...from
-0000d7c0: 2070 796e 6772 6f6b 2069 6d70 6f72 7420   pyngrok import 
-0000d7d0: 636f 6e66 2c20 6e67 726f 6b0a 0a63 6f6e  conf, ngrok..con
-0000d7e0: 662e 6765 745f 6465 6661 756c 7428 292e  f.get_default().
-0000d7f0: 7265 6769 6f6e 203d 2022 6175 220a 0a23  region = "au"..#
-0000d800: 203c 4e67 726f 6b54 756e 6e65 6c3a 2022   <NgrokTunnel: "
-0000d810: 6874 7470 3a2f 2f66 6f6f 2e61 752e 6e67  http://foo.au.ng
-0000d820: 726f 6b2e 696f 2220 2d3e 2022 6874 7470  rok.io" -> "http
-0000d830: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3022  ://localhost:80"
-0000d840: 3e0a 6e67 726f 6b5f 7475 6e6e 656c 203d  >.ngrok_tunnel =
-0000d850: 206e 6772 6f6b 2e63 6f6e 6e65 6374 2873   ngrok.connect(s
-0000d860: 7562 646f 6d61 696e 3d22 666f 6f22 2c0a  ubdomain="foo",.
-0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d880: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-0000d890: 683d 2275 7365 726e 616d 653a 7061 7373  h="username:pass
-0000d8a0: 776f 7264 2229 9468 075d 9468 168c ea66  word").h.].h...f
-0000d8b0: 726f 6d20 7079 6e67 726f 6b20 696d 706f  rom pyngrok impo
-0000d8c0: 7274 2063 6f6e 662c 206e 6772 6f6b 0a0a  rt conf, ngrok..
-0000d8d0: 636f 6e66 2e67 6574 5f64 6566 6175 6c74  conf.get_default
-0000d8e0: 2829 2e72 6567 696f 6e20 3d20 2261 7522  ().region = "au"
-0000d8f0: 0a0a 2320 3c4e 6772 6f6b 5475 6e6e 656c  ..# <NgrokTunnel
-0000d900: 3a20 2268 7474 703a 2f2f 666f 6f2e 6175  : "http://foo.au
-0000d910: 2e6e 6772 6f6b 2e69 6f22 202d 3e20 2268  .ngrok.io" -> "h
-0000d920: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-0000d930: 3830 223e 0a6e 6772 6f6b 5f74 756e 6e65  80">.ngrok_tunne
-0000d940: 6c20 3d20 6e67 726f 6b2e 636f 6e6e 6563  l = ngrok.connec
-0000d950: 7428 7375 6264 6f6d 6169 6e3d 2266 6f6f  t(subdomain="foo
-0000d960: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d980: 6175 7468 3d22 7573 6572 6e61 6d65 3a70  auth="username:p
-0000d990: 6173 7377 6f72 6422 2994 8594 8194 7d94  assword").....}.
-0000d9a0: 681b 6a11 0f00 0073 6261 681f 7d94 2868  h.j....sbah.}.(h
-0000d9b0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-0000d9c0: 295d 946a e401 0000 6ae5 0100 006a e601  )].j....j....j..
-0000d9d0: 0000 896a e701 0000 8c06 7079 7468 6f6e  ...j......python
-0000d9e0: 946a e901 0000 7d94 7568 2b6a d401 0000  .j....}.uh+j....
-0000d9f0: 681d 682c 681e 4d3e 0168 1b6a 360e 0000  h.h,h.M>.h.j6...
-0000da00: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-0000da10: 8c19 7061 7373 696e 672d 6f70 7469 6f6e  ..passing-option
-0000da20: 732d 6173 2d6b 7761 7267 7394 6168 235d  s-as-kwargs.ah#]
-0000da30: 9468 255d 948c 1970 6173 7369 6e67 206f  .h%]...passing o
-0000da40: 7074 696f 6e73 2061 7320 6b77 6172 6773  ptions as kwargs
-0000da50: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
-0000da60: 1b6a 7509 0000 681c 6803 681d 682c 681e  .ju...h.h.h.h,h.
-0000da70: 4d34 0175 6268 0b29 8194 7d94 2868 0568  M4.ubh.)..}.(h.h
-0000da80: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
-0000da90: 8c0b 436f 6e66 6967 2046 696c 6594 6807  ..Config File.h.
-0000daa0: 5d94 6816 8c0b 436f 6e66 6967 2046 696c  ].h...Config Fil
-0000dab0: 6594 8594 8194 7d94 2868 1b6a 2c0f 0000  e.....}.(h.j,...
-0000dac0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-0000dad0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-0000dae0: 5d94 6829 5d94 7568 2b68 0f68 1b6a 290f  ].h)].uh+h.h.j).
-0000daf0: 0000 681c 6803 681d 682c 681e 4d49 0175  ..h.h.h.h,h.MI.u
-0000db00: 6268 ee29 8194 7d94 2868 058c e642 7920  bh.)..}.(h...By 
-0000db10: 6465 6661 756c 742c 2060 6e67 726f 6b20  default, `ngrok 
-0000db20: 7769 6c6c 206c 6f6f 6b20 666f 7220 6974  will look for it
-0000db30: 7320 636f 6e66 6967 2066 696c 6520 3c68  s config file <h
-0000db40: 7474 7073 3a2f 2f6e 6772 6f6b 2e63 6f6d  ttps://ngrok.com
-0000db50: 2f64 6f63 732f 6e67 726f 6b2d 6167 656e  /docs/ngrok-agen
-0000db60: 742f 636f 6e66 6967 3e60 5f20 696e 2074  t/config>`_ in t
-0000db70: 6865 2068 6f6d 6520 6469 7265 6374 6f72  he home director
-0000db80: 7927 7320 6060 2e6e 6772 6f6b 3260 600a  y's ``.ngrok2``.
-0000db90: 666f 6c64 6572 2e20 5765 2063 616e 206f  folder. We can o
-0000dba0: 7665 7272 6964 6520 7468 6973 2062 6568  verride this beh
-0000dbb0: 6176 696f 7220 6279 2075 7064 6174 696e  avior by updatin
-0000dbc0: 6720 6f75 7220 6465 6661 756c 7420 3a63  g our default :c
-0000dbd0: 6c61 7373 3a60 7e70 796e 6772 6f6b 2e63  lass:`~pyngrok.c
-0000dbe0: 6f6e 662e 5079 6e67 726f 6b43 6f6e 6669  onf.PyngrokConfi
-0000dbf0: 6760 3a94 6807 5d94 2868 168c 0c42 7920  g`:.h.].(h...By 
-0000dc00: 6465 6661 756c 742c 2094 8594 8194 7d94  default, .....}.
-0000dc10: 2868 1b6a 3a0f 0000 681c 6803 681d 4e68  (h.j:...h.h.h.Nh
-0000dc20: 1e4e 7562 6843 2981 947d 9428 6805 8c52  .NubhC)..}.(h..R
-0000dc30: 606e 6772 6f6b 2077 696c 6c20 6c6f 6f6b  `ngrok will look
-0000dc40: 2066 6f72 2069 7473 2063 6f6e 6669 6720   for its config 
-0000dc50: 6669 6c65 203c 6874 7470 733a 2f2f 6e67  file <https://ng
-0000dc60: 726f 6b2e 636f 6d2f 646f 6373 2f6e 6772  rok.com/docs/ngr
-0000dc70: 6f6b 2d61 6765 6e74 2f63 6f6e 6669 673e  ok-agent/config>
-0000dc80: 605f 9468 075d 9468 168c 236e 6772 6f6b  `_.h.].h..#ngrok
-0000dc90: 2077 696c 6c20 6c6f 6f6b 2066 6f72 2069   will look for i
-0000dca0: 7473 2063 6f6e 6669 6720 6669 6c65 9485  ts config file..
-0000dcb0: 9481 947d 9428 681b 6a42 0f00 0068 1c68  ...}.(h.jB...h.h
-0000dcc0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-0000dcd0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-0000dce0: 295d 948c 046e 616d 6594 8c23 6e67 726f  )]...name..#ngro
-0000dcf0: 6b20 7769 6c6c 206c 6f6f 6b20 666f 7220  k will look for 
-0000dd00: 6974 7320 636f 6e66 6967 2066 696c 6594  its config file.
-0000dd10: 6a45 0100 008c 2968 7474 7073 3a2f 2f6e  jE....)https://n
-0000dd20: 6772 6f6b 2e63 6f6d 2f64 6f63 732f 6e67  grok.com/docs/ng
-0000dd30: 726f 6b2d 6167 656e 742f 636f 6e66 6967  rok-agent/config
-0000dd40: 9475 682b 6842 681b 6a3a 0f00 0075 626a  .uh+hBh.j:...ubj
-0000dd50: 4801 0000 2981 947d 9428 6805 8c2c 203c  H...)..}.(h.., <
-0000dd60: 6874 7470 733a 2f2f 6e67 726f 6b2e 636f  https://ngrok.co
-0000dd70: 6d2f 646f 6373 2f6e 6772 6f6b 2d61 6765  m/docs/ngrok-age
-0000dd80: 6e74 2f63 6f6e 6669 673e 9468 075d 9468  nt/config>.h.].h
-0000dd90: 1f7d 9428 6821 5d94 8c23 6e67 726f 6b2d  .}.(h!]..#ngrok-
-0000dda0: 7769 6c6c 2d6c 6f6f 6b2d 666f 722d 6974  will-look-for-it
-0000ddb0: 732d 636f 6e66 6967 2d66 696c 6594 6168  s-config-file.ah
-0000ddc0: 235d 9468 255d 948c 236e 6772 6f6b 2077  #].h%]..#ngrok w
-0000ddd0: 696c 6c20 6c6f 6f6b 2066 6f72 2069 7473  ill look for its
-0000dde0: 2063 6f6e 6669 6720 6669 6c65 9461 6827   config file.ah'
-0000ddf0: 5d94 6829 5d94 8c06 7265 6675 7269 946a  ].h)]...refuri.j
-0000de00: 520f 0000 7568 2b6a 4701 0000 6a56 0100  R...uh+jG...jV..
-0000de10: 004b 0168 1b6a 3a0f 0000 7562 6816 8c1b  .K.h.j:...ubh...
-0000de20: 2069 6e20 7468 6520 686f 6d65 2064 6972   in the home dir
-0000de30: 6563 746f 7279 e280 9973 2094 8594 8194  ectory...s .....
-0000de40: 7d94 2868 1b6a 3a0f 0000 681c 6803 681d  }.(h.j:...h.h.h.
-0000de50: 4e68 1e4e 7562 68f4 2981 947d 9428 6805  Nh.Nubh.)..}.(h.
-0000de60: 8c0b 6060 2e6e 6772 6f6b 3260 6094 6807  ..``.ngrok2``.h.
-0000de70: 5d94 6816 8c07 2e6e 6772 6f6b 3294 8594  ].h....ngrok2...
-0000de80: 8194 7d94 2868 1b6a 640f 0000 681c 6803  ..}.(h.jd...h.h.
-0000de90: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
-0000dea0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-0000deb0: 5d94 7568 2b68 f368 1b6a 3a0f 0000 7562  ].uh+h.h.j:...ub
-0000dec0: 6816 8c3f 0a66 6f6c 6465 722e 2057 6520  h..?.folder. We 
-0000ded0: 6361 6e20 6f76 6572 7269 6465 2074 6869  can override thi
-0000dee0: 7320 6265 6861 7669 6f72 2062 7920 7570  s behavior by up
-0000def0: 6461 7469 6e67 206f 7572 2064 6566 6175  dating our defau
-0000df00: 6c74 2094 8594 8194 7d94 2868 1b6a 3a0f  lt .....}.(h.j:.
-0000df10: 0000 681c 6803 681d 4e68 1e4e 7562 6ab3  ..h.h.h.Nh.Nubj.
-0000df20: 0200 0029 8194 7d94 2868 058c 243a 636c  ...)..}.(h..$:cl
-0000df30: 6173 733a 607e 7079 6e67 726f 6b2e 636f  ass:`~pyngrok.co
-0000df40: 6e66 2e50 796e 6772 6f6b 436f 6e66 6967  nf.PyngrokConfig
-0000df50: 6094 6807 5d94 68f4 2981 947d 9428 6805  `.h.].h.)..}.(h.
-0000df60: 6a78 0f00 0068 075d 9468 168c 0d50 796e  jx...h.].h...Pyn
-0000df70: 6772 6f6b 436f 6e66 6967 9485 9481 947d  grokConfig.....}
-0000df80: 9428 681b 6a7a 0f00 0068 1c68 0368 1d4e  .(h.jz...h.h.h.N
-0000df90: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-0000dfa0: 235d 9428 6ac2 0200 008c 0270 7994 8c08  #].(j......py...
-0000dfb0: 7079 2d63 6c61 7373 9465 6825 5d94 6827  py-class.eh%].h'
-0000dfc0: 5d94 6829 5d94 7568 2b68 f368 1b6a 760f  ].h)].uh+h.h.jv.
-0000dfd0: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
-0000dfe0: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
-0000dff0: 7265 6664 6f63 946a cf02 0000 8c09 7265  refdoc.j......re
-0000e000: 6664 6f6d 6169 6e94 6a84 0f00 008c 0772  fdomain.j......r
-0000e010: 6566 7479 7065 948c 0563 6c61 7373 948c  eftype...class..
-0000e020: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
-0000e030: 7265 6677 6172 6e94 896a d502 0000 4e6a  refwarn..j....Nj
-0000e040: d602 0000 4e6a d702 0000 8c1a 7079 6e67  ....Nj......pyng
-0000e050: 726f 6b2e 636f 6e66 2e50 796e 6772 6f6b  rok.conf.Pyngrok
-0000e060: 436f 6e66 6967 9475 682b 6ab2 0200 0068  Config.uh+j....h
-0000e070: 1d68 2c68 1e4d 4b01 681b 6a3a 0f00 0075  .h,h.MK.h.j:...u
-0000e080: 6268 168c 013a 9485 9481 947d 9428 681b  bh...:.....}.(h.
-0000e090: 6a3a 0f00 0068 1c68 0368 1d4e 681e 4e75  j:...h.h.h.Nh.Nu
-0000e0a0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-0000e0b0: 255d 9468 275d 9468 295d 9475 682b 68ed  %].h'].h)].uh+h.
-0000e0c0: 681d 682c 681e 4d4b 0168 1b6a 290f 0000  h.h,h.MK.h.j)...
-0000e0d0: 681c 6803 7562 6ad5 0100 0029 8194 7d94  h.h.ubj....)..}.
-0000e0e0: 2868 058c c266 726f 6d20 7079 6e67 726f  (h...from pyngro
-0000e0f0: 6b20 696d 706f 7274 2063 6f6e 662c 206e  k import conf, n
-0000e100: 6772 6f6b 0a0a 636f 6e66 2e67 6574 5f64  grok..conf.get_d
-0000e110: 6566 6175 6c74 2829 2e63 6f6e 6669 675f  efault().config_
-0000e120: 7061 7468 203d 2022 2f6f 7074 2f6e 6772  path = "/opt/ngr
-0000e130: 6f6b 2f63 6f6e 6669 672e 796d 6c22 0a0a  ok/config.yml"..
-0000e140: 2320 3c4e 6772 6f6b 5475 6e6e 656c 3a20  # <NgrokTunnel: 
-0000e150: 2268 7474 703a 2f2f 3c70 7562 6c69 635f  "http://<public_
-0000e160: 7375 623e 2e6e 6772 6f6b 2e69 6f22 202d  sub>.ngrok.io" -
-0000e170: 3e20 2268 7474 703a 2f2f 6c6f 6361 6c68  > "http://localh
-0000e180: 6f73 743a 3830 223e 0a6e 6772 6f6b 5f74  ost:80">.ngrok_t
-0000e190: 756e 6e65 6c20 3d20 6e67 726f 6b2e 636f  unnel = ngrok.co
-0000e1a0: 6e6e 6563 7428 2994 6807 5d94 6816 8cc2  nnect().h.].h...
-0000e1b0: 6672 6f6d 2070 796e 6772 6f6b 2069 6d70  from pyngrok imp
-0000e1c0: 6f72 7420 636f 6e66 2c20 6e67 726f 6b0a  ort conf, ngrok.
-0000e1d0: 0a63 6f6e 662e 6765 745f 6465 6661 756c  .conf.get_defaul
-0000e1e0: 7428 292e 636f 6e66 6967 5f70 6174 6820  t().config_path 
-0000e1f0: 3d20 222f 6f70 742f 6e67 726f 6b2f 636f  = "/opt/ngrok/co
-0000e200: 6e66 6967 2e79 6d6c 220a 0a23 203c 4e67  nfig.yml"..# <Ng
-0000e210: 726f 6b54 756e 6e65 6c3a 2022 6874 7470  rokTunnel: "http
-0000e220: 3a2f 2f3c 7075 626c 6963 5f73 7562 3e2e  ://<public_sub>.
-0000e230: 6e67 726f 6b2e 696f 2220 2d3e 2022 6874  ngrok.io" -> "ht
-0000e240: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a38  tp://localhost:8
-0000e250: 3022 3e0a 6e67 726f 6b5f 7475 6e6e 656c  0">.ngrok_tunnel
-0000e260: 203d 206e 6772 6f6b 2e63 6f6e 6e65 6374   = ngrok.connect
-0000e270: 2829 9485 9481 947d 9468 1b6a a00f 0000  ().....}.h.j....
-0000e280: 7362 6168 1f7d 9428 6821 5d94 6823 5d94  sbah.}.(h!].h#].
-0000e290: 6825 5d94 6827 5d94 6829 5d94 6ae4 0100  h%].h'].h)].j...
-0000e2a0: 006a e501 0000 6ae6 0100 0089 6ae7 0100  .j....j.....j...
-0000e2b0: 008c 0670 7974 686f 6e94 6ae9 0100 007d  ...python.j....}
-0000e2c0: 9475 682b 6ad4 0100 0068 1d68 2c68 1e4d  .uh+j....h.h,h.M
-0000e2d0: 4e01 681b 6a29 0f00 0068 1c68 0375 6265  N.h.j)...h.h.ube
-0000e2e0: 681f 7d94 2868 215d 948c 0b63 6f6e 6669  h.}.(h!]...confi
-0000e2f0: 672d 6669 6c65 9461 6823 5d94 6825 5d94  g-file.ah#].h%].
-0000e300: 8c0b 636f 6e66 6967 2066 696c 6594 6168  ..config file.ah
-0000e310: 275d 9468 295d 9475 682b 680a 681b 6a75  '].h)].uh+h.h.ju
-0000e320: 0900 0068 1c68 0368 1d68 2c68 1e4d 4901  ...h.h.h.h,h.MI.
-0000e330: 7562 680b 2981 947d 9428 6805 6806 6807  ubh.)..}.(h.h.h.
-0000e340: 5d94 2868 1029 8194 7d94 2868 058c 0b42  ].(h.)..}.(h...B
-0000e350: 696e 6172 7920 5061 7468 9468 075d 9468  inary Path.h.].h
-0000e360: 168c 0b42 696e 6172 7920 5061 7468 9485  ...Binary Path..
-0000e370: 9481 947d 9428 681b 6abb 0f00 0068 1c68  ...}.(h.j....h.h
-0000e380: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-0000e390: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-0000e3a0: 295d 9475 682b 680f 681b 6ab8 0f00 0068  )].uh+h.h.j....h
-0000e3b0: 1c68 0368 1d68 2c68 1e4d 5801 7562 68ee  .h.h.h,h.MX.ubh.
-0000e3c0: 2981 947d 9428 6805 8ca2 5468 6520 6060  )..}.(h...The ``
-0000e3d0: 7079 6e67 726f 6b60 6020 7061 636b 6167  pyngrok`` packag
-0000e3e0: 6520 6d61 6e61 6765 7320 6974 7320 6f77  e manages its ow
-0000e3f0: 6e20 6060 6e67 726f 6b60 6020 6269 6e61  n ``ngrok`` bina
-0000e400: 7279 2e20 5765 2063 616e 2075 7365 206f  ry. We can use o
-0000e410: 7572 2060 606e 6772 6f6b 6060 2062 696e  ur ``ngrok`` bin
-0000e420: 6172 7920 6966 2077 6520 7761 6e74 0a62  ary if we want.b
-0000e430: 7920 7570 6461 7469 6e67 2074 6865 2064  y updating the d
-0000e440: 6566 6175 6c74 203a 636c 6173 733a 607e  efault :class:`~
-0000e450: 7079 6e67 726f 6b2e 636f 6e66 2e50 796e  pyngrok.conf.Pyn
-0000e460: 6772 6f6b 436f 6e66 6967 603a 9468 075d  grokConfig`:.h.]
-0000e470: 9428 6816 8c04 5468 6520 9485 9481 947d  .(h...The .....}
-0000e480: 9428 681b 6ac9 0f00 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-0000e490: 681e 4e75 6268 f429 8194 7d94 2868 058c  h.Nubh.)..}.(h..
-0000e4a0: 0b60 6070 796e 6772 6f6b 6060 9468 075d  .``pyngrok``.h.]
-0000e4b0: 9468 168c 0770 796e 6772 6f6b 9485 9481  .h...pyngrok....
-0000e4c0: 947d 9428 681b 6ad1 0f00 0068 1c68 0368  .}.(h.j....h.h.h
-0000e4d0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-0000e4e0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-0000e4f0: 9475 682b 68f3 681b 6ac9 0f00 0075 6268  .uh+h.h.j....ubh
-0000e500: 168c 1920 7061 636b 6167 6520 6d61 6e61  ... package mana
-0000e510: 6765 7320 6974 7320 6f77 6e20 9485 9481  ges its own ....
-0000e520: 947d 9428 681b 6ac9 0f00 0068 1c68 0368  .}.(h.j....h.h.h
-0000e530: 1d4e 681e 4e75 6268 f429 8194 7d94 2868  .Nh.Nubh.)..}.(h
-0000e540: 058c 0960 606e 6772 6f6b 6060 9468 075d  ...``ngrok``.h.]
-0000e550: 9468 168c 056e 6772 6f6b 9485 9481 947d  .h...ngrok.....}
-0000e560: 9428 681b 6ae3 0f00 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-0000e570: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-0000e580: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-0000e590: 682b 68f3 681b 6ac9 0f00 0075 6268 168c  h+h.h.j....ubh..
-0000e5a0: 1820 6269 6e61 7279 2e20 5765 2063 616e  . binary. We can
-0000e5b0: 2075 7365 206f 7572 2094 8594 8194 7d94   use our .....}.
-0000e5c0: 2868 1b6a c90f 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-0000e5d0: 1e4e 7562 68f4 2981 947d 9428 6805 8c09  .Nubh.)..}.(h...
-0000e5e0: 6060 6e67 726f 6b60 6094 6807 5d94 6816  ``ngrok``.h.].h.
-0000e5f0: 8c05 6e67 726f 6b94 8594 8194 7d94 2868  ..ngrok.....}.(h
-0000e600: 1b6a f50f 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-0000e610: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-0000e620: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-0000e630: f368 1b6a c90f 0000 7562 6816 8c2b 2062  .h.j....ubh..+ b
-0000e640: 696e 6172 7920 6966 2077 6520 7761 6e74  inary if we want
-0000e650: 0a62 7920 7570 6461 7469 6e67 2074 6865  .by updating the
-0000e660: 2064 6566 6175 6c74 2094 8594 8194 7d94   default .....}.
-0000e670: 2868 1b6a c90f 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-0000e680: 1e4e 7562 6ab3 0200 0029 8194 7d94 2868  .Nubj....)..}.(h
-0000e690: 058c 243a 636c 6173 733a 607e 7079 6e67  ..$:class:`~pyng
-0000e6a0: 726f 6b2e 636f 6e66 2e50 796e 6772 6f6b  rok.conf.Pyngrok
-0000e6b0: 436f 6e66 6967 6094 6807 5d94 68f4 2981  Config`.h.].h.).
-0000e6c0: 947d 9428 6805 6a09 1000 0068 075d 9468  .}.(h.j....h.].h
-0000e6d0: 168c 0d50 796e 6772 6f6b 436f 6e66 6967  ...PyngrokConfig
-0000e6e0: 9485 9481 947d 9428 681b 6a0b 1000 0068  .....}.(h.j....h
-0000e6f0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-0000e700: 2868 215d 9468 235d 9428 6ac2 0200 008c  (h!].h#].(j.....
-0000e710: 0270 7994 8c08 7079 2d63 6c61 7373 9465  .py...py-class.e
-0000e720: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
-0000e730: f368 1b6a 0710 0000 7562 6168 1f7d 9428  .h.j....ubah.}.(
-0000e740: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-0000e750: 6829 5d94 8c06 7265 6664 6f63 946a cf02  h)]...refdoc.j..
-0000e760: 0000 8c09 7265 6664 6f6d 6169 6e94 6a15  ....refdomain.j.
-0000e770: 1000 008c 0772 6566 7479 7065 948c 0563  .....reftype...c
-0000e780: 6c61 7373 948c 0b72 6566 6578 706c 6963  lass...refexplic
-0000e790: 6974 9489 8c07 7265 6677 6172 6e94 896a  it....refwarn..j
-0000e7a0: d502 0000 4e6a d602 0000 4e6a d702 0000  ....Nj....Nj....
-0000e7b0: 8c1a 7079 6e67 726f 6b2e 636f 6e66 2e50  ..pyngrok.conf.P
-0000e7c0: 796e 6772 6f6b 436f 6e66 6967 9475 682b  yngrokConfig.uh+
-0000e7d0: 6ab2 0200 0068 1d68 2c68 1e4d 5a01 681b  j....h.h,h.MZ.h.
-0000e7e0: 6ac9 0f00 0075 6268 168c 013a 9485 9481  j....ubh...:....
-0000e7f0: 947d 9428 681b 6ac9 0f00 0068 1c68 0368  .}.(h.j....h.h.h
-0000e800: 1d4e 681e 4e75 6265 681f 7d94 2868 215d  .Nh.Nubeh.}.(h!]
-0000e810: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-0000e820: 9475 682b 68ed 681d 682c 681e 4d5a 0168  .uh+h.h.h,h.MZ.h
-0000e830: 1b6a b80f 0000 681c 6803 7562 6ad5 0100  .j....h.h.ubj...
-0000e840: 0029 8194 7d94 2868 058c c066 726f 6d20  .)..}.(h...from 
-0000e850: 7079 6e67 726f 6b20 696d 706f 7274 2063  pyngrok import c
-0000e860: 6f6e 662c 206e 6772 6f6b 0a0a 636f 6e66  onf, ngrok..conf
-0000e870: 2e67 6574 5f64 6566 6175 6c74 2829 2e6e  .get_default().n
-0000e880: 6772 6f6b 5f70 6174 6820 3d20 222f 7573  grok_path = "/us
-0000e890: 722f 6c6f 6361 6c2f 6269 6e2f 6e67 726f  r/local/bin/ngro
-0000e8a0: 6b22 0a0a 2320 3c4e 6772 6f6b 5475 6e6e  k"..# <NgrokTunn
-0000e8b0: 656c 3a20 2268 7474 703a 2f2f 3c70 7562  el: "http://<pub
-0000e8c0: 6c69 635f 7375 623e 2e6e 6772 6f6b 2e69  lic_sub>.ngrok.i
-0000e8d0: 6f22 202d 3e20 2268 7474 703a 2f2f 6c6f  o" -> "http://lo
-0000e8e0: 6361 6c68 6f73 743a 3830 223e 0a6e 6772  calhost:80">.ngr
-0000e8f0: 6f6b 5f74 756e 6e65 6c20 3d20 6e67 726f  ok_tunnel = ngro
-0000e900: 6b2e 636f 6e6e 6563 7428 2994 6807 5d94  k.connect().h.].
-0000e910: 6816 8cc0 6672 6f6d 2070 796e 6772 6f6b  h...from pyngrok
-0000e920: 2069 6d70 6f72 7420 636f 6e66 2c20 6e67   import conf, ng
-0000e930: 726f 6b0a 0a63 6f6e 662e 6765 745f 6465  rok..conf.get_de
-0000e940: 6661 756c 7428 292e 6e67 726f 6b5f 7061  fault().ngrok_pa
-0000e950: 7468 203d 2022 2f75 7372 2f6c 6f63 616c  th = "/usr/local
-0000e960: 2f62 696e 2f6e 6772 6f6b 220a 0a23 203c  /bin/ngrok"..# <
-0000e970: 4e67 726f 6b54 756e 6e65 6c3a 2022 6874  NgrokTunnel: "ht
-0000e980: 7470 3a2f 2f3c 7075 626c 6963 5f73 7562  tp://<public_sub
-0000e990: 3e2e 6e67 726f 6b2e 696f 2220 2d3e 2022  >.ngrok.io" -> "
-0000e9a0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
-0000e9b0: 3a38 3022 3e0a 6e67 726f 6b5f 7475 6e6e  :80">.ngrok_tunn
-0000e9c0: 656c 203d 206e 6772 6f6b 2e63 6f6e 6e65  el = ngrok.conne
-0000e9d0: 6374 2829 9485 9481 947d 9468 1b6a 3110  ct().....}.h.j1.
-0000e9e0: 0000 7362 6168 1f7d 9428 6821 5d94 6823  ..sbah.}.(h!].h#
-0000e9f0: 5d94 6825 5d94 6827 5d94 6829 5d94 6ae4  ].h%].h'].h)].j.
-0000ea00: 0100 006a e501 0000 6ae6 0100 0089 6ae7  ...j....j.....j.
-0000ea10: 0100 008c 0670 7974 686f 6e94 6ae9 0100  .....python.j...
-0000ea20: 007d 9475 682b 6ad4 0100 0068 1d68 2c68  .}.uh+j....h.h,h
-0000ea30: 1e4d 5d01 681b 6ab8 0f00 0068 1c68 0375  .M].h.j....h.h.u
-0000ea40: 6265 681f 7d94 2868 215d 948c 0b62 696e  beh.}.(h!]...bin
-0000ea50: 6172 792d 7061 7468 9461 6823 5d94 6825  ary-path.ah#].h%
-0000ea60: 5d94 8c0b 6269 6e61 7279 2070 6174 6894  ]...binary path.
-0000ea70: 6168 275d 9468 295d 9475 682b 680a 681b  ah'].h)].uh+h.h.
-0000ea80: 6a75 0900 0068 1c68 0368 1d68 2c68 1e4d  ju...h.h.h.h,h.M
-0000ea90: 5801 7562 6568 1f7d 9428 6821 5d94 8c0d  X.ubeh.}.(h!]...
-0000eaa0: 636f 6e66 6967 7572 6174 696f 6e94 6168  configuration.ah
-0000eab0: 235d 9468 255d 948c 0d63 6f6e 6669 6775  #].h%]...configu
-0000eac0: 7261 7469 6f6e 9461 6827 5d94 6829 5d94  ration.ah'].h)].
-0000ead0: 7568 2b68 0a68 1b68 0c68 1c68 0368 1d68  uh+h.h.h.h.h.h.h
-0000eae0: 2c68 1e4b d875 6268 0b29 8194 7d94 2868  ,h.K.ubh.)..}.(h
-0000eaf0: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-0000eb00: 6805 8c12 436f 6d6d 616e 6420 4c69 6e65  h...Command Line
-0000eb10: 2055 7361 6765 9468 075d 9468 168c 1243   Usage.h.].h...C
-0000eb20: 6f6d 6d61 6e64 204c 696e 6520 5573 6167  ommand Line Usag
-0000eb30: 6594 8594 8194 7d94 2868 1b6a 5410 0000  e.....}.(h.jT...
-0000eb40: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-0000eb50: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-0000eb60: 5d94 6829 5d94 7568 2b68 0f68 1b6a 5110  ].h)].uh+h.h.jQ.
-0000eb70: 0000 681c 6803 681d 682c 681e 4d67 0175  ..h.h.h.h,h.Mg.u
-0000eb80: 6268 ee29 8194 7d94 2868 058c 8054 6869  bh.)..}.(h...Thi
-0000eb90: 7320 7061 636b 6167 6520 7075 7473 2074  s package puts t
-0000eba0: 6865 2064 6566 6175 6c74 2060 606e 6772  he default ``ngr
-0000ebb0: 6f6b 6060 2062 696e 6172 7920 6f6e 206f  ok`` binary on o
-0000ebc0: 7572 2070 6174 682c 2073 6f20 616c 6c20  ur path, so all 
-0000ebd0: 6665 6174 7572 6573 206f 6620 6060 6e67  features of ``ng
-0000ebe0: 726f 6b60 6020 6172 6520 616c 736f 0a61  rok`` are also.a
-0000ebf0: 7661 696c 6162 6c65 206f 6e20 7468 6520  vailable on the 
-0000ec00: 636f 6d6d 616e 6420 6c69 6e65 2e94 6807  command line..h.
-0000ec10: 5d94 2868 168c 1e54 6869 7320 7061 636b  ].(h...This pack
-0000ec20: 6167 6520 7075 7473 2074 6865 2064 6566  age puts the def
-0000ec30: 6175 6c74 2094 8594 8194 7d94 2868 1b6a  ault .....}.(h.j
-0000ec40: 6210 0000 681c 6803 681d 4e68 1e4e 7562  b...h.h.h.Nh.Nub
-0000ec50: 68f4 2981 947d 9428 6805 8c09 6060 6e67  h.)..}.(h...``ng
-0000ec60: 726f 6b60 6094 6807 5d94 6816 8c05 6e67  rok``.h.].h...ng
-0000ec70: 726f 6b94 8594 8194 7d94 2868 1b6a 6a10  rok.....}.(h.jj.
-0000ec80: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-0000ec90: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-0000eca0: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
-0000ecb0: 6210 0000 7562 6816 8c28 2062 696e 6172  b...ubh..( binar
-0000ecc0: 7920 6f6e 206f 7572 2070 6174 682c 2073  y on our path, s
-0000ecd0: 6f20 616c 6c20 6665 6174 7572 6573 206f  o all features o
-0000ece0: 6620 9485 9481 947d 9428 681b 6a62 1000  f .....}.(h.jb..
-0000ecf0: 0068 1c68 0368 1d4e 681e 4e75 6268 f429  .h.h.h.Nh.Nubh.)
-0000ed00: 8194 7d94 2868 058c 0960 606e 6772 6f6b  ..}.(h...``ngrok
-0000ed10: 6060 9468 075d 9468 168c 056e 6772 6f6b  ``.h.].h...ngrok
-0000ed20: 9485 9481 947d 9428 681b 6a7c 1000 0068  .....}.(h.j|...h
-0000ed30: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
-0000ed40: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-0000ed50: 9468 295d 9475 682b 68f3 681b 6a62 1000  .h)].uh+h.h.jb..
-0000ed60: 0075 6268 168c 2820 6172 6520 616c 736f  .ubh..( are also
-0000ed70: 0a61 7661 696c 6162 6c65 206f 6e20 7468  .available on th
-0000ed80: 6520 636f 6d6d 616e 6420 6c69 6e65 2e94  e command line..
-0000ed90: 8594 8194 7d94 2868 1b6a 6210 0000 681c  ....}.(h.jb...h.
-0000eda0: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
-0000edb0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-0000edc0: 6829 5d94 7568 2b68 ed68 1d68 2c68 1e4d  h)].uh+h.h.h,h.M
-0000edd0: 6901 681b 6a51 1000 0068 1c68 0375 626a  i.h.jQ...h.h.ubj
-0000ede0: d501 0000 2981 947d 9428 6805 8c0d 6e67  ....)..}.(h...ng
-0000edf0: 726f 6b20 6874 7470 2038 3094 6807 5d94  rok http 80.h.].
-0000ee00: 6816 8c0d 6e67 726f 6b20 6874 7470 2038  h...ngrok http 8
-0000ee10: 3094 8594 8194 7d94 681b 6a94 1000 0073  0.....}.h.j....s
-0000ee20: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-0000ee30: 255d 9468 275d 9468 295d 946a e401 0000  %].h'].h)].j....
-0000ee40: 6ae5 0100 006a e601 0000 896a e701 0000  j....j.....j....
-0000ee50: 8c02 7368 946a e901 0000 7d94 7568 2b6a  ..sh.j....}.uh+j
-0000ee60: d401 0000 681d 682c 681e 4d6c 0168 1b6a  ....h.h,h.Ml.h.j
-0000ee70: 5110 0000 681c 6803 7562 68ee 2981 947d  Q...h.h.ubh.)..}
-0000ee80: 9428 6805 8c85 466f 7220 6465 7461 696c  .(h...For detail
-0000ee90: 7320 6f6e 2068 6f77 2074 6f20 6675 6c6c  s on how to full
-0000eea0: 7920 6c65 7665 7261 6765 2060 606e 6772  y leverage ``ngr
-0000eeb0: 6f6b 6060 2066 726f 6d20 7468 6520 636f  ok`` from the co
-0000eec0: 6d6d 616e 6420 6c69 6e65 2c20 7365 6520  mmand line, see 
-0000eed0: 606e 6772 6f6b 2773 206f 6666 6963 6961  `ngrok's officia
-0000eee0: 6c20 646f 6375 6d65 6e74 6174 696f 6e20  l documentation 
-0000eef0: 3c68 7474 7073 3a2f 2f6e 6772 6f6b 2e63  <https://ngrok.c
-0000ef00: 6f6d 2f64 6f63 733e 605f 2e94 6807 5d94  om/docs>`_..h.].
-0000ef10: 2868 168c 2546 6f72 2064 6574 6169 6c73  (h..%For details
-0000ef20: 206f 6e20 686f 7720 746f 2066 756c 6c79   on how to fully
-0000ef30: 206c 6576 6572 6167 6520 9485 9481 947d   leverage .....}
-0000ef40: 9428 681b 6aa4 1000 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-0000ef50: 681e 4e75 6268 f429 8194 7d94 2868 058c  h.Nubh.)..}.(h..
-0000ef60: 0960 606e 6772 6f6b 6060 9468 075d 9468  .``ngrok``.h.].h
-0000ef70: 168c 056e 6772 6f6b 9485 9481 947d 9428  ...ngrok.....}.(
-0000ef80: 681b 6aac 1000 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
-0000ef90: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-0000efa0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-0000efb0: 68f3 681b 6aa4 1000 0075 6268 168c 1c20  h.h.j....ubh... 
-0000efc0: 6672 6f6d 2074 6865 2063 6f6d 6d61 6e64  from the command
-0000efd0: 206c 696e 652c 2073 6565 2094 8594 8194   line, see .....
-0000efe0: 7d94 2868 1b6a a410 0000 681c 6803 681d  }.(h.j....h.h.h.
-0000eff0: 4e68 1e4e 7562 6843 2981 947d 9428 6805  Nh.NubhC)..}.(h.
-0000f000: 8c3a 606e 6772 6f6b 2773 206f 6666 6963  .:`ngrok's offic
-0000f010: 6961 6c20 646f 6375 6d65 6e74 6174 696f  ial documentatio
-0000f020: 6e20 3c68 7474 7073 3a2f 2f6e 6772 6f6b  n <https://ngrok
-0000f030: 2e63 6f6d 2f64 6f63 733e 605f 9468 075d  .com/docs>`_.h.]
-0000f040: 9468 168c 206e 6772 6f6b e280 9973 206f  .h.. ngrok...s o
-0000f050: 6666 6963 6961 6c20 646f 6375 6d65 6e74  fficial document
-0000f060: 6174 696f 6e94 8594 8194 7d94 2868 1b6a  ation.....}.(h.j
-0000f070: be10 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-0000f080: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-0000f090: 5d94 6827 5d94 6829 5d94 8c04 6e61 6d65  ].h'].h)]...name
-0000f0a0: 948c 1e6e 6772 6f6b 2773 206f 6666 6963  ...ngrok's offic
-0000f0b0: 6961 6c20 646f 6375 6d65 6e74 6174 696f  ial documentatio
-0000f0c0: 6e94 6a45 0100 008c 1668 7474 7073 3a2f  n.jE.....https:/
-0000f0d0: 2f6e 6772 6f6b 2e63 6f6d 2f64 6f63 7394  /ngrok.com/docs.
-0000f0e0: 7568 2b68 4268 1b6a a410 0000 7562 6a48  uh+hBh.j....ubjH
-0000f0f0: 0100 0029 8194 7d94 2868 058c 1920 3c68  ...)..}.(h... <h
-0000f100: 7474 7073 3a2f 2f6e 6772 6f6b 2e63 6f6d  ttps://ngrok.com
-0000f110: 2f64 6f63 733e 9468 075d 9468 1f7d 9428  /docs>.h.].h.}.(
-0000f120: 6821 5d94 8c1e 6e67 726f 6b2d 732d 6f66  h!]...ngrok-s-of
-0000f130: 6669 6369 616c 2d64 6f63 756d 656e 7461  ficial-documenta
-0000f140: 7469 6f6e 9461 6823 5d94 6825 5d94 8c1e  tion.ah#].h%]...
-0000f150: 6e67 726f 6b27 7320 6f66 6669 6369 616c  ngrok's official
-0000f160: 2064 6f63 756d 656e 7461 7469 6f6e 9461   documentation.a
-0000f170: 6827 5d94 6829 5d94 8c06 7265 6675 7269  h'].h)]...refuri
-0000f180: 946a ce10 0000 7568 2b6a 4701 0000 6a56  .j....uh+jG...jV
-0000f190: 0100 004b 0168 1b6a a410 0000 7562 6816  ...K.h.j....ubh.
-0000f1a0: 8c01 2e94 8594 8194 7d94 2868 1b6a a410  ........}.(h.j..
-0000f1b0: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
-0000f1c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-0000f1d0: 6827 5d94 6829 5d94 7568 2b68 ed68 1d68  h'].h)].uh+h.h.h
-0000f1e0: 2c68 1e4d 7001 681b 6a51 1000 0068 1c68  ,h.Mp.h.jQ...h.h
-0000f1f0: 0375 6265 681f 7d94 2868 215d 948c 1263  .ubeh.}.(h!]...c
-0000f200: 6f6d 6d61 6e64 2d6c 696e 652d 7573 6167  ommand-line-usag
-0000f210: 6594 6168 235d 9468 255d 948c 1263 6f6d  e.ah#].h%]...com
-0000f220: 6d61 6e64 206c 696e 6520 7573 6167 6594  mand line usage.
-0000f230: 6168 275d 9468 295d 9475 682b 680a 681b  ah'].h)].uh+h.h.
-0000f240: 680c 681c 6803 681d 682c 681e 4d67 0175  h.h.h.h.h,h.Mg.u
-0000f250: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
-0000f260: 9428 6810 2981 947d 9428 6805 8c0a 5079  .(h.)..}.(h...Py
-0000f270: 7468 6f6e 2032 2e37 9468 075d 9468 168c  thon 2.7.h.].h..
-0000f280: 0a50 7974 686f 6e20 322e 3794 8594 8194  .Python 2.7.....
-0000f290: 7d94 2868 1b6a f110 0000 681c 6803 681d  }.(h.j....h.h.h.
-0000f2a0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-0000f2b0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-0000f2c0: 7568 2b68 0f68 1b6a ee10 0000 681c 6803  uh+h.h.j....h.h.
-0000f2d0: 681d 682c 681e 4d73 0175 6268 ee29 8194  h.h,h.Ms.ubh.)..
-0000f2e0: 7d94 2868 0558 0501 0000 5468 6520 6c61  }.(h.X....The la
-0000f2f0: 7374 2076 6572 7369 6f6e 206f 6620 6060  st version of ``
-0000f300: 7079 6e67 726f 6b60 6020 7468 6174 2073  pyngrok`` that s
-0000f310: 7570 706f 7274 7320 5079 7468 6f6e 2032  upports Python 2
-0000f320: 2e37 2069 7320 342e 312e 782c 2073 6f20  .7 is 4.1.x, so 
-0000f330: 7765 206e 6565 6420 746f 2070 696e 2060  we need to pin `
-0000f340: 6070 796e 6772 6f6b 3e3d 342e 312c 3c34  `pyngrok>=4.1,<4
-0000f350: 2e32 6060 2069 6620 7765 2073 7469 6c6c  .2`` if we still
-0000f360: 0a77 616e 7420 746f 2075 7365 2060 6070  .want to use ``p
-0000f370: 796e 6772 6f6b 6060 2077 6974 6820 7468  yngrok`` with th
-0000f380: 6973 2076 6572 7369 6f6e 206f 6620 5079  is version of Py
-0000f390: 7468 6f6e 2e20 4974 7320 6c65 6761 6379  thon. Its legacy
-0000f3a0: 2064 6f63 756d 656e 7461 7469 6f6e 2063   documentation c
-0000f3b0: 616e 2062 6520 666f 756e 6420 6068 6572  an be found `her
-0000f3c0: 6520 3c68 7474 7073 3a2f 2f70 796e 6772  e <https://pyngr
-0000f3d0: 6f6b 2e72 6561 6474 6865 646f 6373 2e69  ok.readthedocs.i
-0000f3e0: 6f2f 656e 2f34 2e31 2e78 2f3e 605f 2e94  o/en/4.1.x/>`_..
-0000f3f0: 6807 5d94 2868 168c 1454 6865 206c 6173  h.].(h...The las
-0000f400: 7420 7665 7273 696f 6e20 6f66 2094 8594  t version of ...
-0000f410: 8194 7d94 2868 1b6a ff10 0000 681c 6803  ..}.(h.j....h.h.
-0000f420: 681d 4e68 1e4e 7562 68f4 2981 947d 9428  h.Nh.Nubh.)..}.(
-0000f430: 6805 8c0b 6060 7079 6e67 726f 6b60 6094  h...``pyngrok``.
-0000f440: 6807 5d94 6816 8c07 7079 6e67 726f 6b94  h.].h...pyngrok.
-0000f450: 8594 8194 7d94 2868 1b6a 0711 0000 681c  ....}.(h.j....h.
-0000f460: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
-0000f470: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-0000f480: 6829 5d94 7568 2b68 f368 1b6a ff10 0000  h)].uh+h.h.j....
-0000f490: 7562 6816 8c36 2074 6861 7420 7375 7070  ubh..6 that supp
-0000f4a0: 6f72 7473 2050 7974 686f 6e20 322e 3720  orts Python 2.7 
-0000f4b0: 6973 2034 2e31 2e78 2c20 736f 2077 6520  is 4.1.x, so we 
-0000f4c0: 6e65 6564 2074 6f20 7069 6e20 9485 9481  need to pin ....
-0000f4d0: 947d 9428 681b 6aff 1000 0068 1c68 0368  .}.(h.j....h.h.h
-0000f4e0: 1d4e 681e 4e75 6268 f429 8194 7d94 2868  .Nh.Nubh.)..}.(h
-0000f4f0: 058c 1560 6070 796e 6772 6f6b 3e3d 342e  ...``pyngrok>=4.
-0000f500: 312c 3c34 2e32 6060 9468 075d 9468 168c  1,<4.2``.h.].h..
-0000f510: 1170 796e 6772 6f6b 3e3d 342e 312c 3c34  .pyngrok>=4.1,<4
-0000f520: 2e32 9485 9481 947d 9428 681b 6a19 1100  .2.....}.(h.j...
-0000f530: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-0000f540: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-0000f550: 275d 9468 295d 9475 682b 68f3 681b 6aff  '].h)].uh+h.h.j.
-0000f560: 1000 0075 6268 168c 1920 6966 2077 6520  ...ubh... if we 
-0000f570: 7374 696c 6c0a 7761 6e74 2074 6f20 7573  still.want to us
-0000f580: 6520 9485 9481 947d 9428 681b 6aff 1000  e .....}.(h.j...
-0000f590: 0068 1c68 0368 1d4e 681e 4e75 6268 f429  .h.h.h.Nh.Nubh.)
-0000f5a0: 8194 7d94 2868 058c 0b60 6070 796e 6772  ..}.(h...``pyngr
-0000f5b0: 6f6b 6060 9468 075d 9468 168c 0770 796e  ok``.h.].h...pyn
-0000f5c0: 6772 6f6b 9485 9481 947d 9428 681b 6a2b  grok.....}.(h.j+
-0000f5d0: 1100 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-0000f5e0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-0000f5f0: 9468 275d 9468 295d 9475 682b 68f3 681b  .h'].h)].uh+h.h.
-0000f600: 6aff 1000 0075 6268 168c 4420 7769 7468  j....ubh..D with
-0000f610: 2074 6869 7320 7665 7273 696f 6e20 6f66   this version of
-0000f620: 2050 7974 686f 6e2e 2049 7473 206c 6567   Python. Its leg
-0000f630: 6163 7920 646f 6375 6d65 6e74 6174 696f  acy documentatio
-0000f640: 6e20 6361 6e20 6265 2066 6f75 6e64 2094  n can be found .
-0000f650: 8594 8194 7d94 2868 1b6a ff10 0000 681c  ....}.(h.j....h.
-0000f660: 6803 681d 4e68 1e4e 7562 6843 2981 947d  h.h.Nh.NubhC)..}
-0000f670: 9428 6805 8c32 6068 6572 6520 3c68 7474  .(h..2`here <htt
-0000f680: 7073 3a2f 2f70 796e 6772 6f6b 2e72 6561  ps://pyngrok.rea
-0000f690: 6474 6865 646f 6373 2e69 6f2f 656e 2f34  dthedocs.io/en/4
-0000f6a0: 2e31 2e78 2f3e 605f 9468 075d 9468 168c  .1.x/>`_.h.].h..
-0000f6b0: 0468 6572 6594 8594 8194 7d94 2868 1b6a  .here.....}.(h.j
-0000f6c0: 3d11 0000 681c 6803 681d 4e68 1e4e 7562  =...h.h.h.Nh.Nub
-0000f6d0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-0000f6e0: 5d94 6827 5d94 6829 5d94 8c04 6e61 6d65  ].h'].h)]...name
-0000f6f0: 948c 0468 6572 6594 6a45 0100 008c 2868  ...here.jE....(h
-0000f700: 7474 7073 3a2f 2f70 796e 6772 6f6b 2e72  ttps://pyngrok.r
-0000f710: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-0000f720: 2f34 2e31 2e78 2f94 7568 2b68 4268 1b6a  /4.1.x/.uh+hBh.j
-0000f730: ff10 0000 7562 6a48 0100 0029 8194 7d94  ....ubjH...)..}.
-0000f740: 2868 058c 2b20 3c68 7474 7073 3a2f 2f70  (h..+ <https://p
-0000f750: 796e 6772 6f6b 2e72 6561 6474 6865 646f  yngrok.readthedo
-0000f760: 6373 2e69 6f2f 656e 2f34 2e31 2e78 2f3e  cs.io/en/4.1.x/>
-0000f770: 9468 075d 9468 1f7d 9428 6821 5d94 8c04  .h.].h.}.(h!]...
-0000f780: 6865 7265 9461 6823 5d94 6825 5d94 8c04  here.ah#].h%]...
-0000f790: 6865 7265 9461 6827 5d94 6829 5d94 8c06  here.ah'].h)]...
-0000f7a0: 7265 6675 7269 946a 4d11 0000 7568 2b6a  refuri.jM...uh+j
-0000f7b0: 4701 0000 6a56 0100 004b 0168 1b6a ff10  G...jV...K.h.j..
-0000f7c0: 0000 7562 6816 8c01 2e94 8594 8194 7d94  ..ubh.........}.
-0000f7d0: 2868 1b6a ff10 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
-0000f7e0: 1e4e 7562 6568 1f7d 9428 6821 5d94 6823  .Nubeh.}.(h!].h#
-0000f7f0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-0000f800: 2b68 ed68 1d68 2c68 1e4d 7501 681b 6aee  +h.h.h,h.Mu.h.j.
-0000f810: 1000 0068 1c68 0375 6265 681f 7d94 2868  ...h.h.ubeh.}.(h
-0000f820: 215d 948c 0a70 7974 686f 6e2d 322d 3794  !]...python-2-7.
-0000f830: 6168 235d 9468 255d 948c 0a70 7974 686f  ah#].h%]...pytho
-0000f840: 6e20 322e 3794 6168 275d 9468 295d 9475  n 2.7.ah'].h)].u
-0000f850: 682b 680a 681b 680c 681c 6803 681d 682c  h+h.h.h.h.h.h.h,
-0000f860: 681e 4d73 0175 6268 0b29 8194 7d94 2868  h.Ms.ubh.)..}.(h
-0000f870: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-0000f880: 6805 8c0b 4469 7665 2044 6565 7065 7294  h...Dive Deeper.
-0000f890: 6807 5d94 6816 8c0b 4469 7665 2044 6565  h.].h...Dive Dee
-0000f8a0: 7065 7294 8594 8194 7d94 2868 1b6a 7011  per.....}.(h.jp.
-0000f8b0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
-0000f8c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-0000f8d0: 6827 5d94 6829 5d94 7568 2b68 0f68 1b6a  h'].h)].uh+h.h.j
-0000f8e0: 6d11 0000 681c 6803 681d 682c 681e 4d79  m...h.h.h.h,h.My
-0000f8f0: 0175 6268 ee29 8194 7d94 2868 058c 8746  .ubh.)..}.(h...F
-0000f900: 6f72 206d 6f72 6520 6164 7661 6e63 6564  or more advanced
-0000f910: 2075 7361 6765 2c20 696e 7465 6772 6174   usage, integrat
-0000f920: 696f 6e20 6578 616d 706c 6573 2c20 616e  ion examples, an
-0000f930: 6420 7469 7073 2074 6f20 7472 6f75 626c  d tips to troubl
-0000f940: 6573 686f 6f74 2063 6f6d 6d6f 6e20 6973  eshoot common is
-0000f950: 7375 6573 2c20 6469 7665 2064 6565 7065  sues, dive deepe
-0000f960: 7220 696e 2074 6f20 7468 6520 7265 7374  r in to the rest
-0000f970: 206f 660a 7468 6520 646f 6375 6d65 6e74   of.the document
-0000f980: 6174 696f 6e2e 9468 075d 9468 168c 8746  ation..h.].h...F
-0000f990: 6f72 206d 6f72 6520 6164 7661 6e63 6564  or more advanced
-0000f9a0: 2075 7361 6765 2c20 696e 7465 6772 6174   usage, integrat
-0000f9b0: 696f 6e20 6578 616d 706c 6573 2c20 616e  ion examples, an
-0000f9c0: 6420 7469 7073 2074 6f20 7472 6f75 626c  d tips to troubl
-0000f9d0: 6573 686f 6f74 2063 6f6d 6d6f 6e20 6973  eshoot common is
-0000f9e0: 7375 6573 2c20 6469 7665 2064 6565 7065  sues, dive deepe
-0000f9f0: 7220 696e 2074 6f20 7468 6520 7265 7374  r in to the rest
-0000fa00: 206f 660a 7468 6520 646f 6375 6d65 6e74   of.the document
-0000fa10: 6174 696f 6e2e 9485 9481 947d 9428 681b  ation......}.(h.
-0000fa20: 6a7e 1100 0068 1c68 0368 1d4e 681e 4e75  j~...h.h.h.Nh.Nu
-0000fa30: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-0000fa40: 255d 9468 275d 9468 295d 9475 682b 68ed  %].h'].h)].uh+h.
-0000fa50: 681d 682c 681e 4d7b 0168 1b6a 6d11 0000  h.h,h.M{.h.jm...
-0000fa60: 681c 6803 7562 6809 8c08 636f 6d70 6f75  h.h.ubh...compou
-0000fa70: 6e64 9493 9429 8194 7d94 2868 0568 0668  nd...)..}.(h.h.h
-0000fa80: 075d 9468 008c 0774 6f63 7472 6565 9493  .].h...toctree..
-0000fa90: 9429 8194 7d94 2868 0568 0668 075d 9468  .)..}.(h.h.h.].h
-0000faa0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
-0000fab0: 6827 5d94 6829 5d94 681b 6acf 0200 008c  h'].h)].h.j.....
-0000fac0: 0765 6e74 7269 6573 945d 9428 4e8c 0361  .entries.].(N..a
-0000fad0: 7069 9486 944e 8c0c 696e 7465 6772 6174  pi...N..integrat
-0000fae0: 696f 6e73 9486 944e 8c0f 7472 6f75 626c  ions...N..troubl
-0000faf0: 6573 686f 6f74 696e 6794 8694 658c 0c69  eshooting...e..i
-0000fb00: 6e63 6c75 6465 6669 6c65 7394 5d94 286a  ncludefiles.].(j
-0000fb10: 9e11 0000 6aa0 1100 006a a211 0000 658c  ....j....j....e.
-0000fb20: 086d 6178 6465 7074 6894 4b02 8c07 6361  .maxdepth.K...ca
-0000fb30: 7074 696f 6e94 4e8c 0467 6c6f 6294 898c  ption.N..glob...
-0000fb40: 0668 6964 6465 6e94 898c 0d69 6e63 6c75  .hidden....inclu
-0000fb50: 6465 6869 6464 656e 9489 8c08 6e75 6d62  dehidden....numb
-0000fb60: 6572 6564 944b 008c 0a74 6974 6c65 736f  ered.K...titleso
-0000fb70: 6e6c 7994 898c 0a72 6177 656e 7472 6965  nly....rawentrie
-0000fb80: 7394 5d94 7568 2b6a 9111 0000 681d 682c  s.].uh+j....h.h,
-0000fb90: 681e 4d7e 0168 1b6a 8e11 0000 7562 6168  h.M~.h.j....ubah
-0000fba0: 1f7d 9428 6821 5d94 6823 5d94 8c0f 746f  .}.(h!].h#]...to
-0000fbb0: 6374 7265 652d 7772 6170 7065 7294 6168  ctree-wrapper.ah
-0000fbc0: 255d 9468 275d 9468 295d 9475 682b 6a8c  %].h'].h)].uh+j.
-0000fbd0: 1100 0068 1b6a 6d11 0000 681c 6803 681d  ...h.jm...h.h.h.
-0000fbe0: 682c 681e 4e75 6265 681f 7d94 2868 215d  h,h.Nubeh.}.(h!]
-0000fbf0: 948c 0b64 6976 652d 6465 6570 6572 9461  ...dive-deeper.a
-0000fc00: 6823 5d94 6825 5d94 8c0b 6469 7665 2064  h#].h%]...dive d
-0000fc10: 6565 7065 7294 6168 275d 9468 295d 9475  eeper.ah'].h)].u
-0000fc20: 682b 680a 681b 680c 681c 6803 681d 682c  h+h.h.h.h.h.h.h,
-0000fc30: 681e 4d79 0175 6268 0b29 8194 7d94 2868  h.My.ubh.)..}.(h
-0000fc40: 0568 0668 075d 9428 6810 2981 947d 9428  .h.h.].(h.)..}.(
-0000fc50: 6805 8c0c 436f 6e74 7269 6275 7469 6e67  h...Contributing
-0000fc60: 9468 075d 9468 168c 0c43 6f6e 7472 6962  .h.].h...Contrib
-0000fc70: 7574 696e 6794 8594 8194 7d94 2868 1b6a  uting.....}.(h.j
-0000fc80: c111 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
-0000fc90: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-0000fca0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
-0000fcb0: 1b6a be11 0000 681c 6803 681d 8c10 434f  .j....h.h.h...CO
-0000fcc0: 4e54 5249 4255 5449 4e47 2e72 7374 9468  NTRIBUTING.rst.h
-0000fcd0: 1e4b 0275 6268 ee29 8194 7d94 2868 058c  .K.ubh.)..}.(h..
-0000fce0: 5c49 6620 796f 7520 6669 6e64 2069 7373  \If you find iss
-0000fcf0: 7565 732c 2060 7265 706f 7274 2074 6865  ues, `report the
-0000fd00: 6d20 6f6e 2047 6974 4875 6220 3c68 7474  m on GitHub <htt
-0000fd10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000fd20: 616c 6578 646c 6169 7264 2f70 796e 6772  alexdlaird/pyngr
-0000fd30: 6f6b 2f69 7373 7565 733e 605f 2e94 6807  ok/issues>`_..h.
-0000fd40: 5d94 2868 168c 1449 6620 796f 7520 6669  ].(h...If you fi
-0000fd50: 6e64 2069 7373 7565 732c 2094 8594 8194  nd issues, .....
-0000fd60: 7d94 2868 1b6a d011 0000 681c 6803 681d  }.(h.j....h.h.h.
-0000fd70: 4e68 1e4e 7562 6843 2981 947d 9428 6805  Nh.NubhC)..}.(h.
-0000fd80: 8c47 6072 6570 6f72 7420 7468 656d 206f  .G`report them o
-0000fd90: 6e20 4769 7448 7562 203c 6874 7470 733a  n GitHub <https:
-0000fda0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6c65  //github.com/ale
-0000fdb0: 7864 6c61 6972 642f 7079 6e67 726f 6b2f  xdlaird/pyngrok/
-0000fdc0: 6973 7375 6573 3e60 5f94 6807 5d94 6816  issues>`_.h.].h.
-0000fdd0: 8c15 7265 706f 7274 2074 6865 6d20 6f6e  ..report them on
-0000fde0: 2047 6974 4875 6294 8594 8194 7d94 2868   GitHub.....}.(h
-0000fdf0: 1b6a d811 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
-0000fe00: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-0000fe10: 6825 5d94 6827 5d94 6829 5d94 8c04 6e61  h%].h'].h)]...na
-0000fe20: 6d65 948c 1572 6570 6f72 7420 7468 656d  me...report them
-0000fe30: 206f 6e20 4769 7448 7562 946a 4501 0000   on GitHub.jE...
-0000fe40: 8c2c 6874 7470 733a 2f2f 6769 7468 7562  .,https://github
-0000fe50: 2e63 6f6d 2f61 6c65 7864 6c61 6972 642f  .com/alexdlaird/
-0000fe60: 7079 6e67 726f 6b2f 6973 7375 6573 9475  pyngrok/issues.u
-0000fe70: 682b 6842 681b 6ad0 1100 0075 626a 4801  h+hBh.j....ubjH.
-0000fe80: 0000 2981 947d 9428 6805 8c2f 203c 6874  ..)..}.(h../ <ht
-0000fe90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-0000fea0: 2f61 6c65 7864 6c61 6972 642f 7079 6e67  /alexdlaird/pyng
-0000feb0: 726f 6b2f 6973 7375 6573 3e94 6807 5d94  rok/issues>.h.].
-0000fec0: 681f 7d94 2868 215d 948c 1572 6570 6f72  h.}.(h!]...repor
-0000fed0: 742d 7468 656d 2d6f 6e2d 6769 7468 7562  t-them-on-github
-0000fee0: 9461 6823 5d94 6825 5d94 8c15 7265 706f  .ah#].h%]...repo
-0000fef0: 7274 2074 6865 6d20 6f6e 2067 6974 6875  rt them on githu
-0000ff00: 6294 6168 275d 9468 295d 948c 0672 6566  b.ah'].h)]...ref
-0000ff10: 7572 6994 6ae8 1100 0075 682b 6a47 0100  uri.j....uh+jG..
-0000ff20: 006a 5601 0000 4b01 681b 6ad0 1100 0075  .jV...K.h.j....u
-0000ff30: 6268 168c 012e 9485 9481 947d 9428 681b  bh.........}.(h.
-0000ff40: 6ad0 1100 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
-0000ff50: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-0000ff60: 255d 9468 275d 9468 295d 9475 682b 68ed  %].h'].h)].uh+h.
-0000ff70: 681d 6acf 1100 0068 1e4b 0468 1b6a be11  h.j....h.K.h.j..
-0000ff80: 0000 681c 6803 7562 68ee 2981 947d 9428  ..h.h.ubh.)..}.(
-0000ff90: 6805 8c4a 4966 2079 6f75 2077 6f75 6c64  h..JIf you would
-0000ffa0: 206c 696b 6520 746f 2063 6f6e 7472 6962   like to contrib
-0000ffb0: 7574 6520 746f 2074 6865 2063 6f64 652c  ute to the code,
-0000ffc0: 2074 6865 2070 726f 6365 7373 2069 7320   the process is 
-0000ffd0: 7072 6574 7479 2073 696d 706c 653a 9468  pretty simple:.h
-0000ffe0: 075d 9468 168c 4a49 6620 796f 7520 776f  .].h..JIf you wo
-0000fff0: 756c 6420 6c69 6b65 2074 6f20 636f 6e74  uld like to cont
-00010000: 7269 6275 7465 2074 6f20 7468 6520 636f  ribute to the co
-00010010: 6465 2c20 7468 6520 7072 6f63 6573 7320  de, the process 
-00010020: 6973 2070 7265 7474 7920 7369 6d70 6c65  is pretty simple
-00010030: 3a94 8594 8194 95ad 2300 0000 0000 007d  :.......#......}
-00010040: 9428 681b 6a00 1200 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
-00010050: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
-00010060: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00010070: 682b 68ed 681d 6acf 1100 0068 1e4b 0668  h+h.h.j....h.K.h
-00010080: 1b6a be11 0000 681c 6803 7562 6809 8c0f  .j....h.h.ubh...
-00010090: 656e 756d 6572 6174 6564 5f6c 6973 7494  enumerated_list.
-000100a0: 9394 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-000100b0: 2868 098c 096c 6973 745f 6974 656d 9493  (h...list_item..
-000100c0: 9429 8194 7d94 2868 058c bd46 616d 696c  .)..}.(h...Famil
-000100d0: 6961 7269 7365 2079 6f75 7273 656c 6620  iarise yourself 
-000100e0: 7769 7468 2074 6869 7320 7061 636b 6167  with this packag
-000100f0: 652c 2060 7079 6e67 726f 6b27 7320 4150  e, `pyngrok's AP
-00010100: 4973 203c 6874 7470 733a 2f2f 7079 6e67  Is <https://pyng
-00010110: 726f 6b2e 7265 6164 7468 6564 6f63 732e  rok.readthedocs.
-00010120: 696f 2f65 6e2f 6c61 7465 7374 2f61 7069  io/en/latest/api
-00010130: 2e68 746d 6c3e 605f 2061 6e64 206f 7468  .html>`_ and oth
-00010140: 6572 2064 6f63 756d 656e 7461 7469 6f6e  er documentation
-00010150: 2c20 616e 6420 606e 6772 6f6b 2773 2064  , and `ngrok's d
-00010160: 6f63 756d 656e 7461 7469 6f6e 203c 6874  ocumentation <ht
-00010170: 7470 733a 2f2f 6e67 726f 6b2e 636f 6d2f  tps://ngrok.com/
-00010180: 646f 6373 3e60 5f2e 9468 075d 9468 ee29  docs>`_..h.].h.)
-00010190: 8194 7d94 2868 056a 1712 0000 6807 5d94  ..}.(h.j....h.].
-000101a0: 2868 168c 2846 616d 696c 6961 7269 7365  (h..(Familiarise
-000101b0: 2079 6f75 7273 656c 6620 7769 7468 2074   yourself with t
-000101c0: 6869 7320 7061 636b 6167 652c 2094 8594  his package, ...
-000101d0: 8194 7d94 2868 1b6a 1912 0000 681c 6803  ..}.(h.j....h.h.
-000101e0: 681d 4e68 1e4e 7562 6843 2981 947d 9428  h.Nh.NubhC)..}.(
-000101f0: 6805 8c45 6070 796e 6772 6f6b 2773 2041  h..E`pyngrok's A
-00010200: 5049 7320 3c68 7474 7073 3a2f 2f70 796e  PIs <https://pyn
-00010210: 6772 6f6b 2e72 6561 6474 6865 646f 6373  grok.readthedocs
-00010220: 2e69 6f2f 656e 2f6c 6174 6573 742f 6170  .io/en/latest/ap
-00010230: 692e 6874 6d6c 3e60 5f94 6807 5d94 6816  i.html>`_.h.].h.
-00010240: 8c10 7079 6e67 726f 6be2 8099 7320 4150  ..pyngrok...s AP
-00010250: 4973 9485 9481 947d 9428 681b 6a20 1200  Is.....}.(h.j ..
-00010260: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00010270: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00010280: 275d 9468 295d 948c 046e 616d 6594 8c0e  '].h)]...name...
-00010290: 7079 6e67 726f 6b27 7320 4150 4973 946a  pyngrok's APIs.j
-000102a0: 4501 0000 8c31 6874 7470 733a 2f2f 7079  E....1https://py
-000102b0: 6e67 726f 6b2e 7265 6164 7468 6564 6f63  ngrok.readthedoc
-000102c0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f61  s.io/en/latest/a
-000102d0: 7069 2e68 746d 6c94 7568 2b68 4268 1b6a  pi.html.uh+hBh.j
-000102e0: 1912 0000 7562 6a48 0100 0029 8194 7d94  ....ubjH...)..}.
-000102f0: 2868 058c 3420 3c68 7474 7073 3a2f 2f70  (h..4 <https://p
-00010300: 796e 6772 6f6b 2e72 6561 6474 6865 646f  yngrok.readthedo
-00010310: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00010320: 6170 692e 6874 6d6c 3e94 6807 5d94 681f  api.html>.h.].h.
-00010330: 7d94 2868 215d 948c 0e70 796e 6772 6f6b  }.(h!]...pyngrok
-00010340: 2d73 2d61 7069 7394 6168 235d 9468 255d  -s-apis.ah#].h%]
-00010350: 948c 0e70 796e 6772 6f6b 2773 2061 7069  ...pyngrok's api
-00010360: 7394 6168 275d 9468 295d 948c 0672 6566  s.ah'].h)]...ref
-00010370: 7572 6994 6a30 1200 0075 682b 6a47 0100  uri.j0...uh+jG..
-00010380: 006a 5601 0000 4b01 681b 6a19 1200 0075  .jV...K.h.j....u
-00010390: 6268 168c 1e20 616e 6420 6f74 6865 7220  bh... and other 
-000103a0: 646f 6375 6d65 6e74 6174 696f 6e2c 2061  documentation, a
-000103b0: 6e64 2094 8594 8194 7d94 2868 1b6a 1912  nd .....}.(h.j..
-000103c0: 0000 681c 6803 681d 4e68 1e4e 7562 6843  ..h.h.h.Nh.NubhC
-000103d0: 2981 947d 9428 6805 8c31 606e 6772 6f6b  )..}.(h..1`ngrok
-000103e0: 2773 2064 6f63 756d 656e 7461 7469 6f6e  's documentation
-000103f0: 203c 6874 7470 733a 2f2f 6e67 726f 6b2e   <https://ngrok.
-00010400: 636f 6d2f 646f 6373 3e60 5f94 6807 5d94  com/docs>`_.h.].
-00010410: 6816 8c17 6e67 726f 6be2 8099 7320 646f  h...ngrok...s do
-00010420: 6375 6d65 6e74 6174 696f 6e94 8594 8194  cumentation.....
-00010430: 7d94 2868 1b6a 4212 0000 681c 6803 681d  }.(h.jB...h.h.h.
-00010440: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00010450: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00010460: 8c04 6e61 6d65 948c 156e 6772 6f6b 2773  ..name...ngrok's
-00010470: 2064 6f63 756d 656e 7461 7469 6f6e 946a   documentation.j
-00010480: 4501 0000 8c16 6874 7470 733a 2f2f 6e67  E.....https://ng
-00010490: 726f 6b2e 636f 6d2f 646f 6373 9475 682b  rok.com/docs.uh+
-000104a0: 6842 681b 6a19 1200 0075 626a 4801 0000  hBh.j....ubjH...
-000104b0: 2981 947d 9428 6805 8c19 203c 6874 7470  )..}.(h... <http
-000104c0: 733a 2f2f 6e67 726f 6b2e 636f 6d2f 646f  s://ngrok.com/do
-000104d0: 6373 3e94 6807 5d94 681f 7d94 2868 215d  cs>.h.].h.}.(h!]
-000104e0: 948c 156e 6772 6f6b 2d73 2d64 6f63 756d  ...ngrok-s-docum
-000104f0: 656e 7461 7469 6f6e 9461 6823 5d94 6825  entation.ah#].h%
-00010500: 5d94 8c15 6e67 726f 6b27 7320 646f 6375  ]...ngrok's docu
-00010510: 6d65 6e74 6174 696f 6e94 6168 275d 9468  mentation.ah'].h
-00010520: 295d 948c 0672 6566 7572 6994 6a52 1200  )]...refuri.jR..
-00010530: 0075 682b 6a47 0100 006a 5601 0000 4b01  .uh+jG...jV...K.
-00010540: 681b 6a19 1200 0075 6268 168c 012e 9485  h.j....ubh......
-00010550: 9481 947d 9428 681b 6a19 1200 0068 1c68  ...}.(h.j....h.h
-00010560: 0368 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
-00010570: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00010580: 295d 9475 682b 68ed 681d 6acf 1100 0068  )].uh+h.h.j....h
-00010590: 1e4b 0868 1b6a 1512 0000 7562 6168 1f7d  .K.h.j....ubah.}
-000105a0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000105b0: 5d94 6829 5d94 7568 2b6a 1312 0000 681b  ].h)].uh+j....h.
-000105c0: 6a10 1200 0068 1c68 0368 1d6a cf11 0000  j....h.h.h.j....
-000105d0: 681e 4e75 626a 1412 0000 2981 947d 9428  h.Nubj....)..}.(
-000105e0: 6805 8c68 466f 726b 2060 7468 6520 7265  h..hFork `the re
-000105f0: 706f 7369 746f 7279 206f 6e20 4769 7448  pository on GitH
-00010600: 7562 203c 6874 7470 733a 2f2f 6769 7468  ub <https://gith
-00010610: 7562 2e63 6f6d 2f61 6c65 7864 6c61 6972  ub.com/alexdlair
-00010620: 642f 7079 6e67 726f 6b3e 605f 2061 6e64  d/pyngrok>`_ and
-00010630: 2073 7461 7274 2069 6d70 6c65 6d65 6e74   start implement
-00010640: 696e 6720 6368 616e 6765 732e 9468 075d  ing changes..h.]
-00010650: 9468 ee29 8194 7d94 2868 056a 7212 0000  .h.)..}.(h.jr...
-00010660: 6807 5d94 2868 168c 0546 6f72 6b20 9485  h.].(h...Fork ..
-00010670: 9481 947d 9428 681b 6a74 1200 0068 1c68  ...}.(h.jt...h.h
-00010680: 0368 1d4e 681e 4e75 6268 4329 8194 7d94  .h.Nh.NubhC)..}.
-00010690: 2868 058c 4360 7468 6520 7265 706f 7369  (h..C`the reposi
-000106a0: 746f 7279 206f 6e20 4769 7448 7562 203c  tory on GitHub <
-000106b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000106c0: 6f6d 2f61 6c65 7864 6c61 6972 642f 7079  om/alexdlaird/py
-000106d0: 6e67 726f 6b3e 605f 9468 075d 9468 168c  ngrok>`_.h.].h..
-000106e0: 1874 6865 2072 6570 6f73 6974 6f72 7920  .the repository 
-000106f0: 6f6e 2047 6974 4875 6294 8594 8194 7d94  on GitHub.....}.
-00010700: 2868 1b6a 7b12 0000 681c 6803 681d 4e68  (h.j{...h.h.h.Nh
-00010710: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
-00010720: 5d94 6825 5d94 6827 5d94 6829 5d94 8c04  ].h%].h'].h)]...
-00010730: 6e61 6d65 948c 1874 6865 2072 6570 6f73  name...the repos
-00010740: 6974 6f72 7920 6f6e 2047 6974 4875 6294  itory on GitHub.
-00010750: 6a45 0100 008c 2568 7474 7073 3a2f 2f67  jE....%https://g
-00010760: 6974 6875 622e 636f 6d2f 616c 6578 646c  ithub.com/alexdl
-00010770: 6169 7264 2f70 796e 6772 6f6b 9475 682b  aird/pyngrok.uh+
-00010780: 6842 681b 6a74 1200 0075 626a 4801 0000  hBh.jt...ubjH...
-00010790: 2981 947d 9428 6805 8c28 203c 6874 7470  )..}.(h..( <http
-000107a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-000107b0: 6c65 7864 6c61 6972 642f 7079 6e67 726f  lexdlaird/pyngro
-000107c0: 6b3e 9468 075d 9468 1f7d 9428 6821 5d94  k>.h.].h.}.(h!].
-000107d0: 8c18 7468 652d 7265 706f 7369 746f 7279  ..the-repository
-000107e0: 2d6f 6e2d 6769 7468 7562 9461 6823 5d94  -on-github.ah#].
-000107f0: 6825 5d94 8c18 7468 6520 7265 706f 7369  h%]...the reposi
-00010800: 746f 7279 206f 6e20 6769 7468 7562 9461  tory on github.a
-00010810: 6827 5d94 6829 5d94 8c06 7265 6675 7269  h'].h)]...refuri
-00010820: 946a 8b12 0000 7568 2b6a 4701 0000 6a56  .j....uh+jG...jV
-00010830: 0100 004b 0168 1b6a 7412 0000 7562 6816  ...K.h.jt...ubh.
-00010840: 8c20 2061 6e64 2073 7461 7274 2069 6d70  .  and start imp
-00010850: 6c65 6d65 6e74 696e 6720 6368 616e 6765  lementing change
-00010860: 732e 9485 9481 947d 9428 681b 6a74 1200  s......}.(h.jt..
-00010870: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
-00010880: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00010890: 275d 9468 295d 9475 682b 68ed 681d 6acf  '].h)].uh+h.h.j.
-000108a0: 1100 0068 1e4b 0968 1b6a 7012 0000 7562  ...h.K.h.jp...ub
-000108b0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-000108c0: 5d94 6827 5d94 6829 5d94 7568 2b6a 1312  ].h'].h)].uh+j..
-000108d0: 0000 681b 6a10 1200 0068 1c68 0368 1d6a  ..h.j....h.h.h.j
-000108e0: cf11 0000 681e 4e75 626a 1412 0000 2981  ....h.Nubj....).
-000108f0: 947d 9428 6805 8c35 5772 6974 6520 6120  .}.(h..5Write a 
-00010900: 7465 7374 2074 6861 7420 706c 6169 6e6c  test that plainl
-00010910: 7920 7661 6c69 6461 7465 7320 7468 6520  y validates the 
-00010920: 6368 616e 6765 7320 6d61 6465 2e94 6807  changes made..h.
-00010930: 5d94 68ee 2981 947d 9428 6805 6aab 1200  ].h.)..}.(h.j...
-00010940: 0068 075d 9468 168c 3557 7269 7465 2061  .h.].h..5Write a
-00010950: 2074 6573 7420 7468 6174 2070 6c61 696e   test that plain
-00010960: 6c79 2076 616c 6964 6174 6573 2074 6865  ly validates the
-00010970: 2063 6861 6e67 6573 206d 6164 652e 9485   changes made...
-00010980: 9481 947d 9428 681b 6aad 1200 0068 1c68  ...}.(h.j....h.h
-00010990: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-000109a0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-000109b0: 295d 9475 682b 68ed 681d 6acf 1100 0068  )].uh+h.h.j....h
-000109c0: 1e4b 0a68 1b6a a912 0000 7562 6168 1f7d  .K.h.j....ubah.}
-000109d0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000109e0: 5d94 6829 5d94 7568 2b6a 1312 0000 681b  ].h)].uh+j....h.
-000109f0: 6a10 1200 0068 1c68 0368 1d6a cf11 0000  j....h.h.h.j....
-00010a00: 681e 4e75 626a 1412 0000 2981 947d 9428  h.Nubj....)..}.(
-00010a10: 6805 8c2f 4275 696c 6420 616e 6420 7465  h../Build and te
-00010a20: 7374 206c 6f63 616c 6c79 2077 6974 6820  st locally with 
-00010a30: 6060 6d61 6b65 206c 6f63 616c 2074 6573  ``make local tes
-00010a40: 7460 6094 6807 5d94 68ee 2981 947d 9428  t``.h.].h.)..}.(
-00010a50: 6805 6ac2 1200 0068 075d 9428 6816 8c1c  h.j....h.].(h...
-00010a60: 4275 696c 6420 616e 6420 7465 7374 206c  Build and test l
-00010a70: 6f63 616c 6c79 2077 6974 6820 9485 9481  ocally with ....
-00010a80: 947d 9428 681b 6ac4 1200 0068 1c68 0368  .}.(h.j....h.h.h
-00010a90: 1d4e 681e 4e75 6268 f429 8194 7d94 2868  .Nh.Nubh.)..}.(h
-00010aa0: 058c 1360 606d 616b 6520 6c6f 6361 6c20  ...``make local 
-00010ab0: 7465 7374 6060 9468 075d 9468 168c 0f6d  test``.h.].h...m
-00010ac0: 616b 6520 6c6f 6361 6c20 7465 7374 9485  ake local test..
-00010ad0: 9481 947d 9428 681b 6acb 1200 0068 1c68  ...}.(h.j....h.h
-00010ae0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
-00010af0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00010b00: 295d 9475 682b 68f3 681b 6ac4 1200 0075  )].uh+h.h.j....u
-00010b10: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
-00010b20: 255d 9468 275d 9468 295d 9475 682b 68ed  %].h'].h)].uh+h.
-00010b30: 681d 6acf 1100 0068 1e4b 0b68 1b6a c012  h.j....h.K.h.j..
-00010b40: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
-00010b50: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00010b60: 2b6a 1312 0000 681b 6a10 1200 0068 1c68  +j....h.j....h.h
-00010b70: 0368 1d6a cf11 0000 681e 4e75 626a 1412  .h.j....h.Nubj..
-00010b80: 0000 2981 947d 9428 6805 8c7f 5375 626d  ..)..}.(h...Subm
-00010b90: 6974 2061 2060 7075 6c6c 2072 6571 7565  it a `pull reque
-00010ba0: 7374 7320 3c68 7474 7073 3a2f 2f68 656c  sts <https://hel
-00010bb0: 702e 6769 7468 7562 2e63 6f6d 2f65 6e2f  p.github.com/en/
-00010bc0: 6172 7469 636c 6573 2f63 7265 6174 696e  articles/creatin
-00010bd0: 672d 612d 7075 6c6c 2d72 6571 7565 7374  g-a-pull-request
-00010be0: 2d66 726f 6d2d 612d 666f 726b 3e60 5f20  -from-a-fork>`_ 
-00010bf0: 746f 2067 6574 2074 6865 2063 6861 6e67  to get the chang
-00010c00: 6573 206d 6572 6765 642e 0a94 6807 5d94  es merged...h.].
-00010c10: 68ee 2981 947d 9428 6805 8c7e 5375 626d  h.)..}.(h..~Subm
-00010c20: 6974 2061 2060 7075 6c6c 2072 6571 7565  it a `pull reque
-00010c30: 7374 7320 3c68 7474 7073 3a2f 2f68 656c  sts <https://hel
-00010c40: 702e 6769 7468 7562 2e63 6f6d 2f65 6e2f  p.github.com/en/
-00010c50: 6172 7469 636c 6573 2f63 7265 6174 696e  articles/creatin
-00010c60: 672d 612d 7075 6c6c 2d72 6571 7565 7374  g-a-pull-request
-00010c70: 2d66 726f 6d2d 612d 666f 726b 3e60 5f20  -from-a-fork>`_ 
-00010c80: 746f 2067 6574 2074 6865 2063 6861 6e67  to get the chang
-00010c90: 6573 206d 6572 6765 642e 9468 075d 9428  es merged..h.].(
-00010ca0: 6816 8c09 5375 626d 6974 2061 2094 8594  h...Submit a ...
-00010cb0: 8194 7d94 2868 1b6a e912 0000 681c 6803  ..}.(h.j....h.h.
-00010cc0: 681d 4e68 1e4e 7562 6843 2981 947d 9428  h.Nh.NubhC)..}.(
-00010cd0: 6805 8c5a 6070 756c 6c20 7265 7175 6573  h..Z`pull reques
-00010ce0: 7473 203c 6874 7470 733a 2f2f 6865 6c70  ts <https://help
-00010cf0: 2e67 6974 6875 622e 636f 6d2f 656e 2f61  .github.com/en/a
-00010d00: 7274 6963 6c65 732f 6372 6561 7469 6e67  rticles/creating
-00010d10: 2d61 2d70 756c 6c2d 7265 7175 6573 742d  -a-pull-request-
-00010d20: 6672 6f6d 2d61 2d66 6f72 6b3e 605f 9468  from-a-fork>`_.h
-00010d30: 075d 9468 168c 0d70 756c 6c20 7265 7175  .].h...pull requ
-00010d40: 6573 7473 9485 9481 947d 9428 681b 6af1  ests.....}.(h.j.
-00010d50: 1200 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
-00010d60: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00010d70: 9468 275d 9468 295d 948c 046e 616d 6594  .h'].h)]...name.
-00010d80: 8c0d 7075 6c6c 2072 6571 7565 7374 7394  ..pull requests.
-00010d90: 6a45 0100 008c 4768 7474 7073 3a2f 2f68  jE....Ghttps://h
-00010da0: 656c 702e 6769 7468 7562 2e63 6f6d 2f65  elp.github.com/e
-00010db0: 6e2f 6172 7469 636c 6573 2f63 7265 6174  n/articles/creat
-00010dc0: 696e 672d 612d 7075 6c6c 2d72 6571 7565  ing-a-pull-reque
-00010dd0: 7374 2d66 726f 6d2d 612d 666f 726b 9475  st-from-a-fork.u
-00010de0: 682b 6842 681b 6ae9 1200 0075 626a 4801  h+hBh.j....ubjH.
-00010df0: 0000 2981 947d 9428 6805 8c4a 203c 6874  ..)..}.(h..J <ht
-00010e00: 7470 733a 2f2f 6865 6c70 2e67 6974 6875  tps://help.githu
-00010e10: 622e 636f 6d2f 656e 2f61 7274 6963 6c65  b.com/en/article
-00010e20: 732f 6372 6561 7469 6e67 2d61 2d70 756c  s/creating-a-pul
-00010e30: 6c2d 7265 7175 6573 742d 6672 6f6d 2d61  l-request-from-a
-00010e40: 2d66 6f72 6b3e 9468 075d 9468 1f7d 9428  -fork>.h.].h.}.(
-00010e50: 6821 5d94 8c0d 7075 6c6c 2d72 6571 7565  h!]...pull-reque
-00010e60: 7374 7394 6168 235d 9468 255d 948c 0d70  sts.ah#].h%]...p
-00010e70: 756c 6c20 7265 7175 6573 7473 9461 6827  ull requests.ah'
-00010e80: 5d94 6829 5d94 8c06 7265 6675 7269 946a  ].h)]...refuri.j
-00010e90: 0113 0000 7568 2b6a 4701 0000 6a56 0100  ....uh+jG...jV..
-00010ea0: 004b 0168 1b6a e912 0000 7562 6816 8c1b  .K.h.j....ubh...
-00010eb0: 2074 6f20 6765 7420 7468 6520 6368 616e   to get the chan
-00010ec0: 6765 7320 6d65 7267 6564 2e94 8594 8194  ges merged......
-00010ed0: 7d94 2868 1b6a e912 0000 681c 6803 681d  }.(h.j....h.h.h.
-00010ee0: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
-00010ef0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00010f00: 7568 2b68 ed68 1d6a cf11 0000 681e 4b0c  uh+h.h.j....h.K.
-00010f10: 681b 6ae5 1200 0075 6261 681f 7d94 2868  h.j....ubah.}.(h
-00010f20: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00010f30: 295d 9475 682b 6a13 1200 0068 1b6a 1012  )].uh+j....h.j..
-00010f40: 0000 681c 6803 681d 6acf 1100 0068 1e4e  ..h.h.h.j....h.N
-00010f50: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-00010f60: 6825 5d94 6827 5d94 6829 5d94 8c08 656e  h%].h'].h)]...en
-00010f70: 756d 7479 7065 948c 0661 7261 6269 6394  umtype...arabic.
-00010f80: 8c06 7072 6566 6978 9468 068c 0673 7566  ..prefix.h...suf
-00010f90: 6669 7894 8c01 2e94 7568 2b6a 0e12 0000  fix.....uh+j....
-00010fa0: 681b 6abe 1100 0068 1c68 0368 1d6a cf11  h.j....h.h.h.j..
-00010fb0: 0000 681e 4b08 7562 68ee 2981 947d 9428  ..h.K.ubh.)..}.(
-00010fc0: 6805 8c9d 416c 736f 2062 6520 7375 7265  h...Also be sure
-00010fd0: 2074 6f20 7265 7669 6577 2074 6865 2060   to review the `
-00010fe0: 436f 6465 206f 6620 436f 6e64 7563 7420  Code of Conduct 
-00010ff0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00011000: 636f 6d2f 616c 6578 646c 6169 7264 2f70  com/alexdlaird/p
-00011010: 796e 6772 6f6b 2f62 6c6f 622f 6d61 696e  yngrok/blob/main
-00011020: 2f43 4f44 455f 4f46 5f43 4f4e 4455 4354  /CODE_OF_CONDUCT
-00011030: 2e6d 643e 605f 2062 6566 6f72 650a 7375  .md>`_ before.su
-00011040: 626d 6974 7469 6e67 2069 7373 7565 7320  bmitting issues 
-00011050: 6f72 2070 756c 6c20 7265 7175 6573 7473  or pull requests
-00011060: 2e94 6807 5d94 2868 168c 1b41 6c73 6f20  ..h.].(h...Also 
-00011070: 6265 2073 7572 6520 746f 2072 6576 6965  be sure to revie
-00011080: 7720 7468 6520 9485 9481 947d 9428 681b  w the .....}.(h.
-00011090: 6a2a 1300 0068 1c68 0368 1d4e 681e 4e75  j*...h.h.h.Nh.Nu
-000110a0: 6268 4329 8194 7d94 2868 058c 5760 436f  bhC)..}.(h..W`Co
-000110b0: 6465 206f 6620 436f 6e64 7563 7420 3c68  de of Conduct <h
-000110c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000110d0: 6d2f 616c 6578 646c 6169 7264 2f70 796e  m/alexdlaird/pyn
-000110e0: 6772 6f6b 2f62 6c6f 622f 6d61 696e 2f43  grok/blob/main/C
-000110f0: 4f44 455f 4f46 5f43 4f4e 4455 4354 2e6d  ODE_OF_CONDUCT.m
-00011100: 643e 605f 9468 075d 9468 168c 0f43 6f64  d>`_.h.].h...Cod
-00011110: 6520 6f66 2043 6f6e 6475 6374 9485 9481  e of Conduct....
-00011120: 947d 9428 681b 6a32 1300 0068 1c68 0368  .}.(h.j2...h.h.h
-00011130: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00011140: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00011150: 948c 046e 616d 6594 8c0f 436f 6465 206f  ...name...Code o
-00011160: 6620 436f 6e64 7563 7494 6a45 0100 008c  f Conduct.jE....
-00011170: 4268 7474 7073 3a2f 2f67 6974 6875 622e  Bhttps://github.
-00011180: 636f 6d2f 616c 6578 646c 6169 7264 2f70  com/alexdlaird/p
-00011190: 796e 6772 6f6b 2f62 6c6f 622f 6d61 696e  yngrok/blob/main
-000111a0: 2f43 4f44 455f 4f46 5f43 4f4e 4455 4354  /CODE_OF_CONDUCT
-000111b0: 2e6d 6494 7568 2b68 4268 1b6a 2a13 0000  .md.uh+hBh.j*...
-000111c0: 7562 6a48 0100 0029 8194 7d94 2868 058c  ubjH...)..}.(h..
-000111d0: 4520 3c68 7474 7073 3a2f 2f67 6974 6875  E <https://githu
-000111e0: 622e 636f 6d2f 616c 6578 646c 6169 7264  b.com/alexdlaird
-000111f0: 2f70 796e 6772 6f6b 2f62 6c6f 622f 6d61  /pyngrok/blob/ma
-00011200: 696e 2f43 4f44 455f 4f46 5f43 4f4e 4455  in/CODE_OF_CONDU
-00011210: 4354 2e6d 643e 9468 075d 9468 1f7d 9428  CT.md>.h.].h.}.(
-00011220: 6821 5d94 8c0f 636f 6465 2d6f 662d 636f  h!]...code-of-co
-00011230: 6e64 7563 7494 6168 235d 9468 255d 948c  nduct.ah#].h%]..
-00011240: 0f63 6f64 6520 6f66 2063 6f6e 6475 6374  .code of conduct
-00011250: 9461 6827 5d94 6829 5d94 8c06 7265 6675  .ah'].h)]...refu
-00011260: 7269 946a 4213 0000 7568 2b6a 4701 0000  ri.jB...uh+jG...
-00011270: 6a56 0100 004b 0168 1b6a 2a13 0000 7562  jV...K.h.j*...ub
-00011280: 6816 8c2b 2062 6566 6f72 650a 7375 626d  h..+ before.subm
-00011290: 6974 7469 6e67 2069 7373 7565 7320 6f72  itting issues or
-000112a0: 2070 756c 6c20 7265 7175 6573 7473 2e94   pull requests..
-000112b0: 8594 8194 7d94 2868 1b6a 2a13 0000 681c  ....}.(h.j*...h.
-000112c0: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
-000112d0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000112e0: 6829 5d94 7568 2b68 ed68 1d6a cf11 0000  h)].uh+h.h.j....
-000112f0: 681e 4b0e 681b 6abe 1100 0068 1c68 0375  h.K.h.j....h.h.u
-00011300: 6268 ee29 8194 7d94 2868 058c 9757 616e  bh.)..}.(h...Wan
-00011310: 7420 746f 2063 6f6e 7472 6962 7574 6520  t to contribute 
-00011320: 6669 6e61 6e63 6961 6c6c 793f 2049 6620  financially? If 
-00011330: 796f 7527 7665 2066 6f75 6e64 2060 6070  you've found ``p
-00011340: 796e 6772 6f6b 6060 2075 7365 6675 6c2c  yngrok`` useful,
-00011350: 2060 6120 646f 6e61 7469 6f6e 203c 6874   `a donation <ht
-00011360: 7470 733a 2f2f 7777 772e 7061 7970 616c  tps://www.paypal
-00011370: 2e6d 652f 616c 6578 646c 6169 7264 3e60  .me/alexdlaird>`
-00011380: 5f0a 776f 756c 6420 616c 736f 2062 6520  _.would also be 
-00011390: 6772 6561 746c 7920 6170 7072 6563 6961  greatly apprecia
-000113a0: 7465 6421 9468 075d 9428 6816 8c32 5761  ted!.h.].(h..2Wa
-000113b0: 6e74 2074 6f20 636f 6e74 7269 6275 7465  nt to contribute
-000113c0: 2066 696e 616e 6369 616c 6c79 3f20 4966   financially? If
-000113d0: 2079 6f75 e280 9976 6520 666f 756e 6420   you...ve found 
-000113e0: 9485 9481 947d 9428 681b 6a5a 1300 0068  .....}.(h.jZ...h
-000113f0: 1c68 0368 1d4e 681e 4e75 6268 f429 8194  .h.h.Nh.Nubh.)..
-00011400: 7d94 2868 058c 0b60 6070 796e 6772 6f6b  }.(h...``pyngrok
-00011410: 6060 9468 075d 9468 168c 0770 796e 6772  ``.h.].h...pyngr
-00011420: 6f6b 9485 9481 947d 9428 681b 6a62 1300  ok.....}.(h.jb..
-00011430: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
-00011440: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00011450: 275d 9468 295d 9475 682b 68f3 681b 6a5a  '].h)].uh+h.h.jZ
-00011460: 1300 0075 6268 168c 0920 7573 6566 756c  ...ubh... useful
-00011470: 2c20 9485 9481 947d 9428 681b 6a5a 1300  , .....}.(h.jZ..
-00011480: 0068 1c68 0368 1d4e 681e 4e75 6268 4329  .h.h.h.Nh.NubhC)
-00011490: 8194 7d94 2868 058c 3060 6120 646f 6e61  ..}.(h..0`a dona
-000114a0: 7469 6f6e 203c 6874 7470 733a 2f2f 7777  tion <https://ww
-000114b0: 772e 7061 7970 616c 2e6d 652f 616c 6578  w.paypal.me/alex
-000114c0: 646c 6169 7264 3e60 5f94 6807 5d94 6816  dlaird>`_.h.].h.
-000114d0: 8c0a 6120 646f 6e61 7469 6f6e 9485 9481  ..a donation....
-000114e0: 947d 9428 681b 6a74 1300 0068 1c68 0368  .}.(h.jt...h.h.h
-000114f0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
-00011500: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00011510: 948c 046e 616d 6594 8c0a 6120 646f 6e61  ...name...a dona
-00011520: 7469 6f6e 946a 4501 0000 8c20 6874 7470  tion.jE.... http
-00011530: 733a 2f2f 7777 772e 7061 7970 616c 2e6d  s://www.paypal.m
-00011540: 652f 616c 6578 646c 6169 7264 9475 682b  e/alexdlaird.uh+
-00011550: 6842 681b 6a5a 1300 0075 626a 4801 0000  hBh.jZ...ubjH...
-00011560: 2981 947d 9428 6805 8c23 203c 6874 7470  )..}.(h..# <http
-00011570: 733a 2f2f 7777 772e 7061 7970 616c 2e6d  s://www.paypal.m
-00011580: 652f 616c 6578 646c 6169 7264 3e94 6807  e/alexdlaird>.h.
-00011590: 5d94 681f 7d94 2868 215d 948c 0a61 2d64  ].h.}.(h!]...a-d
-000115a0: 6f6e 6174 696f 6e94 6168 235d 9468 255d  onation.ah#].h%]
-000115b0: 948c 0a61 2064 6f6e 6174 696f 6e94 6168  ...a donation.ah
-000115c0: 275d 9468 295d 948c 0672 6566 7572 6994  '].h)]...refuri.
-000115d0: 6a84 1300 0075 682b 6a47 0100 006a 5601  j....uh+jG...jV.
-000115e0: 0000 4b01 681b 6a5a 1300 0075 6268 168c  ..K.h.jZ...ubh..
-000115f0: 230a 776f 756c 6420 616c 736f 2062 6520  #.would also be 
-00011600: 6772 6561 746c 7920 6170 7072 6563 6961  greatly apprecia
-00011610: 7465 6421 9485 9481 947d 9428 681b 6a5a  ted!.....}.(h.jZ
-00011620: 1300 0068 1c68 0368 1d4e 681e 4e75 6265  ...h.h.h.Nh.Nube
-00011630: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00011640: 9468 275d 9468 295d 9475 682b 68ed 681d  .h'].h)].uh+h.h.
-00011650: 6acf 1100 0068 1e4b 1168 1b6a be11 0000  j....h.K.h.j....
-00011660: 681c 6803 7562 6568 1f7d 9428 6821 5d94  h.h.ubeh.}.(h!].
-00011670: 8c0c 636f 6e74 7269 6275 7469 6e67 9461  ..contributing.a
-00011680: 6823 5d94 6825 5d94 8c0c 636f 6e74 7269  h#].h%]...contri
-00011690: 6275 7469 6e67 9461 6827 5d94 6829 5d94  buting.ah'].h)].
-000116a0: 7568 2b68 0a68 1b68 0c68 1c68 0368 1d6a  uh+h.h.h.h.h.h.j
-000116b0: cf11 0000 681e 4b02 7562 6568 1f7d 9428  ....h.K.ubeh.}.(
-000116c0: 6821 5d94 8c22 7079 6e67 726f 6b2d 612d  h!].."pyngrok-a-
-000116d0: 7079 7468 6f6e 2d77 7261 7070 6572 2d66  python-wrapper-f
-000116e0: 6f72 2d6e 6772 6f6b 9461 6823 5d94 8c0b  or-ngrok.ah#]...
-000116f0: 6869 6465 2d68 6561 6465 7294 6168 255d  hide-header.ah%]
-00011700: 948c 2470 796e 6772 6f6b 202d 2061 2070  ..$pyngrok - a p
-00011710: 7974 686f 6e20 7772 6170 7065 7220 666f  ython wrapper fo
-00011720: 7220 6e67 726f 6b94 6168 275d 9468 295d  r ngrok.ah'].h)]
-00011730: 9475 682b 680a 681b 6803 681c 6803 681d  .uh+h.h.h.h.h.h.
-00011740: 682c 681e 4b05 7562 6168 1f7d 9428 6821  h,h.K.ubah.}.(h!
-00011750: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00011760: 5d94 8c06 736f 7572 6365 9468 2c75 682b  ]...source.h,uh+
-00011770: 6801 8c0e 6375 7272 656e 745f 736f 7572  h...current_sour
-00011780: 6365 944e 8c0c 6375 7272 656e 745f 6c69  ce.N..current_li
-00011790: 6e65 944e 8c08 7365 7474 696e 6773 948c  ne.N..settings..
-000117a0: 1164 6f63 7574 696c 732e 6672 6f6e 7465  .docutils.fronte
-000117b0: 6e64 948c 0656 616c 7565 7394 9394 2981  nd...Values...).
-000117c0: 947d 9428 680f 4e8c 0967 656e 6572 6174  .}.(h.N..generat
-000117d0: 6f72 944e 8c09 6461 7465 7374 616d 7094  or.N..datestamp.
-000117e0: 4e8c 0b73 6f75 7263 655f 6c69 6e6b 944e  N..source_link.N
-000117f0: 8c0a 736f 7572 6365 5f75 726c 944e 8c0d  ..source_url.N..
-00011800: 746f 635f 6261 636b 6c69 6e6b 7394 8c05  toc_backlinks...
-00011810: 656e 7472 7994 8c12 666f 6f74 6e6f 7465  entry...footnote
-00011820: 5f62 6163 6b6c 696e 6b73 944b 018c 0d73  _backlinks.K...s
-00011830: 6563 746e 756d 5f78 666f 726d 944b 018c  ectnum_xform.K..
-00011840: 0e73 7472 6970 5f63 6f6d 6d65 6e74 7394  .strip_comments.
-00011850: 4e8c 1b73 7472 6970 5f65 6c65 6d65 6e74  N..strip_element
-00011860: 735f 7769 7468 5f63 6c61 7373 6573 944e  s_with_classes.N
-00011870: 8c0d 7374 7269 705f 636c 6173 7365 7394  ..strip_classes.
-00011880: 4e8c 0c72 6570 6f72 745f 6c65 7665 6c94  N..report_level.
-00011890: 4b02 8c0a 6861 6c74 5f6c 6576 656c 944b  K...halt_level.K
-000118a0: 058c 1165 7869 745f 7374 6174 7573 5f6c  ...exit_status_l
-000118b0: 6576 656c 944b 058c 0564 6562 7567 944e  evel.K...debug.N
-000118c0: 8c0e 7761 726e 696e 675f 7374 7265 616d  ..warning_stream
-000118d0: 944e 8c09 7472 6163 6562 6163 6b94 888c  .N..traceback...
-000118e0: 0e69 6e70 7574 5f65 6e63 6f64 696e 6794  .input_encoding.
-000118f0: 8c09 7574 662d 382d 7369 6794 8c1c 696e  ..utf-8-sig...in
-00011900: 7075 745f 656e 636f 6469 6e67 5f65 7272  put_encoding_err
-00011910: 6f72 5f68 616e 646c 6572 948c 0673 7472  or_handler...str
-00011920: 6963 7494 8c0f 6f75 7470 7574 5f65 6e63  ict...output_enc
-00011930: 6f64 696e 6794 8c05 7574 662d 3894 8c1d  oding...utf-8...
-00011940: 6f75 7470 7574 5f65 6e63 6f64 696e 675f  output_encoding_
-00011950: 6572 726f 725f 6861 6e64 6c65 7294 6ad0  error_handler.j.
-00011960: 1300 008c 0e65 7272 6f72 5f65 6e63 6f64  .....error_encod
-00011970: 696e 6794 8c05 7574 662d 3894 8c1c 6572  ing...utf-8...er
-00011980: 726f 725f 656e 636f 6469 6e67 5f65 7272  ror_encoding_err
-00011990: 6f72 5f68 616e 646c 6572 948c 1062 6163  or_handler...bac
-000119a0: 6b73 6c61 7368 7265 706c 6163 6594 8c0d  kslashreplace...
-000119b0: 6c61 6e67 7561 6765 5f63 6f64 6594 8c02  language_code...
-000119c0: 656e 948c 1372 6563 6f72 645f 6465 7065  en...record_depe
-000119d0: 6e64 656e 6369 6573 944e 8c06 636f 6e66  ndencies.N..conf
-000119e0: 6967 944e 8c09 6964 5f70 7265 6669 7894  ig.N..id_prefix.
-000119f0: 6806 8c0e 6175 746f 5f69 645f 7072 6566  h...auto_id_pref
-00011a00: 6978 948c 0269 6494 8c0d 6475 6d70 5f73  ix...id...dump_s
-00011a10: 6574 7469 6e67 7394 4e8c 0e64 756d 705f  ettings.N..dump_
-00011a20: 696e 7465 726e 616c 7394 4e8c 0f64 756d  internals.N..dum
-00011a30: 705f 7472 616e 7366 6f72 6d73 944e 8c0f  p_transforms.N..
-00011a40: 6475 6d70 5f70 7365 7564 6f5f 786d 6c94  dump_pseudo_xml.
-00011a50: 4e8c 1065 7870 6f73 655f 696e 7465 726e  N..expose_intern
-00011a60: 616c 7394 4e8c 0e73 7472 6963 745f 7669  als.N..strict_vi
-00011a70: 7369 746f 7294 4e8c 0f5f 6469 7361 626c  sitor.N.._disabl
-00011a80: 655f 636f 6e66 6967 944e 8c07 5f73 6f75  e_config.N.._sou
-00011a90: 7263 6594 682c 8c0c 5f64 6573 7469 6e61  rce.h,.._destina
-00011aa0: 7469 6f6e 944e 8c0d 5f63 6f6e 6669 675f  tion.N.._config_
-00011ab0: 6669 6c65 7394 5d94 8c16 6669 6c65 5f69  files.]...file_i
-00011ac0: 6e73 6572 7469 6f6e 5f65 6e61 626c 6564  nsertion_enabled
-00011ad0: 9488 8c0b 7261 775f 656e 6162 6c65 6494  ....raw_enabled.
-00011ae0: 4b01 8c11 6c69 6e65 5f6c 656e 6774 685f  K...line_length_
-00011af0: 6c69 6d69 7494 4d10 278c 0e70 6570 5f72  limit.M.'..pep_r
-00011b00: 6566 6572 656e 6365 7394 4e8c 0c70 6570  eferences.N..pep
-00011b10: 5f62 6173 655f 7572 6c94 8c18 6874 7470  _base_url...http
-00011b20: 733a 2f2f 7065 7073 2e70 7974 686f 6e2e  s://peps.python.
-00011b30: 6f72 672f 948c 1570 6570 5f66 696c 655f  org/...pep_file_
-00011b40: 7572 6c5f 7465 6d70 6c61 7465 948c 0870  url_template...p
-00011b50: 6570 2d25 3034 6494 8c0e 7266 635f 7265  ep-%04d...rfc_re
-00011b60: 6665 7265 6e63 6573 944e 8c0c 7266 635f  ferences.N..rfc_
-00011b70: 6261 7365 5f75 726c 948c 2668 7474 7073  base_url..&https
-00011b80: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
-00011b90: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
-00011ba0: 2f94 8c09 7461 625f 7769 6474 6894 4b08  /...tab_width.K.
-00011bb0: 8c1d 7472 696d 5f66 6f6f 746e 6f74 655f  ..trim_footnote_
-00011bc0: 7265 6665 7265 6e63 655f 7370 6163 6594  reference_space.
-00011bd0: 898c 1073 796e 7461 785f 6869 6768 6c69  ...syntax_highli
-00011be0: 6768 7494 8c04 6c6f 6e67 948c 0c73 6d61  ght...long...sma
-00011bf0: 7274 5f71 756f 7465 7394 888c 1373 6d61  rt_quotes....sma
-00011c00: 7274 7175 6f74 6573 5f6c 6f63 616c 6573  rtquotes_locales
-00011c10: 945d 948c 1d63 6861 7261 6374 6572 5f6c  .]...character_l
-00011c20: 6576 656c 5f69 6e6c 696e 655f 6d61 726b  evel_inline_mark
-00011c30: 7570 9489 8c0e 646f 6374 6974 6c65 5f78  up....doctitle_x
-00011c40: 666f 726d 9489 8c0d 646f 6369 6e66 6f5f  form....docinfo_
-00011c50: 7866 6f72 6d94 4b01 8c12 7365 6374 7375  xform.K...sectsu
-00011c60: 6274 6974 6c65 5f78 666f 726d 9489 8c0d  btitle_xform....
-00011c70: 696d 6167 655f 6c6f 6164 696e 6794 8c04  image_loading...
-00011c80: 6c69 6e6b 948c 1065 6d62 6564 5f73 7479  link...embed_sty
-00011c90: 6c65 7368 6565 7494 898c 1563 6c6f 616b  lesheet....cloak
-00011ca0: 5f65 6d61 696c 5f61 6464 7265 7373 6573  _email_addresses
-00011cb0: 9488 8c11 7365 6374 696f 6e5f 7365 6c66  ....section_self
-00011cc0: 5f6c 696e 6b94 898c 0365 6e76 944e 7562  _link....env.Nub
-00011cd0: 8c08 7265 706f 7274 6572 944e 8c10 696e  ..reporter.N..in
-00011ce0: 6469 7265 6374 5f74 6172 6765 7473 945d  direct_targets.]
-00011cf0: 948c 1173 7562 7374 6974 7574 696f 6e5f  ...substitution_
-00011d00: 6465 6673 947d 948c 1273 7562 7374 6974  defs.}...substit
-00011d10: 7574 696f 6e5f 6e61 6d65 7394 7d94 8c08  ution_names.}...
-00011d20: 7265 666e 616d 6573 947d 948c 0672 6566  refnames.}...ref
-00011d30: 6964 7394 7d94 8c07 6e61 6d65 6964 7394  ids.}...nameids.
-00011d40: 7d94 286a aa13 0000 6aa6 1300 006a 5201  }.(j....j....jR.
-00011d50: 0000 6a4f 0100 006a 9602 0000 6a93 0200  ..jO...j....j...
-00011d60: 006a b401 0000 6ab1 0100 006a 4f02 0000  .j....j....jO...
-00011d70: 6a4c 0200 006a 8302 0000 6a80 0200 006a  jL...j....j....j
-00011d80: 9904 0000 6a96 0400 006a 9303 0000 6a90  ....j....j....j.
-00011d90: 0300 006a 2a05 0000 6a27 0500 006a 8505  ...j*...j'...j..
-00011da0: 0000 6a82 0500 006a 6807 0000 6a65 0700  ..j....jh...je..
-00011db0: 006a ae06 0000 6aab 0600 006a c508 0000  .j....j....j....
-00011dc0: 6ac2 0800 006a 7209 0000 6a6f 0900 006a  j....jr...jo...j
-00011dd0: 4f09 0000 6a4c 0900 006a 4e10 0000 6a4b  O...jL...jN...jK
-00011de0: 1000 006a b50c 0000 6ab2 0c00 006a 940d  ...j....j....j..
-00011df0: 0000 6a91 0d00 006a 0b0d 0000 6a08 0d00  ..j....j....j...
-00011e00: 006a 330e 0000 6a30 0e00 006a 260f 0000  .j3...j0...j&...
-00011e10: 6a23 0f00 006a b50f 0000 6ab2 0f00 006a  j#...j....j....j
-00011e20: 5c0f 0000 6a59 0f00 006a 4610 0000 6a43  \...jY...jF...jC
-00011e30: 1000 006a eb10 0000 6ae8 1000 006a d810  ...j....j....j..
-00011e40: 0000 6ad5 1000 006a 6a11 0000 6a67 1100  ..j....jj...jg..
-00011e50: 006a 5711 0000 6a54 1100 006a bb11 0000  .jW...jT...j....
-00011e60: 6ab8 1100 006a a113 0000 6a9e 1300 006a  j....j....j....j
-00011e70: f211 0000 6aef 1100 006a 3a12 0000 6a37  ....j....j:...j7
-00011e80: 1200 006a 5c12 0000 6a59 1200 006a 9512  ...j\...jY...j..
-00011e90: 0000 6a92 1200 006a 0b13 0000 6a08 1300  ..j....j....j...
-00011ea0: 006a 4c13 0000 6a49 1300 006a 8e13 0000  .jL...jI...j....
-00011eb0: 6a8b 1300 0075 8c09 6e61 6d65 7479 7065  j....u..nametype
-00011ec0: 7394 7d94 286a aa13 0000 896a 5201 0000  s.}.(j.....jR...
-00011ed0: 886a 9602 0000 896a b401 0000 886a 4f02  .j.....j.....jO.
-00011ee0: 0000 886a 8302 0000 886a 9904 0000 896a  ...j.....j.....j
-00011ef0: 9303 0000 886a 2a05 0000 896a 8505 0000  .....j*....j....
-00011f00: 896a 6807 0000 896a ae06 0000 886a c508  .jh....j.....j..
-00011f10: 0000 896a 7209 0000 896a 4f09 0000 886a  ...jr....jO....j
-00011f20: 4e10 0000 896a b50c 0000 896a 940d 0000  N....j.....j....
-00011f30: 896a 0b0d 0000 886a 330e 0000 896a 260f  .j.....j3....j&.
-00011f40: 0000 896a b50f 0000 896a 5c0f 0000 886a  ...j.....j\....j
-00011f50: 4610 0000 896a eb10 0000 896a d810 0000  F....j.....j....
-00011f60: 886a 6a11 0000 896a 5711 0000 886a bb11  .jj....jW....j..
-00011f70: 0000 896a a113 0000 896a f211 0000 886a  ...j.....j.....j
-00011f80: 3a12 0000 886a 5c12 0000 886a 9512 0000  :....j\....j....
-00011f90: 886a 0b13 0000 886a 4c13 0000 886a 8e13  .j.....jL....j..
-00011fa0: 0000 8875 6821 7d94 286a a613 0000 680c  ...uh!}.(j....h.
-00011fb0: 6a4f 0100 006a 4901 0000 6a93 0200 006a  jO...jI...j....j
-00011fc0: 7301 0000 6ab1 0100 006a ab01 0000 6a4c  s...j....j....jL
-00011fd0: 0200 006a 4602 0000 6a80 0200 006a 7a02  ...jF...j....jz.
-00011fe0: 0000 6a96 0400 006a 9902 0000 6a90 0300  ..j....j....j...
-00011ff0: 006a 8a03 0000 6a27 0500 006a 9c04 0000  .j....j'...j....
-00012000: 6a82 0500 006a 2d05 0000 6a65 0700 006a  j....j-...je...j
-00012010: 8805 0000 6aab 0600 006a a506 0000 6ac2  ....j....j....j.
-00012020: 0800 006a 6b07 0000 6a6f 0900 006a c808  ...jk...jo...j..
-00012030: 0000 6a4c 0900 006a 4609 0000 6a4b 1000  ..jL...jF...jK..
-00012040: 006a 7509 0000 6ab2 0c00 006a 8609 0000  .ju...j....j....
-00012050: 6a91 0d00 006a b80c 0000 6a08 0d00 006a  j....j....j....j
-00012060: 020d 0000 6a30 0e00 006a 970d 0000 6a23  ....j0...j....j#
-00012070: 0f00 006a 360e 0000 6a86 0e00 006a 800e  ...j6...j....j..
-00012080: 0000 6ab2 0f00 006a 290f 0000 6a59 0f00  ..j....j)...jY..
-00012090: 006a 530f 0000 6a43 1000 006a b80f 0000  .jS...jC...j....
-000120a0: 6ae8 1000 006a 5110 0000 6ad5 1000 006a  j....jQ...j....j
-000120b0: cf10 0000 6a67 1100 006a ee10 0000 6a54  ....jg...j....jT
-000120c0: 1100 006a 4e11 0000 6ab8 1100 006a 6d11  ...jN...j....jm.
-000120d0: 0000 6a9e 1300 006a be11 0000 6aef 1100  ..j....j....j...
-000120e0: 006a e911 0000 6a37 1200 006a 3112 0000  .j....j7...j1...
-000120f0: 6a59 1200 006a 5312 0000 6a92 1200 006a  jY...jS...j....j
-00012100: 8c12 0000 6a08 1300 006a 0213 0000 6a49  ....j....j....jI
-00012110: 1300 006a 4313 0000 6a8b 1300 006a 8513  ...jC...j....j..
-00012120: 0000 758c 0d66 6f6f 746e 6f74 655f 7265  ..u..footnote_re
-00012130: 6673 947d 948c 0d63 6974 6174 696f 6e5f  fs.}...citation_
-00012140: 7265 6673 947d 948c 0d61 7574 6f66 6f6f  refs.}...autofoo
-00012150: 746e 6f74 6573 945d 948c 1161 7574 6f66  tnotes.]...autof
-00012160: 6f6f 746e 6f74 655f 7265 6673 945d 948c  ootnote_refs.]..
-00012170: 1073 796d 626f 6c5f 666f 6f74 6e6f 7465  .symbol_footnote
-00012180: 7394 5d94 8c14 7379 6d62 6f6c 5f66 6f6f  s.]...symbol_foo
-00012190: 746e 6f74 655f 7265 6673 945d 948c 0966  tnote_refs.]...f
-000121a0: 6f6f 746e 6f74 6573 945d 948c 0963 6974  ootnotes.]...cit
-000121b0: 6174 696f 6e73 945d 948c 1261 7574 6f66  ations.]...autof
-000121c0: 6f6f 746e 6f74 655f 7374 6172 7494 4b01  ootnote_start.K.
-000121d0: 8c15 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-000121e0: 655f 7374 6172 7494 4b00 8c0a 6964 5f63  e_start.K...id_c
-000121f0: 6f75 6e74 6572 948c 0b63 6f6c 6c65 6374  ounter...collect
-00012200: 696f 6e73 948c 0743 6f75 6e74 6572 9493  ions...Counter..
-00012210: 947d 946a de13 0000 4b01 7385 9452 948c  .}.j....K.s..R..
-00012220: 0e70 6172 7365 5f6d 6573 7361 6765 7394  .parse_messages.
-00012230: 5d94 6809 8c0e 7379 7374 656d 5f6d 6573  ].h...system_mes
-00012240: 7361 6765 9493 9429 8194 7d94 2868 0568  sage...)..}.(h.h
-00012250: 0668 075d 9468 ee29 8194 7d94 2868 058c  .h.].h.)..}.(h..
-00012260: 3544 7570 6c69 6361 7465 2065 7870 6c69  5Duplicate expli
-00012270: 6369 7420 7461 7267 6574 206e 616d 653a  cit target name:
-00012280: 2022 7375 7070 6f72 7465 6420 6279 206e   "supported by n
-00012290: 6772 6f6b 222e 9468 075d 9468 168c 3944  grok"..h.].h..9D
-000122a0: 7570 6c69 6361 7465 2065 7870 6c69 6369  uplicate explici
-000122b0: 7420 7461 7267 6574 206e 616d 653a 20e2  t target name: .
-000122c0: 809c 7375 7070 6f72 7465 6420 6279 206e  ..supported by n
-000122d0: 6772 6f6b e280 9d2e 9485 9481 947d 9428  grok.........}.(
-000122e0: 681b 6a36 1400 0068 1c68 0368 1d4e 681e  h.j6...h.h.h.Nh.
-000122f0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
-00012300: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00012310: 68ed 681b 6a33 1400 0075 6261 681f 7d94  h.h.j3...ubah.}.
-00012320: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
-00012330: 9468 295d 946a 860e 0000 618c 056c 6576  .h)].j....a..lev
-00012340: 656c 944b 018c 0474 7970 6594 8c04 494e  el.K...type...IN
-00012350: 464f 948c 0673 6f75 7263 6594 682c 8c04  FO...source.h,..
-00012360: 6c69 6e65 944b 0575 682b 6a31 1400 0068  line.K.uh+j1...h
-00012370: 1b6a 360e 0000 681c 6803 681d 682c 681e  .j6...h.h.h.h,h.
-00012380: 4d39 0175 6261 8c12 7472 616e 7366 6f72  M9.uba..transfor
-00012390: 6d5f 6d65 7373 6167 6573 945d 948c 0b74  m_messages.]...t
-000123a0: 7261 6e73 666f 726d 6572 944e 8c0b 696e  ransformer.N..in
-000123b0: 636c 7564 655f 6c6f 6794 5d94 8c0e 646f  clude_log.]...do
-000123c0: 6373 2f69 6e64 6578 2e72 7374 9428 4e4e  cs/index.rst.(NN
-000123d0: 4e4e 7494 8694 618c 0a64 6563 6f72 6174  NNt...a..decorat
-000123e0: 696f 6e94 4e68 1c68 0375 622e            ion.Nh.h.ub.
+00009d00: 0000 681c 6803 7562 6ab7 0300 0029 8194  ..h.h.ubj....)..
+00009d10: 7d94 2868 0558 a702 0000 4966 2060 606e  }.(h.X....If ``n
+00009d20: 6772 6f6b 6060 2069 7320 6e6f 7420 616c  grok`` is not al
+00009d30: 7265 6164 7920 696e 7374 616c 6c65 6420  ready installed 
+00009d40: 6174 2074 6865 2060 606e 6772 6f6b 5f70  at the ``ngrok_p
+00009d50: 6174 6860 6020 696e 203a 636c 6173 733a  ath`` in :class:
+00009d60: 607e 7079 6e67 726f 6b2e 636f 6e66 2e50  `~pyngrok.conf.P
+00009d70: 796e 6772 6f6b 436f 6e66 6967 602c 2069  yngrokConfig`, i
+00009d80: 740a 7769 6c6c 2062 6520 696e 7374 616c  t.will be instal
+00009d90: 6c65 6420 7468 6520 6669 7273 7420 7469  led the first ti
+00009da0: 6d65 206d 6f73 7420 6d65 7468 6f64 7320  me most methods 
+00009db0: 696e 2074 6865 203a 6d6f 643a 607e 7079  in the :mod:`~py
+00009dc0: 6e67 726f 6b2e 6e67 726f 6b60 206d 6f64  ngrok.ngrok` mod
+00009dd0: 756c 6520 6172 6520 6361 6c6c 6564 2e0a  ule are called..
+00009de0: 0a49 6620 7765 206e 6565 6420 746f 2063  .If we need to c
+00009df0: 7573 746f 6d69 7a65 2074 6865 2069 6e73  ustomize the ins
+00009e00: 7461 6c6c 6174 696f 6e20 6f66 2060 606e  tallation of ``n
+00009e10: 6772 6f6b 6060 2c20 7065 7268 6170 7320  grok``, perhaps 
+00009e20: 7370 6563 6966 7969 6e67 2061 2074 696d  specifying a tim
+00009e30: 656f 7574 2c20 7072 6f78 792c 2075 7365  eout, proxy, use
+00009e40: 2061 2063 7573 746f 6d20 6d69 7272 6f72   a custom mirror
+00009e50: 0a66 6f72 2074 6865 2064 6f77 6e6c 6f61  .for the downloa
+00009e60: 642c 2065 7463 2e20 7765 2063 616e 2064  d, etc. we can d
+00009e70: 6f20 736f 2062 7920 6c65 7665 7261 6769  o so by leveragi
+00009e80: 6e67 2074 6865 203a 6d6f 643a 607e 7079  ng the :mod:`~py
+00009e90: 6e67 726f 6b2e 696e 7374 616c 6c65 7260  ngrok.installer`
+00009ea0: 206d 6f64 756c 652e 204b 6579 776f 7264   module. Keyword
+00009eb0: 2061 7267 756d 656e 7473 2069 6e20 7468   arguments in th
+00009ec0: 6973 0a6d 6f64 756c 6520 6172 6520 756c  is.module are ul
+00009ed0: 7469 6d61 7465 6c79 2070 6173 7365 6420  timately passed 
+00009ee0: 646f 776e 2074 6f20 3a70 793a 6675 6e63  down to :py:func
+00009ef0: 3a60 7572 6c6c 6962 2e72 6571 7565 7374  :`urllib.request
+00009f00: 2e75 726c 6f70 656e 602c 2073 6f20 6173  .urlopen`, so as
+00009f10: 206c 6f6e 6720 6173 2077 6520 7573 6520   long as we use 
+00009f20: 7468 650a 3a6d 6f64 3a60 7e70 796e 6772  the.:mod:`~pyngr
+00009f30: 6f6b 2e69 6e73 7461 6c6c 6572 6020 6d6f  ok.installer` mo
+00009f40: 6475 6c65 206f 7572 7365 6c76 6573 2070  dule ourselves p
+00009f50: 7269 6f72 2074 6f20 696e 766f 6b69 6e67  rior to invoking
+00009f60: 2061 6e79 203a 6d6f 643a 607e 7079 6e67   any :mod:`~pyng
+00009f70: 726f 6b2e 6e67 726f 6b60 206d 6574 686f  rok.ngrok` metho
+00009f80: 6473 2c20 7765 2063 616e 2063 616e 2063  ds, we can can c
+00009f90: 6f6e 7472 6f6c 0a68 6f77 2060 606e 6772  ontrol.how ``ngr
+00009fa0: 6f6b 6060 2069 7320 696e 7374 616c 6c65  ok`` is installe
+00009fb0: 6420 616e 6420 6672 6f6d 2077 6865 7265  d and from where
+00009fc0: 2e94 6807 5d94 2868 ee29 8194 7d94 2868  ..h.].(h.)..}.(h
+00009fd0: 058c c549 6620 6060 6e67 726f 6b60 6020  ...If ``ngrok`` 
+00009fe0: 6973 206e 6f74 2061 6c72 6561 6479 2069  is not already i
+00009ff0: 6e73 7461 6c6c 6564 2061 7420 7468 6520  nstalled at the 
+0000a000: 6060 6e67 726f 6b5f 7061 7468 6060 2069  ``ngrok_path`` i
+0000a010: 6e20 3a63 6c61 7373 3a60 7e70 796e 6772  n :class:`~pyngr
+0000a020: 6f6b 2e63 6f6e 662e 5079 6e67 726f 6b43  ok.conf.PyngrokC
+0000a030: 6f6e 6669 6760 2c20 6974 0a77 696c 6c20  onfig`, it.will 
+0000a040: 6265 2069 6e73 7461 6c6c 6564 2074 6865  be installed the
+0000a050: 2066 6972 7374 2074 696d 6520 6d6f 7374   first time most
+0000a060: 206d 6574 686f 6473 2069 6e20 7468 6520   methods in the 
+0000a070: 3a6d 6f64 3a60 7e70 796e 6772 6f6b 2e6e  :mod:`~pyngrok.n
+0000a080: 6772 6f6b 6020 6d6f 6475 6c65 2061 7265  grok` module are
+0000a090: 2063 616c 6c65 642e 9468 075d 9428 6816   called..h.].(h.
+0000a0a0: 8c03 4966 2094 8594 8194 7d94 2868 1b6a  ..If .....}.(h.j
+0000a0b0: fa0a 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+0000a0c0: 68f4 2981 947d 9428 6805 8c09 6060 6e67  h.)..}.(h...``ng
+0000a0d0: 726f 6b60 6094 6807 5d94 6816 8c05 6e67  rok``.h.].h...ng
+0000a0e0: 726f 6b94 8594 8194 7d94 2868 1b6a 020b  rok.....}.(h.j..
+0000a0f0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+0000a100: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000a110: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
+0000a120: fa0a 0000 7562 6816 8c21 2069 7320 6e6f  ....ubh..! is no
+0000a130: 7420 616c 7265 6164 7920 696e 7374 616c  t already instal
+0000a140: 6c65 6420 6174 2074 6865 2094 8594 8194  led at the .....
+0000a150: 7d94 2868 1b6a fa0a 0000 681c 6803 681d  }.(h.j....h.h.h.
+0000a160: 4e68 1e4e 7562 68f4 2981 947d 9428 6805  Nh.Nubh.)..}.(h.
+0000a170: 8c0e 6060 6e67 726f 6b5f 7061 7468 6060  ..``ngrok_path``
+0000a180: 9468 075d 9468 168c 0a6e 6772 6f6b 5f70  .h.].h...ngrok_p
+0000a190: 6174 6894 8594 8194 7d94 2868 1b6a 140b  ath.....}.(h.j..
+0000a1a0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+0000a1b0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000a1c0: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
+0000a1d0: fa0a 0000 7562 6816 8c04 2069 6e20 9485  ....ubh... in ..
+0000a1e0: 9481 947d 9428 681b 6afa 0a00 0068 1c68  ...}.(h.j....h.h
+0000a1f0: 0368 1d4e 681e 4e75 626a b302 0000 2981  .h.Nh.Nubj....).
+0000a200: 947d 9428 6805 8c24 3a63 6c61 7373 3a60  .}.(h..$:class:`
+0000a210: 7e70 796e 6772 6f6b 2e63 6f6e 662e 5079  ~pyngrok.conf.Py
+0000a220: 6e67 726f 6b43 6f6e 6669 6760 9468 075d  ngrokConfig`.h.]
+0000a230: 9468 f429 8194 7d94 2868 056a 280b 0000  .h.)..}.(h.j(...
+0000a240: 6807 5d94 6816 8c0d 5079 6e67 726f 6b43  h.].h...PyngrokC
+0000a250: 6f6e 6669 6794 8594 8194 7d94 2868 1b6a  onfig.....}.(h.j
+0000a260: 2a0b 0000 681c 6803 681d 4e68 1e4e 7562  *...h.h.h.Nh.Nub
+0000a270: 6168 1f7d 9428 6821 5d94 6823 5d94 286a  ah.}.(h!].h#].(j
+0000a280: c202 0000 8c02 7079 948c 0870 792d 636c  ......py...py-cl
+0000a290: 6173 7394 6568 255d 9468 275d 9468 295d  ass.eh%].h'].h)]
+0000a2a0: 9475 682b 68f3 681b 6a26 0b00 0075 6261  .uh+h.h.j&...uba
+0000a2b0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+0000a2c0: 9468 275d 9468 295d 948c 0672 6566 646f  .h'].h)]...refdo
+0000a2d0: 6394 6acf 0200 008c 0972 6566 646f 6d61  c.j......refdoma
+0000a2e0: 696e 946a 340b 0000 8c07 7265 6674 7970  in.j4.....reftyp
+0000a2f0: 6594 8c05 636c 6173 7394 8c0b 7265 6665  e...class...refe
+0000a300: 7870 6c69 6369 7494 898c 0772 6566 7761  xplicit....refwa
+0000a310: 726e 9489 6ad5 0200 004e 6ad6 0200 004e  rn..j....Nj....N
+0000a320: 6ad7 0200 008c 1a70 796e 6772 6f6b 2e63  j......pyngrok.c
+0000a330: 6f6e 662e 5079 6e67 726f 6b43 6f6e 6669  onf.PyngrokConfi
+0000a340: 6794 7568 2b6a b202 0000 681d 682c 681e  g.uh+j....h.h,h.
+0000a350: 4bf3 681b 6afa 0a00 0075 6268 168c 3a2c  K.h.j....ubh..:,
+0000a360: 2069 740a 7769 6c6c 2062 6520 696e 7374   it.will be inst
+0000a370: 616c 6c65 6420 7468 6520 6669 7273 7420  alled the first 
+0000a380: 7469 6d65 206d 6f73 7420 6d65 7468 6f64  time most method
+0000a390: 7320 696e 2074 6865 2094 8594 8194 7d94  s in the .....}.
+0000a3a0: 2868 1b6a fa0a 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+0000a3b0: 1e4e 7562 6ab3 0200 0029 8194 7d94 2868  .Nubj....)..}.(h
+0000a3c0: 058c 153a 6d6f 643a 607e 7079 6e67 726f  ...:mod:`~pyngro
+0000a3d0: 6b2e 6e67 726f 6b60 9468 075d 9468 f429  k.ngrok`.h.].h.)
+0000a3e0: 8194 7d94 2868 056a 4c0b 0000 6807 5d94  ..}.(h.jL...h.].
+0000a3f0: 6816 8c05 6e67 726f 6b94 8594 8194 7d94  h...ngrok.....}.
+0000a400: 2868 1b6a 4e0b 0000 681c 6803 681d 4e68  (h.jN...h.h.h.Nh
+0000a410: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000a420: 5d94 286a c202 0000 8c02 7079 948c 0670  ].(j......py...p
+0000a430: 792d 6d6f 6494 6568 255d 9468 275d 9468  y-mod.eh%].h'].h
+0000a440: 295d 9475 682b 68f3 681b 6a4a 0b00 0075  )].uh+h.h.jJ...u
+0000a450: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+0000a460: 255d 9468 275d 9468 295d 948c 0672 6566  %].h'].h)]...ref
+0000a470: 646f 6394 6acf 0200 008c 0972 6566 646f  doc.j......refdo
+0000a480: 6d61 696e 946a 580b 0000 8c07 7265 6674  main.jX.....reft
+0000a490: 7970 6594 8c03 6d6f 6494 8c0b 7265 6665  ype...mod...refe
+0000a4a0: 7870 6c69 6369 7494 898c 0772 6566 7761  xplicit....refwa
+0000a4b0: 726e 9489 6ad5 0200 004e 6ad6 0200 004e  rn..j....Nj....N
+0000a4c0: 6ad7 0200 008c 0d70 796e 6772 6f6b 2e6e  j......pyngrok.n
+0000a4d0: 6772 6f6b 9475 682b 6ab2 0200 0068 1d68  grok.uh+j....h.h
+0000a4e0: 2c68 1e4b f368 1b6a fa0a 0000 7562 6816  ,h.K.h.j....ubh.
+0000a4f0: 8c13 206d 6f64 756c 6520 6172 6520 6361  .. module are ca
+0000a500: 6c6c 6564 2e94 8594 8194 7d94 2868 1b6a  lled......}.(h.j
+0000a510: fa0a 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+0000a520: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+0000a530: 5d94 6827 5d94 6829 5d94 7568 2b68 ed68  ].h'].h)].uh+h.h
+0000a540: 1d68 2c68 1e4b f368 1b6a f60a 0000 7562  .h,h.K.h.j....ub
+0000a550: 68ee 2981 947d 9428 6805 58e0 0100 0049  h.)..}.(h.X....I
+0000a560: 6620 7765 206e 6565 6420 746f 2063 7573  f we need to cus
+0000a570: 746f 6d69 7a65 2074 6865 2069 6e73 7461  tomize the insta
+0000a580: 6c6c 6174 696f 6e20 6f66 2060 606e 6772  llation of ``ngr
+0000a590: 6f6b 6060 2c20 7065 7268 6170 7320 7370  ok``, perhaps sp
+0000a5a0: 6563 6966 7969 6e67 2061 2074 696d 656f  ecifying a timeo
+0000a5b0: 7574 2c20 7072 6f78 792c 2075 7365 2061  ut, proxy, use a
+0000a5c0: 2063 7573 746f 6d20 6d69 7272 6f72 0a66   custom mirror.f
+0000a5d0: 6f72 2074 6865 2064 6f77 6e6c 6f61 642c  or the download,
+0000a5e0: 2065 7463 2e20 7765 2063 616e 2064 6f20   etc. we can do 
+0000a5f0: 736f 2062 7920 6c65 7665 7261 6769 6e67  so by leveraging
+0000a600: 2074 6865 203a 6d6f 643a 607e 7079 6e67   the :mod:`~pyng
+0000a610: 726f 6b2e 696e 7374 616c 6c65 7260 206d  rok.installer` m
+0000a620: 6f64 756c 652e 204b 6579 776f 7264 2061  odule. Keyword a
+0000a630: 7267 756d 656e 7473 2069 6e20 7468 6973  rguments in this
+0000a640: 0a6d 6f64 756c 6520 6172 6520 756c 7469  .module are ulti
+0000a650: 6d61 7465 6c79 2070 6173 7365 6420 646f  mately passed do
+0000a660: 776e 2074 6f20 3a70 793a 6675 6e63 3a60  wn to :py:func:`
+0000a670: 7572 6c6c 6962 2e72 6571 7565 7374 2e75  urllib.request.u
+0000a680: 726c 6f70 656e 602c 2073 6f20 6173 206c  rlopen`, so as l
+0000a690: 6f6e 6720 6173 2077 6520 7573 6520 7468  ong as we use th
+0000a6a0: 650a 3a6d 6f64 3a60 7e70 796e 6772 6f6b  e.:mod:`~pyngrok
+0000a6b0: 2e69 6e73 7461 6c6c 6572 6020 6d6f 6475  .installer` modu
+0000a6c0: 6c65 206f 7572 7365 6c76 6573 2070 7269  le ourselves pri
+0000a6d0: 6f72 2074 6f20 696e 766f 6b69 6e67 2061  or to invoking a
+0000a6e0: 6e79 203a 6d6f 643a 607e 7079 6e67 726f  ny :mod:`~pyngro
+0000a6f0: 6b2e 6e67 726f 6b60 206d 6574 686f 6473  k.ngrok` methods
+0000a700: 2c20 7765 2063 616e 2063 616e 2063 6f6e  , we can can con
+0000a710: 7472 6f6c 0a68 6f77 2060 606e 6772 6f6b  trol.how ``ngrok
+0000a720: 6060 2069 7320 696e 7374 616c 6c65 6420  `` is installed 
+0000a730: 616e 6420 6672 6f6d 2077 6865 7265 2e94  and from where..
+0000a740: 6807 5d94 2868 168c 2c49 6620 7765 206e  h.].(h..,If we n
+0000a750: 6565 6420 746f 2063 7573 746f 6d69 7a65  eed to customize
+0000a760: 2074 6865 2069 6e73 7461 6c6c 6174 696f   the installatio
+0000a770: 6e20 6f66 2094 8594 8194 7d94 2868 1b6a  n of .....}.(h.j
+0000a780: 740b 0000 681c 6803 681d 4e68 1e4e 7562  t...h.h.h.Nh.Nub
+0000a790: 68f4 2981 947d 9428 6805 8c09 6060 6e67  h.)..}.(h...``ng
+0000a7a0: 726f 6b60 6094 6807 5d94 6816 8c05 6e67  rok``.h.].h...ng
+0000a7b0: 726f 6b94 8594 8194 7d94 2868 1b6a 7c0b  rok.....}.(h.j|.
+0000a7c0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+0000a7d0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000a7e0: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
+0000a7f0: 740b 0000 7562 6816 8c71 2c20 7065 7268  t...ubh..q, perh
+0000a800: 6170 7320 7370 6563 6966 7969 6e67 2061  aps specifying a
+0000a810: 2074 696d 656f 7574 2c20 7072 6f78 792c   timeout, proxy,
+0000a820: 2075 7365 2061 2063 7573 746f 6d20 6d69   use a custom mi
+0000a830: 7272 6f72 0a66 6f72 2074 6865 2064 6f77  rror.for the dow
+0000a840: 6e6c 6f61 642c 2065 7463 2e20 7765 2063  nload, etc. we c
+0000a850: 616e 2064 6f20 736f 2062 7920 6c65 7665  an do so by leve
+0000a860: 7261 6769 6e67 2074 6865 2094 8594 8194  raging the .....
+0000a870: 7d94 2868 1b6a 740b 0000 681c 6803 681d  }.(h.jt...h.h.h.
+0000a880: 4e68 1e4e 7562 6ab3 0200 0029 8194 7d94  Nh.Nubj....)..}.
+0000a890: 2868 058c 193a 6d6f 643a 607e 7079 6e67  (h...:mod:`~pyng
+0000a8a0: 726f 6b2e 696e 7374 616c 6c65 7260 9468  rok.installer`.h
+0000a8b0: 075d 9468 f429 8194 7d94 2868 056a 900b  .].h.)..}.(h.j..
+0000a8c0: 0000 6807 5d94 6816 8c09 696e 7374 616c  ..h.].h...instal
+0000a8d0: 6c65 7294 8594 8194 7d94 2868 1b6a 920b  ler.....}.(h.j..
+0000a8e0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+0000a8f0: 1f7d 9428 6821 5d94 6823 5d94 286a c202  .}.(h!].h#].(j..
+0000a900: 0000 8c02 7079 948c 0670 792d 6d6f 6494  ....py...py-mod.
+0000a910: 6568 255d 9468 275d 9468 295d 9475 682b  eh%].h'].h)].uh+
+0000a920: 68f3 681b 6a8e 0b00 0075 6261 681f 7d94  h.h.j....ubah.}.
+0000a930: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+0000a940: 9468 295d 948c 0672 6566 646f 6394 6acf  .h)]...refdoc.j.
+0000a950: 0200 008c 0972 6566 646f 6d61 696e 946a  .....refdomain.j
+0000a960: 9c0b 0000 8c07 7265 6674 7970 6594 8c03  ......reftype...
+0000a970: 6d6f 6494 8c0b 7265 6665 7870 6c69 6369  mod...refexplici
+0000a980: 7494 898c 0772 6566 7761 726e 9489 6ad5  t....refwarn..j.
+0000a990: 0200 004e 6ad6 0200 004e 6ad7 0200 008c  ...Nj....Nj.....
+0000a9a0: 1170 796e 6772 6f6b 2e69 6e73 7461 6c6c  .pyngrok.install
+0000a9b0: 6572 9475 682b 6ab2 0200 0068 1d68 2c68  er.uh+j....h.h,h
+0000a9c0: 1e4b f668 1b6a 740b 0000 7562 6816 8c48  .K.h.jt...ubh..H
+0000a9d0: 206d 6f64 756c 652e 204b 6579 776f 7264   module. Keyword
+0000a9e0: 2061 7267 756d 656e 7473 2069 6e20 7468   arguments in th
+0000a9f0: 6973 0a6d 6f64 756c 6520 6172 6520 756c  is.module are ul
+0000aa00: 7469 6d61 7465 6c79 2070 6173 7365 6420  timately passed 
+0000aa10: 646f 776e 2074 6f20 9485 9481 947d 9428  down to .....}.(
+0000aa20: 681b 6a74 0b00 0068 1c68 0368 1d4e 681e  h.jt...h.h.h.Nh.
+0000aa30: 4e75 626a b302 0000 2981 947d 9428 6805  Nubj....)..}.(h.
+0000aa40: 8c21 3a70 793a 6675 6e63 3a60 7572 6c6c  .!:py:func:`urll
+0000aa50: 6962 2e72 6571 7565 7374 2e75 726c 6f70  ib.request.urlop
+0000aa60: 656e 6094 6807 5d94 68f4 2981 947d 9428  en`.h.].h.)..}.(
+0000aa70: 6805 6ab4 0b00 0068 075d 9468 168c 1675  h.j....h.].h...u
+0000aa80: 726c 6c69 622e 7265 7175 6573 742e 7572  rllib.request.ur
+0000aa90: 6c6f 7065 6e94 8594 8194 7d94 2868 1b6a  lopen.....}.(h.j
+0000aaa0: b60b 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+0000aab0: 6168 1f7d 9428 6821 5d94 6823 5d94 286a  ah.}.(h!].h#].(j
+0000aac0: c202 0000 8c02 7079 948c 0770 792d 6675  ......py...py-fu
+0000aad0: 6e63 9465 6825 5d94 6827 5d94 6829 5d94  nc.eh%].h'].h)].
+0000aae0: 7568 2b68 f368 1b6a b20b 0000 7562 6168  uh+h.h.j....ubah
+0000aaf0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000ab00: 6827 5d94 6829 5d94 8c06 7265 6664 6f63  h'].h)]...refdoc
+0000ab10: 946a cf02 0000 8c09 7265 6664 6f6d 6169  .j......refdomai
+0000ab20: 6e94 6ac0 0b00 008c 0772 6566 7479 7065  n.j......reftype
+0000ab30: 948c 0466 756e 6394 8c0b 7265 6665 7870  ...func...refexp
+0000ab40: 6c69 6369 7494 898c 0772 6566 7761 726e  licit....refwarn
+0000ab50: 9489 6ad5 0200 004e 6ad6 0200 004e 6ad7  ..j....Nj....Nj.
+0000ab60: 0200 008c 1675 726c 6c69 622e 7265 7175  .....urllib.requ
+0000ab70: 6573 742e 7572 6c6f 7065 6e94 7568 2b6a  est.urlopen.uh+j
+0000ab80: b202 0000 681d 682c 681e 4bf6 681b 6a74  ....h.h,h.K.h.jt
+0000ab90: 0b00 0075 6268 168c 1b2c 2073 6f20 6173  ...ubh..., so as
+0000aba0: 206c 6f6e 6720 6173 2077 6520 7573 6520   long as we use 
+0000abb0: 7468 650a 9485 9481 947d 9428 681b 6a74  the......}.(h.jt
+0000abc0: 0b00 0068 1c68 0368 1d4e 681e 4e75 626a  ...h.h.h.Nh.Nubj
+0000abd0: b302 0000 2981 947d 9428 6805 8c19 3a6d  ....)..}.(h...:m
+0000abe0: 6f64 3a60 7e70 796e 6772 6f6b 2e69 6e73  od:`~pyngrok.ins
+0000abf0: 7461 6c6c 6572 6094 6807 5d94 68f4 2981  taller`.h.].h.).
+0000ac00: 947d 9428 6805 6ad8 0b00 0068 075d 9468  .}.(h.j....h.].h
+0000ac10: 168c 0969 6e73 7461 6c6c 6572 9485 9481  ...installer....
+0000ac20: 947d 9428 681b 6ada 0b00 0068 1c68 0368  .}.(h.j....h.h.h
+0000ac30: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+0000ac40: 9468 235d 9428 6ac2 0200 008c 0270 7994  .h#].(j......py.
+0000ac50: 8c06 7079 2d6d 6f64 9465 6825 5d94 6827  ..py-mod.eh%].h'
+0000ac60: 5d94 6829 5d94 7568 2b68 f368 1b6a d60b  ].h)].uh+h.h.j..
+0000ac70: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+0000ac80: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
+0000ac90: 7265 6664 6f63 946a cf02 0000 8c09 7265  refdoc.j......re
+0000aca0: 6664 6f6d 6169 6e94 6ae4 0b00 008c 0772  fdomain.j......r
+0000acb0: 6566 7479 7065 948c 036d 6f64 948c 0b72  eftype...mod...r
+0000acc0: 6566 6578 706c 6963 6974 9489 8c07 7265  efexplicit....re
+0000acd0: 6677 6172 6e94 896a d502 0000 4e6a d602  fwarn..j....Nj..
+0000ace0: 0000 4e6a d702 0000 8c11 7079 6e67 726f  ..Nj......pyngro
+0000acf0: 6b2e 696e 7374 616c 6c65 7294 7568 2b6a  k.installer.uh+j
+0000ad00: b202 0000 681d 682c 681e 4bf6 681b 6a74  ....h.h,h.K.h.jt
+0000ad10: 0b00 0075 6268 168c 2820 6d6f 6475 6c65  ...ubh..( module
+0000ad20: 206f 7572 7365 6c76 6573 2070 7269 6f72   ourselves prior
+0000ad30: 2074 6f20 696e 766f 6b69 6e67 2061 6e79   to invoking any
+0000ad40: 2094 8594 8194 7d94 2868 1b6a 740b 0000   .....}.(h.jt...
+0000ad50: 681c 6803 681d 4e68 1e4e 7562 6ab3 0200  h.h.h.Nh.Nubj...
+0000ad60: 0029 8194 7d94 2868 058c 153a 6d6f 643a  .)..}.(h...:mod:
+0000ad70: 607e 7079 6e67 726f 6b2e 6e67 726f 6b60  `~pyngrok.ngrok`
+0000ad80: 9468 075d 9468 f429 8194 7d94 2868 056a  .h.].h.)..}.(h.j
+0000ad90: fc0b 0000 6807 5d94 6816 8c05 6e67 726f  ....h.].h...ngro
+0000ada0: 6b94 8594 8194 7d94 2868 1b6a fe0b 0000  k.....}.(h.j....
+0000adb0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+0000adc0: 9428 6821 5d94 6823 5d94 286a c202 0000  .(h!].h#].(j....
+0000add0: 8c02 7079 948c 0670 792d 6d6f 6494 6568  ..py...py-mod.eh
+0000ade0: 255d 9468 275d 9468 295d 9475 682b 68f3  %].h'].h)].uh+h.
+0000adf0: 681b 6afa 0b00 0075 6261 681f 7d94 2868  h.j....ubah.}.(h
+0000ae00: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+0000ae10: 295d 948c 0672 6566 646f 6394 6acf 0200  )]...refdoc.j...
+0000ae20: 008c 0972 6566 646f 6d61 696e 946a 080c  ...refdomain.j..
+0000ae30: 0000 8c07 7265 6674 7970 6594 8c03 6d6f  ....reftype...mo
+0000ae40: 6494 8c0b 7265 6665 7870 6c69 6369 7494  d...refexplicit.
+0000ae50: 898c 0772 6566 7761 726e 9489 6ad5 0200  ...refwarn..j...
+0000ae60: 004e 6ad6 0200 004e 6ad7 0200 008c 0d70  .Nj....Nj......p
+0000ae70: 796e 6772 6f6b 2e6e 6772 6f6b 9475 682b  yngrok.ngrok.uh+
+0000ae80: 6ab2 0200 0068 1d68 2c68 1e4b f668 1b6a  j....h.h,h.K.h.j
+0000ae90: 740b 0000 7562 6816 8c21 206d 6574 686f  t...ubh..! metho
+0000aea0: 6473 2c20 7765 2063 616e 2063 616e 2063  ds, we can can c
+0000aeb0: 6f6e 7472 6f6c 0a68 6f77 2094 8594 8194  ontrol.how .....
+0000aec0: 7d94 2868 1b6a 740b 0000 681c 6803 681d  }.(h.jt...h.h.h.
+0000aed0: 4e68 1e4e 7562 68f4 2981 947d 9428 6805  Nh.Nubh.)..}.(h.
+0000aee0: 8c09 6060 6e67 726f 6b60 6094 6807 5d94  ..``ngrok``.h.].
+0000aef0: 6816 8c05 6e67 726f 6b94 8594 8194 7d94  h...ngrok.....}.
+0000af00: 2868 1b6a 1e0c 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+0000af10: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000af20: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+0000af30: 2b68 f368 1b6a 740b 0000 7562 6816 8c1d  +h.h.jt...ubh...
+0000af40: 2069 7320 696e 7374 616c 6c65 6420 616e   is installed an
+0000af50: 6420 6672 6f6d 2077 6865 7265 2e94 8594  d from where....
+0000af60: 8194 7d94 2868 1b6a 740b 0000 681c 6803  ..}.(h.jt...h.h.
+0000af70: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+0000af80: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+0000af90: 5d94 7568 2b68 ed68 1d68 2c68 1e4b f668  ].uh+h.h.h,h.K.h
+0000afa0: 1b6a f60a 0000 7562 6568 1f7d 9428 6821  .j....ubeh.}.(h!
+0000afb0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+0000afc0: 5d94 7568 2b6a b603 0000 681b 6a86 0900  ].uh+j....h.j...
+0000afd0: 0068 1c68 0368 1d68 2c68 1e4e 7562 6568  .h.h.h.h,h.Nubeh
+0000afe0: 1f7d 9428 6821 5d94 8c0d 7079 6e67 726f  .}.(h!]...pyngro
+0000aff0: 6b63 6f6e 6669 6794 6168 235d 9468 255d  kconfig.ah#].h%]
+0000b000: 948c 0d70 796e 6772 6f6b 636f 6e66 6967  ...pyngrokconfig
+0000b010: 9461 6827 5d94 6829 5d94 7568 2b68 0a68  .ah'].h)].uh+h.h
+0000b020: 1b6a 7509 0000 681c 6803 681d 682c 681e  .ju...h.h.h.h,h.
+0000b030: 4bdb 7562 680b 2981 947d 9428 6805 6806  K.ubh.)..}.(h.h.
+0000b040: 6807 5d94 2868 1029 8194 7d94 2868 058c  h.].(h.)..}.(h..
+0000b050: 1f60 606e 6772 6f6b 6060 2056 6572 7369  .``ngrok`` Versi
+0000b060: 6f6e 2043 6f6d 7061 7469 6269 6c69 7479  on Compatibility
+0000b070: 9468 075d 9428 68f4 2981 947d 9428 6805  .h.].(h.)..}.(h.
+0000b080: 8c09 6060 6e67 726f 6b60 6094 6807 5d94  ..``ngrok``.h.].
+0000b090: 6816 8c05 6e67 726f 6b94 8594 8194 7d94  h...ngrok.....}.
+0000b0a0: 2868 1b6a 4b0c 0000 681c 6803 681d 4e68  (h.jK...h.h.h.Nh
+0000b0b0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000b0c0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+0000b0d0: 2b68 f368 1b6a 470c 0000 7562 6816 8c16  +h.h.jG...ubh...
+0000b0e0: 2056 6572 7369 6f6e 2043 6f6d 7061 7469   Version Compati
+0000b0f0: 6269 6c69 7479 9485 9481 947d 9428 681b  bility.....}.(h.
+0000b100: 6a47 0c00 0068 1c68 0368 1d4e 681e 4e75  jG...h.h.h.Nh.Nu
+0000b110: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+0000b120: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
+0000b130: 681b 6a44 0c00 0068 1c68 0368 1d68 2c68  h.jD...h.h.h.h,h
+0000b140: 1e4b fd75 6268 ee29 8194 7d94 2868 058c  .K.ubh.)..}.(h..
+0000b150: ac60 6070 796e 6772 6f6b 6060 2069 7320  .``pyngrok`` is 
+0000b160: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
+0000b170: 6060 6e67 726f 6b60 6020 7632 2061 6e64  ``ngrok`` v2 and
+0000b180: 2076 332c 2062 7574 2062 7920 6465 6661   v3, but by defa
+0000b190: 756c 7420 6974 2077 696c 6c20 696e 7374  ult it will inst
+0000b1a0: 616c 6c20 7632 2e20 546f 2069 6e73 7461  all v2. To insta
+0000b1b0: 6c6c 2076 3320 696e 7374 6561 642c 0a73  ll v3 instead,.s
+0000b1c0: 6574 2060 606e 6772 6f6b 5f76 6572 7369  et ``ngrok_versi
+0000b1d0: 6f6e 6060 2069 6e20 3a63 6c61 7373 3a60  on`` in :class:`
+0000b1e0: 7e70 796e 6772 6f6b 2e63 6f6e 662e 5079  ~pyngrok.conf.Py
+0000b1f0: 6e67 726f 6b43 6f6e 6669 6760 3a94 6807  ngrokConfig`:.h.
+0000b200: 5d94 2868 f429 8194 7d94 2868 058c 0b60  ].(h.)..}.(h...`
+0000b210: 6070 796e 6772 6f6b 6060 9468 075d 9468  `pyngrok``.h.].h
+0000b220: 168c 0770 796e 6772 6f6b 9485 9481 947d  ...pyngrok.....}
+0000b230: 9428 681b 6a67 0c00 0068 1c68 0368 1d4e  .(h.jg...h.h.h.N
+0000b240: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+0000b250: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+0000b260: 682b 68f3 681b 6a63 0c00 0075 6268 168c  h+h.h.jc...ubh..
+0000b270: 1420 6973 2063 6f6d 7061 7469 626c 6520  . is compatible 
+0000b280: 7769 7468 2094 8594 8194 7d94 2868 1b6a  with .....}.(h.j
+0000b290: 630c 0000 681c 6803 681d 4e68 1e4e 7562  c...h.h.h.Nh.Nub
+0000b2a0: 68f4 2981 947d 9428 6805 8c09 6060 6e67  h.)..}.(h...``ng
+0000b2b0: 726f 6b60 6094 6807 5d94 6816 8c05 6e67  rok``.h.].h...ng
+0000b2c0: 726f 6b94 8594 8194 7d94 2868 1b6a 790c  rok.....}.(h.jy.
+0000b2d0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+0000b2e0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000b2f0: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
+0000b300: 630c 0000 7562 6816 8c4a 2076 3220 616e  c...ubh..J v2 an
+0000b310: 6420 7633 2c20 6275 7420 6279 2064 6566  d v3, but by def
+0000b320: 6175 6c74 2069 7420 7769 6c6c 2069 6e73  ault it will ins
+0000b330: 7461 6c6c 2076 322e 2054 6f20 696e 7374  tall v2. To inst
+0000b340: 616c 6c20 7633 2069 6e73 7465 6164 2c0a  all v3 instead,.
+0000b350: 7365 7420 9485 9481 947d 9428 681b 6a63  set .....}.(h.jc
+0000b360: 0c00 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
+0000b370: f429 8194 7d94 2868 058c 1160 606e 6772  .)..}.(h...``ngr
+0000b380: 6f6b 5f76 6572 7369 6f6e 6060 9468 075d  ok_version``.h.]
+0000b390: 9468 168c 0d6e 6772 6f6b 5f76 6572 7369  .h...ngrok_versi
+0000b3a0: 6f6e 9485 9481 947d 9428 681b 6a8b 0c00  on.....}.(h.j...
+0000b3b0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+0000b3c0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+0000b3d0: 275d 9468 295d 9475 682b 68f3 681b 6a63  '].h)].uh+h.h.jc
+0000b3e0: 0c00 0075 6268 168c 0420 696e 2094 8594  ...ubh... in ...
+0000b3f0: 8194 7d94 2868 1b6a 630c 0000 681c 6803  ..}.(h.jc...h.h.
+0000b400: 681d 4e68 1e4e 7562 6ab3 0200 0029 8194  h.Nh.Nubj....)..
+0000b410: 7d94 2868 058c 243a 636c 6173 733a 607e  }.(h..$:class:`~
+0000b420: 7079 6e67 726f 6b2e 636f 6e66 2e50 796e  pyngrok.conf.Pyn
+0000b430: 6772 6f6b 436f 6e66 6967 6094 6807 5d94  grokConfig`.h.].
+0000b440: 68f4 2981 947d 9428 6805 6a9f 0c00 0068  h.)..}.(h.j....h
+0000b450: 075d 9468 168c 0d50 796e 6772 6f6b 436f  .].h...PyngrokCo
+0000b460: 6e66 6967 9485 9481 947d 9428 681b 6aa1  nfig.....}.(h.j.
+0000b470: 0c00 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+0000b480: 681f 7d94 2868 215d 9468 235d 9428 6ac2  h.}.(h!].h#].(j.
+0000b490: 0200 008c 0270 7994 8c08 7079 2d63 6c61  .....py...py-cla
+0000b4a0: 7373 9465 6825 5d94 6827 5d94 6829 5d94  ss.eh%].h'].h)].
+0000b4b0: 7568 2b68 f368 1b6a 9d0c 0000 7562 6168  uh+h.h.j....ubah
+0000b4c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000b4d0: 6827 5d94 6829 5d94 8c06 7265 6664 6f63  h'].h)]...refdoc
+0000b4e0: 946a cf02 0000 8c09 7265 6664 6f6d 6169  .j......refdomai
+0000b4f0: 6e94 6aab 0c00 008c 0772 6566 7479 7065  n.j......reftype
+0000b500: 948c 0563 6c61 7373 948c 0b72 6566 6578  ...class...refex
+0000b510: 706c 6963 6974 9489 8c07 7265 6677 6172  plicit....refwar
+0000b520: 6e94 896a d502 0000 4e6a d602 0000 4e6a  n..j....Nj....Nj
+0000b530: d702 0000 8c1a 7079 6e67 726f 6b2e 636f  ......pyngrok.co
+0000b540: 6e66 2e50 796e 6772 6f6b 436f 6e66 6967  nf.PyngrokConfig
+0000b550: 9475 682b 6ab2 0200 0068 1d68 2c68 1e4b  .uh+j....h.h,h.K
+0000b560: ff68 1b6a 630c 0000 7562 6816 8c01 3a94  .h.jc...ubh...:.
+0000b570: 8594 8194 7d94 2868 1b6a 630c 0000 681c  ....}.(h.jc...h.
+0000b580: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
+0000b590: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+0000b5a0: 6829 5d94 7568 2b68 ed68 1d68 2c68 1e4b  h)].uh+h.h.h,h.K
+0000b5b0: ff68 1b6a 440c 0000 681c 6803 7562 6ad5  .h.jD...h.h.ubj.
+0000b5c0: 0100 0029 8194 7d94 2868 058c 4866 726f  ...)..}.(h..Hfro
+0000b5d0: 6d20 7079 6e67 726f 6b20 696d 706f 7274  m pyngrok import
+0000b5e0: 2063 6f6e 662c 206e 6772 6f6b 0a0a 636f   conf, ngrok..co
+0000b5f0: 6e66 2e67 6574 5f64 6566 6175 6c74 2829  nf.get_default()
+0000b600: 2e6e 6772 6f6b 5f76 6572 7369 6f6e 203d  .ngrok_version =
+0000b610: 2022 7633 2294 6807 5d94 6816 8c48 6672   "v3".h.].h..Hfr
+0000b620: 6f6d 2070 796e 6772 6f6b 2069 6d70 6f72  om pyngrok impor
+0000b630: 7420 636f 6e66 2c20 6e67 726f 6b0a 0a63  t conf, ngrok..c
+0000b640: 6f6e 662e 6765 745f 6465 6661 756c 7428  onf.get_default(
+0000b650: 292e 6e67 726f 6b5f 7665 7273 696f 6e20  ).ngrok_version 
+0000b660: 3d20 2276 3322 9485 9481 947d 9468 1b6a  = "v3".....}.h.j
+0000b670: c70c 0000 7362 6168 1f7d 9428 6821 5d94  ....sbah.}.(h!].
+0000b680: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+0000b690: 6ae4 0100 006a e501 0000 6ae6 0100 0089  j....j....j.....
+0000b6a0: 6ae7 0100 008c 0670 7974 686f 6e94 6ae9  j......python.j.
+0000b6b0: 0100 007d 9475 682b 6ad4 0100 0068 1d68  ...}.uh+j....h.h
+0000b6c0: 2c68 1e4d 0201 681b 6a44 0c00 0068 1c68  ,h.M..h.jD...h.h
+0000b6d0: 0375 6265 681f 7d94 2868 215d 948c 1b6e  .ubeh.}.(h!]...n
+0000b6e0: 6772 6f6b 2d76 6572 7369 6f6e 2d63 6f6d  grok-version-com
+0000b6f0: 7061 7469 6269 6c69 7479 9461 6823 5d94  patibility.ah#].
+0000b700: 6825 5d94 8c1b 6e67 726f 6b20 7665 7273  h%]...ngrok vers
+0000b710: 696f 6e20 636f 6d70 6174 6962 696c 6974  ion compatibilit
+0000b720: 7994 6168 275d 9468 295d 9475 682b 680a  y.ah'].h)].uh+h.
+0000b730: 681b 6a75 0900 0068 1c68 0368 1d68 2c68  h.ju...h.h.h.h,h
+0000b740: 1e4b fd75 6268 0b29 8194 7d94 2868 0568  .K.ubh.)..}.(h.h
+0000b750: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+0000b760: 8c19 5365 7474 696e 6720 7468 6520 6060  ..Setting the ``
+0000b770: 6175 7468 746f 6b65 6e60 6094 6807 5d94  authtoken``.h.].
+0000b780: 2868 168c 0c53 6574 7469 6e67 2074 6865  (h...Setting the
+0000b790: 2094 8594 8194 7d94 2868 1b6a e20c 0000   .....}.(h.j....
+0000b7a0: 681c 6803 681d 4e68 1e4e 7562 68f4 2981  h.h.h.Nh.Nubh.).
+0000b7b0: 947d 9428 6805 8c0d 6060 6175 7468 746f  .}.(h...``authto
+0000b7c0: 6b65 6e60 6094 6807 5d94 6816 8c09 6175  ken``.h.].h...au
+0000b7d0: 7468 746f 6b65 6e94 8594 8194 7d94 2868  thtoken.....}.(h
+0000b7e0: 1b6a ea0c 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000b7f0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+0000b800: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+0000b810: f368 1b6a e20c 0000 7562 6568 1f7d 9428  .h.j....ubeh.}.(
+0000b820: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+0000b830: 6829 5d94 7568 2b68 0f68 1b6a df0c 0000  h)].uh+h.h.j....
+0000b840: 681c 6803 681d 682c 681e 4d09 0175 6268  h.h.h.h,h.M..ubh
+0000b850: ee29 8194 7d94 2868 0558 2801 0000 5275  .)..}.(h.X(...Ru
+0000b860: 6e6e 696e 6720 6060 6e67 726f 6b60 6020  nning ``ngrok`` 
+0000b870: 7769 7468 2061 6e20 6175 7468 2074 6f6b  with an auth tok
+0000b880: 656e 2065 6e61 626c 6573 2061 6464 6974  en enables addit
+0000b890: 696f 6e61 6c20 6665 6174 7572 6573 2061  ional features a
+0000b8a0: 7661 696c 6162 6c65 206f 6e20 6f75 7220  vailable on our 
+0000b8b0: 6163 636f 756e 7420 2866 6f72 0a69 6e73  account (for.ins
+0000b8c0: 7461 6e63 652c 2074 6865 2061 6269 6c69  tance, the abili
+0000b8d0: 7479 2074 6f20 6f70 656e 206d 756c 7469  ty to open multi
+0000b8e0: 706c 6520 7475 6e6e 656c 7320 636f 6e63  ple tunnels conc
+0000b8f0: 7572 7265 6e74 6c79 292e 2057 6520 6361  urrently). We ca
+0000b900: 6e20 6f62 7461 696e 206f 7572 2061 7574  n obtain our aut
+0000b910: 6820 746f 6b65 6e20 6672 6f6d 0a74 6865  h token from.the
+0000b920: 2060 6e67 726f 6b20 6461 7368 626f 6172   `ngrok dashboar
+0000b930: 6420 3c68 7474 7073 3a2f 2f64 6173 6862  d <https://dashb
+0000b940: 6f61 7264 2e6e 6772 6f6b 2e63 6f6d 3e60  oard.ngrok.com>`
+0000b950: 5f20 616e 6420 696e 7374 616c 6c20 6974  _ and install it
+0000b960: 2074 6f20 6060 6e67 726f 6b60 6027 7320   to ``ngrok``'s 
+0000b970: 636f 6e66 6967 2066 696c 6520 6c69 6b65  config file like
+0000b980: 2074 6869 733a 9468 075d 9428 6816 8c08   this:.h.].(h...
+0000b990: 5275 6e6e 696e 6720 9485 9481 947d 9428  Running .....}.(
+0000b9a0: 681b 6afe 0c00 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+0000b9b0: 4e75 6268 f429 8194 7d94 2868 058c 0960  Nubh.)..}.(h...`
+0000b9c0: 606e 6772 6f6b 6060 9468 075d 9468 168c  `ngrok``.h.].h..
+0000b9d0: 056e 6772 6f6b 9485 9481 947d 9428 681b  .ngrok.....}.(h.
+0000b9e0: 6a06 0d00 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+0000b9f0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+0000ba00: 255d 9468 275d 9468 295d 9475 682b 68f3  %].h'].h)].uh+h.
+0000ba10: 681b 6afe 0c00 0075 6268 168c b220 7769  h.j....ubh... wi
+0000ba20: 7468 2061 6e20 6175 7468 2074 6f6b 656e  th an auth token
+0000ba30: 2065 6e61 626c 6573 2061 6464 6974 696f   enables additio
+0000ba40: 6e61 6c20 6665 6174 7572 6573 2061 7661  nal features ava
+0000ba50: 696c 6162 6c65 206f 6e20 6f75 7220 6163  ilable on our ac
+0000ba60: 636f 756e 7420 2866 6f72 0a69 6e73 7461  count (for.insta
+0000ba70: 6e63 652c 2074 6865 2061 6269 6c69 7479  nce, the ability
+0000ba80: 2074 6f20 6f70 656e 206d 756c 7469 706c   to open multipl
+0000ba90: 6520 7475 6e6e 656c 7320 636f 6e63 7572  e tunnels concur
+0000baa0: 7265 6e74 6c79 292e 2057 6520 6361 6e20  rently). We can 
+0000bab0: 6f62 7461 696e 206f 7572 2061 7574 6820  obtain our auth 
+0000bac0: 746f 6b65 6e20 6672 6f6d 0a74 6865 2094  token from.the .
+0000bad0: 8594 8194 7d94 2868 1b6a fe0c 0000 681c  ....}.(h.j....h.
+0000bae0: 6803 681d 4e68 1e4e 7562 6843 2981 947d  h.h.Nh.NubhC)..}
+0000baf0: 9428 6805 8c30 606e 6772 6f6b 2064 6173  .(h..0`ngrok das
+0000bb00: 6862 6f61 7264 203c 6874 7470 733a 2f2f  hboard <https://
+0000bb10: 6461 7368 626f 6172 642e 6e67 726f 6b2e  dashboard.ngrok.
+0000bb20: 636f 6d3e 605f 9468 075d 9468 168c 0f6e  com>`_.h.].h...n
+0000bb30: 6772 6f6b 2064 6173 6862 6f61 7264 9485  grok dashboard..
+0000bb40: 9481 947d 9428 681b 6a18 0d00 0068 1c68  ...}.(h.j....h.h
+0000bb50: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+0000bb60: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+0000bb70: 295d 948c 046e 616d 6594 8c0f 6e67 726f  )]...name...ngro
+0000bb80: 6b20 6461 7368 626f 6172 6494 6a45 0100  k dashboard.jE..
+0000bb90: 008c 1b68 7474 7073 3a2f 2f64 6173 6862  ...https://dashb
+0000bba0: 6f61 7264 2e6e 6772 6f6b 2e63 6f6d 9475  oard.ngrok.com.u
+0000bbb0: 682b 6842 681b 6afe 0c00 0075 626a 4801  h+hBh.j....ubjH.
+0000bbc0: 0000 2981 947d 9428 6805 8c1e 203c 6874  ..)..}.(h... <ht
+0000bbd0: 7470 733a 2f2f 6461 7368 626f 6172 642e  tps://dashboard.
+0000bbe0: 6e67 726f 6b2e 636f 6d3e 9468 075d 9468  ngrok.com>.h.].h
+0000bbf0: 1f7d 9428 6821 5d94 8c0f 6e67 726f 6b2d  .}.(h!]...ngrok-
+0000bc00: 6461 7368 626f 6172 6494 6168 235d 9468  dashboard.ah#].h
+0000bc10: 255d 948c 0f6e 6772 6f6b 2064 6173 6862  %]...ngrok dashb
+0000bc20: 6f61 7264 9461 6827 5d94 6829 5d94 8c06  oard.ah'].h)]...
+0000bc30: 7265 6675 7269 946a 280d 0000 7568 2b6a  refuri.j(...uh+j
+0000bc40: 4701 0000 6a56 0100 004b 0168 1b6a fe0c  G...jV...K.h.j..
+0000bc50: 0000 7562 6816 8c13 2061 6e64 2069 6e73  ..ubh... and ins
+0000bc60: 7461 6c6c 2069 7420 746f 2094 8594 8194  tall it to .....
+0000bc70: 7d94 2868 1b6a fe0c 0000 681c 6803 681d  }.(h.j....h.h.h.
+0000bc80: 4e68 1e4e 7562 68f4 2981 947d 9428 6805  Nh.Nubh.)..}.(h.
+0000bc90: 8c09 6060 6e67 726f 6b60 6094 6807 5d94  ..``ngrok``.h.].
+0000bca0: 6816 8c05 6e67 726f 6b94 8594 8194 7d94  h...ngrok.....}.
+0000bcb0: 2868 1b6a 3a0d 0000 681c 6803 681d 4e68  (h.j:...h.h.h.Nh
+0000bcc0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000bcd0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+0000bce0: 2b68 f368 1b6a fe0c 0000 7562 6816 8c1b  +h.h.j....ubh...
+0000bcf0: e280 9973 2063 6f6e 6669 6720 6669 6c65  ...s config file
+0000bd00: 206c 696b 6520 7468 6973 3a94 8594 8194   like this:.....
+0000bd10: 7d94 2868 1b6a fe0c 0000 681c 6803 681d  }.(h.j....h.h.h.
+0000bd20: 4e68 1e4e 7562 6568 1f7d 9428 6821 5d94  Nh.Nubeh.}.(h!].
+0000bd30: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+0000bd40: 7568 2b68 ed68 1d68 2c68 1e4d 0b01 681b  uh+h.h.h,h.M..h.
+0000bd50: 6adf 0c00 0068 1c68 0375 626a d501 0000  j....h.h.ubj....
+0000bd60: 2981 947d 9428 6805 586e 0100 0066 726f  )..}.(h.Xn...fro
+0000bd70: 6d20 7079 6e67 726f 6b20 696d 706f 7274  m pyngrok import
+0000bd80: 206e 6772 6f6b 0a0a 2320 5365 7474 696e   ngrok..# Settin
+0000bd90: 6720 616e 2061 7574 6820 746f 6b65 6e20  g an auth token 
+0000bda0: 616c 6c6f 7773 2075 7320 746f 206f 7065  allows us to ope
+0000bdb0: 6e20 6d75 6c74 6970 6c65 0a23 2074 756e  n multiple.# tun
+0000bdc0: 6e65 6c73 2061 7420 7468 6520 7361 6d65  nels at the same
+0000bdd0: 2074 696d 650a 6e67 726f 6b2e 7365 745f   time.ngrok.set_
+0000bde0: 6175 7468 5f74 6f6b 656e 2822 3c4e 4752  auth_token("<NGR
+0000bdf0: 4f4b 5f41 5554 485f 544f 4b45 4e3e 2229  OK_AUTH_TOKEN>")
+0000be00: 0a0a 2320 3c4e 6772 6f6b 5475 6e6e 656c  ..# <NgrokTunnel
+0000be10: 3a20 2268 7474 703a 2f2f 3c70 7562 6c69  : "http://<publi
+0000be20: 635f 7375 6231 3e2e 6e67 726f 6b2e 696f  c_sub1>.ngrok.io
+0000be30: 2220 2d3e 2022 6874 7470 3a2f 2f6c 6f63  " -> "http://loc
+0000be40: 616c 686f 7374 3a38 3022 3e0a 6e67 726f  alhost:80">.ngro
+0000be50: 6b5f 7475 6e6e 656c 3120 3d20 6e67 726f  k_tunnel1 = ngro
+0000be60: 6b2e 636f 6e6e 6563 7428 290a 2320 3c4e  k.connect().# <N
+0000be70: 6772 6f6b 5475 6e6e 656c 3a20 2268 7474  grokTunnel: "htt
+0000be80: 703a 2f2f 3c70 7562 6c69 635f 7375 6232  p://<public_sub2
+0000be90: 3e2e 6e67 726f 6b2e 696f 2220 2d3e 2022  >.ngrok.io" -> "
+0000bea0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+0000beb0: 3a38 3030 3022 3e0a 6e67 726f 6b5f 7475  :8000">.ngrok_tu
+0000bec0: 6e6e 656c 3220 3d20 6e67 726f 6b2e 636f  nnel2 = ngrok.co
+0000bed0: 6e6e 6563 7428 3830 3030 2994 6807 5d94  nnect(8000).h.].
+0000bee0: 6816 586e 0100 0066 726f 6d20 7079 6e67  h.Xn...from pyng
+0000bef0: 726f 6b20 696d 706f 7274 206e 6772 6f6b  rok import ngrok
+0000bf00: 0a0a 2320 5365 7474 696e 6720 616e 2061  ..# Setting an a
+0000bf10: 7574 6820 746f 6b65 6e20 616c 6c6f 7773  uth token allows
+0000bf20: 2075 7320 746f 206f 7065 6e20 6d75 6c74   us to open mult
+0000bf30: 6970 6c65 0a23 2074 756e 6e65 6c73 2061  iple.# tunnels a
+0000bf40: 7420 7468 6520 7361 6d65 2074 696d 650a  t the same time.
+0000bf50: 6e67 726f 6b2e 7365 745f 6175 7468 5f74  ngrok.set_auth_t
+0000bf60: 6f6b 656e 2822 3c4e 4752 4f4b 5f41 5554  oken("<NGROK_AUT
+0000bf70: 485f 544f 4b45 4e3e 2229 0a0a 2320 3c4e  H_TOKEN>")..# <N
+0000bf80: 6772 6f6b 5475 6e6e 656c 3a20 2268 7474  grokTunnel: "htt
+0000bf90: 703a 2f2f 3c70 7562 6c69 635f 7375 6231  p://<public_sub1
+0000bfa0: 3e2e 6e67 726f 6b2e 696f 2220 2d3e 2022  >.ngrok.io" -> "
+0000bfb0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+0000bfc0: 3a38 3022 3e0a 6e67 726f 6b5f 7475 6e6e  :80">.ngrok_tunn
+0000bfd0: 656c 3120 3d20 6e67 726f 6b2e 636f 6e6e  el1 = ngrok.conn
+0000bfe0: 6563 7428 290a 2320 3c4e 6772 6f6b 5475  ect().# <NgrokTu
+0000bff0: 6e6e 656c 3a20 2268 7474 703a 2f2f 3c70  nnel: "http://<p
+0000c000: 7562 6c69 635f 7375 6232 3e2e 6e67 726f  ublic_sub2>.ngro
+0000c010: 6b2e 696f 2220 2d3e 2022 6874 7470 3a2f  k.io" -> "http:/
+0000c020: 2f6c 6f63 616c 686f 7374 3a38 3030 3022  /localhost:8000"
+0000c030: 3e0a 6e67 726f 6b5f 7475 6e6e 656c 3220  >.ngrok_tunnel2 
+0000c040: 3d20 6e67 726f 6b2e 636f 6e6e 6563 7428  = ngrok.connect(
+0000c050: 3830 3030 2994 8594 8194 7d94 681b 6a52  8000).....}.h.jR
+0000c060: 0d00 0073 6261 681f 7d94 2868 215d 9468  ...sbah.}.(h!].h
+0000c070: 235d 9468 255d 9468 275d 9468 295d 946a  #].h%].h'].h)].j
+0000c080: e401 0000 6ae5 0100 006a e601 0000 896a  ....j....j.....j
+0000c090: e701 0000 8c06 7079 7468 6f6e 946a e901  ......python.j..
+0000c0a0: 0000 7d94 7568 2b6a d401 0000 681d 682c  ..}.uh+j....h.h,
+0000c0b0: 681e 4d0f 0168 1b6a df0c 0000 681c 6803  h.M..h.j....h.h.
+0000c0c0: 7562 68ee 2981 947d 9428 6805 8c61 5765  ubh.)..}.(h..aWe
+0000c0d0: 2063 616e 2061 6c73 6f20 6f76 6572 7269   can also overri
+0000c0e0: 6465 2060 606e 6772 6f6b 6060 2773 2069  de ``ngrok``'s i
+0000c0f0: 6e73 7461 6c6c 6564 2061 7574 6820 746f  nstalled auth to
+0000c100: 6b65 6e20 7573 696e 6720 3a63 6c61 7373  ken using :class
+0000c110: 3a60 7e70 796e 6772 6f6b 2e63 6f6e 662e  :`~pyngrok.conf.
+0000c120: 5079 6e67 726f 6b43 6f6e 6669 6760 3a94  PyngrokConfig`:.
+0000c130: 6807 5d94 2868 168c 1557 6520 6361 6e20  h.].(h...We can 
+0000c140: 616c 736f 206f 7665 7272 6964 6520 9485  also override ..
+0000c150: 9481 947d 9428 681b 6a62 0d00 0068 1c68  ...}.(h.jb...h.h
+0000c160: 0368 1d4e 681e 4e75 6268 f429 8194 7d94  .h.Nh.Nubh.)..}.
+0000c170: 2868 058c 0960 606e 6772 6f6b 6060 9468  (h...``ngrok``.h
+0000c180: 075d 9468 168c 056e 6772 6f6b 9485 9481  .].h...ngrok....
+0000c190: 947d 9428 681b 6a6a 0d00 0068 1c68 0368  .}.(h.jj...h.h.h
+0000c1a0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+0000c1b0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+0000c1c0: 9475 682b 68f3 681b 6a62 0d00 0075 6268  .uh+h.h.jb...ubh
+0000c1d0: 168c 20e2 8099 7320 696e 7374 616c 6c65  .. ...s installe
+0000c1e0: 6420 6175 7468 2074 6f6b 656e 2075 7369  d auth token usi
+0000c1f0: 6e67 2094 8594 8194 7d94 2868 1b6a 620d  ng .....}.(h.jb.
+0000c200: 0000 681c 6803 681d 4e68 1e4e 7562 6ab3  ..h.h.h.Nh.Nubj.
+0000c210: 0200 0029 8194 7d94 2868 058c 243a 636c  ...)..}.(h..$:cl
+0000c220: 6173 733a 607e 7079 6e67 726f 6b2e 636f  ass:`~pyngrok.co
+0000c230: 6e66 2e50 796e 6772 6f6b 436f 6e66 6967  nf.PyngrokConfig
+0000c240: 6094 6807 5d94 68f4 2981 947d 9428 6805  `.h.].h.)..}.(h.
+0000c250: 6a7e 0d00 0068 075d 9468 168c 0d50 796e  j~...h.].h...Pyn
+0000c260: 6772 6f6b 436f 6e66 6967 9485 9481 947d  grokConfig.....}
+0000c270: 9428 681b 6a80 0d00 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+0000c280: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+0000c290: 235d 9428 6ac2 0200 008c 0270 7994 8c08  #].(j......py...
+0000c2a0: 7079 2d63 6c61 7373 9465 6825 5d94 6827  py-class.eh%].h'
+0000c2b0: 5d94 6829 5d94 7568 2b68 f368 1b6a 7c0d  ].h)].uh+h.h.j|.
+0000c2c0: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+0000c2d0: 5d94 6825 5d94 6827 5d94 6829 5d94 8c06  ].h%].h'].h)]...
+0000c2e0: 7265 6664 6f63 946a cf02 0000 8c09 7265  refdoc.j......re
+0000c2f0: 6664 6f6d 6169 6e94 6a8a 0d00 008c 0772  fdomain.j......r
+0000c300: 6566 7479 7065 948c 0563 6c61 7373 948c  eftype...class..
+0000c310: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+0000c320: 7265 6677 6172 6e94 896a d502 0000 4e6a  refwarn..j....Nj
+0000c330: d602 0000 4e6a d702 0000 8c1a 7079 6e67  ....Nj......pyng
+0000c340: 726f 6b2e 636f 6e66 2e50 796e 6772 6f6b  rok.conf.Pyngrok
+0000c350: 436f 6e66 6967 9475 682b 6ab2 0200 0068  Config.uh+j....h
+0000c360: 1d68 2c68 1e4d 1c01 681b 6a62 0d00 0075  .h,h.M..h.jb...u
+0000c370: 6268 168c 013a 9485 9481 947d 9428 681b  bh...:.....}.(h.
+0000c380: 6a62 0d00 0068 1c68 0368 1d4e 681e 4e75  jb...h.h.h.Nh.Nu
+0000c390: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+0000c3a0: 255d 9468 275d 9468 295d 9475 682b 68ed  %].h'].h)].uh+h.
+0000c3b0: 681d 682c 681e 4d1c 0168 1b6a df0c 0000  h.h,h.M..h.j....
+0000c3c0: 681c 6803 7562 6ad5 0100 0029 8194 7d94  h.h.ubj....)..}.
+0000c3d0: 2868 058c be66 726f 6d20 7079 6e67 726f  (h...from pyngro
+0000c3e0: 6b20 696d 706f 7274 2063 6f6e 662c 206e  k import conf, n
+0000c3f0: 6772 6f6b 0a0a 636f 6e66 2e67 6574 5f64  grok..conf.get_d
+0000c400: 6566 6175 6c74 2829 2e61 7574 685f 746f  efault().auth_to
+0000c410: 6b65 6e20 3d20 223c 4e47 524f 4b5f 4155  ken = "<NGROK_AU
+0000c420: 5448 5f54 4f4b 454e 3e22 0a0a 2320 3c4e  TH_TOKEN>"..# <N
+0000c430: 6772 6f6b 5475 6e6e 656c 3a20 2268 7474  grokTunnel: "htt
+0000c440: 703a 2f2f 3c70 7562 6c69 635f 7375 623e  p://<public_sub>
+0000c450: 2e6e 6772 6f6b 2e69 6f22 202d 3e20 2268  .ngrok.io" -> "h
+0000c460: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+0000c470: 3830 223e 0a6e 6772 6f6b 5f74 756e 6e65  80">.ngrok_tunne
+0000c480: 6c20 3d20 6e67 726f 6b2e 636f 6e6e 6563  l = ngrok.connec
+0000c490: 7428 2994 6807 5d94 6816 8cbe 6672 6f6d  t().h.].h...from
+0000c4a0: 2070 796e 6772 6f6b 2069 6d70 6f72 7420   pyngrok import 
+0000c4b0: 636f 6e66 2c20 6e67 726f 6b0a 0a63 6f6e  conf, ngrok..con
+0000c4c0: 662e 6765 745f 6465 6661 756c 7428 292e  f.get_default().
+0000c4d0: 6175 7468 5f74 6f6b 656e 203d 2022 3c4e  auth_token = "<N
+0000c4e0: 4752 4f4b 5f41 5554 485f 544f 4b45 4e3e  GROK_AUTH_TOKEN>
+0000c4f0: 220a 0a23 203c 4e67 726f 6b54 756e 6e65  "..# <NgrokTunne
+0000c500: 6c3a 2022 6874 7470 3a2f 2f3c 7075 626c  l: "http://<publ
+0000c510: 6963 5f73 7562 3e2e 6e67 726f 6b2e 696f  ic_sub>.ngrok.io
+0000c520: 2220 2d3e 2022 6874 7470 3a2f 2f6c 6f63  " -> "http://loc
+0000c530: 616c 686f 7374 3a38 3022 3e0a 6e67 726f  alhost:80">.ngro
+0000c540: 6b5f 7475 6e6e 656c 203d 206e 6772 6f6b  k_tunnel = ngrok
+0000c550: 2e63 6f6e 6e65 6374 2829 9485 9481 947d  .connect().....}
+0000c560: 9468 1b6a a60d 0000 7362 6168 1f7d 9428  .h.j....sbah.}.(
+0000c570: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+0000c580: 6829 5d94 6ae4 0100 006a e501 0000 6ae6  h)].j....j....j.
+0000c590: 0100 0089 6ae7 0100 008c 0670 7974 686f  ....j......pytho
+0000c5a0: 6e94 6ae9 0100 007d 9475 682b 6ad4 0100  n.j....}.uh+j...
+0000c5b0: 0068 1d68 2c68 1e4d 1e01 681b 6adf 0c00  .h.h,h.M..h.j...
+0000c5c0: 0068 1c68 0375 6265 681f 7d94 2868 215d  .h.h.ubeh.}.(h!]
+0000c5d0: 948c 1573 6574 7469 6e67 2d74 6865 2d61  ...setting-the-a
+0000c5e0: 7574 6874 6f6b 656e 9461 6823 5d94 6825  uthtoken.ah#].h%
+0000c5f0: 5d94 8c15 7365 7474 696e 6720 7468 6520  ]...setting the 
+0000c600: 6175 7468 746f 6b65 6e94 6168 275d 9468  authtoken.ah'].h
+0000c610: 295d 9475 682b 680a 681b 6a75 0900 0068  )].uh+h.h.ju...h
+0000c620: 1c68 0368 1d68 2c68 1e4d 0901 7562 680b  .h.h.h,h.M..ubh.
+0000c630: 2981 947d 9428 6805 6806 6807 5d94 2868  )..}.(h.h.h.].(h
+0000c640: 1029 8194 7d94 2868 058c 1653 6574 7469  .)..}.(h...Setti
+0000c650: 6e67 2074 6865 2060 6072 6567 696f 6e60  ng the ``region`
+0000c660: 6094 6807 5d94 2868 168c 0c53 6574 7469  `.h.].(h...Setti
+0000c670: 6e67 2074 6865 2094 8594 8194 7d94 2868  ng the .....}.(h
+0000c680: 1b6a c10d 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000c690: 7562 68f4 2981 947d 9428 6805 8c0a 6060  ubh.)..}.(h...``
+0000c6a0: 7265 6769 6f6e 6060 9468 075d 9468 168c  region``.h.].h..
+0000c6b0: 0672 6567 696f 6e94 8594 8194 7d94 2868  .region.....}.(h
+0000c6c0: 1b6a c90d 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000c6d0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+0000c6e0: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+0000c6f0: f368 1b6a c10d 0000 7562 6568 1f7d 9428  .h.j....ubeh.}.(
+0000c700: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+0000c710: 6829 5d94 7568 2b68 0f68 1b6a be0d 0000  h)].uh+h.h.j....
+0000c720: 681c 6803 681d 682c 681e 4d28 0175 6268  h.h.h.h,h.M(.ubh
+0000c730: ee29 8194 7d94 2868 058c 9642 7920 6465  .)..}.(h...By de
+0000c740: 6661 756c 742c 2060 606e 6772 6f6b 6060  fault, ``ngrok``
+0000c750: 2077 696c 6c20 6f70 656e 2061 2074 756e   will open a tun
+0000c760: 6e65 6c20 696e 2074 6865 2060 6075 7360  nel in the ``us`
+0000c770: 6020 7265 6769 6f6e 2e20 546f 206f 7665  ` region. To ove
+0000c780: 7272 6964 6520 7468 6973 2c20 7573 650a  rride this, use.
+0000c790: 7468 6520 6060 7265 6769 6f6e 6060 2070  the ``region`` p
+0000c7a0: 6172 616d 6574 6572 2069 6e20 3a63 6c61  arameter in :cla
+0000c7b0: 7373 3a60 7e70 796e 6772 6f6b 2e63 6f6e  ss:`~pyngrok.con
+0000c7c0: 662e 5079 6e67 726f 6b43 6f6e 6669 6760  f.PyngrokConfig`
+0000c7d0: 3a94 6807 5d94 2868 168c 0c42 7920 6465  :.h.].(h...By de
+0000c7e0: 6661 756c 742c 2094 8594 8194 7d94 2868  fault, .....}.(h
+0000c7f0: 1b6a dd0d 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000c800: 7562 68f4 2981 947d 9428 6805 8c09 6060  ubh.)..}.(h...``
+0000c810: 6e67 726f 6b60 6094 6807 5d94 6816 8c05  ngrok``.h.].h...
+0000c820: 6e67 726f 6b94 8594 8194 7d94 2868 1b6a  ngrok.....}.(h.j
+0000c830: e50d 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+0000c840: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+0000c850: 5d94 6827 5d94 6829 5d94 7568 2b68 f368  ].h'].h)].uh+h.h
+0000c860: 1b6a dd0d 0000 7562 6816 8c1b 2077 696c  .j....ubh... wil
+0000c870: 6c20 6f70 656e 2061 2074 756e 6e65 6c20  l open a tunnel 
+0000c880: 696e 2074 6865 2094 8594 8194 7d94 2868  in the .....}.(h
+0000c890: 1b6a dd0d 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000c8a0: 7562 68f4 2981 947d 9428 6805 8c06 6060  ubh.)..}.(h...``
+0000c8b0: 7573 6060 9468 075d 9468 168c 0275 7394  us``.h.].h...us.
+0000c8c0: 8594 8194 7d94 2868 1b6a f70d 0000 681c  ....}.(h.j....h.
+0000c8d0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+0000c8e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+0000c8f0: 6829 5d94 7568 2b68 f368 1b6a dd0d 0000  h)].uh+h.h.j....
+0000c900: 7562 6816 8c23 2072 6567 696f 6e2e 2054  ubh..# region. T
+0000c910: 6f20 6f76 6572 7269 6465 2074 6869 732c  o override this,
+0000c920: 2075 7365 0a74 6865 2094 8594 8194 7d94   use.the .....}.
+0000c930: 2868 1b6a dd0d 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+0000c940: 1e4e 7562 68f4 2981 947d 9428 6805 8c0a  .Nubh.)..}.(h...
+0000c950: 6060 7265 6769 6f6e 6060 9468 075d 9468  ``region``.h.].h
+0000c960: 168c 0672 6567 696f 6e94 8594 8194 7d94  ...region.....}.
+0000c970: 2868 1b6a 090e 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+0000c980: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000c990: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+0000c9a0: 2b68 f368 1b6a dd0d 0000 7562 6816 8c0e  +h.h.j....ubh...
+0000c9b0: 2070 6172 616d 6574 6572 2069 6e20 9485   parameter in ..
+0000c9c0: 9481 947d 9428 681b 6add 0d00 0068 1c68  ...}.(h.j....h.h
+0000c9d0: 0368 1d4e 681e 4e75 626a b302 0000 2981  .h.Nh.Nubj....).
+0000c9e0: 947d 9428 6805 8c24 3a63 6c61 7373 3a60  .}.(h..$:class:`
+0000c9f0: 7e70 796e 6772 6f6b 2e63 6f6e 662e 5079  ~pyngrok.conf.Py
+0000ca00: 6e67 726f 6b43 6f6e 6669 6760 9468 075d  ngrokConfig`.h.]
+0000ca10: 9468 f429 8194 7d94 2868 056a 1d0e 0000  .h.)..}.(h.j....
+0000ca20: 6807 5d94 6816 8c0d 5079 6e67 726f 6b43  h.].h...PyngrokC
+0000ca30: 6f6e 6669 6794 8594 8194 7d94 2868 1b6a  onfig.....}.(h.j
+0000ca40: 1f0e 0000 681c 6803 681d 4e68 1e4e 7562  ....h.h.h.Nh.Nub
+0000ca50: 6168 1f7d 9428 6821 5d94 6823 5d94 286a  ah.}.(h!].h#].(j
+0000ca60: c202 0000 8c02 7079 948c 0870 792d 636c  ......py...py-cl
+0000ca70: 6173 7394 6568 255d 9468 275d 9468 295d  ass.eh%].h'].h)]
+0000ca80: 9475 682b 68f3 681b 6a1b 0e00 0075 6261  .uh+h.h.j....uba
+0000ca90: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+0000caa0: 9468 275d 9468 295d 948c 0672 6566 646f  .h'].h)]...refdo
+0000cab0: 6394 6acf 0200 008c 0972 6566 646f 6d61  c.j......refdoma
+0000cac0: 696e 946a 290e 0000 8c07 7265 6674 7970  in.j).....reftyp
+0000cad0: 6594 8c05 636c 6173 7394 8c0b 7265 6665  e...class...refe
+0000cae0: 7870 6c69 6369 7494 898c 0772 6566 7761  xplicit....refwa
+0000caf0: 726e 9489 6ad5 0200 004e 6ad6 0200 004e  rn..j....Nj....N
+0000cb00: 6ad7 0200 008c 1a70 796e 6772 6f6b 2e63  j......pyngrok.c
+0000cb10: 6f6e 662e 5079 6e67 726f 6b43 6f6e 6669  onf.PyngrokConfi
+0000cb20: 6794 7568 2b6a b202 0000 681d 682c 681e  g.uh+j....h.h,h.
+0000cb30: 4d2a 0168 1b6a dd0d 0000 7562 6816 8c01  M*.h.j....ubh...
+0000cb40: 3a94 8594 8194 7d94 2868 1b6a dd0d 0000  :.....}.(h.j....
+0000cb50: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
+0000cb60: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+0000cb70: 5d94 6829 5d94 7568 2b68 ed68 1d68 2c68  ].h)].uh+h.h.h,h
+0000cb80: 1e4d 2a01 681b 6abe 0d00 0068 1c68 0375  .M*.h.j....h.h.u
+0000cb90: 626a d501 0000 2981 947d 9428 6805 8cad  bj....)..}.(h...
+0000cba0: 6672 6f6d 2070 796e 6772 6f6b 2069 6d70  from pyngrok imp
+0000cbb0: 6f72 7420 636f 6e66 2c20 6e67 726f 6b0a  ort conf, ngrok.
+0000cbc0: 0a63 6f6e 662e 6765 745f 6465 6661 756c  .conf.get_defaul
+0000cbd0: 7428 292e 7265 6769 6f6e 203d 2022 6175  t().region = "au
+0000cbe0: 220a 0a23 203c 4e67 726f 6b54 756e 6e65  "..# <NgrokTunne
+0000cbf0: 6c3a 2022 6874 7470 3a2f 2f3c 7075 626c  l: "http://<publ
+0000cc00: 6963 5f73 7562 3e2e 6175 2e6e 6772 6f6b  ic_sub>.au.ngrok
+0000cc10: 2e69 6f22 202d 3e20 2268 7474 703a 2f2f  .io" -> "http://
+0000cc20: 6c6f 6361 6c68 6f73 743a 3830 223e 0a6e  localhost:80">.n
+0000cc30: 6772 6f6b 5f74 756e 6e65 6c20 3d20 6e67  grok_tunnel = ng
+0000cc40: 726f 6b2e 636f 6e6e 6563 7428 2994 6807  rok.connect().h.
+0000cc50: 5d94 6816 8cad 6672 6f6d 2070 796e 6772  ].h...from pyngr
+0000cc60: 6f6b 2069 6d70 6f72 7420 636f 6e66 2c20  ok import conf, 
+0000cc70: 6e67 726f 6b0a 0a63 6f6e 662e 6765 745f  ngrok..conf.get_
+0000cc80: 6465 6661 756c 7428 292e 7265 6769 6f6e  default().region
+0000cc90: 203d 2022 6175 220a 0a23 203c 4e67 726f   = "au"..# <Ngro
+0000cca0: 6b54 756e 6e65 6c3a 2022 6874 7470 3a2f  kTunnel: "http:/
+0000ccb0: 2f3c 7075 626c 6963 5f73 7562 3e2e 6175  /<public_sub>.au
+0000ccc0: 2e6e 6772 6f6b 2e69 6f22 202d 3e20 2268  .ngrok.io" -> "h
+0000ccd0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+0000cce0: 3830 223e 0a6e 6772 6f6b 5f74 756e 6e65  80">.ngrok_tunne
+0000ccf0: 6c20 3d20 6e67 726f 6b2e 636f 6e6e 6563  l = ngrok.connec
+0000cd00: 7428 2994 8594 8194 7d94 681b 6a45 0e00  t().....}.h.jE..
+0000cd10: 0073 6261 681f 7d94 2868 215d 9468 235d  .sbah.}.(h!].h#]
+0000cd20: 9468 255d 9468 275d 9468 295d 946a e401  .h%].h'].h)].j..
+0000cd30: 0000 6ae5 0100 006a e601 0000 896a e701  ..j....j.....j..
+0000cd40: 0000 8c06 7079 7468 6f6e 946a e901 0000  ....python.j....
+0000cd50: 7d94 7568 2b6a d401 0000 681d 682c 681e  }.uh+j....h.h,h.
+0000cd60: 4d2d 0168 1b6a be0d 0000 681c 6803 7562  M-.h.j....h.h.ub
+0000cd70: 6568 1f7d 9428 6821 5d94 8c12 7365 7474  eh.}.(h!]...sett
+0000cd80: 696e 672d 7468 652d 7265 6769 6f6e 9461  ing-the-region.a
+0000cd90: 6823 5d94 6825 5d94 8c12 7365 7474 696e  h#].h%]...settin
+0000cda0: 6720 7468 6520 7265 6769 6f6e 9461 6827  g the region.ah'
+0000cdb0: 5d94 6829 5d94 7568 2b68 0a68 1b6a 7509  ].h)].uh+h.h.ju.
+0000cdc0: 0000 681c 6803 681d 682c 681e 4d28 0175  ..h.h.h.h,h.M(.u
+0000cdd0: 6268 0b29 8194 7d94 2868 0568 0668 075d  bh.)..}.(h.h.h.]
+0000cde0: 9428 6810 2981 947d 9428 6805 8c21 5061  .(h.)..}.(h..!Pa
+0000cdf0: 7373 696e 6720 6060 6f70 7469 6f6e 7360  ssing ``options`
+0000ce00: 6020 6173 2060 606b 7761 7267 7360 6094  ` as ``kwargs``.
+0000ce10: 6807 5d94 2868 168c 0850 6173 7369 6e67  h.].(h...Passing
+0000ce20: 2094 8594 8194 7d94 2868 1b6a 600e 0000   .....}.(h.j`...
+0000ce30: 681c 6803 681d 4e68 1e4e 7562 68f4 2981  h.h.h.Nh.Nubh.).
+0000ce40: 947d 9428 6805 8c0b 6060 6f70 7469 6f6e  .}.(h...``option
+0000ce50: 7360 6094 6807 5d94 6816 8c07 6f70 7469  s``.h.].h...opti
+0000ce60: 6f6e 7394 8594 8194 7d94 2868 1b6a 680e  ons.....}.(h.jh.
+0000ce70: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+0000ce80: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000ce90: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
+0000cea0: 600e 0000 7562 6816 8c04 2061 7320 9485  `...ubh... as ..
+0000ceb0: 9481 947d 9428 681b 6a60 0e00 0068 1c68  ...}.(h.j`...h.h
+0000cec0: 0368 1d4e 681e 4e75 6268 f429 8194 7d94  .h.Nh.Nubh.)..}.
+0000ced0: 2868 058c 0a60 606b 7761 7267 7360 6094  (h...``kwargs``.
+0000cee0: 6807 5d94 6816 8c06 6b77 6172 6773 9485  h.].h...kwargs..
+0000cef0: 9481 947d 9428 681b 6a7a 0e00 0068 1c68  ...}.(h.jz...h.h
+0000cf00: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+0000cf10: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+0000cf20: 295d 9475 682b 68f3 681b 6a60 0e00 0075  )].uh+h.h.j`...u
+0000cf30: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+0000cf40: 255d 9468 275d 9468 295d 9475 682b 680f  %].h'].h)].uh+h.
+0000cf50: 681b 6a5d 0e00 0068 1c68 0368 1d68 2c68  h.j]...h.h.h.h,h
+0000cf60: 1e4d 3701 7562 68ee 2981 947d 9428 6805  .M7.ubh.)..}.(h.
+0000cf70: 5889 0100 0049 7420 6973 2070 6f73 7369  X....It is possi
+0000cf80: 626c 6520 746f 2063 6f6e 6669 6775 7265  ble to configure
+0000cf90: 2074 6865 2074 756e 6e65 6c20 7768 656e   the tunnel when
+0000cfa0: 2069 7420 6973 2063 7265 6174 6564 2c20   it is created, 
+0000cfb0: 666f 7220 696e 7374 616e 6365 2061 6464  for instance add
+0000cfc0: 696e 6720 6175 7468 656e 7469 6361 7469  ing authenticati
+0000cfd0: 6f6e 2c0a 6120 7375 6264 6f6d 6169 6e2c  on,.a subdomain,
+0000cfe0: 206f 7220 6f74 6865 7220 7475 6e6e 656c   or other tunnel
+0000cff0: 2070 726f 7065 7274 6965 7320 6073 7570   properties `sup
+0000d000: 706f 7274 6564 2062 7920 6e67 726f 6b20  ported by ngrok 
+0000d010: 3c68 7474 7073 3a2f 2f6e 6772 6f6b 2e63  <https://ngrok.c
+0000d020: 6f6d 2f64 6f63 732f 6e67 726f 6b2d 6167  om/docs/ngrok-ag
+0000d030: 656e 742f 6170 6923 7374 6172 742d 7475  ent/api#start-tu
+0000d040: 6e6e 656c 3e60 5f2e 0a54 6869 7320 6973  nnel>`_..This is
+0000d050: 2061 6363 6f6d 706c 6973 6865 6420 6279   accomplished by
+0000d060: 2070 6173 7369 6e67 2074 6865 7365 2060   passing these `
+0000d070: 606f 7074 696f 6e73 6060 2061 7320 6164  `options`` as ad
+0000d080: 6469 7469 6f6e 616c 2060 606b 7761 7267  ditional ``kwarg
+0000d090: 7360 6020 746f 203a 6675 6e63 3a60 7e70  s`` to :func:`~p
+0000d0a0: 796e 6772 6f6b 2e6e 6772 6f6b 2e63 6f6e  yngrok.ngrok.con
+0000d0b0: 6e65 6374 602c 0a74 6865 6e20 7468 6579  nect`,.then they
+0000d0c0: 2077 696c 6c20 6265 2075 7365 6420 6173   will be used as
+0000d0d0: 2070 726f 7065 7274 6965 7320 666f 7220   properties for 
+0000d0e0: 7468 6520 7475 6e6e 656c 2077 6865 6e20  the tunnel when 
+0000d0f0: 6974 2069 7320 6372 6561 7465 642e 9468  it is created..h
+0000d100: 075d 9428 6816 8c87 4974 2069 7320 706f  .].(h...It is po
+0000d110: 7373 6962 6c65 2074 6f20 636f 6e66 6967  ssible to config
+0000d120: 7572 6520 7468 6520 7475 6e6e 656c 2077  ure the tunnel w
+0000d130: 6865 6e20 6974 2069 7320 6372 6561 7465  hen it is create
+0000d140: 642c 2066 6f72 2069 6e73 7461 6e63 6520  d, for instance 
+0000d150: 6164 6469 6e67 2061 7574 6865 6e74 6963  adding authentic
+0000d160: 6174 696f 6e2c 0a61 2073 7562 646f 6d61  ation,.a subdoma
+0000d170: 696e 2c20 6f72 206f 7468 6572 2074 756e  in, or other tun
+0000d180: 6e65 6c20 7072 6f70 6572 7469 6573 2094  nel properties .
+0000d190: 8594 8194 7d94 2868 1b6a 8e0e 0000 681c  ....}.(h.j....h.
+0000d1a0: 6803 681d 4e68 1e4e 7562 6843 2981 947d  h.h.Nh.NubhC)..}
+0000d1b0: 9428 6805 8c4b 6073 7570 706f 7274 6564  .(h..K`supported
+0000d1c0: 2062 7920 6e67 726f 6b20 3c68 7474 7073   by ngrok <https
+0000d1d0: 3a2f 2f6e 6772 6f6b 2e63 6f6d 2f64 6f63  ://ngrok.com/doc
+0000d1e0: 732f 6e67 726f 6b2d 6167 656e 742f 6170  s/ngrok-agent/ap
+0000d1f0: 6923 7374 6172 742d 7475 6e6e 656c 3e60  i#start-tunnel>`
+0000d200: 5f94 6807 5d94 6816 8c12 7375 7070 6f72  _.h.].h...suppor
+0000d210: 7465 6420 6279 206e 6772 6f6b 9485 9481  ted by ngrok....
+0000d220: 947d 9428 681b 6a96 0e00 0068 1c68 0368  .}.(h.j....h.h.h
+0000d230: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+0000d240: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+0000d250: 948c 046e 616d 6594 8c12 7375 7070 6f72  ...name...suppor
+0000d260: 7465 6420 6279 206e 6772 6f6b 946a 4501  ted by ngrok.jE.
+0000d270: 0000 8c33 6874 7470 733a 2f2f 6e67 726f  ...3https://ngro
+0000d280: 6b2e 636f 6d2f 646f 6373 2f6e 6772 6f6b  k.com/docs/ngrok
+0000d290: 2d61 6765 6e74 2f61 7069 2373 7461 7274  -agent/api#start
+0000d2a0: 2d74 756e 6e65 6c94 7568 2b68 4268 1b6a  -tunnel.uh+hBh.j
+0000d2b0: 8e0e 0000 7562 6a48 0100 0029 8194 7d94  ....ubjH...)..}.
+0000d2c0: 2868 058c 3620 3c68 7474 7073 3a2f 2f6e  (h..6 <https://n
+0000d2d0: 6772 6f6b 2e63 6f6d 2f64 6f63 732f 6e67  grok.com/docs/ng
+0000d2e0: 726f 6b2d 6167 656e 742f 6170 6923 7374  rok-agent/api#st
+0000d2f0: 6172 742d 7475 6e6e 656c 3e94 6807 5d94  art-tunnel>.h.].
+0000d300: 681f 7d94 2868 215d 948c 0369 6431 9461  h.}.(h!]...id1.a
+0000d310: 6823 5d94 6825 5d94 6827 5d94 8c12 7375  h#].h%].h']...su
+0000d320: 7070 6f72 7465 6420 6279 206e 6772 6f6b  pported by ngrok
+0000d330: 9461 6829 5d94 8c06 7265 6675 7269 946a  .ah)]...refuri.j
+0000d340: a60e 0000 7568 2b6a 4701 0000 6a56 0100  ....uh+jG...jV..
+0000d350: 004b 0168 1b6a 8e0e 0000 7562 6816 8c28  .K.h.j....ubh..(
+0000d360: 2e0a 5468 6973 2069 7320 6163 636f 6d70  ..This is accomp
+0000d370: 6c69 7368 6564 2062 7920 7061 7373 696e  lished by passin
+0000d380: 6720 7468 6573 6520 9485 9481 947d 9428  g these .....}.(
+0000d390: 681b 6a8e 0e00 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+0000d3a0: 4e75 6268 f429 8194 7d94 2868 058c 0b60  Nubh.)..}.(h...`
+0000d3b0: 606f 7074 696f 6e73 6060 9468 075d 9468  `options``.h.].h
+0000d3c0: 168c 076f 7074 696f 6e73 9485 9481 947d  ...options.....}
+0000d3d0: 9428 681b 6ab8 0e00 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+0000d3e0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+0000d3f0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+0000d400: 682b 68f3 681b 6a8e 0e00 0075 6268 168c  h+h.h.j....ubh..
+0000d410: 0f20 6173 2061 6464 6974 696f 6e61 6c20  . as additional 
+0000d420: 9485 9481 947d 9428 681b 6a8e 0e00 0068  .....}.(h.j....h
+0000d430: 1c68 0368 1d4e 681e 4e75 6268 f429 8194  .h.h.Nh.Nubh.)..
+0000d440: 7d94 2868 058c 0a60 606b 7761 7267 7360  }.(h...``kwargs`
+0000d450: 6094 6807 5d94 6816 8c06 6b77 6172 6773  `.h.].h...kwargs
+0000d460: 9485 9481 947d 9428 681b 6aca 0e00 0068  .....}.(h.j....h
+0000d470: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+0000d480: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+0000d490: 9468 295d 9475 682b 68f3 681b 6a8e 0e00  .h)].uh+h.h.j...
+0000d4a0: 0075 6268 168c 0420 746f 2094 8594 8194  .ubh... to .....
+0000d4b0: 7d94 2868 1b6a 8e0e 0000 681c 6803 681d  }.(h.j....h.h.h.
+0000d4c0: 4e68 1e4e 7562 6ab3 0200 0029 8194 7d94  Nh.Nubj....)..}.
+0000d4d0: 2868 058c 1e3a 6675 6e63 3a60 7e70 796e  (h...:func:`~pyn
+0000d4e0: 6772 6f6b 2e6e 6772 6f6b 2e63 6f6e 6e65  grok.ngrok.conne
+0000d4f0: 6374 6094 6807 5d94 68f4 2981 947d 9428  ct`.h.].h.)..}.(
+0000d500: 6805 6ade 0e00 0068 075d 9468 168c 0763  h.j....h.].h...c
+0000d510: 6f6e 6e65 6374 9485 9481 947d 9428 681b  onnect.....}.(h.
+0000d520: 6ae0 0e00 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+0000d530: 6261 681f 7d94 2868 215d 9468 235d 9428  bah.}.(h!].h#].(
+0000d540: 6ac2 0200 008c 0270 7994 8c07 7079 2d66  j......py...py-f
+0000d550: 756e 6394 6568 255d 9468 275d 9468 295d  unc.eh%].h'].h)]
+0000d560: 9475 682b 68f3 681b 6adc 0e00 0075 6261  .uh+h.h.j....uba
+0000d570: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+0000d580: 9468 275d 9468 295d 948c 0672 6566 646f  .h'].h)]...refdo
+0000d590: 6394 6acf 0200 008c 0972 6566 646f 6d61  c.j......refdoma
+0000d5a0: 696e 946a ea0e 0000 8c07 7265 6674 7970  in.j......reftyp
+0000d5b0: 6594 8c04 6675 6e63 948c 0b72 6566 6578  e...func...refex
+0000d5c0: 706c 6963 6974 9489 8c07 7265 6677 6172  plicit....refwar
+0000d5d0: 6e94 896a d502 0000 4e6a d602 0000 4e6a  n..j....Nj....Nj
+0000d5e0: d702 0000 8c15 7079 6e67 726f 6b2e 6e67  ......pyngrok.ng
+0000d5f0: 726f 6b2e 636f 6e6e 6563 7494 7568 2b6a  rok.connect.uh+j
+0000d600: b202 0000 681d 682c 681e 4d39 0168 1b6a  ....h.h,h.M9.h.j
+0000d610: 8e0e 0000 7562 6816 8c49 2c0a 7468 656e  ....ubh..I,.then
+0000d620: 2074 6865 7920 7769 6c6c 2062 6520 7573   they will be us
+0000d630: 6564 2061 7320 7072 6f70 6572 7469 6573  ed as properties
+0000d640: 2066 6f72 2074 6865 2074 756e 6e65 6c20   for the tunnel 
+0000d650: 7768 656e 2069 7420 6973 2063 7265 6174  when it is creat
+0000d660: 6564 2e94 8594 8194 7d94 2868 1b6a 8e0e  ed......}.(h.j..
+0000d670: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+0000d680: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000d690: 6827 5d94 6829 5d94 7568 2b68 ed68 1d68  h'].h)].uh+h.h.h
+0000d6a0: 2c68 1e4d 3901 681b 6a5d 0e00 0068 1c68  ,h.M9.h.j]...h.h
+0000d6b0: 0375 6268 ee29 8194 7d94 2868 058c 9148  .ubh.)..}.(h...H
+0000d6c0: 6572 6520 6973 2061 6e20 6578 616d 706c  ere is an exampl
+0000d6d0: 6520 7374 6172 7469 6e67 2060 606e 6772  e starting ``ngr
+0000d6e0: 6f6b 6060 2069 6e20 4175 7374 7261 6c69  ok`` in Australi
+0000d6f0: 612c 2074 6865 6e20 6f70 656e 696e 6720  a, then opening 
+0000d700: 6120 7475 6e6e 656c 2077 6974 6820 7375  a tunnel with su
+0000d710: 6264 6f6d 6169 6e0a 6060 666f 6f60 6020  bdomain.``foo`` 
+0000d720: 7468 6174 2072 6571 7569 7265 7320 6261  that requires ba
+0000d730: 7369 6320 6175 7468 656e 7469 6361 7469  sic authenticati
+0000d740: 6f6e 2066 6f72 2072 6571 7565 7374 732e  on for requests.
+0000d750: 9468 075d 9428 6816 8c1c 4865 7265 2069  .h.].(h...Here i
+0000d760: 7320 616e 2065 7861 6d70 6c65 2073 7461  s an example sta
+0000d770: 7274 696e 6720 9485 9481 947d 9428 681b  rting .....}.(h.
+0000d780: 6a06 0f00 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+0000d790: 6268 f429 8194 7d94 2868 058c 0960 606e  bh.)..}.(h...``n
+0000d7a0: 6772 6f6b 6060 9468 075d 9468 168c 056e  grok``.h.].h...n
+0000d7b0: 6772 6f6b 9485 9481 947d 9428 681b 6a0e  grok.....}.(h.j.
+0000d7c0: 0f00 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+0000d7d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+0000d7e0: 9468 275d 9468 295d 9475 682b 68f3 681b  .h'].h)].uh+h.h.
+0000d7f0: 6a06 0f00 0075 6268 168c 3420 696e 2041  j....ubh..4 in A
+0000d800: 7573 7472 616c 6961 2c20 7468 656e 206f  ustralia, then o
+0000d810: 7065 6e69 6e67 2061 2074 756e 6e65 6c20  pening a tunnel 
+0000d820: 7769 7468 2073 7562 646f 6d61 696e 0a94  with subdomain..
+0000d830: 8594 8194 7d94 2868 1b6a 060f 0000 681c  ....}.(h.j....h.
+0000d840: 6803 681d 4e68 1e4e 7562 68f4 2981 947d  h.h.Nh.Nubh.)..}
+0000d850: 9428 6805 8c07 6060 666f 6f60 6094 6807  .(h...``foo``.h.
+0000d860: 5d94 6816 8c03 666f 6f94 8594 8194 7d94  ].h...foo.....}.
+0000d870: 2868 1b6a 200f 0000 681c 6803 681d 4e68  (h.j ...h.h.h.Nh
+0000d880: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000d890: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+0000d8a0: 2b68 f368 1b6a 060f 0000 7562 6816 8c31  +h.h.j....ubh..1
+0000d8b0: 2074 6861 7420 7265 7175 6972 6573 2062   that requires b
+0000d8c0: 6173 6963 2061 7574 6865 6e74 6963 6174  asic authenticat
+0000d8d0: 696f 6e20 666f 7220 7265 7175 6573 7473  ion for requests
+0000d8e0: 2e94 8594 8194 7d94 2868 1b6a 060f 0000  ......}.(h.j....
+0000d8f0: 681c 6803 681d 4e68 1e4e 7562 6568 1f7d  h.h.h.Nh.Nubeh.}
+0000d900: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+0000d910: 5d94 6829 5d94 7568 2b68 ed68 1d68 2c68  ].h)].uh+h.h.h,h
+0000d920: 1e4d 3e01 681b 6a5d 0e00 0068 1c68 0375  .M>.h.j]...h.h.u
+0000d930: 626a d501 0000 2981 947d 9428 6805 8cea  bj....)..}.(h...
+0000d940: 6672 6f6d 2070 796e 6772 6f6b 2069 6d70  from pyngrok imp
+0000d950: 6f72 7420 636f 6e66 2c20 6e67 726f 6b0a  ort conf, ngrok.
+0000d960: 0a63 6f6e 662e 6765 745f 6465 6661 756c  .conf.get_defaul
+0000d970: 7428 292e 7265 6769 6f6e 203d 2022 6175  t().region = "au
+0000d980: 220a 0a23 203c 4e67 726f 6b54 756e 6e65  "..# <NgrokTunne
+0000d990: 6c3a 2022 6874 7470 3a2f 2f66 6f6f 2e61  l: "http://foo.a
+0000d9a0: 752e 6e67 726f 6b2e 696f 2220 2d3e 2022  u.ngrok.io" -> "
+0000d9b0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+0000d9c0: 3a38 3022 3e0a 6e67 726f 6b5f 7475 6e6e  :80">.ngrok_tunn
+0000d9d0: 656c 203d 206e 6772 6f6b 2e63 6f6e 6e65  el = ngrok.conne
+0000d9e0: 6374 2873 7562 646f 6d61 696e 3d22 666f  ct(subdomain="fo
+0000d9f0: 6f22 2c0a 2020 2020 2020 2020 2020 2020  o",.            
+0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da10: 2061 7574 683d 2275 7365 726e 616d 653a   auth="username:
+0000da20: 7061 7373 776f 7264 2229 9468 075d 9468  password").h.].h
+0000da30: 168c ea66 726f 6d20 7079 6e67 726f 6b20  ...from pyngrok 
+0000da40: 696d 706f 7274 2063 6f6e 662c 206e 6772  import conf, ngr
+0000da50: 6f6b 0a0a 636f 6e66 2e67 6574 5f64 6566  ok..conf.get_def
+0000da60: 6175 6c74 2829 2e72 6567 696f 6e20 3d20  ault().region = 
+0000da70: 2261 7522 0a0a 2320 3c4e 6772 6f6b 5475  "au"..# <NgrokTu
+0000da80: 6e6e 656c 3a20 2268 7474 703a 2f2f 666f  nnel: "http://fo
+0000da90: 6f2e 6175 2e6e 6772 6f6b 2e69 6f22 202d  o.au.ngrok.io" -
+0000daa0: 3e20 2268 7474 703a 2f2f 6c6f 6361 6c68  > "http://localh
+0000dab0: 6f73 743a 3830 223e 0a6e 6772 6f6b 5f74  ost:80">.ngrok_t
+0000dac0: 756e 6e65 6c20 3d20 6e67 726f 6b2e 636f  unnel = ngrok.co
+0000dad0: 6e6e 6563 7428 7375 6264 6f6d 6169 6e3d  nnect(subdomain=
+0000dae0: 2266 6f6f 222c 0a20 2020 2020 2020 2020  "foo",.         
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 2020 2020 6175 7468 3d22 7573 6572 6e61      auth="userna
+0000db10: 6d65 3a70 6173 7377 6f72 6422 2994 8594  me:password")...
+0000db20: 8194 7d94 681b 6a38 0f00 0073 6261 681f  ..}.h.j8...sbah.
+0000db30: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+0000db40: 275d 9468 295d 946a e401 0000 6ae5 0100  '].h)].j....j...
+0000db50: 006a e601 0000 896a e701 0000 8c06 7079  .j.....j......py
+0000db60: 7468 6f6e 946a e901 0000 7d94 7568 2b6a  thon.j....}.uh+j
+0000db70: d401 0000 681d 682c 681e 4d41 0168 1b6a  ....h.h,h.MA.h.j
+0000db80: 5d0e 0000 681c 6803 7562 6568 1f7d 9428  ]...h.h.ubeh.}.(
+0000db90: 6821 5d94 8c19 7061 7373 696e 672d 6f70  h!]...passing-op
+0000dba0: 7469 6f6e 732d 6173 2d6b 7761 7267 7394  tions-as-kwargs.
+0000dbb0: 6168 235d 9468 255d 948c 1970 6173 7369  ah#].h%]...passi
+0000dbc0: 6e67 206f 7074 696f 6e73 2061 7320 6b77  ng options as kw
+0000dbd0: 6172 6773 9461 6827 5d94 6829 5d94 7568  args.ah'].h)].uh
+0000dbe0: 2b68 0a68 1b6a 7509 0000 681c 6803 681d  +h.h.ju...h.h.h.
+0000dbf0: 682c 681e 4d37 0175 6268 0b29 8194 7d94  h,h.M7.ubh.)..}.
+0000dc00: 2868 0568 0668 075d 9428 6810 2981 947d  (h.h.h.].(h.)..}
+0000dc10: 9428 6805 8c0b 436f 6e66 6967 2046 696c  .(h...Config Fil
+0000dc20: 6594 6807 5d94 6816 8c0b 436f 6e66 6967  e.h.].h...Config
+0000dc30: 2046 696c 6594 8594 8194 7d94 2868 1b6a   File.....}.(h.j
+0000dc40: 530f 0000 681c 6803 681d 4e68 1e4e 7562  S...h.h.h.Nh.Nub
+0000dc50: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+0000dc60: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+0000dc70: 1b6a 500f 0000 681c 6803 681d 682c 681e  .jP...h.h.h.h,h.
+0000dc80: 4d4c 0175 6268 ee29 8194 7d94 2868 058c  ML.ubh.)..}.(h..
+0000dc90: e642 7920 6465 6661 756c 742c 2060 6e67  .By default, `ng
+0000dca0: 726f 6b20 7769 6c6c 206c 6f6f 6b20 666f  rok will look fo
+0000dcb0: 7220 6974 7320 636f 6e66 6967 2066 696c  r its config fil
+0000dcc0: 6520 3c68 7474 7073 3a2f 2f6e 6772 6f6b  e <https://ngrok
+0000dcd0: 2e63 6f6d 2f64 6f63 732f 6e67 726f 6b2d  .com/docs/ngrok-
+0000dce0: 6167 656e 742f 636f 6e66 6967 3e60 5f20  agent/config>`_ 
+0000dcf0: 696e 2074 6865 2068 6f6d 6520 6469 7265  in the home dire
+0000dd00: 6374 6f72 7927 7320 6060 2e6e 6772 6f6b  ctory's ``.ngrok
+0000dd10: 3260 600a 666f 6c64 6572 2e20 5765 2063  2``.folder. We c
+0000dd20: 616e 206f 7665 7272 6964 6520 7468 6973  an override this
+0000dd30: 2062 6568 6176 696f 7220 6279 2075 7064   behavior by upd
+0000dd40: 6174 696e 6720 6f75 7220 6465 6661 756c  ating our defaul
+0000dd50: 7420 3a63 6c61 7373 3a60 7e70 796e 6772  t :class:`~pyngr
+0000dd60: 6f6b 2e63 6f6e 662e 5079 6e67 726f 6b43  ok.conf.PyngrokC
+0000dd70: 6f6e 6669 6760 3a94 6807 5d94 2868 168c  onfig`:.h.].(h..
+0000dd80: 0c42 7920 6465 6661 756c 742c 2094 8594  .By default, ...
+0000dd90: 8194 7d94 2868 1b6a 610f 0000 681c 6803  ..}.(h.ja...h.h.
+0000dda0: 681d 4e68 1e4e 7562 6843 2981 947d 9428  h.Nh.NubhC)..}.(
+0000ddb0: 6805 8c52 606e 6772 6f6b 2077 696c 6c20  h..R`ngrok will 
+0000ddc0: 6c6f 6f6b 2066 6f72 2069 7473 2063 6f6e  look for its con
+0000ddd0: 6669 6720 6669 6c65 203c 6874 7470 733a  fig file <https:
+0000dde0: 2f2f 6e67 726f 6b2e 636f 6d2f 646f 6373  //ngrok.com/docs
+0000ddf0: 2f6e 6772 6f6b 2d61 6765 6e74 2f63 6f6e  /ngrok-agent/con
+0000de00: 6669 673e 605f 9468 075d 9468 168c 236e  fig>`_.h.].h..#n
+0000de10: 6772 6f6b 2077 696c 6c20 6c6f 6f6b 2066  grok will look f
+0000de20: 6f72 2069 7473 2063 6f6e 6669 6720 6669  or its config fi
+0000de30: 6c65 9485 9481 947d 9428 681b 6a69 0f00  le.....}.(h.ji..
+0000de40: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+0000de50: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+0000de60: 275d 9468 295d 948c 046e 616d 6594 8c23  '].h)]...name..#
+0000de70: 6e67 726f 6b20 7769 6c6c 206c 6f6f 6b20  ngrok will look 
+0000de80: 666f 7220 6974 7320 636f 6e66 6967 2066  for its config f
+0000de90: 696c 6594 6a45 0100 008c 2968 7474 7073  ile.jE....)https
+0000dea0: 3a2f 2f6e 6772 6f6b 2e63 6f6d 2f64 6f63  ://ngrok.com/doc
+0000deb0: 732f 6e67 726f 6b2d 6167 656e 742f 636f  s/ngrok-agent/co
+0000dec0: 6e66 6967 9475 682b 6842 681b 6a61 0f00  nfig.uh+hBh.ja..
+0000ded0: 0075 626a 4801 0000 2981 947d 9428 6805  .ubjH...)..}.(h.
+0000dee0: 8c2c 203c 6874 7470 733a 2f2f 6e67 726f  ., <https://ngro
+0000def0: 6b2e 636f 6d2f 646f 6373 2f6e 6772 6f6b  k.com/docs/ngrok
+0000df00: 2d61 6765 6e74 2f63 6f6e 6669 673e 9468  -agent/config>.h
+0000df10: 075d 9468 1f7d 9428 6821 5d94 8c23 6e67  .].h.}.(h!]..#ng
+0000df20: 726f 6b2d 7769 6c6c 2d6c 6f6f 6b2d 666f  rok-will-look-fo
+0000df30: 722d 6974 732d 636f 6e66 6967 2d66 696c  r-its-config-fil
+0000df40: 6594 6168 235d 9468 255d 948c 236e 6772  e.ah#].h%]..#ngr
+0000df50: 6f6b 2077 696c 6c20 6c6f 6f6b 2066 6f72  ok will look for
+0000df60: 2069 7473 2063 6f6e 6669 6720 6669 6c65   its config file
+0000df70: 9461 6827 5d94 6829 5d94 8c06 7265 6675  .ah'].h)]...refu
+0000df80: 7269 946a 790f 0000 7568 2b6a 4701 0000  ri.jy...uh+jG...
+0000df90: 6a56 0100 004b 0168 1b6a 610f 0000 7562  jV...K.h.ja...ub
+0000dfa0: 6816 8c1b 2069 6e20 7468 6520 686f 6d65  h... in the home
+0000dfb0: 2064 6972 6563 746f 7279 e280 9973 2094   directory...s .
+0000dfc0: 8594 8194 7d94 2868 1b6a 610f 0000 681c  ....}.(h.ja...h.
+0000dfd0: 6803 681d 4e68 1e4e 7562 68f4 2981 947d  h.h.Nh.Nubh.)..}
+0000dfe0: 9428 6805 8c0b 6060 2e6e 6772 6f6b 3260  .(h...``.ngrok2`
+0000dff0: 6094 6807 5d94 6816 8c07 2e6e 6772 6f6b  `.h.].h....ngrok
+0000e000: 3294 8594 8194 7d94 2868 1b6a 8b0f 0000  2.....}.(h.j....
+0000e010: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
+0000e020: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+0000e030: 5d94 6829 5d94 7568 2b68 f368 1b6a 610f  ].h)].uh+h.h.ja.
+0000e040: 0000 7562 6816 8c3f 0a66 6f6c 6465 722e  ..ubh..?.folder.
+0000e050: 2057 6520 6361 6e20 6f76 6572 7269 6465   We can override
+0000e060: 2074 6869 7320 6265 6861 7669 6f72 2062   this behavior b
+0000e070: 7920 7570 6461 7469 6e67 206f 7572 2064  y updating our d
+0000e080: 6566 6175 6c74 2094 8594 8194 7d94 2868  efault .....}.(h
+0000e090: 1b6a 610f 0000 681c 6803 681d 4e68 1e4e  .ja...h.h.h.Nh.N
+0000e0a0: 7562 6ab3 0200 0029 8194 7d94 2868 058c  ubj....)..}.(h..
+0000e0b0: 243a 636c 6173 733a 607e 7079 6e67 726f  $:class:`~pyngro
+0000e0c0: 6b2e 636f 6e66 2e50 796e 6772 6f6b 436f  k.conf.PyngrokCo
+0000e0d0: 6e66 6967 6094 6807 5d94 68f4 2981 947d  nfig`.h.].h.)..}
+0000e0e0: 9428 6805 6a9f 0f00 0068 075d 9468 168c  .(h.j....h.].h..
+0000e0f0: 0d50 796e 6772 6f6b 436f 6e66 6967 9485  .PyngrokConfig..
+0000e100: 9481 947d 9428 681b 6aa1 0f00 0068 1c68  ...}.(h.j....h.h
+0000e110: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+0000e120: 215d 9468 235d 9428 6ac2 0200 008c 0270  !].h#].(j......p
+0000e130: 7994 8c08 7079 2d63 6c61 7373 9465 6825  y...py-class.eh%
+0000e140: 5d94 6827 5d94 6829 5d94 7568 2b68 f368  ].h'].h)].uh+h.h
+0000e150: 1b6a 9d0f 0000 7562 6168 1f7d 9428 6821  .j....ubah.}.(h!
+0000e160: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+0000e170: 5d94 8c06 7265 6664 6f63 946a cf02 0000  ]...refdoc.j....
+0000e180: 8c09 7265 6664 6f6d 6169 6e94 6aab 0f00  ..refdomain.j...
+0000e190: 008c 0772 6566 7479 7065 948c 0563 6c61  ...reftype...cla
+0000e1a0: 7373 948c 0b72 6566 6578 706c 6963 6974  ss...refexplicit
+0000e1b0: 9489 8c07 7265 6677 6172 6e94 896a d502  ....refwarn..j..
+0000e1c0: 0000 4e6a d602 0000 4e6a d702 0000 8c1a  ..Nj....Nj......
+0000e1d0: 7079 6e67 726f 6b2e 636f 6e66 2e50 796e  pyngrok.conf.Pyn
+0000e1e0: 6772 6f6b 436f 6e66 6967 9475 682b 6ab2  grokConfig.uh+j.
+0000e1f0: 0200 0068 1d68 2c68 1e4d 4e01 681b 6a61  ...h.h,h.MN.h.ja
+0000e200: 0f00 0075 6268 168c 013a 9485 9481 947d  ...ubh...:.....}
+0000e210: 9428 681b 6a61 0f00 0068 1c68 0368 1d4e  .(h.ja...h.h.h.N
+0000e220: 681e 4e75 6265 681f 7d94 2868 215d 9468  h.Nubeh.}.(h!].h
+0000e230: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+0000e240: 682b 68ed 681d 682c 681e 4d4e 0168 1b6a  h+h.h.h,h.MN.h.j
+0000e250: 500f 0000 681c 6803 7562 6ad5 0100 0029  P...h.h.ubj....)
+0000e260: 8194 7d94 2868 058c c266 726f 6d20 7079  ..}.(h...from py
+0000e270: 6e67 726f 6b20 696d 706f 7274 2063 6f6e  ngrok import con
+0000e280: 662c 206e 6772 6f6b 0a0a 636f 6e66 2e67  f, ngrok..conf.g
+0000e290: 6574 5f64 6566 6175 6c74 2829 2e63 6f6e  et_default().con
+0000e2a0: 6669 675f 7061 7468 203d 2022 2f6f 7074  fig_path = "/opt
+0000e2b0: 2f6e 6772 6f6b 2f63 6f6e 6669 672e 796d  /ngrok/config.ym
+0000e2c0: 6c22 0a0a 2320 3c4e 6772 6f6b 5475 6e6e  l"..# <NgrokTunn
+0000e2d0: 656c 3a20 2268 7474 703a 2f2f 3c70 7562  el: "http://<pub
+0000e2e0: 6c69 635f 7375 623e 2e6e 6772 6f6b 2e69  lic_sub>.ngrok.i
+0000e2f0: 6f22 202d 3e20 2268 7474 703a 2f2f 6c6f  o" -> "http://lo
+0000e300: 6361 6c68 6f73 743a 3830 223e 0a6e 6772  calhost:80">.ngr
+0000e310: 6f6b 5f74 756e 6e65 6c20 3d20 6e67 726f  ok_tunnel = ngro
+0000e320: 6b2e 636f 6e6e 6563 7428 2994 6807 5d94  k.connect().h.].
+0000e330: 6816 8cc2 6672 6f6d 2070 796e 6772 6f6b  h...from pyngrok
+0000e340: 2069 6d70 6f72 7420 636f 6e66 2c20 6e67   import conf, ng
+0000e350: 726f 6b0a 0a63 6f6e 662e 6765 745f 6465  rok..conf.get_de
+0000e360: 6661 756c 7428 292e 636f 6e66 6967 5f70  fault().config_p
+0000e370: 6174 6820 3d20 222f 6f70 742f 6e67 726f  ath = "/opt/ngro
+0000e380: 6b2f 636f 6e66 6967 2e79 6d6c 220a 0a23  k/config.yml"..#
+0000e390: 203c 4e67 726f 6b54 756e 6e65 6c3a 2022   <NgrokTunnel: "
+0000e3a0: 6874 7470 3a2f 2f3c 7075 626c 6963 5f73  http://<public_s
+0000e3b0: 7562 3e2e 6e67 726f 6b2e 696f 2220 2d3e  ub>.ngrok.io" ->
+0000e3c0: 2022 6874 7470 3a2f 2f6c 6f63 616c 686f   "http://localho
+0000e3d0: 7374 3a38 3022 3e0a 6e67 726f 6b5f 7475  st:80">.ngrok_tu
+0000e3e0: 6e6e 656c 203d 206e 6772 6f6b 2e63 6f6e  nnel = ngrok.con
+0000e3f0: 6e65 6374 2829 9485 9481 947d 9468 1b6a  nect().....}.h.j
+0000e400: c70f 0000 7362 6168 1f7d 9428 6821 5d94  ....sbah.}.(h!].
+0000e410: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+0000e420: 6ae4 0100 006a e501 0000 6ae6 0100 0089  j....j....j.....
+0000e430: 6ae7 0100 008c 0670 7974 686f 6e94 6ae9  j......python.j.
+0000e440: 0100 007d 9475 682b 6ad4 0100 0068 1d68  ...}.uh+j....h.h
+0000e450: 2c68 1e4d 5101 681b 6a50 0f00 0068 1c68  ,h.MQ.h.jP...h.h
+0000e460: 0375 6265 681f 7d94 2868 215d 948c 0b63  .ubeh.}.(h!]...c
+0000e470: 6f6e 6669 672d 6669 6c65 9461 6823 5d94  onfig-file.ah#].
+0000e480: 6825 5d94 8c0b 636f 6e66 6967 2066 696c  h%]...config fil
+0000e490: 6594 6168 275d 9468 295d 9475 682b 680a  e.ah'].h)].uh+h.
+0000e4a0: 681b 6a75 0900 0068 1c68 0368 1d68 2c68  h.ju...h.h.h.h,h
+0000e4b0: 1e4d 4c01 7562 680b 2981 947d 9428 6805  .ML.ubh.)..}.(h.
+0000e4c0: 6806 6807 5d94 2868 1029 8194 7d94 2868  h.h.].(h.)..}.(h
+0000e4d0: 058c 0b42 696e 6172 7920 5061 7468 9468  ...Binary Path.h
+0000e4e0: 075d 9468 168c 0b42 696e 6172 7920 5061  .].h...Binary Pa
+0000e4f0: 7468 9485 9481 947d 9428 681b 6ae2 0f00  th.....}.(h.j...
+0000e500: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+0000e510: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+0000e520: 275d 9468 295d 9475 682b 680f 681b 6adf  '].h)].uh+h.h.j.
+0000e530: 0f00 0068 1c68 0368 1d68 2c68 1e4d 5b01  ...h.h.h.h,h.M[.
+0000e540: 7562 68ee 2981 947d 9428 6805 8ca2 5468  ubh.)..}.(h...Th
+0000e550: 6520 6060 7079 6e67 726f 6b60 6020 7061  e ``pyngrok`` pa
+0000e560: 636b 6167 6520 6d61 6e61 6765 7320 6974  ckage manages it
+0000e570: 7320 6f77 6e20 6060 6e67 726f 6b60 6020  s own ``ngrok`` 
+0000e580: 6269 6e61 7279 2e20 5765 2063 616e 2075  binary. We can u
+0000e590: 7365 206f 7572 2060 606e 6772 6f6b 6060  se our ``ngrok``
+0000e5a0: 2062 696e 6172 7920 6966 2077 6520 7761   binary if we wa
+0000e5b0: 6e74 0a62 7920 7570 6461 7469 6e67 2074  nt.by updating t
+0000e5c0: 6865 2064 6566 6175 6c74 203a 636c 6173  he default :clas
+0000e5d0: 733a 607e 7079 6e67 726f 6b2e 636f 6e66  s:`~pyngrok.conf
+0000e5e0: 2e50 796e 6772 6f6b 436f 6e66 6967 603a  .PyngrokConfig`:
+0000e5f0: 9468 075d 9428 6816 8c04 5468 6520 9485  .h.].(h...The ..
+0000e600: 9481 947d 9428 681b 6af0 0f00 0068 1c68  ...}.(h.j....h.h
+0000e610: 0368 1d4e 681e 4e75 6268 f429 8194 7d94  .h.Nh.Nubh.)..}.
+0000e620: 2868 058c 0b60 6070 796e 6772 6f6b 6060  (h...``pyngrok``
+0000e630: 9468 075d 9468 168c 0770 796e 6772 6f6b  .h.].h...pyngrok
+0000e640: 9485 9481 947d 9428 681b 6af8 0f00 0068  .....}.(h.j....h
+0000e650: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+0000e660: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+0000e670: 9468 295d 9475 682b 68f3 681b 6af0 0f00  .h)].uh+h.h.j...
+0000e680: 0075 6268 168c 1920 7061 636b 6167 6520  .ubh... package 
+0000e690: 6d61 6e61 6765 7320 6974 7320 6f77 6e20  manages its own 
+0000e6a0: 9485 9481 947d 9428 681b 6af0 0f00 0068  .....}.(h.j....h
+0000e6b0: 1c68 0368 1d4e 681e 4e75 6268 f429 8194  .h.h.Nh.Nubh.)..
+0000e6c0: 7d94 2868 058c 0960 606e 6772 6f6b 6060  }.(h...``ngrok``
+0000e6d0: 9468 075d 9468 168c 056e 6772 6f6b 9485  .h.].h...ngrok..
+0000e6e0: 9481 947d 9428 681b 6a0a 1000 0068 1c68  ...}.(h.j....h.h
+0000e6f0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+0000e700: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+0000e710: 295d 9475 682b 68f3 681b 6af0 0f00 0075  )].uh+h.h.j....u
+0000e720: 6268 168c 1820 6269 6e61 7279 2e20 5765  bh... binary. We
+0000e730: 2063 616e 2075 7365 206f 7572 2094 8594   can use our ...
+0000e740: 8194 7d94 2868 1b6a f00f 0000 681c 6803  ..}.(h.j....h.h.
+0000e750: 681d 4e68 1e4e 7562 68f4 2981 947d 9428  h.Nh.Nubh.)..}.(
+0000e760: 6805 8c09 6060 6e67 726f 6b60 6094 6807  h...``ngrok``.h.
+0000e770: 5d94 6816 8c05 6e67 726f 6b94 8594 8194  ].h...ngrok.....
+0000e780: 7d94 2868 1b6a 1c10 0000 681c 6803 681d  }.(h.j....h.h.h.
+0000e790: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+0000e7a0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+0000e7b0: 7568 2b68 f368 1b6a f00f 0000 7562 6816  uh+h.h.j....ubh.
+0000e7c0: 8c2b 2062 696e 6172 7920 6966 2077 6520  .+ binary if we 
+0000e7d0: 7761 6e74 0a62 7920 7570 6461 7469 6e67  want.by updating
+0000e7e0: 2074 6865 2064 6566 6175 6c74 2094 8594   the default ...
+0000e7f0: 8194 7d94 2868 1b6a f00f 0000 681c 6803  ..}.(h.j....h.h.
+0000e800: 681d 4e68 1e4e 7562 6ab3 0200 0029 8194  h.Nh.Nubj....)..
+0000e810: 7d94 2868 058c 243a 636c 6173 733a 607e  }.(h..$:class:`~
+0000e820: 7079 6e67 726f 6b2e 636f 6e66 2e50 796e  pyngrok.conf.Pyn
+0000e830: 6772 6f6b 436f 6e66 6967 6094 6807 5d94  grokConfig`.h.].
+0000e840: 68f4 2981 947d 9428 6805 6a30 1000 0068  h.)..}.(h.j0...h
+0000e850: 075d 9468 168c 0d50 796e 6772 6f6b 436f  .].h...PyngrokCo
+0000e860: 6e66 6967 9485 9481 947d 9428 681b 6a32  nfig.....}.(h.j2
+0000e870: 1000 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+0000e880: 681f 7d94 2868 215d 9468 235d 9428 6ac2  h.}.(h!].h#].(j.
+0000e890: 0200 008c 0270 7994 8c08 7079 2d63 6c61  .....py...py-cla
+0000e8a0: 7373 9465 6825 5d94 6827 5d94 6829 5d94  ss.eh%].h'].h)].
+0000e8b0: 7568 2b68 f368 1b6a 2e10 0000 7562 6168  uh+h.h.j....ubah
+0000e8c0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000e8d0: 6827 5d94 6829 5d94 8c06 7265 6664 6f63  h'].h)]...refdoc
+0000e8e0: 946a cf02 0000 8c09 7265 6664 6f6d 6169  .j......refdomai
+0000e8f0: 6e94 6a3c 1000 008c 0772 6566 7479 7065  n.j<.....reftype
+0000e900: 948c 0563 6c61 7373 948c 0b72 6566 6578  ...class...refex
+0000e910: 706c 6963 6974 9489 8c07 7265 6677 6172  plicit....refwar
+0000e920: 6e94 896a d502 0000 4e6a d602 0000 4e6a  n..j....Nj....Nj
+0000e930: d702 0000 8c1a 7079 6e67 726f 6b2e 636f  ......pyngrok.co
+0000e940: 6e66 2e50 796e 6772 6f6b 436f 6e66 6967  nf.PyngrokConfig
+0000e950: 9475 682b 6ab2 0200 0068 1d68 2c68 1e4d  .uh+j....h.h,h.M
+0000e960: 5d01 681b 6af0 0f00 0075 6268 168c 013a  ].h.j....ubh...:
+0000e970: 9485 9481 947d 9428 681b 6af0 0f00 0068  .....}.(h.j....h
+0000e980: 1c68 0368 1d4e 681e 4e75 6265 681f 7d94  .h.h.Nh.Nubeh.}.
+0000e990: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+0000e9a0: 9468 295d 9475 682b 68ed 681d 682c 681e  .h)].uh+h.h.h,h.
+0000e9b0: 4d5d 0168 1b6a df0f 0000 681c 6803 7562  M].h.j....h.h.ub
+0000e9c0: 6ad5 0100 0029 8194 7d94 2868 058c c066  j....)..}.(h...f
+0000e9d0: 726f 6d20 7079 6e67 726f 6b20 696d 706f  rom pyngrok impo
+0000e9e0: 7274 2063 6f6e 662c 206e 6772 6f6b 0a0a  rt conf, ngrok..
+0000e9f0: 636f 6e66 2e67 6574 5f64 6566 6175 6c74  conf.get_default
+0000ea00: 2829 2e6e 6772 6f6b 5f70 6174 6820 3d20  ().ngrok_path = 
+0000ea10: 222f 7573 722f 6c6f 6361 6c2f 6269 6e2f  "/usr/local/bin/
+0000ea20: 6e67 726f 6b22 0a0a 2320 3c4e 6772 6f6b  ngrok"..# <Ngrok
+0000ea30: 5475 6e6e 656c 3a20 2268 7474 703a 2f2f  Tunnel: "http://
+0000ea40: 3c70 7562 6c69 635f 7375 623e 2e6e 6772  <public_sub>.ngr
+0000ea50: 6f6b 2e69 6f22 202d 3e20 2268 7474 703a  ok.io" -> "http:
+0000ea60: 2f2f 6c6f 6361 6c68 6f73 743a 3830 223e  //localhost:80">
+0000ea70: 0a6e 6772 6f6b 5f74 756e 6e65 6c20 3d20  .ngrok_tunnel = 
+0000ea80: 6e67 726f 6b2e 636f 6e6e 6563 7428 2994  ngrok.connect().
+0000ea90: 6807 5d94 6816 8cc0 6672 6f6d 2070 796e  h.].h...from pyn
+0000eaa0: 6772 6f6b 2069 6d70 6f72 7420 636f 6e66  grok import conf
+0000eab0: 2c20 6e67 726f 6b0a 0a63 6f6e 662e 6765  , ngrok..conf.ge
+0000eac0: 745f 6465 6661 756c 7428 292e 6e67 726f  t_default().ngro
+0000ead0: 6b5f 7061 7468 203d 2022 2f75 7372 2f6c  k_path = "/usr/l
+0000eae0: 6f63 616c 2f62 696e 2f6e 6772 6f6b 220a  ocal/bin/ngrok".
+0000eaf0: 0a23 203c 4e67 726f 6b54 756e 6e65 6c3a  .# <NgrokTunnel:
+0000eb00: 2022 6874 7470 3a2f 2f3c 7075 626c 6963   "http://<public
+0000eb10: 5f73 7562 3e2e 6e67 726f 6b2e 696f 2220  _sub>.ngrok.io" 
+0000eb20: 2d3e 2022 6874 7470 3a2f 2f6c 6f63 616c  -> "http://local
+0000eb30: 686f 7374 3a38 3022 3e0a 6e67 726f 6b5f  host:80">.ngrok_
+0000eb40: 7475 6e6e 656c 203d 206e 6772 6f6b 2e63  tunnel = ngrok.c
+0000eb50: 6f6e 6e65 6374 2829 9485 9481 947d 9468  onnect().....}.h
+0000eb60: 1b6a 5810 0000 7362 6168 1f7d 9428 6821  .jX...sbah.}.(h!
+0000eb70: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+0000eb80: 5d94 6ae4 0100 006a e501 0000 6ae6 0100  ].j....j....j...
+0000eb90: 0089 6ae7 0100 008c 0670 7974 686f 6e94  ..j......python.
+0000eba0: 6ae9 0100 007d 9475 682b 6ad4 0100 0068  j....}.uh+j....h
+0000ebb0: 1d68 2c68 1e4d 6001 681b 6adf 0f00 0068  .h,h.M`.h.j....h
+0000ebc0: 1c68 0375 6265 681f 7d94 2868 215d 948c  .h.ubeh.}.(h!]..
+0000ebd0: 0b62 696e 6172 792d 7061 7468 9461 6823  .binary-path.ah#
+0000ebe0: 5d94 6825 5d94 8c0b 6269 6e61 7279 2070  ].h%]...binary p
+0000ebf0: 6174 6894 6168 275d 9468 295d 9475 682b  ath.ah'].h)].uh+
+0000ec00: 680a 681b 6a75 0900 0068 1c68 0368 1d68  h.h.ju...h.h.h.h
+0000ec10: 2c68 1e4d 5b01 7562 6568 1f7d 9428 6821  ,h.M[.ubeh.}.(h!
+0000ec20: 5d94 8c0d 636f 6e66 6967 7572 6174 696f  ]...configuratio
+0000ec30: 6e94 6168 235d 9468 255d 948c 0d63 6f6e  n.ah#].h%]...con
+0000ec40: 6669 6775 7261 7469 6f6e 9461 6827 5d94  figuration.ah'].
+0000ec50: 6829 5d94 7568 2b68 0a68 1b68 0c68 1c68  h)].uh+h.h.h.h.h
+0000ec60: 0368 1d68 2c68 1e4b d875 6268 0b29 8194  .h.h,h.K.ubh.)..
+0000ec70: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+0000ec80: 947d 9428 6805 8c12 436f 6d6d 616e 6420  .}.(h...Command 
+0000ec90: 4c69 6e65 2055 7361 6765 9468 075d 9468  Line Usage.h.].h
+0000eca0: 168c 1243 6f6d 6d61 6e64 204c 696e 6520  ...Command Line 
+0000ecb0: 5573 6167 6594 8594 8194 7d94 2868 1b6a  Usage.....}.(h.j
+0000ecc0: 7b10 0000 681c 6803 681d 4e68 1e4e 7562  {...h.h.h.Nh.Nub
+0000ecd0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+0000ece0: 5d94 6827 5d94 6829 5d94 7568 2b68 0f68  ].h'].h)].uh+h.h
+0000ecf0: 1b6a 7810 0000 681c 6803 681d 682c 681e  .jx...h.h.h.h,h.
+0000ed00: 4d6a 0175 6268 ee29 8194 7d94 2868 058c  Mj.ubh.)..}.(h..
+0000ed10: 8054 6869 7320 7061 636b 6167 6520 7075  .This package pu
+0000ed20: 7473 2074 6865 2064 6566 6175 6c74 2060  ts the default `
+0000ed30: 606e 6772 6f6b 6060 2062 696e 6172 7920  `ngrok`` binary 
+0000ed40: 6f6e 206f 7572 2070 6174 682c 2073 6f20  on our path, so 
+0000ed50: 616c 6c20 6665 6174 7572 6573 206f 6620  all features of 
+0000ed60: 6060 6e67 726f 6b60 6020 6172 6520 616c  ``ngrok`` are al
+0000ed70: 736f 0a61 7661 696c 6162 6c65 206f 6e20  so.available on 
+0000ed80: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
+0000ed90: 2e94 6807 5d94 2868 168c 1e54 6869 7320  ..h.].(h...This 
+0000eda0: 7061 636b 6167 6520 7075 7473 2074 6865  package puts the
+0000edb0: 2064 6566 6175 6c74 2094 8594 8194 7d94   default .....}.
+0000edc0: 2868 1b6a 8910 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+0000edd0: 1e4e 7562 68f4 2981 947d 9428 6805 8c09  .Nubh.)..}.(h...
+0000ede0: 6060 6e67 726f 6b60 6094 6807 5d94 6816  ``ngrok``.h.].h.
+0000edf0: 8c05 6e67 726f 6b94 8594 8194 7d94 2868  ..ngrok.....}.(h
+0000ee00: 1b6a 9110 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000ee10: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+0000ee20: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+0000ee30: f368 1b6a 8910 0000 7562 6816 8c28 2062  .h.j....ubh..( b
+0000ee40: 696e 6172 7920 6f6e 206f 7572 2070 6174  inary on our pat
+0000ee50: 682c 2073 6f20 616c 6c20 6665 6174 7572  h, so all featur
+0000ee60: 6573 206f 6620 9485 9481 947d 9428 681b  es of .....}.(h.
+0000ee70: 6a89 1000 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+0000ee80: 6268 f429 8194 7d94 2868 058c 0960 606e  bh.)..}.(h...``n
+0000ee90: 6772 6f6b 6060 9468 075d 9468 168c 056e  grok``.h.].h...n
+0000eea0: 6772 6f6b 9485 9481 947d 9428 681b 6aa3  grok.....}.(h.j.
+0000eeb0: 1000 0068 1c68 0368 1d4e 681e 4e75 6261  ...h.h.h.Nh.Nuba
+0000eec0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+0000eed0: 9468 275d 9468 295d 9475 682b 68f3 681b  .h'].h)].uh+h.h.
+0000eee0: 6a89 1000 0075 6268 168c 2820 6172 6520  j....ubh..( are 
+0000eef0: 616c 736f 0a61 7661 696c 6162 6c65 206f  also.available o
+0000ef00: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
+0000ef10: 6e65 2e94 8594 8194 7d94 2868 1b6a 8910  ne......}.(h.j..
+0000ef20: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+0000ef30: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000ef40: 6827 5d94 6829 5d94 7568 2b68 ed68 1d68  h'].h)].uh+h.h.h
+0000ef50: 2c68 1e4d 6c01 681b 6a78 1000 0068 1c68  ,h.Ml.h.jx...h.h
+0000ef60: 0375 626a d501 0000 2981 947d 9428 6805  .ubj....)..}.(h.
+0000ef70: 8c0d 6e67 726f 6b20 6874 7470 2038 3094  ..ngrok http 80.
+0000ef80: 6807 5d94 6816 8c0d 6e67 726f 6b20 6874  h.].h...ngrok ht
+0000ef90: 7470 2038 3094 8594 8194 7d94 681b 6abb  tp 80.....}.h.j.
+0000efa0: 1000 0073 6261 681f 7d94 2868 215d 9468  ...sbah.}.(h!].h
+0000efb0: 235d 9468 255d 9468 275d 9468 295d 946a  #].h%].h'].h)].j
+0000efc0: e401 0000 6ae5 0100 006a e601 0000 896a  ....j....j.....j
+0000efd0: e701 0000 8c02 7368 946a e901 0000 7d94  ......sh.j....}.
+0000efe0: 7568 2b6a d401 0000 681d 682c 681e 4d6f  uh+j....h.h,h.Mo
+0000eff0: 0168 1b6a 7810 0000 681c 6803 7562 68ee  .h.jx...h.h.ubh.
+0000f000: 2981 947d 9428 6805 8c85 466f 7220 6465  )..}.(h...For de
+0000f010: 7461 696c 7320 6f6e 2068 6f77 2074 6f20  tails on how to 
+0000f020: 6675 6c6c 7920 6c65 7665 7261 6765 2060  fully leverage `
+0000f030: 606e 6772 6f6b 6060 2066 726f 6d20 7468  `ngrok`` from th
+0000f040: 6520 636f 6d6d 616e 6420 6c69 6e65 2c20  e command line, 
+0000f050: 7365 6520 606e 6772 6f6b 2773 206f 6666  see `ngrok's off
+0000f060: 6963 6961 6c20 646f 6375 6d65 6e74 6174  icial documentat
+0000f070: 696f 6e20 3c68 7474 7073 3a2f 2f6e 6772  ion <https://ngr
+0000f080: 6f6b 2e63 6f6d 2f64 6f63 733e 605f 2e94  ok.com/docs>`_..
+0000f090: 6807 5d94 2868 168c 2546 6f72 2064 6574  h.].(h..%For det
+0000f0a0: 6169 6c73 206f 6e20 686f 7720 746f 2066  ails on how to f
+0000f0b0: 756c 6c79 206c 6576 6572 6167 6520 9485  ully leverage ..
+0000f0c0: 9481 947d 9428 681b 6acb 1000 0068 1c68  ...}.(h.j....h.h
+0000f0d0: 0368 1d4e 681e 4e75 6268 f429 8194 7d94  .h.Nh.Nubh.)..}.
+0000f0e0: 2868 058c 0960 606e 6772 6f6b 6060 9468  (h...``ngrok``.h
+0000f0f0: 075d 9468 168c 056e 6772 6f6b 9485 9481  .].h...ngrok....
+0000f100: 947d 9428 681b 6ad3 1000 0068 1c68 0368  .}.(h.j....h.h.h
+0000f110: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+0000f120: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+0000f130: 9475 682b 68f3 681b 6acb 1000 0075 6268  .uh+h.h.j....ubh
+0000f140: 168c 1c20 6672 6f6d 2074 6865 2063 6f6d  ... from the com
+0000f150: 6d61 6e64 206c 696e 652c 2073 6565 2094  mand line, see .
+0000f160: 8594 8194 7d94 2868 1b6a cb10 0000 681c  ....}.(h.j....h.
+0000f170: 6803 681d 4e68 1e4e 7562 6843 2981 947d  h.h.Nh.NubhC)..}
+0000f180: 9428 6805 8c3a 606e 6772 6f6b 2773 206f  .(h..:`ngrok's o
+0000f190: 6666 6963 6961 6c20 646f 6375 6d65 6e74  fficial document
+0000f1a0: 6174 696f 6e20 3c68 7474 7073 3a2f 2f6e  ation <https://n
+0000f1b0: 6772 6f6b 2e63 6f6d 2f64 6f63 733e 605f  grok.com/docs>`_
+0000f1c0: 9468 075d 9468 168c 206e 6772 6f6b e280  .h.].h.. ngrok..
+0000f1d0: 9973 206f 6666 6963 6961 6c20 646f 6375  .s official docu
+0000f1e0: 6d65 6e74 6174 696f 6e94 8594 8194 7d94  mentation.....}.
+0000f1f0: 2868 1b6a e510 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+0000f200: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000f210: 5d94 6825 5d94 6827 5d94 6829 5d94 8c04  ].h%].h'].h)]...
+0000f220: 6e61 6d65 948c 1e6e 6772 6f6b 2773 206f  name...ngrok's o
+0000f230: 6666 6963 6961 6c20 646f 6375 6d65 6e74  fficial document
+0000f240: 6174 696f 6e94 6a45 0100 008c 1668 7474  ation.jE.....htt
+0000f250: 7073 3a2f 2f6e 6772 6f6b 2e63 6f6d 2f64  ps://ngrok.com/d
+0000f260: 6f63 7394 7568 2b68 4268 1b6a cb10 0000  ocs.uh+hBh.j....
+0000f270: 7562 6a48 0100 0029 8194 7d94 2868 058c  ubjH...)..}.(h..
+0000f280: 1920 3c68 7474 7073 3a2f 2f6e 6772 6f6b  . <https://ngrok
+0000f290: 2e63 6f6d 2f64 6f63 733e 9468 075d 9468  .com/docs>.h.].h
+0000f2a0: 1f7d 9428 6821 5d94 8c1e 6e67 726f 6b2d  .}.(h!]...ngrok-
+0000f2b0: 732d 6f66 6669 6369 616c 2d64 6f63 756d  s-official-docum
+0000f2c0: 656e 7461 7469 6f6e 9461 6823 5d94 6825  entation.ah#].h%
+0000f2d0: 5d94 8c1e 6e67 726f 6b27 7320 6f66 6669  ]...ngrok's offi
+0000f2e0: 6369 616c 2064 6f63 756d 656e 7461 7469  cial documentati
+0000f2f0: 6f6e 9461 6827 5d94 6829 5d94 8c06 7265  on.ah'].h)]...re
+0000f300: 6675 7269 946a f510 0000 7568 2b6a 4701  furi.j....uh+jG.
+0000f310: 0000 6a56 0100 004b 0168 1b6a cb10 0000  ..jV...K.h.j....
+0000f320: 7562 6816 8c01 2e94 8594 8194 7d94 2868  ubh.........}.(h
+0000f330: 1b6a cb10 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000f340: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
+0000f350: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+0000f360: ed68 1d68 2c68 1e4d 7301 681b 6a78 1000  .h.h,h.Ms.h.jx..
+0000f370: 0068 1c68 0375 6265 681f 7d94 2868 215d  .h.h.ubeh.}.(h!]
+0000f380: 948c 1263 6f6d 6d61 6e64 2d6c 696e 652d  ...command-line-
+0000f390: 7573 6167 6594 6168 235d 9468 255d 948c  usage.ah#].h%]..
+0000f3a0: 1263 6f6d 6d61 6e64 206c 696e 6520 7573  .command line us
+0000f3b0: 6167 6594 6168 275d 9468 295d 9475 682b  age.ah'].h)].uh+
+0000f3c0: 680a 681b 680c 681c 6803 681d 682c 681e  h.h.h.h.h.h.h,h.
+0000f3d0: 4d6a 0175 6268 0b29 8194 7d94 2868 0568  Mj.ubh.)..}.(h.h
+0000f3e0: 0668 075d 9428 6810 2981 947d 9428 6805  .h.].(h.)..}.(h.
+0000f3f0: 8c0a 5079 7468 6f6e 2032 2e37 9468 075d  ..Python 2.7.h.]
+0000f400: 9468 168c 0a50 7974 686f 6e20 322e 3794  .h...Python 2.7.
+0000f410: 8594 8194 7d94 2868 1b6a 1811 0000 681c  ....}.(h.j....h.
+0000f420: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+0000f430: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+0000f440: 6829 5d94 7568 2b68 0f68 1b6a 1511 0000  h)].uh+h.h.j....
+0000f450: 681c 6803 681d 682c 681e 4d76 0175 6268  h.h.h.h,h.Mv.ubh
+0000f460: ee29 8194 7d94 2868 0558 0501 0000 5468  .)..}.(h.X....Th
+0000f470: 6520 6c61 7374 2076 6572 7369 6f6e 206f  e last version o
+0000f480: 6620 6060 7079 6e67 726f 6b60 6020 7468  f ``pyngrok`` th
+0000f490: 6174 2073 7570 706f 7274 7320 5079 7468  at supports Pyth
+0000f4a0: 6f6e 2032 2e37 2069 7320 342e 312e 782c  on 2.7 is 4.1.x,
+0000f4b0: 2073 6f20 7765 206e 6565 6420 746f 2070   so we need to p
+0000f4c0: 696e 2060 6070 796e 6772 6f6b 3e3d 342e  in ``pyngrok>=4.
+0000f4d0: 312c 3c34 2e32 6060 2069 6620 7765 2073  1,<4.2`` if we s
+0000f4e0: 7469 6c6c 0a77 616e 7420 746f 2075 7365  till.want to use
+0000f4f0: 2060 6070 796e 6772 6f6b 6060 2077 6974   ``pyngrok`` wit
+0000f500: 6820 7468 6973 2076 6572 7369 6f6e 206f  h this version o
+0000f510: 6620 5079 7468 6f6e 2e20 4974 7320 6c65  f Python. Its le
+0000f520: 6761 6379 2064 6f63 756d 656e 7461 7469  gacy documentati
+0000f530: 6f6e 2063 616e 2062 6520 666f 756e 6420  on can be found 
+0000f540: 6068 6572 6520 3c68 7474 7073 3a2f 2f70  `here <https://p
+0000f550: 796e 6772 6f6b 2e72 6561 6474 6865 646f  yngrok.readthedo
+0000f560: 6373 2e69 6f2f 656e 2f34 2e31 2e78 2f3e  cs.io/en/4.1.x/>
+0000f570: 605f 2e94 6807 5d94 2868 168c 1454 6865  `_..h.].(h...The
+0000f580: 206c 6173 7420 7665 7273 696f 6e20 6f66   last version of
+0000f590: 2094 8594 8194 7d94 2868 1b6a 2611 0000   .....}.(h.j&...
+0000f5a0: 681c 6803 681d 4e68 1e4e 7562 68f4 2981  h.h.h.Nh.Nubh.).
+0000f5b0: 947d 9428 6805 8c0b 6060 7079 6e67 726f  .}.(h...``pyngro
+0000f5c0: 6b60 6094 6807 5d94 6816 8c07 7079 6e67  k``.h.].h...pyng
+0000f5d0: 726f 6b94 8594 8194 7d94 2868 1b6a 2e11  rok.....}.(h.j..
+0000f5e0: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+0000f5f0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+0000f600: 6827 5d94 6829 5d94 7568 2b68 f368 1b6a  h'].h)].uh+h.h.j
+0000f610: 2611 0000 7562 6816 8c36 2074 6861 7420  &...ubh..6 that 
+0000f620: 7375 7070 6f72 7473 2050 7974 686f 6e20  supports Python 
+0000f630: 322e 3720 6973 2034 2e31 2e78 2c20 736f  2.7 is 4.1.x, so
+0000f640: 2077 6520 6e65 6564 2074 6f20 7069 6e20   we need to pin 
+0000f650: 9485 9481 947d 9428 681b 6a26 1100 0068  .....}.(h.j&...h
+0000f660: 1c68 0368 1d4e 681e 4e75 6268 f429 8194  .h.h.Nh.Nubh.)..
+0000f670: 7d94 2868 058c 1560 6070 796e 6772 6f6b  }.(h...``pyngrok
+0000f680: 3e3d 342e 312c 3c34 2e32 6060 9468 075d  >=4.1,<4.2``.h.]
+0000f690: 9468 168c 1170 796e 6772 6f6b 3e3d 342e  .h...pyngrok>=4.
+0000f6a0: 312c 3c34 2e32 9485 9481 947d 9428 681b  1,<4.2.....}.(h.
+0000f6b0: 6a40 1100 0068 1c68 0368 1d4e 681e 4e75  j@...h.h.h.Nh.Nu
+0000f6c0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+0000f6d0: 255d 9468 275d 9468 295d 9475 682b 68f3  %].h'].h)].uh+h.
+0000f6e0: 681b 6a26 1100 0075 6268 168c 1920 6966  h.j&...ubh... if
+0000f6f0: 2077 6520 7374 696c 6c0a 7761 6e74 2074   we still.want t
+0000f700: 6f20 7573 6520 9485 9481 947d 9428 681b  o use .....}.(h.
+0000f710: 6a26 1100 0068 1c68 0368 1d4e 681e 4e75  j&...h.h.h.Nh.Nu
+0000f720: 6268 f429 8194 7d94 2868 058c 0b60 6070  bh.)..}.(h...``p
+0000f730: 796e 6772 6f6b 6060 9468 075d 9468 168c  yngrok``.h.].h..
+0000f740: 0770 796e 6772 6f6b 9485 9481 947d 9428  .pyngrok.....}.(
+0000f750: 681b 6a52 1100 0068 1c68 0368 1d4e 681e  h.jR...h.h.h.Nh.
+0000f760: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+0000f770: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+0000f780: 68f3 681b 6a26 1100 0075 6268 168c 4420  h.h.j&...ubh..D 
+0000f790: 7769 7468 2074 6869 7320 7665 7273 696f  with this versio
+0000f7a0: 6e20 6f66 2050 7974 686f 6e2e 2049 7473  n of Python. Its
+0000f7b0: 206c 6567 6163 7920 646f 6375 6d65 6e74   legacy document
+0000f7c0: 6174 696f 6e20 6361 6e20 6265 2066 6f75  ation can be fou
+0000f7d0: 6e64 2094 8594 8194 7d94 2868 1b6a 2611  nd .....}.(h.j&.
+0000f7e0: 0000 681c 6803 681d 4e68 1e4e 7562 6843  ..h.h.h.Nh.NubhC
+0000f7f0: 2981 947d 9428 6805 8c32 6068 6572 6520  )..}.(h..2`here 
+0000f800: 3c68 7474 7073 3a2f 2f70 796e 6772 6f6b  <https://pyngrok
+0000f810: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+0000f820: 656e 2f34 2e31 2e78 2f3e 605f 9468 075d  en/4.1.x/>`_.h.]
+0000f830: 9468 168c 0468 6572 6594 8594 8194 7d94  .h...here.....}.
+0000f840: 2868 1b6a 6411 0000 681c 6803 681d 4e68  (h.jd...h.h.h.Nh
+0000f850: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000f860: 5d94 6825 5d94 6827 5d94 6829 5d94 8c04  ].h%].h'].h)]...
+0000f870: 6e61 6d65 948c 0468 6572 6594 6a45 0100  name...here.jE..
+0000f880: 008c 2868 7474 7073 3a2f 2f70 796e 6772  ..(https://pyngr
+0000f890: 6f6b 2e72 6561 6474 6865 646f 6373 2e69  ok.readthedocs.i
+0000f8a0: 6f2f 656e 2f34 2e31 2e78 2f94 7568 2b68  o/en/4.1.x/.uh+h
+0000f8b0: 4268 1b6a 2611 0000 7562 6a48 0100 0029  Bh.j&...ubjH...)
+0000f8c0: 8194 7d94 2868 058c 2b20 3c68 7474 7073  ..}.(h..+ <https
+0000f8d0: 3a2f 2f70 796e 6772 6f6b 2e72 6561 6474  ://pyngrok.readt
+0000f8e0: 6865 646f 6373 2e69 6f2f 656e 2f34 2e31  hedocs.io/en/4.1
+0000f8f0: 2e78 2f3e 9468 075d 9468 1f7d 9428 6821  .x/>.h.].h.}.(h!
+0000f900: 5d94 8c04 6865 7265 9461 6823 5d94 6825  ]...here.ah#].h%
+0000f910: 5d94 8c04 6865 7265 9461 6827 5d94 6829  ]...here.ah'].h)
+0000f920: 5d94 8c06 7265 6675 7269 946a 7411 0000  ]...refuri.jt...
+0000f930: 7568 2b6a 4701 0000 6a56 0100 004b 0168  uh+jG...jV...K.h
+0000f940: 1b6a 2611 0000 7562 6816 8c01 2e94 8594  .j&...ubh.......
+0000f950: 8194 7d94 2868 1b6a 2611 0000 681c 6803  ..}.(h.j&...h.h.
+0000f960: 681d 4e68 1e4e 7562 6568 1f7d 9428 6821  h.Nh.Nubeh.}.(h!
+0000f970: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+0000f980: 5d94 7568 2b68 ed68 1d68 2c68 1e4d 7801  ].uh+h.h.h,h.Mx.
+0000f990: 681b 6a15 1100 0068 1c68 0375 6265 681f  h.j....h.h.ubeh.
+0000f9a0: 7d94 2868 215d 948c 0a70 7974 686f 6e2d  }.(h!]...python-
+0000f9b0: 322d 3794 6168 235d 9468 255d 948c 0a70  2-7.ah#].h%]...p
+0000f9c0: 7974 686f 6e20 322e 3794 6168 275d 9468  ython 2.7.ah'].h
+0000f9d0: 295d 9475 682b 680a 681b 680c 681c 6803  )].uh+h.h.h.h.h.
+0000f9e0: 681d 682c 681e 4d76 0175 6268 0b29 8194  h.h,h.Mv.ubh.)..
+0000f9f0: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+0000fa00: 947d 9428 6805 8c0b 4469 7665 2044 6565  .}.(h...Dive Dee
+0000fa10: 7065 7294 6807 5d94 6816 8c0b 4469 7665  per.h.].h...Dive
+0000fa20: 2044 6565 7065 7294 8594 8194 7d94 2868   Deeper.....}.(h
+0000fa30: 1b6a 9711 0000 681c 6803 681d 4e68 1e4e  .j....h.h.h.Nh.N
+0000fa40: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+0000fa50: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+0000fa60: 0f68 1b6a 9411 0000 681c 6803 681d 682c  .h.j....h.h.h.h,
+0000fa70: 681e 4d7c 0175 6268 ee29 8194 7d94 2868  h.M|.ubh.)..}.(h
+0000fa80: 058c 8746 6f72 206d 6f72 6520 6164 7661  ...For more adva
+0000fa90: 6e63 6564 2075 7361 6765 2c20 696e 7465  nced usage, inte
+0000faa0: 6772 6174 696f 6e20 6578 616d 706c 6573  gration examples
+0000fab0: 2c20 616e 6420 7469 7073 2074 6f20 7472  , and tips to tr
+0000fac0: 6f75 626c 6573 686f 6f74 2063 6f6d 6d6f  oubleshoot commo
+0000fad0: 6e20 6973 7375 6573 2c20 6469 7665 2064  n issues, dive d
+0000fae0: 6565 7065 7220 696e 2074 6f20 7468 6520  eeper in to the 
+0000faf0: 7265 7374 206f 660a 7468 6520 646f 6375  rest of.the docu
+0000fb00: 6d65 6e74 6174 696f 6e2e 9468 075d 9468  mentation..h.].h
+0000fb10: 168c 8746 6f72 206d 6f72 6520 6164 7661  ...For more adva
+0000fb20: 6e63 6564 2075 7361 6765 2c20 696e 7465  nced usage, inte
+0000fb30: 6772 6174 696f 6e20 6578 616d 706c 6573  gration examples
+0000fb40: 2c20 616e 6420 7469 7073 2074 6f20 7472  , and tips to tr
+0000fb50: 6f75 626c 6573 686f 6f74 2063 6f6d 6d6f  oubleshoot commo
+0000fb60: 6e20 6973 7375 6573 2c20 6469 7665 2064  n issues, dive d
+0000fb70: 6565 7065 7220 696e 2074 6f20 7468 6520  eeper in to the 
+0000fb80: 7265 7374 206f 660a 7468 6520 646f 6375  rest of.the docu
+0000fb90: 6d65 6e74 6174 696f 6e2e 9485 9481 947d  mentation......}
+0000fba0: 9428 681b 6aa5 1100 0068 1c68 0368 1d4e  .(h.j....h.h.h.N
+0000fbb0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+0000fbc0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+0000fbd0: 682b 68ed 681d 682c 681e 4d7e 0168 1b6a  h+h.h.h,h.M~.h.j
+0000fbe0: 9411 0000 681c 6803 7562 6809 8c08 636f  ....h.h.ubh...co
+0000fbf0: 6d70 6f75 6e64 9493 9429 8194 7d94 2868  mpound...)..}.(h
+0000fc00: 0568 0668 075d 9468 008c 0774 6f63 7472  .h.h.].h...toctr
+0000fc10: 6565 9493 9429 8194 7d94 2868 0568 0668  ee...)..}.(h.h.h
+0000fc20: 075d 9468 1f7d 9428 6821 5d94 6823 5d94  .].h.}.(h!].h#].
+0000fc30: 6825 5d94 6827 5d94 6829 5d94 681b 6acf  h%].h'].h)].h.j.
+0000fc40: 0200 008c 0765 6e74 7269 6573 945d 9428  .....entries.].(
+0000fc50: 4e8c 0361 7069 9486 944e 8c0c 696e 7465  N..api...N..inte
+0000fc60: 6772 6174 696f 6e73 9486 944e 8c0f 7472  grations...N..tr
+0000fc70: 6f75 626c 6573 686f 6f74 696e 6794 8694  oubleshooting...
+0000fc80: 658c 0c69 6e63 6c75 6465 6669 6c65 7394  e..includefiles.
+0000fc90: 5d94 286a c511 0000 6ac7 1100 006a c911  ].(j....j....j..
+0000fca0: 0000 658c 086d 6178 6465 7074 6894 4b02  ..e..maxdepth.K.
+0000fcb0: 8c07 6361 7074 696f 6e94 4e8c 0467 6c6f  ..caption.N..glo
+0000fcc0: 6294 898c 0668 6964 6465 6e94 898c 0d69  b....hidden....i
+0000fcd0: 6e63 6c75 6465 6869 6464 656e 9489 8c08  ncludehidden....
+0000fce0: 6e75 6d62 6572 6564 944b 008c 0a74 6974  numbered.K...tit
+0000fcf0: 6c65 736f 6e6c 7994 898c 0a72 6177 656e  lesonly....rawen
+0000fd00: 7472 6965 7394 5d94 7568 2b6a b811 0000  tries.].uh+j....
+0000fd10: 681d 682c 681e 4d81 0168 1b6a b511 0000  h.h,h.M..h.j....
+0000fd20: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+0000fd30: 8c0f 746f 6374 7265 652d 7772 6170 7065  ..toctree-wrappe
+0000fd40: 7294 6168 255d 9468 275d 9468 295d 9475  r.ah%].h'].h)].u
+0000fd50: 682b 6ab3 1100 0068 1b6a 9411 0000 681c  h+j....h.j....h.
+0000fd60: 6803 681d 682c 681e 4e75 6265 681f 7d94  h.h.h,h.Nubeh.}.
+0000fd70: 2868 215d 948c 0b64 6976 652d 6465 6570  (h!]...dive-deep
+0000fd80: 6572 9461 6823 5d94 6825 5d94 8c0b 6469  er.ah#].h%]...di
+0000fd90: 7665 2064 6565 7065 7294 6168 275d 9468  ve deeper.ah'].h
+0000fda0: 295d 9475 682b 680a 681b 680c 681c 6803  )].uh+h.h.h.h.h.
+0000fdb0: 681d 682c 681e 4d7c 0175 6268 0b29 8194  h.h,h.M|.ubh.)..
+0000fdc0: 7d94 2868 0568 0668 075d 9428 6810 2981  }.(h.h.h.].(h.).
+0000fdd0: 947d 9428 6805 8c0c 436f 6e74 7269 6275  .}.(h...Contribu
+0000fde0: 7469 6e67 9468 075d 9468 168c 0c43 6f6e  ting.h.].h...Con
+0000fdf0: 7472 6962 7574 696e 6794 8594 8194 7d94  tributing.....}.
+0000fe00: 2868 1b6a e811 0000 681c 6803 681d 4e68  (h.j....h.h.h.Nh
+0000fe10: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+0000fe20: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+0000fe30: 2b68 0f68 1b6a e511 0000 681c 6803 681d  +h.h.j....h.h.h.
+0000fe40: 8c10 434f 4e54 5249 4255 5449 4e47 2e72  ..CONTRIBUTING.r
+0000fe50: 7374 9468 1e4b 0275 6268 ee29 8194 7d94  st.h.K.ubh.)..}.
+0000fe60: 2868 058c 5c49 6620 796f 7520 6669 6e64  (h..\If you find
+0000fe70: 2069 7373 7565 732c 2060 7265 706f 7274   issues, `report
+0000fe80: 2074 6865 6d20 6f6e 2047 6974 4875 6220   them on GitHub 
+0000fe90: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+0000fea0: 636f 6d2f 616c 6578 646c 6169 7264 2f70  com/alexdlaird/p
+0000feb0: 796e 6772 6f6b 2f69 7373 7565 733e 605f  yngrok/issues>`_
+0000fec0: 2e94 6807 5d94 2868 168c 1449 6620 796f  ..h.].(h...If yo
+0000fed0: 7520 6669 6e64 2069 7373 7565 732c 2094  u find issues, .
+0000fee0: 8594 8194 7d94 2868 1b6a f711 0000 681c  ....}.(h.j....h.
+0000fef0: 6803 681d 4e68 1e4e 7562 6843 2981 947d  h.h.Nh.NubhC)..}
+0000ff00: 9428 6805 8c47 6072 6570 6f72 7420 7468  .(h..G`report th
+0000ff10: 656d 206f 6e20 4769 7448 7562 203c 6874  em on GitHub <ht
+0000ff20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000ff30: 2f61 6c65 7864 6c61 6972 642f 7079 6e67  /alexdlaird/pyng
+0000ff40: 726f 6b2f 6973 7375 6573 3e60 5f94 6807  rok/issues>`_.h.
+0000ff50: 5d94 6816 8c15 7265 706f 7274 2074 6865  ].h...report the
+0000ff60: 6d20 6f6e 2047 6974 4875 6294 8594 8194  m on GitHub.....
+0000ff70: 7d94 2868 1b6a ff11 0000 681c 6803 681d  }.(h.j....h.h.h.
+0000ff80: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+0000ff90: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+0000ffa0: 8c04 6e61 6d65 948c 1572 6570 6f72 7420  ..name...report 
+0000ffb0: 7468 656d 206f 6e20 4769 7448 7562 946a  them on GitHub.j
+0000ffc0: 4501 0000 8c2c 6874 7470 733a 2f2f 6769  E....,https://gi
+0000ffd0: 7468 7562 2e63 6f6d 2f61 6c65 7864 6c61  thub.com/alexdla
+0000ffe0: 6972 642f 7079 6e67 726f 6b2f 6973 7375  ird/pyngrok/issu
+0000fff0: 6573 9475 682b 6842 681b 6af7 1100 0075  es.uh+hBh.j....u
+00010000: 626a 4801 0000 2981 947d 9428 9575 2500  bjH...)..}.(.u%.
+00010010: 0000 0000 0068 058c 2f20 3c68 7474 7073  .....h../ <https
+00010020: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
+00010030: 6578 646c 6169 7264 2f70 796e 6772 6f6b  exdlaird/pyngrok
+00010040: 2f69 7373 7565 733e 9468 075d 9468 1f7d  /issues>.h.].h.}
+00010050: 9428 6821 5d94 8c15 7265 706f 7274 2d74  .(h!]...report-t
+00010060: 6865 6d2d 6f6e 2d67 6974 6875 6294 6168  hem-on-github.ah
+00010070: 235d 9468 255d 948c 1572 6570 6f72 7420  #].h%]...report 
+00010080: 7468 656d 206f 6e20 6769 7468 7562 9461  them on github.a
+00010090: 6827 5d94 6829 5d94 8c06 7265 6675 7269  h'].h)]...refuri
+000100a0: 946a 0f12 0000 7568 2b6a 4701 0000 6a56  .j....uh+jG...jV
+000100b0: 0100 004b 0168 1b6a f711 0000 7562 6816  ...K.h.j....ubh.
+000100c0: 8c01 2e94 8594 8194 7d94 2868 1b6a f711  ........}.(h.j..
+000100d0: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+000100e0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000100f0: 6827 5d94 6829 5d94 7568 2b68 ed68 1d6a  h'].h)].uh+h.h.j
+00010100: f611 0000 681e 4b04 681b 6ae5 1100 0068  ....h.K.h.j....h
+00010110: 1c68 0375 6268 ee29 8194 7d94 2868 058c  .h.ubh.)..}.(h..
+00010120: 4a49 6620 796f 7520 776f 756c 6420 6c69  JIf you would li
+00010130: 6b65 2074 6f20 636f 6e74 7269 6275 7465  ke to contribute
+00010140: 2074 6f20 7468 6520 636f 6465 2c20 7468   to the code, th
+00010150: 6520 7072 6f63 6573 7320 6973 2070 7265  e process is pre
+00010160: 7474 7920 7369 6d70 6c65 3a94 6807 5d94  tty simple:.h.].
+00010170: 6816 8c4a 4966 2079 6f75 2077 6f75 6c64  h..JIf you would
+00010180: 206c 696b 6520 746f 2063 6f6e 7472 6962   like to contrib
+00010190: 7574 6520 746f 2074 6865 2063 6f64 652c  ute to the code,
+000101a0: 2074 6865 2070 726f 6365 7373 2069 7320   the process is 
+000101b0: 7072 6574 7479 2073 696d 706c 653a 9485  pretty simple:..
+000101c0: 9481 947d 9428 681b 6a27 1200 0068 1c68  ...}.(h.j'...h.h
+000101d0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000101e0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000101f0: 295d 9475 682b 68ed 681d 6af6 1100 0068  )].uh+h.h.j....h
+00010200: 1e4b 0668 1b6a e511 0000 681c 6803 7562  .K.h.j....h.h.ub
+00010210: 6809 8c0f 656e 756d 6572 6174 6564 5f6c  h...enumerated_l
+00010220: 6973 7494 9394 2981 947d 9428 6805 6806  ist...)..}.(h.h.
+00010230: 6807 5d94 2868 098c 096c 6973 745f 6974  h.].(h...list_it
+00010240: 656d 9493 9429 8194 7d94 2868 058c bd46  em...)..}.(h...F
+00010250: 616d 696c 6961 7269 7365 2079 6f75 7273  amiliarise yours
+00010260: 656c 6620 7769 7468 2074 6869 7320 7061  elf with this pa
+00010270: 636b 6167 652c 2060 7079 6e67 726f 6b27  ckage, `pyngrok'
+00010280: 7320 4150 4973 203c 6874 7470 733a 2f2f  s APIs <https://
+00010290: 7079 6e67 726f 6b2e 7265 6164 7468 6564  pyngrok.readthed
+000102a0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000102b0: 2f61 7069 2e68 746d 6c3e 605f 2061 6e64  /api.html>`_ and
+000102c0: 206f 7468 6572 2064 6f63 756d 656e 7461   other documenta
+000102d0: 7469 6f6e 2c20 616e 6420 606e 6772 6f6b  tion, and `ngrok
+000102e0: 2773 2064 6f63 756d 656e 7461 7469 6f6e  's documentation
+000102f0: 203c 6874 7470 733a 2f2f 6e67 726f 6b2e   <https://ngrok.
+00010300: 636f 6d2f 646f 6373 3e60 5f2e 9468 075d  com/docs>`_..h.]
+00010310: 9468 ee29 8194 7d94 2868 056a 3e12 0000  .h.)..}.(h.j>...
+00010320: 6807 5d94 2868 168c 2846 616d 696c 6961  h.].(h..(Familia
+00010330: 7269 7365 2079 6f75 7273 656c 6620 7769  rise yourself wi
+00010340: 7468 2074 6869 7320 7061 636b 6167 652c  th this package,
+00010350: 2094 8594 8194 7d94 2868 1b6a 4012 0000   .....}.(h.j@...
+00010360: 681c 6803 681d 4e68 1e4e 7562 6843 2981  h.h.h.Nh.NubhC).
+00010370: 947d 9428 6805 8c45 6070 796e 6772 6f6b  .}.(h..E`pyngrok
+00010380: 2773 2041 5049 7320 3c68 7474 7073 3a2f  's APIs <https:/
+00010390: 2f70 796e 6772 6f6b 2e72 6561 6474 6865  /pyngrok.readthe
+000103a0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+000103b0: 742f 6170 692e 6874 6d6c 3e60 5f94 6807  t/api.html>`_.h.
+000103c0: 5d94 6816 8c10 7079 6e67 726f 6be2 8099  ].h...pyngrok...
+000103d0: 7320 4150 4973 9485 9481 947d 9428 681b  s APIs.....}.(h.
+000103e0: 6a47 1200 0068 1c68 0368 1d4e 681e 4e75  jG...h.h.h.Nh.Nu
+000103f0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00010400: 255d 9468 275d 9468 295d 948c 046e 616d  %].h'].h)]...nam
+00010410: 6594 8c0e 7079 6e67 726f 6b27 7320 4150  e...pyngrok's AP
+00010420: 4973 946a 4501 0000 8c31 6874 7470 733a  Is.jE....1https:
+00010430: 2f2f 7079 6e67 726f 6b2e 7265 6164 7468  //pyngrok.readth
+00010440: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00010450: 7374 2f61 7069 2e68 746d 6c94 7568 2b68  st/api.html.uh+h
+00010460: 4268 1b6a 4012 0000 7562 6a48 0100 0029  Bh.j@...ubjH...)
+00010470: 8194 7d94 2868 058c 3420 3c68 7474 7073  ..}.(h..4 <https
+00010480: 3a2f 2f70 796e 6772 6f6b 2e72 6561 6474  ://pyngrok.readt
+00010490: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+000104a0: 6573 742f 6170 692e 6874 6d6c 3e94 6807  est/api.html>.h.
+000104b0: 5d94 681f 7d94 2868 215d 948c 0e70 796e  ].h.}.(h!]...pyn
+000104c0: 6772 6f6b 2d73 2d61 7069 7394 6168 235d  grok-s-apis.ah#]
+000104d0: 9468 255d 948c 0e70 796e 6772 6f6b 2773  .h%]...pyngrok's
+000104e0: 2061 7069 7394 6168 275d 9468 295d 948c   apis.ah'].h)]..
+000104f0: 0672 6566 7572 6994 6a57 1200 0075 682b  .refuri.jW...uh+
+00010500: 6a47 0100 006a 5601 0000 4b01 681b 6a40  jG...jV...K.h.j@
+00010510: 1200 0075 6268 168c 1e20 616e 6420 6f74  ...ubh... and ot
+00010520: 6865 7220 646f 6375 6d65 6e74 6174 696f  her documentatio
+00010530: 6e2c 2061 6e64 2094 8594 8194 7d94 2868  n, and .....}.(h
+00010540: 1b6a 4012 0000 681c 6803 681d 4e68 1e4e  .j@...h.h.h.Nh.N
+00010550: 7562 6843 2981 947d 9428 6805 8c31 606e  ubhC)..}.(h..1`n
+00010560: 6772 6f6b 2773 2064 6f63 756d 656e 7461  grok's documenta
+00010570: 7469 6f6e 203c 6874 7470 733a 2f2f 6e67  tion <https://ng
+00010580: 726f 6b2e 636f 6d2f 646f 6373 3e60 5f94  rok.com/docs>`_.
+00010590: 6807 5d94 6816 8c17 6e67 726f 6be2 8099  h.].h...ngrok...
+000105a0: 7320 646f 6375 6d65 6e74 6174 696f 6e94  s documentation.
+000105b0: 8594 8194 7d94 2868 1b6a 6912 0000 681c  ....}.(h.ji...h.
+000105c0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000105d0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000105e0: 6829 5d94 8c04 6e61 6d65 948c 156e 6772  h)]...name...ngr
+000105f0: 6f6b 2773 2064 6f63 756d 656e 7461 7469  ok's documentati
+00010600: 6f6e 946a 4501 0000 8c16 6874 7470 733a  on.jE.....https:
+00010610: 2f2f 6e67 726f 6b2e 636f 6d2f 646f 6373  //ngrok.com/docs
+00010620: 9475 682b 6842 681b 6a40 1200 0075 626a  .uh+hBh.j@...ubj
+00010630: 4801 0000 2981 947d 9428 6805 8c19 203c  H...)..}.(h... <
+00010640: 6874 7470 733a 2f2f 6e67 726f 6b2e 636f  https://ngrok.co
+00010650: 6d2f 646f 6373 3e94 6807 5d94 681f 7d94  m/docs>.h.].h.}.
+00010660: 2868 215d 948c 156e 6772 6f6b 2d73 2d64  (h!]...ngrok-s-d
+00010670: 6f63 756d 656e 7461 7469 6f6e 9461 6823  ocumentation.ah#
+00010680: 5d94 6825 5d94 8c15 6e67 726f 6b27 7320  ].h%]...ngrok's 
+00010690: 646f 6375 6d65 6e74 6174 696f 6e94 6168  documentation.ah
+000106a0: 275d 9468 295d 948c 0672 6566 7572 6994  '].h)]...refuri.
+000106b0: 6a79 1200 0075 682b 6a47 0100 006a 5601  jy...uh+jG...jV.
+000106c0: 0000 4b01 681b 6a40 1200 0075 6268 168c  ..K.h.j@...ubh..
+000106d0: 012e 9485 9481 947d 9428 681b 6a40 1200  .......}.(h.j@..
+000106e0: 0068 1c68 0368 1d4e 681e 4e75 6265 681f  .h.h.h.Nh.Nubeh.
+000106f0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00010700: 275d 9468 295d 9475 682b 68ed 681d 6af6  '].h)].uh+h.h.j.
+00010710: 1100 0068 1e4b 0868 1b6a 3c12 0000 7562  ...h.K.h.j<...ub
+00010720: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00010730: 5d94 6827 5d94 6829 5d94 7568 2b6a 3a12  ].h'].h)].uh+j:.
+00010740: 0000 681b 6a37 1200 0068 1c68 0368 1d6a  ..h.j7...h.h.h.j
+00010750: f611 0000 681e 4e75 626a 3b12 0000 2981  ....h.Nubj;...).
+00010760: 947d 9428 6805 8c68 466f 726b 2060 7468  .}.(h..hFork `th
+00010770: 6520 7265 706f 7369 746f 7279 206f 6e20  e repository on 
+00010780: 4769 7448 7562 203c 6874 7470 733a 2f2f  GitHub <https://
+00010790: 6769 7468 7562 2e63 6f6d 2f61 6c65 7864  github.com/alexd
+000107a0: 6c61 6972 642f 7079 6e67 726f 6b3e 605f  laird/pyngrok>`_
+000107b0: 2061 6e64 2073 7461 7274 2069 6d70 6c65   and start imple
+000107c0: 6d65 6e74 696e 6720 6368 616e 6765 732e  menting changes.
+000107d0: 9468 075d 9468 ee29 8194 7d94 2868 056a  .h.].h.)..}.(h.j
+000107e0: 9912 0000 6807 5d94 2868 168c 0546 6f72  ....h.].(h...For
+000107f0: 6b20 9485 9481 947d 9428 681b 6a9b 1200  k .....}.(h.j...
+00010800: 0068 1c68 0368 1d4e 681e 4e75 6268 4329  .h.h.h.Nh.NubhC)
+00010810: 8194 7d94 2868 058c 4360 7468 6520 7265  ..}.(h..C`the re
+00010820: 706f 7369 746f 7279 206f 6e20 4769 7448  pository on GitH
+00010830: 7562 203c 6874 7470 733a 2f2f 6769 7468  ub <https://gith
+00010840: 7562 2e63 6f6d 2f61 6c65 7864 6c61 6972  ub.com/alexdlair
+00010850: 642f 7079 6e67 726f 6b3e 605f 9468 075d  d/pyngrok>`_.h.]
+00010860: 9468 168c 1874 6865 2072 6570 6f73 6974  .h...the reposit
+00010870: 6f72 7920 6f6e 2047 6974 4875 6294 8594  ory on GitHub...
+00010880: 8194 7d94 2868 1b6a a212 0000 681c 6803  ..}.(h.j....h.h.
+00010890: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+000108a0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+000108b0: 5d94 8c04 6e61 6d65 948c 1874 6865 2072  ]...name...the r
+000108c0: 6570 6f73 6974 6f72 7920 6f6e 2047 6974  epository on Git
+000108d0: 4875 6294 6a45 0100 008c 2568 7474 7073  Hub.jE....%https
+000108e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
+000108f0: 6578 646c 6169 7264 2f70 796e 6772 6f6b  exdlaird/pyngrok
+00010900: 9475 682b 6842 681b 6a9b 1200 0075 626a  .uh+hBh.j....ubj
+00010910: 4801 0000 2981 947d 9428 6805 8c28 203c  H...)..}.(h..( <
+00010920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00010930: 6f6d 2f61 6c65 7864 6c61 6972 642f 7079  om/alexdlaird/py
+00010940: 6e67 726f 6b3e 9468 075d 9468 1f7d 9428  ngrok>.h.].h.}.(
+00010950: 6821 5d94 8c18 7468 652d 7265 706f 7369  h!]...the-reposi
+00010960: 746f 7279 2d6f 6e2d 6769 7468 7562 9461  tory-on-github.a
+00010970: 6823 5d94 6825 5d94 8c18 7468 6520 7265  h#].h%]...the re
+00010980: 706f 7369 746f 7279 206f 6e20 6769 7468  pository on gith
+00010990: 7562 9461 6827 5d94 6829 5d94 8c06 7265  ub.ah'].h)]...re
+000109a0: 6675 7269 946a b212 0000 7568 2b6a 4701  furi.j....uh+jG.
+000109b0: 0000 6a56 0100 004b 0168 1b6a 9b12 0000  ..jV...K.h.j....
+000109c0: 7562 6816 8c20 2061 6e64 2073 7461 7274  ubh..  and start
+000109d0: 2069 6d70 6c65 6d65 6e74 696e 6720 6368   implementing ch
+000109e0: 616e 6765 732e 9485 9481 947d 9428 681b  anges......}.(h.
+000109f0: 6a9b 1200 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00010a00: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00010a10: 255d 9468 275d 9468 295d 9475 682b 68ed  %].h'].h)].uh+h.
+00010a20: 681d 6af6 1100 0068 1e4b 0968 1b6a 9712  h.j....h.K.h.j..
+00010a30: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+00010a40: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00010a50: 2b6a 3a12 0000 681b 6a37 1200 0068 1c68  +j:...h.j7...h.h
+00010a60: 0368 1d6a f611 0000 681e 4e75 626a 3b12  .h.j....h.Nubj;.
+00010a70: 0000 2981 947d 9428 6805 8c35 5772 6974  ..)..}.(h..5Writ
+00010a80: 6520 6120 7465 7374 2074 6861 7420 706c  e a test that pl
+00010a90: 6169 6e6c 7920 7661 6c69 6461 7465 7320  ainly validates 
+00010aa0: 7468 6520 6368 616e 6765 7320 6d61 6465  the changes made
+00010ab0: 2e94 6807 5d94 68ee 2981 947d 9428 6805  ..h.].h.)..}.(h.
+00010ac0: 6ad2 1200 0068 075d 9468 168c 3557 7269  j....h.].h..5Wri
+00010ad0: 7465 2061 2074 6573 7420 7468 6174 2070  te a test that p
+00010ae0: 6c61 696e 6c79 2076 616c 6964 6174 6573  lainly validates
+00010af0: 2074 6865 2063 6861 6e67 6573 206d 6164   the changes mad
+00010b00: 652e 9485 9481 947d 9428 681b 6ad4 1200  e......}.(h.j...
+00010b10: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00010b20: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00010b30: 275d 9468 295d 9475 682b 68ed 681d 6af6  '].h)].uh+h.h.j.
+00010b40: 1100 0068 1e4b 0a68 1b6a d012 0000 7562  ...h.K.h.j....ub
+00010b50: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00010b60: 5d94 6827 5d94 6829 5d94 7568 2b6a 3a12  ].h'].h)].uh+j:.
+00010b70: 0000 681b 6a37 1200 0068 1c68 0368 1d6a  ..h.j7...h.h.h.j
+00010b80: f611 0000 681e 4e75 626a 3b12 0000 2981  ....h.Nubj;...).
+00010b90: 947d 9428 6805 8c2f 4275 696c 6420 616e  .}.(h../Build an
+00010ba0: 6420 7465 7374 206c 6f63 616c 6c79 2077  d test locally w
+00010bb0: 6974 6820 6060 6d61 6b65 206c 6f63 616c  ith ``make local
+00010bc0: 2074 6573 7460 6094 6807 5d94 68ee 2981   test``.h.].h.).
+00010bd0: 947d 9428 6805 6ae9 1200 0068 075d 9428  .}.(h.j....h.].(
+00010be0: 6816 8c1c 4275 696c 6420 616e 6420 7465  h...Build and te
+00010bf0: 7374 206c 6f63 616c 6c79 2077 6974 6820  st locally with 
+00010c00: 9485 9481 947d 9428 681b 6aeb 1200 0068  .....}.(h.j....h
+00010c10: 1c68 0368 1d4e 681e 4e75 6268 f429 8194  .h.h.Nh.Nubh.)..
+00010c20: 7d94 2868 058c 1360 606d 616b 6520 6c6f  }.(h...``make lo
+00010c30: 6361 6c20 7465 7374 6060 9468 075d 9468  cal test``.h.].h
+00010c40: 168c 0f6d 616b 6520 6c6f 6361 6c20 7465  ...make local te
+00010c50: 7374 9485 9481 947d 9428 681b 6af2 1200  st.....}.(h.j...
+00010c60: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00010c70: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00010c80: 275d 9468 295d 9475 682b 68f3 681b 6aeb  '].h)].uh+h.h.j.
+00010c90: 1200 0075 6265 681f 7d94 2868 215d 9468  ...ubeh.}.(h!].h
+00010ca0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00010cb0: 682b 68ed 681d 6af6 1100 0068 1e4b 0b68  h+h.h.j....h.K.h
+00010cc0: 1b6a e712 0000 7562 6168 1f7d 9428 6821  .j....ubah.}.(h!
+00010cd0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00010ce0: 5d94 7568 2b6a 3a12 0000 681b 6a37 1200  ].uh+j:...h.j7..
+00010cf0: 0068 1c68 0368 1d6a f611 0000 681e 4e75  .h.h.h.j....h.Nu
+00010d00: 626a 3b12 0000 2981 947d 9428 6805 8c7f  bj;...)..}.(h...
+00010d10: 5375 626d 6974 2061 2060 7075 6c6c 2072  Submit a `pull r
+00010d20: 6571 7565 7374 7320 3c68 7474 7073 3a2f  equests <https:/
+00010d30: 2f68 656c 702e 6769 7468 7562 2e63 6f6d  /help.github.com
+00010d40: 2f65 6e2f 6172 7469 636c 6573 2f63 7265  /en/articles/cre
+00010d50: 6174 696e 672d 612d 7075 6c6c 2d72 6571  ating-a-pull-req
+00010d60: 7565 7374 2d66 726f 6d2d 612d 666f 726b  uest-from-a-fork
+00010d70: 3e60 5f20 746f 2067 6574 2074 6865 2063  >`_ to get the c
+00010d80: 6861 6e67 6573 206d 6572 6765 642e 0a94  hanges merged...
+00010d90: 6807 5d94 68ee 2981 947d 9428 6805 8c7e  h.].h.)..}.(h..~
+00010da0: 5375 626d 6974 2061 2060 7075 6c6c 2072  Submit a `pull r
+00010db0: 6571 7565 7374 7320 3c68 7474 7073 3a2f  equests <https:/
+00010dc0: 2f68 656c 702e 6769 7468 7562 2e63 6f6d  /help.github.com
+00010dd0: 2f65 6e2f 6172 7469 636c 6573 2f63 7265  /en/articles/cre
+00010de0: 6174 696e 672d 612d 7075 6c6c 2d72 6571  ating-a-pull-req
+00010df0: 7565 7374 2d66 726f 6d2d 612d 666f 726b  uest-from-a-fork
+00010e00: 3e60 5f20 746f 2067 6574 2074 6865 2063  >`_ to get the c
+00010e10: 6861 6e67 6573 206d 6572 6765 642e 9468  hanges merged..h
+00010e20: 075d 9428 6816 8c09 5375 626d 6974 2061  .].(h...Submit a
+00010e30: 2094 8594 8194 7d94 2868 1b6a 1013 0000   .....}.(h.j....
+00010e40: 681c 6803 681d 4e68 1e4e 7562 6843 2981  h.h.h.Nh.NubhC).
+00010e50: 947d 9428 6805 8c5a 6070 756c 6c20 7265  .}.(h..Z`pull re
+00010e60: 7175 6573 7473 203c 6874 7470 733a 2f2f  quests <https://
+00010e70: 6865 6c70 2e67 6974 6875 622e 636f 6d2f  help.github.com/
+00010e80: 656e 2f61 7274 6963 6c65 732f 6372 6561  en/articles/crea
+00010e90: 7469 6e67 2d61 2d70 756c 6c2d 7265 7175  ting-a-pull-requ
+00010ea0: 6573 742d 6672 6f6d 2d61 2d66 6f72 6b3e  est-from-a-fork>
+00010eb0: 605f 9468 075d 9468 168c 0d70 756c 6c20  `_.h.].h...pull 
+00010ec0: 7265 7175 6573 7473 9485 9481 947d 9428  requests.....}.(
+00010ed0: 681b 6a18 1300 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+00010ee0: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00010ef0: 9468 255d 9468 275d 9468 295d 948c 046e  .h%].h'].h)]...n
+00010f00: 616d 6594 8c0d 7075 6c6c 2072 6571 7565  ame...pull reque
+00010f10: 7374 7394 6a45 0100 008c 4768 7474 7073  sts.jE....Ghttps
+00010f20: 3a2f 2f68 656c 702e 6769 7468 7562 2e63  ://help.github.c
+00010f30: 6f6d 2f65 6e2f 6172 7469 636c 6573 2f63  om/en/articles/c
+00010f40: 7265 6174 696e 672d 612d 7075 6c6c 2d72  reating-a-pull-r
+00010f50: 6571 7565 7374 2d66 726f 6d2d 612d 666f  equest-from-a-fo
+00010f60: 726b 9475 682b 6842 681b 6a10 1300 0075  rk.uh+hBh.j....u
+00010f70: 626a 4801 0000 2981 947d 9428 6805 8c4a  bjH...)..}.(h..J
+00010f80: 203c 6874 7470 733a 2f2f 6865 6c70 2e67   <https://help.g
+00010f90: 6974 6875 622e 636f 6d2f 656e 2f61 7274  ithub.com/en/art
+00010fa0: 6963 6c65 732f 6372 6561 7469 6e67 2d61  icles/creating-a
+00010fb0: 2d70 756c 6c2d 7265 7175 6573 742d 6672  -pull-request-fr
+00010fc0: 6f6d 2d61 2d66 6f72 6b3e 9468 075d 9468  om-a-fork>.h.].h
+00010fd0: 1f7d 9428 6821 5d94 8c0d 7075 6c6c 2d72  .}.(h!]...pull-r
+00010fe0: 6571 7565 7374 7394 6168 235d 9468 255d  equests.ah#].h%]
+00010ff0: 948c 0d70 756c 6c20 7265 7175 6573 7473  ...pull requests
+00011000: 9461 6827 5d94 6829 5d94 8c06 7265 6675  .ah'].h)]...refu
+00011010: 7269 946a 2813 0000 7568 2b6a 4701 0000  ri.j(...uh+jG...
+00011020: 6a56 0100 004b 0168 1b6a 1013 0000 7562  jV...K.h.j....ub
+00011030: 6816 8c1b 2074 6f20 6765 7420 7468 6520  h... to get the 
+00011040: 6368 616e 6765 7320 6d65 7267 6564 2e94  changes merged..
+00011050: 8594 8194 7d94 2868 1b6a 1013 0000 681c  ....}.(h.j....h.
+00011060: 6803 681d 4e68 1e4e 7562 6568 1f7d 9428  h.h.Nh.Nubeh.}.(
+00011070: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00011080: 6829 5d94 7568 2b68 ed68 1d6a f611 0000  h)].uh+h.h.j....
+00011090: 681e 4b0c 681b 6a0c 1300 0075 6261 681f  h.K.h.j....ubah.
+000110a0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+000110b0: 275d 9468 295d 9475 682b 6a3a 1200 0068  '].h)].uh+j:...h
+000110c0: 1b6a 3712 0000 681c 6803 681d 6af6 1100  .j7...h.h.h.j...
+000110d0: 0068 1e4e 7562 6568 1f7d 9428 6821 5d94  .h.Nubeh.}.(h!].
+000110e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000110f0: 8c08 656e 756d 7479 7065 948c 0661 7261  ..enumtype...ara
+00011100: 6269 6394 8c06 7072 6566 6978 9468 068c  bic...prefix.h..
+00011110: 0673 7566 6669 7894 8c01 2e94 7568 2b6a  .suffix.....uh+j
+00011120: 3512 0000 681b 6ae5 1100 0068 1c68 0368  5...h.j....h.h.h
+00011130: 1d6a f611 0000 681e 4b08 7562 68ee 2981  .j....h.K.ubh.).
+00011140: 947d 9428 6805 8c9d 416c 736f 2062 6520  .}.(h...Also be 
+00011150: 7375 7265 2074 6f20 7265 7669 6577 2074  sure to review t
+00011160: 6865 2060 436f 6465 206f 6620 436f 6e64  he `Code of Cond
+00011170: 7563 7420 3c68 7474 7073 3a2f 2f67 6974  uct <https://git
+00011180: 6875 622e 636f 6d2f 616c 6578 646c 6169  hub.com/alexdlai
+00011190: 7264 2f70 796e 6772 6f6b 2f62 6c6f 622f  rd/pyngrok/blob/
+000111a0: 6d61 696e 2f43 4f44 455f 4f46 5f43 4f4e  main/CODE_OF_CON
+000111b0: 4455 4354 2e6d 643e 605f 2062 6566 6f72  DUCT.md>`_ befor
+000111c0: 650a 7375 626d 6974 7469 6e67 2069 7373  e.submitting iss
+000111d0: 7565 7320 6f72 2070 756c 6c20 7265 7175  ues or pull requ
+000111e0: 6573 7473 2e94 6807 5d94 2868 168c 1b41  ests..h.].(h...A
+000111f0: 6c73 6f20 6265 2073 7572 6520 746f 2072  lso be sure to r
+00011200: 6576 6965 7720 7468 6520 9485 9481 947d  eview the .....}
+00011210: 9428 681b 6a51 1300 0068 1c68 0368 1d4e  .(h.jQ...h.h.h.N
+00011220: 681e 4e75 6268 4329 8194 7d94 2868 058c  h.NubhC)..}.(h..
+00011230: 5760 436f 6465 206f 6620 436f 6e64 7563  W`Code of Conduc
+00011240: 7420 3c68 7474 7073 3a2f 2f67 6974 6875  t <https://githu
+00011250: 622e 636f 6d2f 616c 6578 646c 6169 7264  b.com/alexdlaird
+00011260: 2f70 796e 6772 6f6b 2f62 6c6f 622f 6d61  /pyngrok/blob/ma
+00011270: 696e 2f43 4f44 455f 4f46 5f43 4f4e 4455  in/CODE_OF_CONDU
+00011280: 4354 2e6d 643e 605f 9468 075d 9468 168c  CT.md>`_.h.].h..
+00011290: 0f43 6f64 6520 6f66 2043 6f6e 6475 6374  .Code of Conduct
+000112a0: 9485 9481 947d 9428 681b 6a59 1300 0068  .....}.(h.jY...h
+000112b0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000112c0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000112d0: 9468 295d 948c 046e 616d 6594 8c0f 436f  .h)]...name...Co
+000112e0: 6465 206f 6620 436f 6e64 7563 7494 6a45  de of Conduct.jE
+000112f0: 0100 008c 4268 7474 7073 3a2f 2f67 6974  ....Bhttps://git
+00011300: 6875 622e 636f 6d2f 616c 6578 646c 6169  hub.com/alexdlai
+00011310: 7264 2f70 796e 6772 6f6b 2f62 6c6f 622f  rd/pyngrok/blob/
+00011320: 6d61 696e 2f43 4f44 455f 4f46 5f43 4f4e  main/CODE_OF_CON
+00011330: 4455 4354 2e6d 6494 7568 2b68 4268 1b6a  DUCT.md.uh+hBh.j
+00011340: 5113 0000 7562 6a48 0100 0029 8194 7d94  Q...ubjH...)..}.
+00011350: 2868 058c 4520 3c68 7474 7073 3a2f 2f67  (h..E <https://g
+00011360: 6974 6875 622e 636f 6d2f 616c 6578 646c  ithub.com/alexdl
+00011370: 6169 7264 2f70 796e 6772 6f6b 2f62 6c6f  aird/pyngrok/blo
+00011380: 622f 6d61 696e 2f43 4f44 455f 4f46 5f43  b/main/CODE_OF_C
+00011390: 4f4e 4455 4354 2e6d 643e 9468 075d 9468  ONDUCT.md>.h.].h
+000113a0: 1f7d 9428 6821 5d94 8c0f 636f 6465 2d6f  .}.(h!]...code-o
+000113b0: 662d 636f 6e64 7563 7494 6168 235d 9468  f-conduct.ah#].h
+000113c0: 255d 948c 0f63 6f64 6520 6f66 2063 6f6e  %]...code of con
+000113d0: 6475 6374 9461 6827 5d94 6829 5d94 8c06  duct.ah'].h)]...
+000113e0: 7265 6675 7269 946a 6913 0000 7568 2b6a  refuri.ji...uh+j
+000113f0: 4701 0000 6a56 0100 004b 0168 1b6a 5113  G...jV...K.h.jQ.
+00011400: 0000 7562 6816 8c2b 2062 6566 6f72 650a  ..ubh..+ before.
+00011410: 7375 626d 6974 7469 6e67 2069 7373 7565  submitting issue
+00011420: 7320 6f72 2070 756c 6c20 7265 7175 6573  s or pull reques
+00011430: 7473 2e94 8594 8194 7d94 2868 1b6a 5113  ts......}.(h.jQ.
+00011440: 0000 681c 6803 681d 4e68 1e4e 7562 6568  ..h.h.h.Nh.Nubeh
+00011450: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00011460: 6827 5d94 6829 5d94 7568 2b68 ed68 1d6a  h'].h)].uh+h.h.j
+00011470: f611 0000 681e 4b0e 681b 6ae5 1100 0068  ....h.K.h.j....h
+00011480: 1c68 0375 6268 ee29 8194 7d94 2868 058c  .h.ubh.)..}.(h..
+00011490: 9757 616e 7420 746f 2063 6f6e 7472 6962  .Want to contrib
+000114a0: 7574 6520 6669 6e61 6e63 6961 6c6c 793f  ute financially?
+000114b0: 2049 6620 796f 7527 7665 2066 6f75 6e64   If you've found
+000114c0: 2060 6070 796e 6772 6f6b 6060 2075 7365   ``pyngrok`` use
+000114d0: 6675 6c2c 2060 6120 646f 6e61 7469 6f6e  ful, `a donation
+000114e0: 203c 6874 7470 733a 2f2f 7777 772e 7061   <https://www.pa
+000114f0: 7970 616c 2e6d 652f 616c 6578 646c 6169  ypal.me/alexdlai
+00011500: 7264 3e60 5f0a 776f 756c 6420 616c 736f  rd>`_.would also
+00011510: 2062 6520 6772 6561 746c 7920 6170 7072   be greatly appr
+00011520: 6563 6961 7465 6421 9468 075d 9428 6816  eciated!.h.].(h.
+00011530: 8c32 5761 6e74 2074 6f20 636f 6e74 7269  .2Want to contri
+00011540: 6275 7465 2066 696e 616e 6369 616c 6c79  bute financially
+00011550: 3f20 4966 2079 6f75 e280 9976 6520 666f  ? If you...ve fo
+00011560: 756e 6420 9485 9481 947d 9428 681b 6a81  und .....}.(h.j.
+00011570: 1300 0068 1c68 0368 1d4e 681e 4e75 6268  ...h.h.h.Nh.Nubh
+00011580: f429 8194 7d94 2868 058c 0b60 6070 796e  .)..}.(h...``pyn
+00011590: 6772 6f6b 6060 9468 075d 9468 168c 0770  grok``.h.].h...p
+000115a0: 796e 6772 6f6b 9485 9481 947d 9428 681b  yngrok.....}.(h.
+000115b0: 6a89 1300 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+000115c0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000115d0: 255d 9468 275d 9468 295d 9475 682b 68f3  %].h'].h)].uh+h.
+000115e0: 681b 6a81 1300 0075 6268 168c 0920 7573  h.j....ubh... us
+000115f0: 6566 756c 2c20 9485 9481 947d 9428 681b  eful, .....}.(h.
+00011600: 6a81 1300 0068 1c68 0368 1d4e 681e 4e75  j....h.h.h.Nh.Nu
+00011610: 6268 4329 8194 7d94 2868 058c 3060 6120  bhC)..}.(h..0`a 
+00011620: 646f 6e61 7469 6f6e 203c 6874 7470 733a  donation <https:
+00011630: 2f2f 7777 772e 7061 7970 616c 2e6d 652f  //www.paypal.me/
+00011640: 616c 6578 646c 6169 7264 3e60 5f94 6807  alexdlaird>`_.h.
+00011650: 5d94 6816 8c0a 6120 646f 6e61 7469 6f6e  ].h...a donation
+00011660: 9485 9481 947d 9428 681b 6a9b 1300 0068  .....}.(h.j....h
+00011670: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+00011680: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00011690: 9468 295d 948c 046e 616d 6594 8c0a 6120  .h)]...name...a 
+000116a0: 646f 6e61 7469 6f6e 946a 4501 0000 8c20  donation.jE.... 
+000116b0: 6874 7470 733a 2f2f 7777 772e 7061 7970  https://www.payp
+000116c0: 616c 2e6d 652f 616c 6578 646c 6169 7264  al.me/alexdlaird
+000116d0: 9475 682b 6842 681b 6a81 1300 0075 626a  .uh+hBh.j....ubj
+000116e0: 4801 0000 2981 947d 9428 6805 8c23 203c  H...)..}.(h..# <
+000116f0: 6874 7470 733a 2f2f 7777 772e 7061 7970  https://www.payp
+00011700: 616c 2e6d 652f 616c 6578 646c 6169 7264  al.me/alexdlaird
+00011710: 3e94 6807 5d94 681f 7d94 2868 215d 948c  >.h.].h.}.(h!]..
+00011720: 0a61 2d64 6f6e 6174 696f 6e94 6168 235d  .a-donation.ah#]
+00011730: 9468 255d 948c 0a61 2064 6f6e 6174 696f  .h%]...a donatio
+00011740: 6e94 6168 275d 9468 295d 948c 0672 6566  n.ah'].h)]...ref
+00011750: 7572 6994 6aab 1300 0075 682b 6a47 0100  uri.j....uh+jG..
+00011760: 006a 5601 0000 4b01 681b 6a81 1300 0075  .jV...K.h.j....u
+00011770: 6268 168c 230a 776f 756c 6420 616c 736f  bh..#.would also
+00011780: 2062 6520 6772 6561 746c 7920 6170 7072   be greatly appr
+00011790: 6563 6961 7465 6421 9485 9481 947d 9428  eciated!.....}.(
+000117a0: 681b 6a81 1300 0068 1c68 0368 1d4e 681e  h.j....h.h.h.Nh.
+000117b0: 4e75 6265 681f 7d94 2868 215d 9468 235d  Nubeh.}.(h!].h#]
+000117c0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000117d0: 68ed 681d 6af6 1100 0068 1e4b 1168 1b6a  h.h.j....h.K.h.j
+000117e0: e511 0000 681c 6803 7562 6568 1f7d 9428  ....h.h.ubeh.}.(
+000117f0: 6821 5d94 8c0c 636f 6e74 7269 6275 7469  h!]...contributi
+00011800: 6e67 9461 6823 5d94 6825 5d94 8c0c 636f  ng.ah#].h%]...co
+00011810: 6e74 7269 6275 7469 6e67 9461 6827 5d94  ntributing.ah'].
+00011820: 6829 5d94 7568 2b68 0a68 1b68 0c68 1c68  h)].uh+h.h.h.h.h
+00011830: 0368 1d6a f611 0000 681e 4b02 7562 6568  .h.j....h.K.ubeh
+00011840: 1f7d 9428 6821 5d94 8c22 7079 6e67 726f  .}.(h!].."pyngro
+00011850: 6b2d 612d 7079 7468 6f6e 2d77 7261 7070  k-a-python-wrapp
+00011860: 6572 2d66 6f72 2d6e 6772 6f6b 9461 6823  er-for-ngrok.ah#
+00011870: 5d94 8c0b 6869 6465 2d68 6561 6465 7294  ]...hide-header.
+00011880: 6168 255d 948c 2470 796e 6772 6f6b 202d  ah%]..$pyngrok -
+00011890: 2061 2070 7974 686f 6e20 7772 6170 7065   a python wrappe
+000118a0: 7220 666f 7220 6e67 726f 6b94 6168 275d  r for ngrok.ah']
+000118b0: 9468 295d 9475 682b 680a 681b 6803 681c  .h)].uh+h.h.h.h.
+000118c0: 6803 681d 682c 681e 4b05 7562 6168 1f7d  h.h.h,h.K.ubah.}
+000118d0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000118e0: 5d94 6829 5d94 8c06 736f 7572 6365 9468  ].h)]...source.h
+000118f0: 2c75 682b 6801 8c0e 6375 7272 656e 745f  ,uh+h...current_
+00011900: 736f 7572 6365 944e 8c0c 6375 7272 656e  source.N..curren
+00011910: 745f 6c69 6e65 944e 8c08 7365 7474 696e  t_line.N..settin
+00011920: 6773 948c 1164 6f63 7574 696c 732e 6672  gs...docutils.fr
+00011930: 6f6e 7465 6e64 948c 0656 616c 7565 7394  ontend...Values.
+00011940: 9394 2981 947d 9428 680f 4e8c 0967 656e  ..)..}.(h.N..gen
+00011950: 6572 6174 6f72 944e 8c09 6461 7465 7374  erator.N..datest
+00011960: 616d 7094 4e8c 0b73 6f75 7263 655f 6c69  amp.N..source_li
+00011970: 6e6b 944e 8c0a 736f 7572 6365 5f75 726c  nk.N..source_url
+00011980: 944e 8c0d 746f 635f 6261 636b 6c69 6e6b  .N..toc_backlink
+00011990: 7394 8c05 656e 7472 7994 8c12 666f 6f74  s...entry...foot
+000119a0: 6e6f 7465 5f62 6163 6b6c 696e 6b73 944b  note_backlinks.K
+000119b0: 018c 0d73 6563 746e 756d 5f78 666f 726d  ...sectnum_xform
+000119c0: 944b 018c 0e73 7472 6970 5f63 6f6d 6d65  .K...strip_comme
+000119d0: 6e74 7394 4e8c 1b73 7472 6970 5f65 6c65  nts.N..strip_ele
+000119e0: 6d65 6e74 735f 7769 7468 5f63 6c61 7373  ments_with_class
+000119f0: 6573 944e 8c0d 7374 7269 705f 636c 6173  es.N..strip_clas
+00011a00: 7365 7394 4e8c 0c72 6570 6f72 745f 6c65  ses.N..report_le
+00011a10: 7665 6c94 4b02 8c0a 6861 6c74 5f6c 6576  vel.K...halt_lev
+00011a20: 656c 944b 058c 1165 7869 745f 7374 6174  el.K...exit_stat
+00011a30: 7573 5f6c 6576 656c 944b 058c 0564 6562  us_level.K...deb
+00011a40: 7567 944e 8c0e 7761 726e 696e 675f 7374  ug.N..warning_st
+00011a50: 7265 616d 944e 8c09 7472 6163 6562 6163  ream.N..tracebac
+00011a60: 6b94 888c 0e69 6e70 7574 5f65 6e63 6f64  k....input_encod
+00011a70: 696e 6794 8c09 7574 662d 382d 7369 6794  ing...utf-8-sig.
+00011a80: 8c1c 696e 7075 745f 656e 636f 6469 6e67  ..input_encoding
+00011a90: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00011aa0: 0673 7472 6963 7494 8c0f 6f75 7470 7574  .strict...output
+00011ab0: 5f65 6e63 6f64 696e 6794 8c05 7574 662d  _encoding...utf-
+00011ac0: 3894 8c1d 6f75 7470 7574 5f65 6e63 6f64  8...output_encod
+00011ad0: 696e 675f 6572 726f 725f 6861 6e64 6c65  ing_error_handle
+00011ae0: 7294 6af7 1300 008c 0e65 7272 6f72 5f65  r.j......error_e
+00011af0: 6e63 6f64 696e 6794 8c05 7574 662d 3894  ncoding...utf-8.
+00011b00: 8c1c 6572 726f 725f 656e 636f 6469 6e67  ..error_encoding
+00011b10: 5f65 7272 6f72 5f68 616e 646c 6572 948c  _error_handler..
+00011b20: 1062 6163 6b73 6c61 7368 7265 706c 6163  .backslashreplac
+00011b30: 6594 8c0d 6c61 6e67 7561 6765 5f63 6f64  e...language_cod
+00011b40: 6594 8c02 656e 948c 1372 6563 6f72 645f  e...en...record_
+00011b50: 6465 7065 6e64 656e 6369 6573 944e 8c06  dependencies.N..
+00011b60: 636f 6e66 6967 944e 8c09 6964 5f70 7265  config.N..id_pre
+00011b70: 6669 7894 6806 8c0e 6175 746f 5f69 645f  fix.h...auto_id_
+00011b80: 7072 6566 6978 948c 0269 6494 8c0d 6475  prefix...id...du
+00011b90: 6d70 5f73 6574 7469 6e67 7394 4e8c 0e64  mp_settings.N..d
+00011ba0: 756d 705f 696e 7465 726e 616c 7394 4e8c  ump_internals.N.
+00011bb0: 0f64 756d 705f 7472 616e 7366 6f72 6d73  .dump_transforms
+00011bc0: 944e 8c0f 6475 6d70 5f70 7365 7564 6f5f  .N..dump_pseudo_
+00011bd0: 786d 6c94 4e8c 1065 7870 6f73 655f 696e  xml.N..expose_in
+00011be0: 7465 726e 616c 7394 4e8c 0e73 7472 6963  ternals.N..stric
+00011bf0: 745f 7669 7369 746f 7294 4e8c 0f5f 6469  t_visitor.N.._di
+00011c00: 7361 626c 655f 636f 6e66 6967 944e 8c07  sable_config.N..
+00011c10: 5f73 6f75 7263 6594 682c 8c0c 5f64 6573  _source.h,.._des
+00011c20: 7469 6e61 7469 6f6e 944e 8c0d 5f63 6f6e  tination.N.._con
+00011c30: 6669 675f 6669 6c65 7394 5d94 8c16 6669  fig_files.]...fi
+00011c40: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
+00011c50: 626c 6564 9488 8c0b 7261 775f 656e 6162  bled....raw_enab
+00011c60: 6c65 6494 4b01 8c11 6c69 6e65 5f6c 656e  led.K...line_len
+00011c70: 6774 685f 6c69 6d69 7494 4d10 278c 0e70  gth_limit.M.'..p
+00011c80: 6570 5f72 6566 6572 656e 6365 7394 4e8c  ep_references.N.
+00011c90: 0c70 6570 5f62 6173 655f 7572 6c94 8c18  .pep_base_url...
+00011ca0: 6874 7470 733a 2f2f 7065 7073 2e70 7974  https://peps.pyt
+00011cb0: 686f 6e2e 6f72 672f 948c 1570 6570 5f66  hon.org/...pep_f
+00011cc0: 696c 655f 7572 6c5f 7465 6d70 6c61 7465  ile_url_template
+00011cd0: 948c 0870 6570 2d25 3034 6494 8c0e 7266  ...pep-%04d...rf
+00011ce0: 635f 7265 6665 7265 6e63 6573 944e 8c0c  c_references.N..
+00011cf0: 7266 635f 6261 7365 5f75 726c 948c 2668  rfc_base_url..&h
+00011d00: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+00011d10: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+00011d20: 6874 6d6c 2f94 8c09 7461 625f 7769 6474  html/...tab_widt
+00011d30: 6894 4b08 8c1d 7472 696d 5f66 6f6f 746e  h.K...trim_footn
+00011d40: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
+00011d50: 6163 6594 898c 1073 796e 7461 785f 6869  ace....syntax_hi
+00011d60: 6768 6c69 6768 7494 8c04 6c6f 6e67 948c  ghlight...long..
+00011d70: 0c73 6d61 7274 5f71 756f 7465 7394 888c  .smart_quotes...
+00011d80: 1373 6d61 7274 7175 6f74 6573 5f6c 6f63  .smartquotes_loc
+00011d90: 616c 6573 945d 948c 1d63 6861 7261 6374  ales.]...charact
+00011da0: 6572 5f6c 6576 656c 5f69 6e6c 696e 655f  er_level_inline_
+00011db0: 6d61 726b 7570 9489 8c0e 646f 6374 6974  markup....doctit
+00011dc0: 6c65 5f78 666f 726d 9489 8c0d 646f 6369  le_xform....doci
+00011dd0: 6e66 6f5f 7866 6f72 6d94 4b01 8c12 7365  nfo_xform.K...se
+00011de0: 6374 7375 6274 6974 6c65 5f78 666f 726d  ctsubtitle_xform
+00011df0: 9489 8c0d 696d 6167 655f 6c6f 6164 696e  ....image_loadin
+00011e00: 6794 8c04 6c69 6e6b 948c 1065 6d62 6564  g...link...embed
+00011e10: 5f73 7479 6c65 7368 6565 7494 898c 1563  _stylesheet....c
+00011e20: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
+00011e30: 7373 6573 9488 8c11 7365 6374 696f 6e5f  sses....section_
+00011e40: 7365 6c66 5f6c 696e 6b94 898c 0365 6e76  self_link....env
+00011e50: 944e 7562 8c08 7265 706f 7274 6572 944e  .Nub..reporter.N
+00011e60: 8c10 696e 6469 7265 6374 5f74 6172 6765  ..indirect_targe
+00011e70: 7473 945d 948c 1173 7562 7374 6974 7574  ts.]...substitut
+00011e80: 696f 6e5f 6465 6673 947d 948c 1273 7562  ion_defs.}...sub
+00011e90: 7374 6974 7574 696f 6e5f 6e61 6d65 7394  stitution_names.
+00011ea0: 7d94 8c08 7265 666e 616d 6573 947d 948c  }...refnames.}..
+00011eb0: 0672 6566 6964 7394 7d94 8c07 6e61 6d65  .refids.}...name
+00011ec0: 6964 7394 7d94 286a d113 0000 6acd 1300  ids.}.(j....j...
+00011ed0: 006a 5201 0000 6a4f 0100 006a 9602 0000  .jR...jO...j....
+00011ee0: 6a93 0200 006a b401 0000 6ab1 0100 006a  j....j....j....j
+00011ef0: 4f02 0000 6a4c 0200 006a 8302 0000 6a80  O...jL...j....j.
+00011f00: 0200 006a 9904 0000 6a96 0400 006a 9303  ...j....j....j..
+00011f10: 0000 6a90 0300 006a 2a05 0000 6a27 0500  ..j....j*...j'..
+00011f20: 006a 8505 0000 6a82 0500 006a 6807 0000  .j....j....jh...
+00011f30: 6a65 0700 006a ae06 0000 6aab 0600 006a  je...j....j....j
+00011f40: c508 0000 6ac2 0800 006a 7209 0000 6a6f  ....j....jr...jo
+00011f50: 0900 006a 4f09 0000 6a4c 0900 006a 7510  ...jO...jL...ju.
+00011f60: 0000 6a72 1000 006a 410c 0000 6a3e 0c00  ..jr...jA...j>..
+00011f70: 006a dc0c 0000 6ad9 0c00 006a bb0d 0000  .j....j....j....
+00011f80: 6ab8 0d00 006a 320d 0000 6a2f 0d00 006a  j....j2...j/...j
+00011f90: 5a0e 0000 6a57 0e00 006a 4d0f 0000 6a4a  Z...jW...jM...jJ
+00011fa0: 0f00 006a dc0f 0000 6ad9 0f00 006a 830f  ...j....j....j..
+00011fb0: 0000 6a80 0f00 006a 6d10 0000 6a6a 1000  ..j....jm...jj..
+00011fc0: 006a 1211 0000 6a0f 1100 006a ff10 0000  .j....j....j....
+00011fd0: 6afc 1000 006a 9111 0000 6a8e 1100 006a  j....j....j....j
+00011fe0: 7e11 0000 6a7b 1100 006a e211 0000 6adf  ~...j{...j....j.
+00011ff0: 1100 006a c813 0000 6ac5 1300 006a 1912  ...j....j....j..
+00012000: 0000 6a16 1200 006a 6112 0000 6a5e 1200  ..j....ja...j^..
+00012010: 006a 8312 0000 6a80 1200 006a bc12 0000  .j....j....j....
+00012020: 6ab9 1200 006a 3213 0000 6a2f 1300 006a  j....j2...j/...j
+00012030: 7313 0000 6a70 1300 006a b513 0000 6ab2  s...jp...j....j.
+00012040: 1300 0075 8c09 6e61 6d65 7479 7065 7394  ...u..nametypes.
+00012050: 7d94 286a d113 0000 896a 5201 0000 886a  }.(j.....jR....j
+00012060: 9602 0000 896a b401 0000 886a 4f02 0000  .....j.....jO...
+00012070: 886a 8302 0000 886a 9904 0000 896a 9303  .j.....j.....j..
+00012080: 0000 886a 2a05 0000 896a 8505 0000 896a  ...j*....j.....j
+00012090: 6807 0000 896a ae06 0000 886a c508 0000  h....j.....j....
+000120a0: 896a 7209 0000 896a 4f09 0000 886a 7510  .jr....jO....ju.
+000120b0: 0000 896a 410c 0000 896a dc0c 0000 896a  ...jA....j.....j
+000120c0: bb0d 0000 896a 320d 0000 886a 5a0e 0000  .....j2....jZ...
+000120d0: 896a 4d0f 0000 896a dc0f 0000 896a 830f  .jM....j.....j..
+000120e0: 0000 886a 6d10 0000 896a 1211 0000 896a  ...jm....j.....j
+000120f0: ff10 0000 886a 9111 0000 896a 7e11 0000  .....j.....j~...
+00012100: 886a e211 0000 896a c813 0000 896a 1912  .j.....j.....j..
+00012110: 0000 886a 6112 0000 886a 8312 0000 886a  ...ja....j.....j
+00012120: bc12 0000 886a 3213 0000 886a 7313 0000  .....j2....js...
+00012130: 886a b513 0000 8875 6821 7d94 286a cd13  .j.....uh!}.(j..
+00012140: 0000 680c 6a4f 0100 006a 4901 0000 6a93  ..h.jO...jI...j.
+00012150: 0200 006a 7301 0000 6ab1 0100 006a ab01  ...js...j....j..
+00012160: 0000 6a4c 0200 006a 4602 0000 6a80 0200  ..jL...jF...j...
+00012170: 006a 7a02 0000 6a96 0400 006a 9902 0000  .jz...j....j....
+00012180: 6a90 0300 006a 8a03 0000 6a27 0500 006a  j....j....j'...j
+00012190: 9c04 0000 6a82 0500 006a 2d05 0000 6a65  ....j....j-...je
+000121a0: 0700 006a 8805 0000 6aab 0600 006a a506  ...j....j....j..
+000121b0: 0000 6ac2 0800 006a 6b07 0000 6a6f 0900  ..j....jk...jo..
+000121c0: 006a c808 0000 6a4c 0900 006a 4609 0000  .j....jL...jF...
+000121d0: 6a72 1000 006a 7509 0000 6a3e 0c00 006a  jr...ju...j>...j
+000121e0: 8609 0000 6ad9 0c00 006a 440c 0000 6ab8  ....j....jD...j.
+000121f0: 0d00 006a df0c 0000 6a2f 0d00 006a 290d  ...j....j/...j).
+00012200: 0000 6a57 0e00 006a be0d 0000 6a4a 0f00  ..jW...j....jJ..
+00012210: 006a 5d0e 0000 6aad 0e00 006a a70e 0000  .j]...j....j....
+00012220: 6ad9 0f00 006a 500f 0000 6a80 0f00 006a  j....jP...j....j
+00012230: 7a0f 0000 6a6a 1000 006a df0f 0000 6a0f  z...jj...j....j.
+00012240: 1100 006a 7810 0000 6afc 1000 006a f610  ...jx...j....j..
+00012250: 0000 6a8e 1100 006a 1511 0000 6a7b 1100  ..j....j....j{..
+00012260: 006a 7511 0000 6adf 1100 006a 9411 0000  .ju...j....j....
+00012270: 6ac5 1300 006a e511 0000 6a16 1200 006a  j....j....j....j
+00012280: 1012 0000 6a5e 1200 006a 5812 0000 6a80  ....j^...jX...j.
+00012290: 1200 006a 7a12 0000 6ab9 1200 006a b312  ...jz...j....j..
+000122a0: 0000 6a2f 1300 006a 2913 0000 6a70 1300  ..j/...j)...jp..
+000122b0: 006a 6a13 0000 6ab2 1300 006a ac13 0000  .jj...j....j....
+000122c0: 758c 0d66 6f6f 746e 6f74 655f 7265 6673  u..footnote_refs
+000122d0: 947d 948c 0d63 6974 6174 696f 6e5f 7265  .}...citation_re
+000122e0: 6673 947d 948c 0d61 7574 6f66 6f6f 746e  fs.}...autofootn
+000122f0: 6f74 6573 945d 948c 1161 7574 6f66 6f6f  otes.]...autofoo
+00012300: 746e 6f74 655f 7265 6673 945d 948c 1073  tnote_refs.]...s
+00012310: 796d 626f 6c5f 666f 6f74 6e6f 7465 7394  ymbol_footnotes.
+00012320: 5d94 8c14 7379 6d62 6f6c 5f66 6f6f 746e  ]...symbol_footn
+00012330: 6f74 655f 7265 6673 945d 948c 0966 6f6f  ote_refs.]...foo
+00012340: 746e 6f74 6573 945d 948c 0963 6974 6174  tnotes.]...citat
+00012350: 696f 6e73 945d 948c 1261 7574 6f66 6f6f  ions.]...autofoo
+00012360: 746e 6f74 655f 7374 6172 7494 4b01 8c15  tnote_start.K...
+00012370: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
+00012380: 7374 6172 7494 4b00 8c0a 6964 5f63 6f75  start.K...id_cou
+00012390: 6e74 6572 948c 0b63 6f6c 6c65 6374 696f  nter...collectio
+000123a0: 6e73 948c 0743 6f75 6e74 6572 9493 947d  ns...Counter...}
+000123b0: 946a 0514 0000 4b01 7385 9452 948c 0e70  .j....K.s..R...p
+000123c0: 6172 7365 5f6d 6573 7361 6765 7394 5d94  arse_messages.].
+000123d0: 6809 8c0e 7379 7374 656d 5f6d 6573 7361  h...system_messa
+000123e0: 6765 9493 9429 8194 7d94 2868 0568 0668  ge...)..}.(h.h.h
+000123f0: 075d 9468 ee29 8194 7d94 2868 058c 3544  .].h.)..}.(h..5D
+00012400: 7570 6c69 6361 7465 2065 7870 6c69 6369  uplicate explici
+00012410: 7420 7461 7267 6574 206e 616d 653a 2022  t target name: "
+00012420: 7375 7070 6f72 7465 6420 6279 206e 6772  supported by ngr
+00012430: 6f6b 222e 9468 075d 9468 168c 3944 7570  ok"..h.].h..9Dup
+00012440: 6c69 6361 7465 2065 7870 6c69 6369 7420  licate explicit 
+00012450: 7461 7267 6574 206e 616d 653a 20e2 809c  target name: ...
+00012460: 7375 7070 6f72 7465 6420 6279 206e 6772  supported by ngr
+00012470: 6f6b e280 9d2e 9485 9481 947d 9428 681b  ok.........}.(h.
+00012480: 6a5d 1400 0068 1c68 0368 1d4e 681e 4e75  j]...h.h.h.Nh.Nu
+00012490: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+000124a0: 255d 9468 275d 9468 295d 9475 682b 68ed  %].h'].h)].uh+h.
+000124b0: 681b 6a5a 1400 0075 6261 681f 7d94 2868  h.jZ...ubah.}.(h
+000124c0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000124d0: 295d 946a ad0e 0000 618c 056c 6576 656c  )].j....a..level
+000124e0: 944b 018c 0474 7970 6594 8c04 494e 464f  .K...type...INFO
+000124f0: 948c 0673 6f75 7263 6594 682c 8c04 6c69  ...source.h,..li
+00012500: 6e65 944b 0575 682b 6a58 1400 0068 1b6a  ne.K.uh+jX...h.j
+00012510: 5d0e 0000 681c 6803 681d 682c 681e 4d3c  ]...h.h.h.h,h.M<
+00012520: 0175 6261 8c12 7472 616e 7366 6f72 6d5f  .uba..transform_
+00012530: 6d65 7373 6167 6573 945d 948c 0b74 7261  messages.]...tra
+00012540: 6e73 666f 726d 6572 944e 8c0b 696e 636c  nsformer.N..incl
+00012550: 7564 655f 6c6f 6794 5d94 8c0e 646f 6373  ude_log.]...docs
+00012560: 2f69 6e64 6578 2e72 7374 9428 4e4e 4e4e  /index.rst.(NNNN
+00012570: 7494 8694 618c 0a64 6563 6f72 6174 696f  t...a..decoratio
+00012580: 6e94 4e68 1c68 0375 622e                 n.Nh.h.ub.
```

### Comparing `pyngrok-5.2.2/_build/docs/doctrees/integrations.doctree` & `pyngrok-5.2.3/_build/docs/doctrees/integrations.doctree`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/doctrees/troubleshooting.doctree` & `pyngrok-5.2.3/_build/docs/doctrees/troubleshooting.doctree`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/404.html` & `pyngrok-5.2.3/_build/docs/html/404.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Page not found &#8212; pyngrok 5.2.2 documentation</title>
+    <title>Page not found &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="/en/latest/_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="/en/latest/_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="/en/latest/_static/custom.css" />
     <script data-url_root="#" id="documentation_options" src="/en/latest/_static/documentation_options.js"></script>
     <script src="/en/latest/_static/doctools.js"></script>
     <script src="/en/latest/_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="/en/latest/genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_images/logo.png` & `pyngrok-5.2.3/_build/docs/html/_images/logo.png`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_modules/index.html` & `pyngrok-5.2.3/_build/docs/html/_modules/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Overview: module code &#8212; pyngrok 5.2.2 documentation</title>
+    <title>Overview: module code &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="../_static/custom.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
     <script src="../_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/conf.html` & `pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/conf.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>pyngrok.conf &#8212; pyngrok 5.2.2 documentation</title>
+    <title>pyngrok.conf &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/custom.css" />
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
     <script src="../../_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/exception.html` & `pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/exception.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>pyngrok.exception &#8212; pyngrok 5.2.2 documentation</title>
+    <title>pyngrok.exception &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/custom.css" />
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
     <script src="../../_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/installer.html` & `pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/installer.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>pyngrok.installer &#8212; pyngrok 5.2.2 documentation</title>
+    <title>pyngrok.installer &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/custom.css" />
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
     <script src="../../_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/ngrok.html` & `pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/ngrok.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>pyngrok.ngrok &#8212; pyngrok 5.2.2 documentation</title>
+    <title>pyngrok.ngrok &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/custom.css" />
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
     <script src="../../_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
@@ -75,15 +75,15 @@
 <span class="kn">from</span> <span class="nn">urllib.request</span> <span class="kn">import</span> <span class="n">urlopen</span><span class="p">,</span> <span class="n">Request</span>
 
 <span class="kn">from</span> <span class="nn">pyngrok</span> <span class="kn">import</span> <span class="n">process</span><span class="p">,</span> <span class="n">conf</span><span class="p">,</span> <span class="n">installer</span>
 <span class="kn">from</span> <span class="nn">pyngrok.exception</span> <span class="kn">import</span> <span class="n">PyngrokNgrokHTTPError</span><span class="p">,</span> <span class="n">PyngrokNgrokURLError</span><span class="p">,</span> <span class="n">PyngrokSecurityError</span><span class="p">,</span> <span class="n">PyngrokError</span>
 
 <span class="n">__author__</span> <span class="o">=</span> <span class="s2">&quot;Alex Laird&quot;</span>
 <span class="n">__copyright__</span> <span class="o">=</span> <span class="s2">&quot;Copyright 2023, Alex Laird&quot;</span>
-<span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;5.2.2&quot;</span>
+<span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;5.2.3&quot;</span>
 
 <span class="kn">from</span> <span class="nn">pyngrok.installer</span> <span class="kn">import</span> <span class="n">get_default_config</span>
 
 <span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="vm">__name__</span><span class="p">)</span>
 
 <span class="n">_current_tunnels</span> <span class="o">=</span> <span class="p">{}</span>
 
@@ -315,23 +315,33 @@
         <span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span>
         <span class="s2">&quot;addr&quot;</span><span class="p">:</span> <span class="n">addr</span><span class="p">,</span>
         <span class="s2">&quot;proto&quot;</span><span class="p">:</span> <span class="n">proto</span>
     <span class="p">}</span>
     <span class="n">options</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">config</span><span class="p">)</span>
 
     <span class="c1"># Upgrade legacy parameters, if present</span>
-    <span class="k">if</span> <span class="n">pyngrok_config</span><span class="o">.</span><span class="n">ngrok_version</span> <span class="o">==</span> <span class="s2">&quot;v3&quot;</span> <span class="ow">and</span> <span class="s2">&quot;bind_tls&quot;</span> <span class="ow">in</span> <span class="n">options</span><span class="p">:</span>
-        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="ow">is</span> <span class="kc">True</span> <span class="ow">or</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="o">==</span> <span class="s2">&quot;true&quot;</span><span class="p">:</span>
-            <span class="n">options</span><span class="p">[</span><span class="s2">&quot;schemes&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;https&quot;</span><span class="p">]</span>
-        <span class="k">elif</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">False</span> <span class="ow">or</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="o">==</span> <span class="s2">&quot;false&quot;</span><span class="p">:</span>
-            <span class="n">options</span><span class="p">[</span><span class="s2">&quot;schemes&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;http&quot;</span><span class="p">]</span>
-        <span class="k">else</span><span class="p">:</span>
-            <span class="n">options</span><span class="p">[</span><span class="s2">&quot;schemes&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;http&quot;</span><span class="p">,</span> <span class="s2">&quot;https&quot;</span><span class="p">]</span>
+    <span class="k">if</span> <span class="n">pyngrok_config</span><span class="o">.</span><span class="n">ngrok_version</span> <span class="o">==</span> <span class="s2">&quot;v3&quot;</span><span class="p">:</span>
+        <span class="k">if</span> <span class="s2">&quot;bind_tls&quot;</span> <span class="ow">in</span> <span class="n">options</span><span class="p">:</span>
+            <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="ow">is</span> <span class="kc">True</span> <span class="ow">or</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="o">==</span> <span class="s2">&quot;true&quot;</span><span class="p">:</span>
+                <span class="n">options</span><span class="p">[</span><span class="s2">&quot;schemes&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;https&quot;</span><span class="p">]</span>
+            <span class="k">elif</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">False</span> <span class="ow">or</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span> <span class="o">==</span> <span class="s2">&quot;false&quot;</span><span class="p">:</span>
+                <span class="n">options</span><span class="p">[</span><span class="s2">&quot;schemes&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;http&quot;</span><span class="p">]</span>
+            <span class="k">else</span><span class="p">:</span>
+                <span class="n">options</span><span class="p">[</span><span class="s2">&quot;schemes&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;http&quot;</span><span class="p">,</span> <span class="s2">&quot;https&quot;</span><span class="p">]</span>
+
+            <span class="n">options</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span>
+
+        <span class="k">if</span> <span class="s2">&quot;auth&quot;</span> <span class="ow">in</span> <span class="n">options</span><span class="p">:</span>
+            <span class="n">auth</span> <span class="o">=</span> <span class="n">options</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;auth&quot;</span><span class="p">)</span>
+            <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">auth</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
+                <span class="n">options</span><span class="p">[</span><span class="s2">&quot;basic_auth&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">auth</span>
+            <span class="k">else</span><span class="p">:</span>
+                <span class="n">options</span><span class="p">[</span><span class="s2">&quot;basic_auth&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">auth</span><span class="p">]</span>
 
-        <span class="n">options</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="s2">&quot;bind_tls&quot;</span><span class="p">)</span>
+            <span class="n">options</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="s2">&quot;auth&quot;</span><span class="p">)</span>
 
     <span class="n">api_url</span> <span class="o">=</span> <span class="n">get_ngrok_process</span><span class="p">(</span><span class="n">pyngrok_config</span><span class="p">)</span><span class="o">.</span><span class="n">api_url</span>
 
     <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="s2">&quot;Creating tunnel with options: </span><span class="si">{}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">options</span><span class="p">))</span>
 
     <span class="n">tunnel</span> <span class="o">=</span> <span class="n">NgrokTunnel</span><span class="p">(</span><span class="n">api_request</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{}</span><span class="s2">/api/tunnels&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">api_url</span><span class="p">),</span> <span class="n">method</span><span class="o">=</span><span class="s2">&quot;POST&quot;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">options</span><span class="p">,</span>
                                      <span class="n">timeout</span><span class="o">=</span><span class="n">pyngrok_config</span><span class="o">.</span><span class="n">request_timeout</span><span class="p">),</span>
```

#### html2text {}

```diff
@@ -29,15 +29,15 @@
 
 from pyngrok import process, conf, installer
 from pyngrok.exception import PyngrokNgrokHTTPError, PyngrokNgrokURLError,
 PyngrokSecurityError, PyngrokError
 
 __author__ = "Alex Laird"
 __copyright__ = "Copyright 2023, Alex Laird"
-__version__ = "5.2.2"
+__version__ = "5.2.3"
 
 from pyngrok.installer import get_default_config
 
 logger = logging.getLogger(__name__)
 
 _current_tunnels = {}
 
@@ -312,25 +312,35 @@
         "name": name,
         "addr": addr,
         "proto": proto
     }
     options.update(config)
 
     # Upgrade legacy parameters, if present
-    if pyngrok_config.ngrok_version == "v3" and "bind_tls" in options:
-        if options.get("bind_tls") is True or options.get("bind_tls") ==
+    if pyngrok_config.ngrok_version == "v3":
+        if "bind_tls" in options:
+            if options.get("bind_tls") is True or options.get("bind_tls") ==
 "true":
-            options["schemes"] = ["https"]
-        elif not options.get("bind_tls") is not False or options.get
+                options["schemes"] = ["https"]
+            elif not options.get("bind_tls") is not False or options.get
 ("bind_tls") == "false":
-            options["schemes"] = ["http"]
-        else:
-            options["schemes"] = ["http", "https"]
+                options["schemes"] = ["http"]
+            else:
+                options["schemes"] = ["http", "https"]
+
+            options.pop("bind_tls")
+
+        if "auth" in options:
+            auth = options.get("auth")
+            if isinstance(auth, list):
+                options["basic_auth"] = auth
+            else:
+                options["basic_auth"] = [auth]
 
-        options.pop("bind_tls")
+            options.pop("auth")
 
     api_url = get_ngrok_process(pyngrok_config).api_url
 
     logger.debug("Creating tunnel with options: {}".format(options))
 
     tunnel = NgrokTunnel(api_request("{}/api/tunnels".format(api_url),
 method="POST", data=options,
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_modules/pyngrok/process.html` & `pyngrok-5.2.3/_build/docs/html/_modules/pyngrok/process.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>pyngrok.process &#8212; pyngrok 5.2.2 documentation</title>
+    <title>pyngrok.process &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/custom.css" />
     <script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
     <script src="../../_static/doctools.js"></script>
     <script src="../../_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="../../genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_sources/api.rst.txt` & `pyngrok-5.2.3/_build/docs/html/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_sources/index.rst.txt` & `pyngrok-5.2.3/_build/docs/html/_sources/index.rst.txt`

 * *Files 1% similar despite different names*

```diff
@@ -234,34 +234,37 @@
 Most methods in the :mod:`~pyngrok.ngrok` module also accept a ``pyngrok_config`` keyword arg, which can be used
 to pass in the config rather than updating the default as shown above.
 
 The ``pyngrok_config`` argument is only used when the ``ngrok`` process is first started, which will be
 the first time most methods in the :mod:`~pyngrok.ngrok` module are called. We can check if a process is already or
 still running by calling its :func:`~pyngrok.process.NgrokProcess.healthy` method.
 
-``pyngrok`` is compatible with ``ngrok`` v2 and v3, but by default it will install v2. To install v3 instead,
-set ``ngrok_version`` in :class:`~pyngrok.conf.PyngrokConfig`:
-
-.. code-block:: python
-
-    from pyngrok import conf, ngrok
-
-    conf.get_default().ngrok_version = "v3"
-
 .. note::
 
     If ``ngrok`` is not already installed at the ``ngrok_path`` in :class:`~pyngrok.conf.PyngrokConfig`, it
     will be installed the first time most methods in the :mod:`~pyngrok.ngrok` module are called.
 
     If we need to customize the installation of ``ngrok``, perhaps specifying a timeout, proxy, use a custom mirror
     for the download, etc. we can do so by leveraging the :mod:`~pyngrok.installer` module. Keyword arguments in this
     module are ultimately passed down to :py:func:`urllib.request.urlopen`, so as long as we use the
     :mod:`~pyngrok.installer` module ourselves prior to invoking any :mod:`~pyngrok.ngrok` methods, we can can control
     how ``ngrok`` is installed and from where.
 
+``ngrok`` Version Compatibility
+-------------------------------
+
+``pyngrok`` is compatible with ``ngrok`` v2 and v3, but by default it will install v2. To install v3 instead,
+set ``ngrok_version`` in :class:`~pyngrok.conf.PyngrokConfig`:
+
+.. code-block:: python
+
+    from pyngrok import conf, ngrok
+
+    conf.get_default().ngrok_version = "v3"
+
 Setting the ``authtoken``
 -------------------------
 
 Running ``ngrok`` with an auth token enables additional features available on our account (for
 instance, the ability to open multiple tunnels concurrently). We can obtain our auth token from
 the `ngrok dashboard <https://dashboard.ngrok.com>`_ and install it to ``ngrok``'s config file like this:
```

### Comparing `pyngrok-5.2.2/_build/docs/html/_sources/integrations.rst.txt` & `pyngrok-5.2.3/_build/docs/html/_sources/integrations.rst.txt`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_sources/troubleshooting.rst.txt` & `pyngrok-5.2.3/_build/docs/html/_sources/troubleshooting.rst.txt`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_static/alabaster.css` & `pyngrok-5.2.3/_build/docs/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_static/basic.css` & `pyngrok-5.2.3/_build/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_static/doctools.js` & `pyngrok-5.2.3/_build/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_static/language_data.js` & `pyngrok-5.2.3/_build/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_static/pygments.css` & `pyngrok-5.2.3/_build/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_static/searchtools.js` & `pyngrok-5.2.3/_build/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/_static/sphinx_highlight.js` & `pyngrok-5.2.3/_build/docs/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/api.html` & `pyngrok-5.2.3/_build/docs/html/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>API Documentation &#8212; pyngrok 5.2.2 documentation</title>
+    <title>API Documentation &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/genindex.html` & `pyngrok-5.2.3/_build/docs/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; pyngrok 5.2.2 documentation</title>
+    <title>Index &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="#" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/index.html` & `pyngrok-5.2.3/_build/docs/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>pyngrok - a Python wrapper for ngrok &#8212; pyngrok 5.2.2 documentation</title>
+    <title>pyngrok - a Python wrapper for ngrok &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -247,32 +247,35 @@
 </pre></div>
 </div>
 <p>Most methods in the <a class="reference internal" href="api.html#module-pyngrok.ngrok" title="pyngrok.ngrok"><code class="xref py py-mod docutils literal notranslate"><span class="pre">ngrok</span></code></a> module also accept a <code class="docutils literal notranslate"><span class="pre">pyngrok_config</span></code> keyword arg, which can be used
 to pass in the config rather than updating the default as shown above.</p>
 <p>The <code class="docutils literal notranslate"><span class="pre">pyngrok_config</span></code> argument is only used when the <code class="docutils literal notranslate"><span class="pre">ngrok</span></code> process is first started, which will be
 the first time most methods in the <a class="reference internal" href="api.html#module-pyngrok.ngrok" title="pyngrok.ngrok"><code class="xref py py-mod docutils literal notranslate"><span class="pre">ngrok</span></code></a> module are called. We can check if a process is already or
 still running by calling its <a class="reference internal" href="api.html#pyngrok.process.NgrokProcess.healthy" title="pyngrok.process.NgrokProcess.healthy"><code class="xref py py-func docutils literal notranslate"><span class="pre">healthy</span></code></a> method.</p>
-<p><code class="docutils literal notranslate"><span class="pre">pyngrok</span></code> is compatible with <code class="docutils literal notranslate"><span class="pre">ngrok</span></code> v2 and v3, but by default it will install v2. To install v3 instead,
-set <code class="docutils literal notranslate"><span class="pre">ngrok_version</span></code> in <a class="reference internal" href="api.html#pyngrok.conf.PyngrokConfig" title="pyngrok.conf.PyngrokConfig"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyngrokConfig</span></code></a>:</p>
-<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">pyngrok</span> <span class="kn">import</span> <span class="n">conf</span><span class="p">,</span> <span class="n">ngrok</span>
-
-<span class="n">conf</span><span class="o">.</span><span class="n">get_default</span><span class="p">()</span><span class="o">.</span><span class="n">ngrok_version</span> <span class="o">=</span> <span class="s2">&quot;v3&quot;</span>
-</pre></div>
-</div>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>If <code class="docutils literal notranslate"><span class="pre">ngrok</span></code> is not already installed at the <code class="docutils literal notranslate"><span class="pre">ngrok_path</span></code> in <a class="reference internal" href="api.html#pyngrok.conf.PyngrokConfig" title="pyngrok.conf.PyngrokConfig"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyngrokConfig</span></code></a>, it
 will be installed the first time most methods in the <a class="reference internal" href="api.html#module-pyngrok.ngrok" title="pyngrok.ngrok"><code class="xref py py-mod docutils literal notranslate"><span class="pre">ngrok</span></code></a> module are called.</p>
 <p>If we need to customize the installation of <code class="docutils literal notranslate"><span class="pre">ngrok</span></code>, perhaps specifying a timeout, proxy, use a custom mirror
 for the download, etc. we can do so by leveraging the <a class="reference internal" href="api.html#module-pyngrok.installer" title="pyngrok.installer"><code class="xref py py-mod docutils literal notranslate"><span class="pre">installer</span></code></a> module. Keyword arguments in this
 module are ultimately passed down to <a class="reference external" href="https://docs.python.org/3/library/urllib.request.html#urllib.request.urlopen" title="(in Python v3.11)"><code class="xref py py-func docutils literal notranslate"><span class="pre">urllib.request.urlopen</span></code></a>, so as long as we use the
 <a class="reference internal" href="api.html#module-pyngrok.installer" title="pyngrok.installer"><code class="xref py py-mod docutils literal notranslate"><span class="pre">installer</span></code></a> module ourselves prior to invoking any <a class="reference internal" href="api.html#module-pyngrok.ngrok" title="pyngrok.ngrok"><code class="xref py py-mod docutils literal notranslate"><span class="pre">ngrok</span></code></a> methods, we can can control
 how <code class="docutils literal notranslate"><span class="pre">ngrok</span></code> is installed and from where.</p>
 </div>
 </section>
+<section id="ngrok-version-compatibility">
+<h3><code class="docutils literal notranslate"><span class="pre">ngrok</span></code> Version Compatibility<a class="headerlink" href="#ngrok-version-compatibility" title="Permalink to this heading">¶</a></h3>
+<p><code class="docutils literal notranslate"><span class="pre">pyngrok</span></code> is compatible with <code class="docutils literal notranslate"><span class="pre">ngrok</span></code> v2 and v3, but by default it will install v2. To install v3 instead,
+set <code class="docutils literal notranslate"><span class="pre">ngrok_version</span></code> in <a class="reference internal" href="api.html#pyngrok.conf.PyngrokConfig" title="pyngrok.conf.PyngrokConfig"><code class="xref py py-class docutils literal notranslate"><span class="pre">PyngrokConfig</span></code></a>:</p>
+<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">pyngrok</span> <span class="kn">import</span> <span class="n">conf</span><span class="p">,</span> <span class="n">ngrok</span>
+
+<span class="n">conf</span><span class="o">.</span><span class="n">get_default</span><span class="p">()</span><span class="o">.</span><span class="n">ngrok_version</span> <span class="o">=</span> <span class="s2">&quot;v3&quot;</span>
+</pre></div>
+</div>
+</section>
 <section id="setting-the-authtoken">
 <h3>Setting the <code class="docutils literal notranslate"><span class="pre">authtoken</span></code><a class="headerlink" href="#setting-the-authtoken" title="Permalink to this heading">¶</a></h3>
 <p>Running <code class="docutils literal notranslate"><span class="pre">ngrok</span></code> with an auth token enables additional features available on our account (for
 instance, the ability to open multiple tunnels concurrently). We can obtain our auth token from
 the <a class="reference external" href="https://dashboard.ngrok.com">ngrok dashboard</a> and install it to <code class="docutils literal notranslate"><span class="pre">ngrok</span></code>’s config file like this:</p>
 <div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">pyngrok</span> <span class="kn">import</span> <span class="n">ngrok</span>
```

#### html2text {}

```diff
@@ -170,29 +170,31 @@
 Most methods in the ngrok module also accept a pyngrok_config keyword arg,
 which can be used to pass in the config rather than updating the default as
 shown above.
 The pyngrok_config argument is only used when the ngrok process is first
 started, which will be the first time most methods in the ngrok module are
 called. We can check if a process is already or still running by calling its
 healthy method.
-pyngrok is compatible with ngrok v2 and v3, but by default it will install v2.
-To install v3 instead, set ngrok_version in PyngrokConfig:
-from pyngrok import conf, ngrok
-
-conf.get_default().ngrok_version = "v3"
 Note
 If ngrok is not already installed at the ngrok_path in PyngrokConfig, it will
 be installed the first time most methods in the ngrok module are called.
 If we need to customize the installation of ngrok, perhaps specifying a
 timeout, proxy, use a custom mirror for the download, etc. we can do so by
 leveraging the installer module. Keyword arguments in this module are
 ultimately passed down to urllib.request.urlopen, so as long as we use the
 installer module ourselves prior to invoking any ngrok methods, we can can
 control how ngrok is installed and from where.
 
+**** ngrok Version CompatibilityÂ¶ ****
+pyngrok is compatible with ngrok v2 and v3, but by default it will install v2.
+To install v3 instead, set ngrok_version in PyngrokConfig:
+from pyngrok import conf, ngrok
+
+conf.get_default().ngrok_version = "v3"
+
 **** Setting the authtokenÂ¶ ****
 Running ngrok with an auth token enables additional features available on our
 account (for instance, the ability to open multiple tunnels concurrently). We
 can obtain our auth token from the ngrok_dashboard and install it to ngrokâs
 config file like this:
 from pyngrok import ngrok
```

### Comparing `pyngrok-5.2.2/_build/docs/html/integrations.html` & `pyngrok-5.2.3/_build/docs/html/integrations.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>Integration Examples &#8212; pyngrok 5.2.2 documentation</title>
+    <title>Integration Examples &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/logo.png` & `pyngrok-5.2.3/_build/docs/html/logo.png`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/objects.inv` & `pyngrok-5.2.3/_build/docs/html/objects.inv`

 * *Files 2% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: pyngrok
-# Version: 5.2.2
+# Version: 5.2.3
 # The remainder of this file is compressed using zlib.
 
 pyngrok.conf py:module 0 api.html#module-$ -
 pyngrok.conf.PyngrokConfig py:class 1 api.html#$ -
 pyngrok.conf.get_default py:function 1 api.html#$ -
 pyngrok.conf.set_default py:function 1 api.html#$ -
 pyngrok.exception py:module 0 api.html#module-$ -
```

### Comparing `pyngrok-5.2.2/_build/docs/html/py-modindex.html` & `pyngrok-5.2.3/_build/docs/html/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; pyngrok 5.2.2 documentation</title>
+    <title>Python Module Index &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyngrok-5.2.2/_build/docs/html/search.html` & `pyngrok-5.2.3/_build/docs/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; pyngrok 5.2.2 documentation</title>
+    <title>Search &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
```

### Comparing `pyngrok-5.2.2/_build/docs/html/searchindex.js` & `pyngrok-5.2.3/_build/docs/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -101,15 +101,15 @@
         "pass": [0, 2],
         "overrid": [0, 1],
         "properti": [0, 1],
         "ngrok_path": [0, 1],
         "call": [0, 1, 2, 3],
         "first": [0, 1, 2, 3],
         "download": [0, 1],
-        "compat": [0, 1],
+        "compat": 0,
         "v2": [0, 1],
         "v3": [0, 1],
         "To": [0, 1, 2, 3],
         "instead": [0, 1, 2, 3],
         "set": [0, 2, 3],
         "ngrok_vers": [0, 1],
         "run": [0, 1, 2, 3],
@@ -150,15 +150,15 @@
         "implicitli": 0,
         "ngrokprocess": [0, 1, 3],
         "get_tunnel": [0, 1],
         "list": [0, 1],
         "activ": 0,
         "get_vers": 0,
         "tupl": 0,
-        "version": [0, 1, 3],
+        "version": [0, 3],
         "pyngrok_vers": 0,
         "install_ngrok": 0,
         "initi": [0, 1, 2],
         "its": [0, 1, 2, 3],
         "alreadi": [0, 1],
         "do": [0, 1, 2, 3],
         "noth": 0,
@@ -1016,14 +1016,16 @@
         "The": 1,
         "event": 1,
         "log": [1, 3],
         "expos": 1,
         "other": 1,
         "servic": 1,
         "pyngrokconfig": 1,
+        "version": 1,
+        "compat": 1,
         "set": 1,
         "authtoken": 1,
         "region": 1,
         "pass": 1,
         "option": 1,
         "kwarg": 1,
         "config": 1,
@@ -1124,14 +1126,17 @@
         ],
         "Expose Other Services": [
             [1, "expose-other-services"]
         ],
         "PyngrokConfig": [
             [1, "pyngrokconfig"]
         ],
+        "ngrok Version Compatibility": [
+            [1, "ngrok-version-compatibility"]
+        ],
         "Setting the authtoken": [
             [1, "setting-the-authtoken"]
         ],
         "Setting the region": [
             [1, "setting-the-region"]
         ],
         "Passing options as kwargs": [
```

### Comparing `pyngrok-5.2.2/_build/docs/html/sitemap-index.xml` & `pyngrok-5.2.3/_build/docs/html/sitemap-index.xml`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/_build/docs/html/troubleshooting.html` & `pyngrok-5.2.3/_build/docs/html/troubleshooting.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
-    <title>Troubleshooting &#8212; pyngrok 5.2.2 documentation</title>
+    <title>Troubleshooting &#8212; pyngrok 5.2.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <link rel="stylesheet" type="text/css" href="_static/custom.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyngrok-5.2.2/pyngrok/conf.py` & `pyngrok-5.2.3/pyngrok/conf.py`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/pyngrok/exception.py` & `pyngrok-5.2.3/pyngrok/exception.py`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/pyngrok/installer.py` & `pyngrok-5.2.3/pyngrok/installer.py`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/pyngrok/ngrok.py` & `pyngrok-5.2.3/pyngrok/ngrok.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from urllib.request import urlopen, Request
 
 from pyngrok import process, conf, installer
 from pyngrok.exception import PyngrokNgrokHTTPError, PyngrokNgrokURLError, PyngrokSecurityError, PyngrokError
 
 __author__ = "Alex Laird"
 __copyright__ = "Copyright 2023, Alex Laird"
-__version__ = "5.2.2"
+__version__ = "5.2.3"
 
 from pyngrok.installer import get_default_config
 
 logger = logging.getLogger(__name__)
 
 _current_tunnels = {}
 
@@ -250,23 +250,33 @@
         "name": name,
         "addr": addr,
         "proto": proto
     }
     options.update(config)
 
     # Upgrade legacy parameters, if present
-    if pyngrok_config.ngrok_version == "v3" and "bind_tls" in options:
-        if options.get("bind_tls") is True or options.get("bind_tls") == "true":
-            options["schemes"] = ["https"]
-        elif not options.get("bind_tls") is not False or options.get("bind_tls") == "false":
-            options["schemes"] = ["http"]
-        else:
-            options["schemes"] = ["http", "https"]
+    if pyngrok_config.ngrok_version == "v3":
+        if "bind_tls" in options:
+            if options.get("bind_tls") is True or options.get("bind_tls") == "true":
+                options["schemes"] = ["https"]
+            elif not options.get("bind_tls") is not False or options.get("bind_tls") == "false":
+                options["schemes"] = ["http"]
+            else:
+                options["schemes"] = ["http", "https"]
+
+            options.pop("bind_tls")
+
+        if "auth" in options:
+            auth = options.get("auth")
+            if isinstance(auth, list):
+                options["basic_auth"] = auth
+            else:
+                options["basic_auth"] = [auth]
 
-        options.pop("bind_tls")
+            options.pop("auth")
 
     api_url = get_ngrok_process(pyngrok_config).api_url
 
     logger.debug("Creating tunnel with options: {}".format(options))
 
     tunnel = NgrokTunnel(api_request("{}/api/tunnels".format(api_url), method="POST", data=options,
                                      timeout=pyngrok_config.request_timeout),
```

### Comparing `pyngrok-5.2.2/pyngrok/process.py` & `pyngrok-5.2.3/pyngrok/process.py`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/pyngrok.egg-info/PKG-INFO` & `pyngrok-5.2.3/pyngrok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyngrok
-Version: 5.2.2
+Version: 5.2.3
 Summary: A Python wrapper for ngrok.
 Home-page: https://github.com/alexdlaird/pyngrok
-Download-URL: https://github.com/alexdlaird/pyngrok/archive/5.2.2.tar.gz
+Download-URL: https://github.com/alexdlaird/pyngrok/archive/5.2.3.tar.gz
 Author: Alex Laird
 Author-email: contact@alexlaird.com
 License: MIT
 Project-URL: Documentation, https://pyngrok.readthedocs.io
 Project-URL: Changelog, https://github.com/alexdlaird/pyngrok/blob/main/CHANGELOG.md
 Project-URL: Sponsor, https://www.paypal.me/alexdlaird
 Keywords: ngrok,tunnel,tunneling,webhook,localhost,reverse-proxy,localtunnel
```

### Comparing `pyngrok-5.2.2/pyngrok.egg-info/SOURCES.txt` & `pyngrok-5.2.3/pyngrok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyngrok-5.2.2/setup.py` & `pyngrok-5.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from setuptools import setup
 
 __author__ = "Alex Laird"
 __copyright__ = "Copyright 2023, Alex Laird"
-__version__ = "5.2.2"
+__version__ = "5.2.3"
 
 name = "pyngrok" if os.environ.get("BUILD_PACKAGE_AS_NGROK", "False") != "True" else "ngrok"
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
```

