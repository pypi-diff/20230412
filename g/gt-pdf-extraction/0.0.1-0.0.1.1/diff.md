# Comparing `tmp/gt-pdf-extraction-0.0.1.tar.gz` & `tmp/gt-pdf-extraction-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gt-pdf-extraction-0.0.1.tar", last modified: Mon Apr  3 09:05:49 2023, max compression
+gzip compressed data, was "gt-pdf-extraction-0.0.1.1.tar", last modified: Wed Apr 12 10:25:49 2023, max compression
```

## Comparing `gt-pdf-extraction-0.0.1.tar` & `gt-pdf-extraction-0.0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-03 09:05:49.604845 gt-pdf-extraction-0.0.1/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     2736 2023-04-03 09:05:49.604727 gt-pdf-extraction-0.0.1/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)     2302 2023-04-03 09:00:00.000000 gt-pdf-extraction-0.0.1/README.md
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-03 09:05:49.603995 gt-pdf-extraction-0.0.1/gt_pdf_extraction/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     7771 2023-04-03 09:05:15.000000 gt-pdf-extraction-0.0.1/gt_pdf_extraction/__init__.py
-drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-03 09:05:49.604571 gt-pdf-extraction-0.0.1/gt_pdf_extraction.egg-info/
--rw-r--r--   0 guangyuhe   (501) staff       (20)     2736 2023-04-03 09:05:49.000000 gt-pdf-extraction-0.0.1/gt_pdf_extraction.egg-info/PKG-INFO
--rw-r--r--   0 guangyuhe   (501) staff       (20)      252 2023-04-03 09:05:49.000000 gt-pdf-extraction-0.0.1/gt_pdf_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-04-03 09:05:49.000000 gt-pdf-extraction-0.0.1/gt_pdf_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       47 2023-04-03 09:05:49.000000 gt-pdf-extraction-0.0.1/gt_pdf_extraction.egg-info/requires.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       18 2023-04-03 09:05:49.000000 gt-pdf-extraction-0.0.1/gt_pdf_extraction.egg-info/top_level.txt
--rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-04-03 09:05:49.604876 gt-pdf-extraction-0.0.1/setup.cfg
--rw-r--r--   0 guangyuhe   (501) staff       (20)      839 2023-04-03 09:00:00.000000 gt-pdf-extraction-0.0.1/setup.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:25:49.869974 gt-pdf-extraction-0.0.1.1/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2833 2023-04-12 10:25:49.869865 gt-pdf-extraction-0.0.1.1/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2397 2023-04-12 10:25:16.000000 gt-pdf-extraction-0.0.1.1/README.md
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:25:49.869165 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     7771 2023-04-03 09:05:15.000000 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction/__init__.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:25:49.869708 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction.egg-info/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2833 2023-04-12 10:25:49.000000 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      252 2023-04-12 10:25:49.000000 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-04-12 10:25:49.000000 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       47 2023-04-12 10:25:49.000000 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction.egg-info/requires.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       18 2023-04-12 10:25:49.000000 gt-pdf-extraction-0.0.1.1/gt_pdf_extraction.egg-info/top_level.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-04-12 10:25:49.870011 gt-pdf-extraction-0.0.1.1/setup.cfg
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      938 2023-04-12 10:24:45.000000 gt-pdf-extraction-0.0.1.1/setup.py
```

### Comparing `gt-pdf-extraction-0.0.1/PKG-INFO` & `gt-pdf-extraction-0.0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt-pdf-extraction
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A python pdf extraction package.
 Home-page: https://bitbucket.org/guangyuhe/pdf-extraction/src/main/
 Author: Guangyu He
 Author-email: guangyu.he@golden-tech.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -117,11 +117,17 @@
 
 ### v0.0.1
 
 #### initial upload
 
 - first version
 
+### v0.0.1.1
+
+#### bug fix
+
+- fix the long desc error in setup.py causing installation failed
+
 ## Support
 
 2023&copy;GoldenTech, for further support please contact author. <br>
 Email: <a href="mailto:guangyu.he@golden-tech.de">guangyu.he@golden-tech.de</a>
```

### Comparing `gt-pdf-extraction-0.0.1/README.md` & `gt-pdf-extraction-0.0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -104,11 +104,17 @@
 
 ### v0.0.1
 
 #### initial upload
 
 - first version
 
+### v0.0.1.1
+
+#### bug fix
+
+- fix the long desc error in setup.py causing installation failed
+
 ## Support
 
 2023&copy;GoldenTech, for further support please contact author. <br>
 Email: <a href="mailto:guangyu.he@golden-tech.de">guangyu.he@golden-tech.de</a>
```

### Comparing `gt-pdf-extraction-0.0.1/gt_pdf_extraction/__init__.py` & `gt-pdf-extraction-0.0.1.1/gt_pdf_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `gt-pdf-extraction-0.0.1/gt_pdf_extraction.egg-info/PKG-INFO` & `gt-pdf-extraction-0.0.1.1/gt_pdf_extraction.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt-pdf-extraction
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A python pdf extraction package.
 Home-page: https://bitbucket.org/guangyuhe/pdf-extraction/src/main/
 Author: Guangyu He
 Author-email: guangyu.he@golden-tech.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -117,11 +117,17 @@
 
 ### v0.0.1
 
 #### initial upload
 
 - first version
 
+### v0.0.1.1
+
+#### bug fix
+
+- fix the long desc error in setup.py causing installation failed
+
 ## Support
 
 2023&copy;GoldenTech, for further support please contact author. <br>
 Email: <a href="mailto:guangyu.he@golden-tech.de">guangyu.he@golden-tech.de</a>
```

### Comparing `gt-pdf-extraction-0.0.1/setup.py` & `gt-pdf-extraction-0.0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 
-with open('README.md') as fh:
-    long_description = fh.read()
+this_directory = Path(__file__).parent
+with open(this_directory / "README.md", encoding="utf-8") as f:
+    long_description = f.read()
 
 setup(
     name="gt-pdf-extraction",
-    version="0.0.1",
+    version="0.0.1.1",
     author="Guangyu He",
     author_email="guangyu.he@golden-tech.de",
     description="A python pdf extraction package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/guangyuhe/pdf-extraction/src/main/",
     install_requires=[
```

