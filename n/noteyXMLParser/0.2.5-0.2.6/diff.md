# Comparing `tmp/noteyXMLParser-0.2.5.tar.gz` & `tmp/noteyXMLParser-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/noteyXMLParser-0.2.5.tar", last modified: Wed Apr 12 03:53:28 2023, max compression
+gzip compressed data, was "dist/noteyXMLParser-0.2.6.tar", last modified: Wed Apr 12 08:08:26 2023, max compression
```

## Comparing `noteyXMLParser-0.2.5.tar` & `noteyXMLParser-0.2.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-04-12 03:53:28.412520 noteyXMLParser-0.2.5/
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      904 2023-04-12 03:53:28.412158 noteyXMLParser-0.2.5/PKG-INFO
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      359 2023-04-11 06:22:11.000000 noteyXMLParser-0.2.5/README.md
--rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-04-12 03:53:28.412709 noteyXMLParser-0.2.5/setup.cfg
--rw-r--r--   0 aminmahjoub   (501) staff       (20)      689 2023-04-12 03:53:17.000000 noteyXMLParser-0.2.5/setup.py
+drwxr-xr-x   0 aminmahjoub   (501) staff       (20)        0 2023-04-12 08:08:26.145157 noteyXMLParser-0.2.6/
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      904 2023-04-12 08:08:26.144878 noteyXMLParser-0.2.6/PKG-INFO
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      359 2023-04-11 06:22:11.000000 noteyXMLParser-0.2.6/README.md
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)       38 2023-04-12 08:08:26.145259 noteyXMLParser-0.2.6/setup.cfg
+-rw-r--r--   0 aminmahjoub   (501) staff       (20)      689 2023-04-12 08:08:21.000000 noteyXMLParser-0.2.6/setup.py
```

### Comparing `noteyXMLParser-0.2.5/PKG-INFO` & `noteyXMLParser-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noteyXMLParser
-Version: 0.2.5
+Version: 0.2.6
 Summary: Music XML Parser
 Home-page: https://github.com/mmahjoub5/NoteyXMLParser
 Author: Amin Mahjoub
 Author-email: mahjoub@usc.edu
 License: UNKNOWN
 Description: my parser
```

### Comparing `noteyXMLParser-0.2.5/setup.py` & `noteyXMLParser-0.2.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='noteyXMLParser',  
-     version='0.2.5',
+     version='0.2.6',
      author="Amin Mahjoub",
      author_email="mahjoub@usc.edu",
      description="Music XML Parser",
      long_description=long_description,
      package_dir={"":"/Users/aminmahjoub/NoteyXMLParser/xmlParser/src"},
      url="https://github.com/mmahjoub5/NoteyXMLParser",
    long_description_content_type="text/markdown",
```

