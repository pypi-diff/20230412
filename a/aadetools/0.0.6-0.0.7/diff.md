# Comparing `tmp/aadetools-0.0.6.tar.gz` & `tmp/aadetools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aadetools-0.0.6.tar", last modified: Wed Apr 12 20:14:10 2023, max compression
+gzip compressed data, was "aadetools-0.0.7.tar", last modified: Wed Apr 12 20:52:56 2023, max compression
```

## Comparing `aadetools-0.0.6.tar` & `aadetools-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.636325 aadetools-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       35 2023-03-19 10:52:53.000000 aadetools-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      521 2023-04-12 20:14:10.633856 aadetools-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.587211 aadetools-0.0.6/aadetools.egg-info/
--rw-rw-rw-   0        0        0      521 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 20:14:10.000000 aadetools-0.0.6/aadetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 20:14:10.637317 aadetools-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1564 2023-04-12 20:13:56.000000 aadetools-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.563139 aadetools-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.622895 aadetools-0.0.6/src/morph/
--rw-rw-rw-   0        0        0        0 2023-04-01 19:28:21.000000 aadetools-0.0.6/src/morph/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-02-26 06:10:53.000000 aadetools-0.0.6/src/morph/charsets.py
--rw-rw-rw-   0        0        0     2765 2023-04-11 20:43:08.000000 aadetools-0.0.6/src/morph/lemmatizeSentence.py
--rw-rw-rw-   0        0        0     7774 2023-04-12 18:50:43.000000 aadetools-0.0.6/src/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 aadetools-0.0.6/src/morph/settings.py
--rw-rw-rw-   0        0        0      574 2023-04-11 20:44:33.000000 aadetools-0.0.6/src/morph/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-12 20:14:10.630565 aadetools-0.0.6/src/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 aadetools-0.0.6/src/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 aadetools-0.0.6/src/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:52:56.621376 aadetools-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-03-26 19:25:02.000000 aadetools-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       81 2023-04-12 20:21:25.000000 aadetools-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      521 2023-04-12 20:52:56.619322 aadetools-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-19 11:00:03.000000 aadetools-0.0.7/README.md
+-rw-rw-rw-   0        0        0      674 2023-04-10 21:58:24.000000 aadetools-0.0.7/instructions.txt
+-rw-rw-rw-   0        0        0      873 2023-04-11 20:50:14.000000 aadetools-0.0.7/req.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 20:52:56.621376 aadetools-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-04-12 20:52:35.000000 aadetools-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:52:56.603969 aadetools-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 20:52:56.616371 aadetools-0.0.7/src/aadetools.egg-info/
+-rw-rw-rw-   0        0        0      521 2023-04-12 20:52:56.000000 aadetools-0.0.7/src/aadetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-12 20:52:56.000000 aadetools-0.0.7/src/aadetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 20:52:56.000000 aadetools-0.0.7/src/aadetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-12 20:52:56.000000 aadetools-0.0.7/src/aadetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-12 20:52:56.000000 aadetools-0.0.7/src/aadetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      125 2023-03-26 18:52:41.000000 aadetools-0.0.7/src/aadetools.py
+-rw-rw-rw-   0        0        0       87 2023-04-12 20:48:19.000000 aadetools-0.0.7/tox.ini
```

### Comparing `aadetools-0.0.6/LICENSE.txt` & `aadetools-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aadetools-0.0.6/PKG-INFO` & `aadetools-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: Dev
+Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `aadetools-0.0.6/aadetools.egg-info/PKG-INFO` & `aadetools-0.0.7/src/aadetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aadetools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Test Package Demo
 Home-page: 
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: Dev
+Provides-Extra: dev
 License-File: LICENSE.txt
```

### Comparing `aadetools-0.0.6/setup.py` & `aadetools-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,31 +9,34 @@
     'tqdm==4.62.2',
     'requests==2.25.1',
     'regex==2021.4.4'
 ]
 
 setup(
     name="aadetools",                     # This is the name of the package
-    version="0.0.6",                        # The initial release version
+    version="0.0.7",                        # The initial release version
     url="",                                  #
     author_email="alaa.omer2009@gmail.com",   #
     author="Alaa' Omar",                     # Full name of the author
     description="Test Package Demo",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
-    packages=find_packages(include=['src.*']),    # List of all python modules to be installed
+    #packages=find_packages(include=['src','src.*']),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.9',                # Minimum version requirement of the package
     py_modules=["aadetools"],             # Name of the python package
     install_requires=requirements,         # Install other dependencies if any
-    extras_require={
-        "Dev":[
-            "pytest>=3.7",
+    package_dir={"": "src"},
+     extras_require = {
+        "dev": [
+            "pytest >= 3.7",
+            "check-manifest",
+            "twine",
         ],
     },
 )
```

