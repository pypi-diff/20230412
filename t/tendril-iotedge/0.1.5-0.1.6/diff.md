# Comparing `tmp/tendril-iotedge-0.1.5.tar.gz` & `tmp/tendril-iotedge-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-iotedge-0.1.5.tar", last modified: Fri Apr  7 02:36:09 2023, max compression
+gzip compressed data, was "tendril-iotedge-0.1.6.tar", last modified: Wed Apr 12 18:22:05 2023, max compression
```

## Comparing `tendril-iotedge-0.1.5.tar` & `tendril-iotedge-0.1.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.155695 tendril-iotedge-0.1.5/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-04-07 02:36:09.159695 tendril-iotedge-0.1.5/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.107696 tendril-iotedge-0.1.5/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.119696 tendril-iotedge-0.1.5/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.119696 tendril-iotedge-0.1.5/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.119696 tendril-iotedge-0.1.5/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.123696 tendril-iotedge-0.1.5/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-07 02:36:09.159695 tendril-iotedge-0.1.5/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-03-16 07:26:30.000000 tendril-iotedge-0.1.5/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.091696 tendril-iotedge-0.1.5/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.123696 tendril-iotedge-0.1.5/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.123696 tendril-iotedge-0.1.5/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.127696 tendril-iotedge-0.1.5/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1855 2023-04-05 18:31:23.000000 tendril-iotedge-0.1.5/src/tendril/apiserver/routers/iotcore.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2266 2023-04-05 09:34:19.000000 tendril-iotedge-0.1.5/src/tendril/apiserver/routers/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.131695 tendril-iotedge-0.1.5/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.131695 tendril-iotedge-0.1.5/src/tendril/common/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 15:45:45.000000 tendril-iotedge-0.1.5/src/tendril/common/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril-iotedge-0.1.5/src/tendril/common/iotcore/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.135695 tendril-iotedge-0.1.5/src/tendril/common/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/common/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/common/iotedge/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      759 2023-04-05 04:03:03.000000 tendril-iotedge-0.1.5/src/tendril/common/iotedge/formats.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.135695 tendril-iotedge-0.1.5/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril-iotedge-0.1.5/src/tendril/config/iotedge.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.139695 tendril-iotedge-0.1.5/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.139695 tendril-iotedge-0.1.5/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4351 2023-04-05 17:19:08.000000 tendril-iotedge-0.1.5/src/tendril/db/models/deviceconfig.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.139695 tendril-iotedge-0.1.5/src/tendril/iotcore/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril-iotedge-0.1.5/src/tendril/iotcore/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1074 2023-04-05 18:01:28.000000 tendril-iotedge-0.1.5/src/tendril/iotcore/settings.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.147695 tendril-iotedge-0.1.5/src/tendril/iotedge/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2670 2023-04-03 17:43:43.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/announce.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      422 2023-04-05 04:43:55.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/config.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/heartbeat.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.151695 tendril-iotedge-0.1.5/src/tendril/iotedge/profiles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/profiles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      963 2023-04-05 18:20:26.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/profiles/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3655 2023-04-05 16:24:45.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/profiles/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.5/src/tendril/iotedge/registration.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.155695 tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-04-07 02:36:08.000000 tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1534 2023-04-07 02:36:09.000000 tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-07 02:36:08.000000 tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-07 02:36:08.000000 tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-07 02:36:08.000000 tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-07 02:36:09.155695 tendril-iotedge-0.1.5/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.5/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.299721 tendril-iotedge-0.1.6/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-04-12 18:22:05.299721 tendril-iotedge-0.1.6/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2192 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.231723 tendril-iotedge-0.1.6/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.243723 tendril-iotedge-0.1.6/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.243723 tendril-iotedge-0.1.6/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.243723 tendril-iotedge-0.1.6/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13460 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1536 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.247723 tendril-iotedge-0.1.6/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-12 18:22:05.303721 tendril-iotedge-0.1.6/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3214 2023-03-16 07:26:30.000000 tendril-iotedge-0.1.6/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.215724 tendril-iotedge-0.1.6/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.247723 tendril-iotedge-0.1.6/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.251723 tendril-iotedge-0.1.6/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.255723 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1855 2023-04-05 18:31:23.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotcore.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2266 2023-04-05 09:34:19.000000 tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.255723 tendril-iotedge-0.1.6/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.259723 tendril-iotedge-0.1.6/src/tendril/common/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 15:45:45.000000 tendril-iotedge-0.1.6/src/tendril/common/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       54 2023-04-05 15:48:55.000000 tendril-iotedge-0.1.6/src/tendril/common/iotcore/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.263723 tendril-iotedge-0.1.6/src/tendril/common/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/common/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/common/iotedge/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      733 2023-04-12 18:16:23.000000 tendril-iotedge-0.1.6/src/tendril/common/iotedge/formats.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.267722 tendril-iotedge-0.1.6/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1830 2023-03-28 11:11:29.000000 tendril-iotedge-0.1.6/src/tendril/config/iotedge.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.267722 tendril-iotedge-0.1.6/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.271722 tendril-iotedge-0.1.6/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4351 2023-04-05 17:19:08.000000 tendril-iotedge-0.1.6/src/tendril/db/models/deviceconfig.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.275722 tendril-iotedge-0.1.6/src/tendril/iotcore/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-05 16:12:42.000000 tendril-iotedge-0.1.6/src/tendril/iotcore/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1037 2023-04-08 07:05:40.000000 tendril-iotedge-0.1.6/src/tendril/iotcore/settings.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.279722 tendril-iotedge-0.1.6/src/tendril/iotedge/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2636 2023-04-12 18:17:22.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/announce.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      422 2023-04-05 04:43:55.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/config.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/heartbeat.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.287721 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      258 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      963 2023-04-05 18:20:26.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4026 2023-04-08 07:11:19.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1980 2023-04-03 17:40:48.000000 tendril-iotedge-0.1.6/src/tendril/iotedge/registration.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.291721 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3485 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1534 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      565 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-12 18:22:04.000000 tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 18:22:05.295721 tendril-iotedge-0.1.6/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-03-15 16:03:10.000000 tendril-iotedge-0.1.6/tox.ini
```

### Comparing `tendril-iotedge-0.1.5/.gitignore` & `tendril-iotedge-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/.readthedocs.yml` & `tendril-iotedge-0.1.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/.travis.yml` & `tendril-iotedge-0.1.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/LICENSE` & `tendril-iotedge-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/PKG-INFO` & `tendril-iotedge-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril-iotedge-0.1.5/README.rst` & `tendril-iotedge-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/Makefile` & `tendril-iotedge-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/_static/custom.css` & `tendril-iotedge-0.1.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/_static/favicon.ico` & `tendril-iotedge-0.1.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/_static/logo.png` & `tendril-iotedge-0.1.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/_static/logo_packed.png` & `tendril-iotedge-0.1.6/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/_templates/about.html` & `tendril-iotedge-0.1.6/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/conf.py` & `tendril-iotedge-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/index.rst` & `tendril-iotedge-0.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/docs/installation.rst` & `tendril-iotedge-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/setup.py` & `tendril-iotedge-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/apiserver/routers/iotcore.py` & `tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotcore.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/apiserver/routers/iotedge.py` & `tendril-iotedge-0.1.6/src/tendril/apiserver/routers/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/common/iotedge/exceptions.py` & `tendril-iotedge-0.1.6/src/tendril/common/iotedge/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/common/iotedge/formats.py` & `tendril-iotedge-0.1.6/src/tendril/common/iotedge/formats.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 from typing import Literal
 from typing import Optional
 from tendril.utils.pydantic import TendrilTBaseModel
