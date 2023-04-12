# Comparing `tmp/spade_artifact-0.1.1.tar.gz` & `tmp/spade_artifact-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spade_artifact-0.1.1.tar", last modified: Mon Jul  5 12:30:56 2021, max compression
+gzip compressed data, was "spade_artifact-0.1.2.tar", last modified: Wed Apr 12 13:15:53 2023, max compression
```

## Comparing `spade_artifact-0.1.1.tar` & `spade_artifact-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/
--rw-r--r--   0 jpalanca   (501) staff       (20)      158 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/AUTHORS.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     3602 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      158 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/HISTORY.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/LICENSE
--rw-r--r--   0 jpalanca   (501) staff       (20)      317 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/MANIFEST.in
--rw-r--r--   0 jpalanca   (501) staff       (20)     2290 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)     1062 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/README.rst
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/docs/
--rw-r--r--   0 jpalanca   (501) staff       (20)      615 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/docs/Makefile
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/docs/_build/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/docs/_build/html/
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/docs/_build/html/_static/
--rw-r--r--   0 jpalanca   (501) staff       (20)      286 2021-04-16 14:05:14.000000 spade_artifact-0.1.1/docs/_build/html/_static/file.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2021-04-16 14:05:14.000000 spade_artifact-0.1.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       90 2021-04-16 14:05:14.000000 spade_artifact-0.1.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 jpalanca   (501) staff       (20)       85 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/docs/api.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/docs/authors.rst
--rwxr-xr-x   0 jpalanca   (501) staff       (20)     4907 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/docs/conf.py
--rw-r--r--   0 jpalanca   (501) staff       (20)       33 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/docs/contributing.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       28 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/docs/history.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      307 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/docs/index.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     1182 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/docs/installation.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      776 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/docs/make.bat
--rw-r--r--   0 jpalanca   (501) staff       (20)       79 2021-07-05 12:24:36.000000 spade_artifact-0.1.1/docs/modules.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       27 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/docs/readme.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)      501 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/docs/spade_artifact.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)     4736 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/docs/usage.rst
--rw-r--r--   0 jpalanca   (501) staff       (20)       46 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/requirements.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)      448 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/requirements_dev.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)      457 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/setup.cfg
--rw-r--r--   0 jpalanca   (501) staff       (20)     1574 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/setup.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/spade_artifact/
--rw-r--r--   0 jpalanca   (501) staff       (20)      223 2021-07-05 12:30:21.000000 spade_artifact-0.1.1/spade_artifact/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     1427 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/spade_artifact/agent.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    10758 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/spade_artifact/artifact.py
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/spade_artifact.egg-info/
--rw-r--r--   0 jpalanca   (501) staff       (20)     2290 2021-07-05 12:30:55.000000 spade_artifact-0.1.1/spade_artifact.egg-info/PKG-INFO
--rw-r--r--   0 jpalanca   (501) staff       (20)      881 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/spade_artifact.egg-info/SOURCES.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2021-07-05 12:30:55.000000 spade_artifact-0.1.1/spade_artifact.egg-info/dependency_links.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)        1 2021-07-05 12:30:55.000000 spade_artifact-0.1.1/spade_artifact.egg-info/not-zip-safe
--rw-r--r--   0 jpalanca   (501) staff       (20)       47 2021-07-05 12:30:55.000000 spade_artifact-0.1.1/spade_artifact.egg-info/requires.txt
--rw-r--r--   0 jpalanca   (501) staff       (20)       15 2021-07-05 12:30:55.000000 spade_artifact-0.1.1/spade_artifact.egg-info/top_level.txt
-drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2021-07-05 12:30:56.000000 spade_artifact-0.1.1/tests/
--rw-r--r--   0 jpalanca   (501) staff       (20)        0 2021-04-16 09:57:27.000000 spade_artifact-0.1.1/tests/__init__.py
--rw-r--r--   0 jpalanca   (501) staff       (20)      325 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/tests/conftest.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     2367 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/tests/factories.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     2369 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/tests/test_agent_mixin.py
--rw-r--r--   0 jpalanca   (501) staff       (20)     2959 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/tests/test_artifact.py
--rw-r--r--   0 jpalanca   (501) staff       (20)    15071 2021-07-05 12:17:06.000000 spade_artifact-0.1.1/tests/test_presence.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.459613 spade_artifact-0.1.2/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      158 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/AUTHORS.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     3602 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      222 2023-04-12 13:08:38.000000 spade_artifact-0.1.2/HISTORY.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1071 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/LICENSE
+-rw-r--r--   0 jpalanca   (501) staff       (20)      317 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/MANIFEST.in
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2102 2023-04-12 13:15:53.459911 spade_artifact-0.1.2/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1062 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/README.rst
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.447420 spade_artifact-0.1.2/docs/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      615 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/docs/Makefile
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.432930 spade_artifact-0.1.2/docs/_build/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.433222 spade_artifact-0.1.2/docs/_build/html/
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.449464 spade_artifact-0.1.2/docs/_build/html/_static/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      286 2021-04-16 14:05:14.000000 spade_artifact-0.1.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2021-04-16 14:05:14.000000 spade_artifact-0.1.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       90 2021-04-16 14:05:14.000000 spade_artifact-0.1.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jpalanca   (501) staff       (20)       85 2021-07-05 12:30:21.000000 spade_artifact-0.1.2/docs/api.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 jpalanca   (501) staff       (20)     4907 2021-07-05 12:30:21.000000 spade_artifact-0.1.2/docs/conf.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)       33 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/docs/contributing.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       28 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/docs/history.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      307 2021-07-05 12:30:21.000000 spade_artifact-0.1.2/docs/index.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1182 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/docs/installation.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      776 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/docs/make.bat
+-rw-r--r--   0 jpalanca   (501) staff       (20)       79 2021-07-05 12:24:36.000000 spade_artifact-0.1.2/docs/modules.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       27 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/docs/readme.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)      501 2021-07-05 12:30:21.000000 spade_artifact-0.1.2/docs/spade_artifact.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)     4736 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/docs/usage.rst
+-rw-r--r--   0 jpalanca   (501) staff       (20)       46 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/requirements.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      425 2023-04-12 13:08:32.000000 spade_artifact-0.1.2/requirements_dev.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)      457 2023-04-12 13:15:53.461629 spade_artifact-0.1.2/setup.cfg
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1722 2023-04-12 13:08:38.000000 spade_artifact-0.1.2/setup.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.451222 spade_artifact-0.1.2/spade_artifact/
+-rw-r--r--   0 jpalanca   (501) staff       (20)      223 2023-04-12 13:08:38.000000 spade_artifact-0.1.2/spade_artifact/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     1427 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/spade_artifact/agent.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    10461 2023-04-12 13:08:32.000000 spade_artifact-0.1.2/spade_artifact/artifact.py
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.455103 spade_artifact-0.1.2/spade_artifact.egg-info/
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2102 2023-04-12 13:15:53.000000 spade_artifact-0.1.2/spade_artifact.egg-info/PKG-INFO
+-rw-r--r--   0 jpalanca   (501) staff       (20)      881 2023-04-12 13:15:53.000000 spade_artifact-0.1.2/spade_artifact.egg-info/SOURCES.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-04-12 13:15:53.000000 spade_artifact-0.1.2/spade_artifact.egg-info/dependency_links.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)        1 2023-04-12 13:15:53.000000 spade_artifact-0.1.2/spade_artifact.egg-info/not-zip-safe
+-rw-r--r--   0 jpalanca   (501) staff       (20)       47 2023-04-12 13:15:53.000000 spade_artifact-0.1.2/spade_artifact.egg-info/requires.txt
+-rw-r--r--   0 jpalanca   (501) staff       (20)       15 2023-04-12 13:15:53.000000 spade_artifact-0.1.2/spade_artifact.egg-info/top_level.txt
+drwxr-xr-x   0 jpalanca   (501) staff       (20)        0 2023-04-12 13:15:53.459056 spade_artifact-0.1.2/tests/
+-rw-r--r--   0 jpalanca   (501) staff       (20)        0 2021-04-16 09:57:27.000000 spade_artifact-0.1.2/tests/__init__.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)      325 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/tests/conftest.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2367 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/tests/factories.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2369 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/tests/test_agent_mixin.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)     2959 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/tests/test_artifact.py
+-rw-r--r--   0 jpalanca   (501) staff       (20)    15071 2021-07-05 12:17:06.000000 spade_artifact-0.1.2/tests/test_presence.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spade_artifact-0.1.1/CONTRIBUTING.rst` & `spade_artifact-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/LICENSE` & `spade_artifact-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/PKG-INFO` & `spade_artifact-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,85 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: spade_artifact
-Version: 0.1.1
+Version: 0.1.2
 Summary: Plugin for SPADE 3 to develop artifacts.
 Home-page: https://github.com/javipalanca/spade_artifact
 Author: Javi Palanca
 Author-email: jpalanca@gmail.com
 License: MIT license
