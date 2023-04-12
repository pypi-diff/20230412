# Comparing `tmp/napari-bigfish-0.1.tar.gz` & `tmp/napari-bigfish-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bigfish-0.1.tar", last modified: Fri Apr  7 16:03:57 2023, max compression
+gzip compressed data, was "napari-bigfish-0.2.tar", last modified: Wed Apr 12 08:49:48 2023, max compression
```

## Comparing `napari-bigfish-0.1.tar` & `napari-bigfish-0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/.github/
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/.github/workflows/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     2814 2023-02-25 23:33:23.000000 napari-bigfish-0.1/.github/workflows/test_and_deploy.yml
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      992 2023-02-25 23:33:23.000000 napari-bigfish-0.1/.gitignore
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/.napari-hub/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      463 2023-02-25 23:33:23.000000 napari-bigfish-0.1/.napari-hub/DESCRIPTION.md
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      542 2023-02-25 23:33:23.000000 napari-bigfish-0.1/.napari-hub/config.yml
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1169 2023-02-25 23:33:23.000000 napari-bigfish-0.1/.pre-commit-config.yaml
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1082 2023-02-25 23:33:23.000000 napari-bigfish-0.1/LICENSE
--rw-rw-r--   0 baecker   (1000) baecker   (1000)       96 2023-02-25 23:33:23.000000 napari-bigfish-0.1/MANIFEST.in
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     4005 2023-04-07 16:03:57.155673 napari-bigfish-0.1/PKG-INFO
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     3051 2023-03-22 13:11:54.000000 napari-bigfish-0.1/README.md
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/docs/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      638 2023-03-31 14:32:04.000000 napari-bigfish-0.1/docs/Makefile
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      804 2023-03-31 14:32:04.000000 napari-bigfish-0.1/docs/make.bat
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/docs/source/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1959 2023-03-31 15:26:32.000000 napari-bigfish-0.1/docs/source/conf.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      139 2023-04-07 14:14:59.000000 napari-bigfish-0.1/docs/source/index.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)       85 2023-04-07 14:14:48.000000 napari-bigfish-0.1/docs/source/modules.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      167 2023-04-04 12:08:46.000000 napari-bigfish-0.1/docs/source/napari_bigfish.array_util.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      165 2023-04-04 12:08:46.000000 napari-bigfish-0.1/docs/source/napari_bigfish.bigfishapp.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      170 2023-04-04 12:08:46.000000 napari-bigfish-0.1/docs/source/napari_bigfish.napari_util.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      153 2023-04-04 12:08:46.000000 napari-bigfish-0.1/docs/source/napari_bigfish.qtutil.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      334 2023-04-04 12:08:46.000000 napari-bigfish-0.1/docs/source/napari_bigfish.rst
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/docs/source/user/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1957 2023-04-06 16:37:08.000000 napari-bigfish-0.1/docs/source/user/batch_processing.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      477 2023-04-04 16:06:52.000000 napari-bigfish-0.1/docs/source/user/installation.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1202 2023-04-04 15:27:17.000000 napari-bigfish-0.1/docs/source/user/introduction.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     5916 2023-04-05 15:50:47.000000 napari-bigfish-0.1/docs/source/user/spot_detection.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      139 2023-04-04 14:58:48.000000 napari-bigfish-0.1/docs/source/user/user_documentation.rst
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      315 2023-04-07 16:03:53.000000 napari-bigfish-0.1/pyproject.toml
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1447 2023-04-07 16:03:57.155673 napari-bigfish-0.1/setup.cfg
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/src/
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/src/napari_bigfish/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      318 2023-03-22 13:23:02.000000 napari-bigfish-0.1/src/napari_bigfish/__init__.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1536 2023-04-07 13:18:09.000000 napari-bigfish-0.1/src/napari_bigfish/_sample_data.py
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/src/napari_bigfish/_tests/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)        0 2023-02-25 23:33:23.000000 napari-bigfish-0.1/src/napari_bigfish/_tests/__init__.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      383 2023-03-29 12:37:31.000000 napari-bigfish-0.1/src/napari_bigfish/_tests/test_array_util.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     4739 2023-03-31 13:57:30.000000 napari-bigfish-0.1/src/napari_bigfish/_tests/test_bigfishapp.py
--rw-r--r--   0 baecker   (1000) baecker   (1000)      605 2023-03-29 12:37:31.000000 napari-bigfish-0.1/src/napari_bigfish/_tests/test_napari_util.py
--rw-r--r--   0 baecker   (1000) baecker   (1000)     2768 2023-03-29 12:37:31.000000 napari-bigfish-0.1/src/napari_bigfish/_tests/test_qtutil.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      192 2023-03-22 10:21:19.000000 napari-bigfish-0.1/src/napari_bigfish/_tests/test_sample_data.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)    21669 2023-03-31 13:47:36.000000 napari-bigfish-0.1/src/napari_bigfish/_tests/test_widget.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      209 2023-04-07 16:03:57.000000 napari-bigfish-0.1/src/napari_bigfish/_version.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)    38099 2023-04-07 13:52:21.000000 napari-bigfish-0.1/src/napari_bigfish/_widget.py
--rw-r--r--   0 baecker   (1000) baecker   (1000)     1531 2023-04-04 12:04:30.000000 napari-bigfish-0.1/src/napari_bigfish/array_util.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)    14682 2023-04-04 12:00:28.000000 napari-bigfish-0.1/src/napari_bigfish/bigfishapp.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      623 2023-03-02 10:29:54.000000 napari-bigfish-0.1/src/napari_bigfish/napari.yaml
--rw-r--r--   0 baecker   (1000) baecker   (1000)     1591 2023-04-04 09:30:06.000000 napari-bigfish-0.1/src/napari_bigfish/napari_util.py
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     5491 2023-03-29 16:05:09.000000 napari-bigfish-0.1/src/napari_bigfish/qtutil.py
-drwxrwxr-x   0 baecker   (1000) baecker   (1000)        0 2023-04-07 16:03:57.155673 napari-bigfish-0.1/src/napari_bigfish.egg-info/
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     4005 2023-04-07 16:03:57.000000 napari-bigfish-0.1/src/napari_bigfish.egg-info/PKG-INFO
--rw-rw-r--   0 baecker   (1000) baecker   (1000)     1500 2023-04-07 16:03:57.000000 napari-bigfish-0.1/src/napari_bigfish.egg-info/SOURCES.txt
--rw-rw-r--   0 baecker   (1000) baecker   (1000)        1 2023-04-07 16:03:57.000000 napari-bigfish-0.1/src/napari_bigfish.egg-info/dependency_links.txt
--rw-rw-r--   0 baecker   (1000) baecker   (1000)       62 2023-04-07 16:03:57.000000 napari-bigfish-0.1/src/napari_bigfish.egg-info/entry_points.txt
--rw-rw-r--   0 baecker   (1000) baecker   (1000)       95 2023-04-07 16:03:57.000000 napari-bigfish-0.1/src/napari_bigfish.egg-info/requires.txt
--rw-rw-r--   0 baecker   (1000) baecker   (1000)       15 2023-04-07 16:03:57.000000 napari-bigfish-0.1/src/napari_bigfish.egg-info/top_level.txt
--rw-rw-r--   0 baecker   (1000) baecker   (1000)      613 2023-02-25 23:33:23.000000 napari-bigfish-0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.548974 napari-bigfish-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.540974 napari-bigfish-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.544974 napari-bigfish-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-12 08:49:31.000000 napari-bigfish-0.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-12 08:49:31.000000 napari-bigfish-0.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.544974 napari-bigfish-0.2/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 08:49:31.000000 napari-bigfish-0.2/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 08:49:31.000000 napari-bigfish-0.2/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-12 08:49:31.000000 napari-bigfish-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-12 08:49:31.000000 napari-bigfish-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 08:49:31.000000 napari-bigfish-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-12 08:49:48.548974 napari-bigfish-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-12 08:49:31.000000 napari-bigfish-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.544974 napari-bigfish-0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.544974 napari-bigfish-0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/napari_bigfish.array_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/napari_bigfish.bigfishapp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/napari_bigfish.napari_util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/napari_bigfish.qtutil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/napari_bigfish.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.544974 napari-bigfish-0.2/docs/source/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/user/batch_processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/user/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/user/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/user/spot_detection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 08:49:31.000000 napari-bigfish-0.2/docs/source/user/user_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 08:49:31.000000 napari-bigfish-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-12 08:49:48.548974 napari-bigfish-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.540974 napari-bigfish-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.548974 napari-bigfish-0.2/src/napari_bigfish/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.548974 napari-bigfish-0.2/src/napari_bigfish/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_tests/test_array_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_tests/test_bigfishapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_tests/test_napari_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_tests/test_qtutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 08:49:48.000000 napari-bigfish-0.2/src/napari_bigfish/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38099 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/array_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/bigfishapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/napari_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-12 08:49:31.000000 napari-bigfish-0.2/src/napari_bigfish/qtutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:48.548974 napari-bigfish-0.2/src/napari_bigfish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-12 08:49:48.000000 napari-bigfish-0.2/src/napari_bigfish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-12 08:49:48.000000 napari-bigfish-0.2/src/napari_bigfish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:49:48.000000 napari-bigfish-0.2/src/napari_bigfish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 08:49:48.000000 napari-bigfish-0.2/src/napari_bigfish.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 08:49:48.000000 napari-bigfish-0.2/src/napari_bigfish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 08:49:48.000000 napari-bigfish-0.2/src/napari_bigfish.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 08:49:31.000000 napari-bigfish-0.2/tox.ini
```

### Comparing `napari-bigfish-0.1/.github/workflows/test_and_deploy.yml` & `napari-bigfish-0.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/.gitignore` & `napari-bigfish-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/.napari-hub/config.yml` & `napari-bigfish-0.2/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/.pre-commit-config.yaml` & `napari-bigfish-0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/LICENSE` & `napari-bigfish-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/PKG-INFO` & `napari-bigfish-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bigfish
-Version: 0.1
+Version: 0.2
 Summary: A napari-plugin providing an alternative GUI for Big-FISH. Big-FISH is a python package for the analysis of smFISH images.
 Author: Volker Baecker
 Author-email: volker.baecker@mri.cnrs.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-bigfish-0.1/README.md` & `napari-bigfish-0.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/docs/Makefile` & `napari-bigfish-0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/docs/make.bat` & `napari-bigfish-0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/docs/source/conf.py` & `napari-bigfish-0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/docs/source/user/batch_processing.rst` & `napari-bigfish-0.2/docs/source/user/batch_processing.rst`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/docs/source/user/introduction.rst` & `napari-bigfish-0.2/docs/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/docs/source/user/spot_detection.rst` & `napari-bigfish-0.2/docs/source/user/spot_detection.rst`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/setup.cfg` & `napari-bigfish-0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/_sample_data.py` & `napari-bigfish-0.2/src/napari_bigfish/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/_tests/test_bigfishapp.py` & `napari-bigfish-0.2/src/napari_bigfish/_tests/test_bigfishapp.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/_tests/test_napari_util.py` & `napari-bigfish-0.2/src/napari_bigfish/_tests/test_napari_util.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/_tests/test_qtutil.py` & `napari-bigfish-0.2/src/napari_bigfish/_tests/test_qtutil.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/_tests/test_widget.py` & `napari-bigfish-0.2/src/napari_bigfish/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/_widget.py` & `napari-bigfish-0.2/src/napari_bigfish/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/array_util.py` & `napari-bigfish-0.2/src/napari_bigfish/array_util.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/bigfishapp.py` & `napari-bigfish-0.2/src/napari_bigfish/bigfishapp.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/napari.yaml` & `napari-bigfish-0.2/src/napari_bigfish/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/napari_util.py` & `napari-bigfish-0.2/src/napari_bigfish/napari_util.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish/qtutil.py` & `napari-bigfish-0.2/src/napari_bigfish/qtutil.py`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/src/napari_bigfish.egg-info/PKG-INFO` & `napari-bigfish-0.2/src/napari_bigfish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bigfish
-Version: 0.1
+Version: 0.2
 Summary: A napari-plugin providing an alternative GUI for Big-FISH. Big-FISH is a python package for the analysis of smFISH images.
 Author: Volker Baecker
 Author-email: volker.baecker@mri.cnrs.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
```

### Comparing `napari-bigfish-0.1/src/napari_bigfish.egg-info/SOURCES.txt` & `napari-bigfish-0.2/src/napari_bigfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-bigfish-0.1/tox.ini` & `napari-bigfish-0.2/tox.ini`

 * *Files identical despite different names*

