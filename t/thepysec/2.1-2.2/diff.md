# Comparing `tmp/thepysec-2.1.tar.gz` & `tmp/thepysec-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepysec-2.1.tar", last modified: Tue Mar  1 17:22:23 2022, max compression
+gzip compressed data, was "thepysec-2.2.tar", last modified: Wed Apr 12 10:46:27 2023, max compression
```

## Comparing `thepysec-2.1.tar` & `thepysec-2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2022-03-01 17:22:23.052265 thepysec-2.1/
--rw-r--r--   0 carmen    (1000) carmen    (1000)     1523 2022-03-01 17:02:48.000000 thepysec-2.1/LICENSE
--rw-r--r--   0 carmen    (1000) carmen    (1000)     2526 2022-03-01 17:22:23.052265 thepysec-2.1/PKG-INFO
--rw-r--r--   0 carmen    (1000) carmen    (1000)     1591 2022-03-01 17:20:16.000000 thepysec-2.1/README.md
--rw-r--r--   0 carmen    (1000) carmen    (1000)      342 2022-03-01 17:22:23.052265 thepysec-2.1/setup.cfg
--rw-r--r--   0 carmen    (1000) carmen    (1000)     1511 2022-03-01 17:02:48.000000 thepysec-2.1/setup.py
-drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2022-03-01 17:22:23.048264 thepysec-2.1/thepysec/
--rw-r--r--   0 carmen    (1000) carmen    (1000)      497 2022-03-01 17:20:16.000000 thepysec-2.1/thepysec/__init__.py
-drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2022-03-01 17:22:23.052265 thepysec-2.1/thepysec/john/
--rw-r--r--   0 carmen    (1000) carmen    (1000)      394 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/john/__init__.py
-drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2022-03-01 17:22:23.052265 thepysec-2.1/thepysec/john/tests/
--rw-r--r--   0 carmen    (1000) carmen    (1000)        0 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/john/tests/__init__.py
--rw-r--r--   0 carmen    (1000) carmen    (1000)     2546 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/john/tests/test_version.py
--rw-r--r--   0 carmen    (1000) carmen    (1000)     3297 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/john/version.py
--rw-r--r--   0 carmen    (1000) carmen    (1000)     3576 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/lia.py
--rw-r--r--   0 carmen    (1000) carmen    (1000)      750 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/matina.py
--rw-r--r--   0 carmen    (1000) carmen    (1000)     1335 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/myriam.py
--rw-r--r--   0 carmen    (1000) carmen    (1000)      465 2022-03-01 17:20:16.000000 thepysec-2.1/thepysec/otto.py
--rw-r--r--   0 carmen    (1000) carmen    (1000)     2024 2022-03-01 17:02:48.000000 thepysec-2.1/thepysec/thanos.py
-drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2022-03-01 17:22:23.052265 thepysec-2.1/thepysec.egg-info/
--rw-r--r--   0 carmen    (1000) carmen    (1000)     2526 2022-03-01 17:22:22.000000 thepysec-2.1/thepysec.egg-info/PKG-INFO
--rw-r--r--   0 carmen    (1000) carmen    (1000)      425 2022-03-01 17:22:23.000000 thepysec-2.1/thepysec.egg-info/SOURCES.txt
--rw-r--r--   0 carmen    (1000) carmen    (1000)        1 2022-03-01 17:22:22.000000 thepysec-2.1/thepysec.egg-info/dependency_links.txt
--rw-r--r--   0 carmen    (1000) carmen    (1000)       56 2022-03-01 17:22:22.000000 thepysec-2.1/thepysec.egg-info/requires.txt
--rw-r--r--   0 carmen    (1000) carmen    (1000)        9 2022-03-01 17:22:23.000000 thepysec-2.1/thepysec.egg-info/top_level.txt
+drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2023-04-12 10:46:27.126770 thepysec-2.2/
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     1523 2022-03-01 17:02:48.000000 thepysec-2.2/LICENSE
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     3574 2023-04-12 10:46:27.126770 thepysec-2.2/PKG-INFO
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     2658 2023-04-12 10:45:12.000000 thepysec-2.2/README.md
+-rw-r--r--   0 carmen    (1000) carmen    (1000)      342 2023-04-12 10:46:27.126770 thepysec-2.2/setup.cfg
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     1512 2023-04-12 08:56:05.000000 thepysec-2.2/setup.py
+drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2023-04-12 10:46:27.122770 thepysec-2.2/thepysec/
+-rw-r--r--   0 carmen    (1000) carmen    (1000)      497 2023-04-12 10:45:12.000000 thepysec-2.2/thepysec/__init__.py
+drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2023-04-12 10:46:27.122770 thepysec-2.2/thepysec/john/
+-rw-r--r--   0 carmen    (1000) carmen    (1000)      394 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/john/__init__.py
+drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2023-04-12 10:46:27.126770 thepysec-2.2/thepysec/john/tests/
+-rw-r--r--   0 carmen    (1000) carmen    (1000)        0 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/john/tests/__init__.py
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     2546 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/john/tests/test_version.py
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     3297 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/john/version.py
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     3576 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/lia.py
+-rw-r--r--   0 carmen    (1000) carmen    (1000)      750 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/matina.py
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     1335 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/myriam.py
+-rw-r--r--   0 carmen    (1000) carmen    (1000)      857 2023-04-12 08:50:25.000000 thepysec-2.2/thepysec/otto.py
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     2024 2022-03-01 17:02:48.000000 thepysec-2.2/thepysec/thanos.py
+drwxr-xr-x   0 carmen    (1000) carmen    (1000)        0 2023-04-12 10:46:27.122770 thepysec-2.2/thepysec.egg-info/
+-rw-r--r--   0 carmen    (1000) carmen    (1000)     3574 2023-04-12 10:46:27.000000 thepysec-2.2/thepysec.egg-info/PKG-INFO
+-rw-r--r--   0 carmen    (1000) carmen    (1000)      425 2023-04-12 10:46:27.000000 thepysec-2.2/thepysec.egg-info/SOURCES.txt
+-rw-r--r--   0 carmen    (1000) carmen    (1000)        1 2023-04-12 10:46:27.000000 thepysec-2.2/thepysec.egg-info/dependency_links.txt
+-rw-r--r--   0 carmen    (1000) carmen    (1000)       56 2023-04-12 10:46:27.000000 thepysec-2.2/thepysec.egg-info/requires.txt
+-rw-r--r--   0 carmen    (1000) carmen    (1000)        9 2023-04-12 10:46:27.000000 thepysec-2.2/thepysec.egg-info/top_level.txt
```

### Comparing `thepysec-2.1/LICENSE` & `thepysec-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thepysec-2.1/PKG-INFO` & `thepysec-2.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: thepysec
-Version: 2.1
+Version: 2.2
 Summary: Python secretaries you call at will, for instant py-relief.
 Home-page: https://github.com/raratiru/thepysec
 Author: Raratiru
 Author-email: info@musicaloffering.gr
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Build Status](https://github.com/raratiru/thepysec/actions/workflows/python-package.yml/badge.svg)](https://github.com/raratiru/thepysec/actions)
 [![Coverage Status](https://coveralls.io/repos/github/raratiru/thepysec/badge.svg?branch=master&service=github)](https://coveralls.io/github/raratiru/thepysec?branch=master)
 
@@ -35,46 +34,45 @@
 John is the Battler. He will serve the necessary files needed to run thepysec.
 
 Lia
 ---
 
 Lia is here to take a detailed look at your strings.
 
-* `pop_wsp`: Remove extra whitespace.
-* `pre_slug`: Prepare a string to become a wise slug.
+* [`pop_wsp`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L19): Remove extra whitespace.
+* [`pre_slug`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L87): Prepare a string to become a wise slug.
     * 'r33a!bc' -> 'r 33 abc'.
-* `fast_pre_slug`: Prepare a string to become a fast slug.
+* [`fast_pre_slug`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L23): Prepare a string to become a fast slug.
     * 'r33a!bc' -> 'r 3 3 a bc'.
-* `cap_sentence`: Carefully capitalize first letter and remove white space
+* [`cap_sentence`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L141): Carefully capitalize first letter and remove white space
     * "O'Connor is &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; INVITED to UK" -> "O'Connor Is Invited To UK"
 
 Matina
 ------
 
 Matina performs operations on django model instances
 
-* `pop_i18n_wsp`: Apply `pop_wsp` for a list of fields in a given model instance.
+* [`pop_i18n_wsp`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/matina.py#L18): Apply `pop_wsp` for a list of fields in a given model instance.
 
 Myriam
 ------
 
 Myriam a mathematical kind of jelly roll.
 
-* `validate_overlap`: Receives a list of DateRange or DateTimeRange and examines if contents overlap.
+* [`validate_overlap`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/myriam.py#L16): Receives a list of DateRange or DateTimeRange and examines if contents overlap.
 
 
 Thanos
 ------
 
 Thanos is a Django test assistant
 
-* `get_formset_alive`: Receives a formset class with data dictionary and returns a formset instance.
+* [`get_formset_alive`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/thanos.py#L16): Receives a formset class with data dictionary and returns a formset instance.
 
 
 Otto
 ----
 
 A pythonista who slightly bends the borders of the language
 
-* `deep_getattr`: Dives in an object by performing successive getattrs for each word in a dotted string.
-
-
+* [`deep_getattr`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/otto.py#L8): Dives in an object by performing successive getattrs for each word in a dotted string.
+* [`deep_get`](https://github.com/raratiru/thepysec/blob/4ee944291b832beeb75d6d22dd0a3bc045c108de/thepysec/otto.py#L22): Dives in a dictionary by performing successive getats for each word in a dotted string.
```

### Comparing `thepysec-2.1/setup.py` & `thepysec-2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open(path.join(path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="thepysec",
     version=version,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     description="Python secretaries you call at will, for instant py-relief.",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/raratiru/thepysec",
     author="Raratiru",
     author_email="info@musicaloffering.gr",
     license="BSD 3-Clause License",
@@ -27,18 +27,18 @@
     setup_requires=["pytest-runner"],
     tests_require=["pytest", "pytest-cov", "psycopg2-binary"],
     extras_require={"dev": ["pytest", "pytest-cov", "ipdb", "psycopg2-binary"]},
     install_requires=["unidecode"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `thepysec-2.1/thepysec/john/tests/test_version.py` & `thepysec-2.2/thepysec/john/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `thepysec-2.1/thepysec/john/version.py` & `thepysec-2.2/thepysec/john/version.py`

 * *Files identical despite different names*

### Comparing `thepysec-2.1/thepysec/lia.py` & `thepysec-2.2/thepysec/lia.py`

 * *Files identical despite different names*

### Comparing `thepysec-2.1/thepysec/matina.py` & `thepysec-2.2/thepysec/matina.py`

 * *Files identical despite different names*

### Comparing `thepysec-2.1/thepysec/myriam.py` & `thepysec-2.2/thepysec/myriam.py`

 * *Files identical despite different names*

### Comparing `thepysec-2.1/thepysec/thanos.py` & `thepysec-2.2/thepysec/thanos.py`

 * *Files identical despite different names*

### Comparing `thepysec-2.1/thepysec.egg-info/PKG-INFO` & `thepysec-2.2/thepysec.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: thepysec
-Version: 2.1
+Version: 2.2
 Summary: Python secretaries you call at will, for instant py-relief.
 Home-page: https://github.com/raratiru/thepysec
 Author: Raratiru
 Author-email: info@musicaloffering.gr
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Build Status](https://github.com/raratiru/thepysec/actions/workflows/python-package.yml/badge.svg)](https://github.com/raratiru/thepysec/actions)
 [![Coverage Status](https://coveralls.io/repos/github/raratiru/thepysec/badge.svg?branch=master&service=github)](https://coveralls.io/github/raratiru/thepysec?branch=master)
 
@@ -35,46 +34,45 @@
 John is the Battler. He will serve the necessary files needed to run thepysec.
 
 Lia
 ---
 
 Lia is here to take a detailed look at your strings.
 
-* `pop_wsp`: Remove extra whitespace.
-* `pre_slug`: Prepare a string to become a wise slug.
+* [`pop_wsp`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L19): Remove extra whitespace.
+* [`pre_slug`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L87): Prepare a string to become a wise slug.
     * 'r33a!bc' -> 'r 33 abc'.
-* `fast_pre_slug`: Prepare a string to become a fast slug.
+* [`fast_pre_slug`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L23): Prepare a string to become a fast slug.
     * 'r33a!bc' -> 'r 3 3 a bc'.
-* `cap_sentence`: Carefully capitalize first letter and remove white space
+* [`cap_sentence`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/lia.py#L141): Carefully capitalize first letter and remove white space
     * "O'Connor is &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; INVITED to UK" -> "O'Connor Is Invited To UK"
 
 Matina
 ------
 
 Matina performs operations on django model instances
 
-* `pop_i18n_wsp`: Apply `pop_wsp` for a list of fields in a given model instance.
+* [`pop_i18n_wsp`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/matina.py#L18): Apply `pop_wsp` for a list of fields in a given model instance.
 
 Myriam
 ------
 
 Myriam a mathematical kind of jelly roll.
 
-* `validate_overlap`: Receives a list of DateRange or DateTimeRange and examines if contents overlap.
+* [`validate_overlap`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/myriam.py#L16): Receives a list of DateRange or DateTimeRange and examines if contents overlap.
 
 
 Thanos
 ------
 
 Thanos is a Django test assistant
 
-* `get_formset_alive`: Receives a formset class with data dictionary and returns a formset instance.
+* [`get_formset_alive`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/thanos.py#L16): Receives a formset class with data dictionary and returns a formset instance.
 
 
 Otto
 ----
 
 A pythonista who slightly bends the borders of the language
 
-* `deep_getattr`: Dives in an object by performing successive getattrs for each word in a dotted string.
-
-
+* [`deep_getattr`](https://github.com/raratiru/thepysec/blob/571cf49798e571f542c5ec65f45cf62ec5262399/thepysec/otto.py#L8): Dives in an object by performing successive getattrs for each word in a dotted string.
+* [`deep_get`](https://github.com/raratiru/thepysec/blob/4ee944291b832beeb75d6d22dd0a3bc045c108de/thepysec/otto.py#L22): Dives in a dictionary by performing successive getats for each word in a dotted string.
```