-Description: ==============
-        spade-artifact
-        ==============
-        
-        
-        .. image:: https://img.shields.io/pypi/v/spade_artifact.svg
-                :target: https://pypi.python.org/pypi/spade_artifact
-        
-        .. image:: https://img.shields.io/travis/javipalanca/spade_artifact.svg
-                :target: https://travis-ci.org/javipalanca/spade_artifact
-        
-        .. image:: https://readthedocs.org/projects/spade-artifact/badge/?version=latest
-                :target: https://spade-artifact.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Plugin for SPADE 3 to develop artifacts.
-        
-        
-        * Free software: MIT license
-        * Documentation: https://spade-artifact.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * Focus on observable properties (based on PubSub).
-        * Presence notifiaction support.
-        * Artifact class.
-        * ArtifactMixin for SPADE agents.
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.1 (2021-07-05)
-        ------------------
-        
-        * Fixed documentation style.
-        
-        0.1.0 (2021-07-05)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: spade_artifact
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+==============
+spade-artifact
+==============
+
+
+.. image:: https://img.shields.io/pypi/v/spade_artifact.svg
+        :target: https://pypi.python.org/pypi/spade_artifact
+
+.. image:: https://img.shields.io/travis/javipalanca/spade_artifact.svg
+        :target: https://travis-ci.org/javipalanca/spade_artifact
+
+.. image:: https://readthedocs.org/projects/spade-artifact/badge/?version=latest
+        :target: https://spade-artifact.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+Plugin for SPADE 3 to develop artifacts.
+
+
+* Free software: MIT license
+* Documentation: https://spade-artifact.readthedocs.io.
+
+
+Features
+--------
+
+* Focus on observable properties (based on PubSub).
+* Presence notifiaction support.
+* Artifact class.
+* ArtifactMixin for SPADE agents.
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.2 (2023-04-12)
+------------------
+
+* Added abstract class.
+
+0.1.1 (2021-07-05)
+------------------
+
+* Fixed documentation style.
+
+0.1.0 (2021-07-05)
+------------------
+
+* First release on PyPI.
+
+
```

### Comparing `spade_artifact-0.1.1/README.rst` & `spade_artifact-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/docs/Makefile` & `spade_artifact-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/docs/conf.py` & `spade_artifact-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/docs/installation.rst` & `spade_artifact-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/docs/make.bat` & `spade_artifact-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/docs/usage.rst` & `spade_artifact-0.1.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/setup.py` & `spade_artifact-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,23 +35,26 @@
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     description="Plugin for SPADE 3 to develop artifacts.",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="spade_artifact",
     name="spade_artifact",
     packages=find_packages(include=["spade_artifact"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/javipalanca/spade_artifact",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `spade_artifact-0.1.1/spade_artifact/agent.py` & `spade_artifact-0.1.2/spade_artifact/agent.py`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/spade_artifact/artifact.py` & `spade_artifact-0.1.2/spade_artifact/artifact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 # -*- coding: utf-8 -*-
+import abc
 import asyncio
 import logging
 import sys
 import time
 from asyncio import Event
-from contextlib import suppress
 from typing import Union
 
 import aiosasl
 import aioxmpp
 from aiosasl import AuthenticationFailure
 from aioxmpp import ibr, XMPPCancelError, XMPPAuthError
 from aioxmpp.dispatcher import SimpleMessageDispatcher
 from loguru import logger
 from spade.container import Container
 from spade.message import Message
 from spade.presence import PresenceManager
 from spade_pubsub import PubSubMixin
 
 
-class Artifact(PubSubMixin):
+class AbstractArtifact(object, metaclass=abc.ABCMeta):
+    async def _hook_plugin_before_connection(self, *args, **kwargs):
+        """
+        Overload this method to hook a plugin before connection is done
+        """
+        pass
+
+    async def _hook_plugin_after_connection(self, *args, **kwargs):
+        """
+        Overload this method to hook a plugin after connection is done
+        """
+        pass
+
+
+class Artifact(PubSubMixin, AbstractArtifact):
     def __init__(self, jid, password, pubsub_server=None, verify_security=False):
         """
         Creates an artifact
 
         Args:
           jid (str): The identifier of the artifact in the form username@server
           password (str): The password to connect to the server
@@ -130,32 +144,14 @@
             logger.error(f"Artifact {self._node} is not allowed to publish properties.")
             raise e
 
         await self.setup()
         self._alive.set()
         asyncio.run_coroutine_threadsafe(self.run(), loop=self.loop)
 
-    async def _hook_plugin_before_connection(self, *args, **kwargs):
-        """
-        Overload this method to hook a plugin before connetion is done
-        """
-        try:
-            await super()._hook_plugin_before_connection(*args, **kwargs)
-        except AttributeError:
-            logger.debug("_hook_plugin_before_connection is undefined")
-
-    async def _hook_plugin_after_connection(self, *args, **kwargs):
-        """
-        Overload this method to hook a plugin after connetion is done
-        """
-        try:
-            await super()._hook_plugin_after_connection(*args, **kwargs)
-        except AttributeError:
-            logger.debug("_hook_plugin_after_connection is undefined")
-
     async def _async_connect(self):  # pragma: no cover
         """ connect and authenticate to the XMPP server. Async mode. """
         try:
             self.conn_coro = self.client.connected()
             aenter = type(self.conn_coro).__aenter__(self.conn_coro)
             self.stream = await aenter
             logger.info(f"Artifact {str(self.jid)} connected and authenticated.")
```

### Comparing `spade_artifact-0.1.1/spade_artifact.egg-info/SOURCES.txt` & `spade_artifact-0.1.2/spade_artifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/tests/factories.py` & `spade_artifact-0.1.2/tests/factories.py`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/tests/test_agent_mixin.py` & `spade_artifact-0.1.2/tests/test_agent_mixin.py`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/tests/test_artifact.py` & `spade_artifact-0.1.2/tests/test_artifact.py`

 * *Files identical despite different names*

### Comparing `spade_artifact-0.1.1/tests/test_presence.py` & `spade_artifact-0.1.2/tests/test_presence.py`

 * *Files identical despite different names*