-from tendril.common.interests.states import InterestLifecycleStatus
+from tendril.common.states import LifecycleStatus
 
 
 IoTDeviceIDTModel = str
 IoTDeviceAppnameTModel = str
 
 
 class IoTDeviceMessageTModel(TendrilTBaseModel):
@@ -20,14 +20,14 @@
 
 
 class IoTDevicePingTModel(IoTDeviceMessageTModel):
     status: Optional[dict]
 
 
 class IoTDeviceAnnounceResponseTModel(IoTDeviceMessageTModel):
-    status: InterestLifecycleStatus
+    status: LifecycleStatus
     interest_id: int
     password: Optional[str]
 
 
 class IoTDeviceSettingRequestTModel(IoTDeviceMessageTModel):
     appname: IoTDeviceAppnameTModel
```

### Comparing `tendril-iotedge-0.1.5/src/tendril/config/__init__.py` & `tendril-iotedge-0.1.6/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/config/iotedge.py` & `tendril-iotedge-0.1.6/src/tendril/config/iotedge.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/db/models/deviceconfig.py` & `tendril-iotedge-0.1.6/src/tendril/db/models/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/iotcore/settings.py` & `tendril-iotedge-0.1.6/src/tendril/iotcore/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 
 from tendril.libraries import interests
-from tendril.iotedge import profiles
 from tendril.common.interests.exceptions import InterestTypeUnsupported
 
 from tendril.utils.db import with_db
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
```

### Comparing `tendril-iotedge-0.1.5/src/tendril/iotedge/announce.py` & `tendril-iotedge-0.1.6/src/tendril/iotedge/announce.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
 from tendril.caching import transit
-from tendril.common.interests.states import InterestLifecycleStatus
+from tendril.common.states import LifecycleStatus
 
 from .registration import get_registration
 from .registration import register
 
 from tendril.utils.db import with_db
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
@@ -15,15 +15,15 @@
 def announce_device(device_id, appname, have_credentials, session=None):
     # TODO Handle other device lifecycle states
     rv = {}
     device = get_registration(device_id, appname, session=session)
     if device:
         logger.debug(f"Got announce from a registered device {device_id} "
                      f"in state {device.model_instance.status}.")
-        if device.model_instance.status == InterestLifecycleStatus.ACTIVE:
+        if device.model_instance.status == LifecycleStatus.ACTIVE:
             if not have_credentials:
                 # If there is a password waiting for one-time transmission,
                 # transmit it.
                 password = transit.read(namespace="ott:dp", key=device_id)
                 if not password:
                     logger.warning(f"Active registered device {device_id} does not have a token")
                     # If there is no password waiting for one-time transmission,
@@ -31,15 +31,15 @@
                     # manually reset password and load it up for one-time transmission.
                     # Raise manual password reset request here. Changing device status to
                     # NEW should get the job done as presently implemented.
                 else:
                     logger.info(f"Found password for {device_id} on transit cache.")
                     transit.delete(namespace="ott:dp", key=device_id)
                     rv['password'] = password
-        if device.model_instance.status == InterestLifecycleStatus.NEW:
+        if device.model_instance.status == LifecycleStatus.NEW:
             # We're waiting for activation and don't need to do anything here.
             pass
     else:
         logger.info(f"Registering new device '{device_id}' "
                     f"of type '{appname}' from announce.")
         if have_credentials:
             logger.warning(f"Unregistered device {device_id} seems to already have a token")
```

### Comparing `tendril-iotedge-0.1.5/src/tendril/iotedge/heartbeat.py` & `tendril-iotedge-0.1.6/src/tendril/iotedge/heartbeat.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/iotedge/profiles/base.py` & `tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/base.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril/iotedge/profiles/manager.py` & `tendril-iotedge-0.1.6/src/tendril/iotedge/profiles/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 import importlib
 from typing import Union
 from pydantic import Field
 from typing_extensions import Annotated
 
 from tendril.utils.versions import get_namespace_package_names
+from tendril.iotedge.profiles.base import DeviceConfigurationModel
 from tendril.common.iotedge.exceptions import DeviceTypeUnrecognized
 
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEBUG)
 
 
 class IoTDeviceProfilesManager(object):
@@ -77,16 +78,23 @@
         try:
             return self._device_profiles[appname]
         except KeyError:
             raise DeviceTypeUnrecognized(appname, device_id)
 
     def finalize(self):
         logger.info("Building device configuration message models")
-        self.device_config_unified_model = Annotated[Union[tuple(self.device_config_tmodels.values())],
-                                                     Field(discriminator='appname')]
+        if len(self.device_profiles) > 1:
+            self.device_config_unified_model = \
+                Annotated[Union[tuple(self.device_config_tmodels.values())],
+                          Field(discriminator='appname')]
+        elif len(self.device_profiles) == 1:
+            self.device_config_unified_model = \
+                list(self._device_profiles.values())[0].config_model.tmodel()
+        else:
+            self.device_config_unified_model = DeviceConfigurationModel.tmodel()
 
     def __getattr__(self, item):
         if item == '__file__':
             return None
         if item == '__path__':
             return None
         if item == '__len__':
```

### Comparing `tendril-iotedge-0.1.5/src/tendril/iotedge/registration.py` & `tendril-iotedge-0.1.6/src/tendril/iotedge/registration.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/PKG-INFO` & `tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-iotedge
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tendril IoT Edge Server Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-iotedge
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-iotedge.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-iotedge/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-iotedge
```

### Comparing `tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/SOURCES.txt` & `tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/src/tendril_iotedge.egg-info/requires.txt` & `tendril-iotedge-0.1.6/src/tendril_iotedge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/tests/coveralls.py` & `tendril-iotedge-0.1.6/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-iotedge-0.1.5/tox.ini` & `tendril-iotedge-0.1.6/tox.ini`

 * *Files identical despite different names*

