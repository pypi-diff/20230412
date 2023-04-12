# Comparing `tmp/tlcGIS-0.0.2.tar.gz` & `tmp/tlcGIS-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlcGIS-0.0.2.tar", last modified: Wed Apr 12 05:44:13 2023, max compression
+gzip compressed data, was "tlcGIS-0.0.3.tar", last modified: Wed Apr 12 06:49:44 2023, max compression
```

## Comparing `tlcGIS-0.0.2.tar` & `tlcGIS-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 05:44:13.216488 tlcGIS-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-12 03:56:18.000000 tlcGIS-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      655 2023-04-12 05:44:13.215492 tlcGIS-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      144 2023-04-12 05:43:54.000000 tlcGIS-0.0.2/README.md
--rw-rw-rw-   0        0        0      589 2023-04-12 05:40:58.000000 tlcGIS-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 05:44:13.216488 tlcGIS-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 05:44:13.199089 tlcGIS-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 05:44:13.210621 tlcGIS-0.0.2/src/tlcGIS/
--rw-rw-rw-   0        0        0        0 2023-04-12 03:52:12.000000 tlcGIS-0.0.2/src/tlcGIS/__init__.py
--rw-rw-rw-   0        0        0    14420 2023-04-12 03:52:03.000000 tlcGIS-0.0.2/src/tlcGIS/wct.py
-drwxrwxrwx   0        0        0        0 2023-04-12 05:44:13.214482 tlcGIS-0.0.2/src/tlcGIS.egg-info/
--rw-rw-rw-   0        0        0      655 2023-04-12 05:44:13.000000 tlcGIS-0.0.2/src/tlcGIS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-04-12 05:44:13.000000 tlcGIS-0.0.2/src/tlcGIS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 05:44:13.000000 tlcGIS-0.0.2/src/tlcGIS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-12 05:44:13.000000 tlcGIS-0.0.2/src/tlcGIS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 06:49:44.793642 tlcGIS-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-12 03:56:18.000000 tlcGIS-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      655 2023-04-12 06:49:44.793642 tlcGIS-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      144 2023-04-12 05:43:54.000000 tlcGIS-0.0.3/README.md
+-rw-rw-rw-   0        0        0      641 2023-04-12 06:49:26.000000 tlcGIS-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 06:49:44.793642 tlcGIS-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 06:49:44.758789 tlcGIS-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 06:49:44.762609 tlcGIS-0.0.3/src/tlcGIS/
+-rw-rw-rw-   0        0        0        0 2023-04-12 03:52:12.000000 tlcGIS-0.0.3/src/tlcGIS/__init__.py
+-rw-rw-rw-   0        0        0    14420 2023-04-12 03:52:03.000000 tlcGIS-0.0.3/src/tlcGIS/wct.py
+drwxrwxrwx   0        0        0        0 2023-04-12 06:49:44.792645 tlcGIS-0.0.3/src/tlcGIS.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-04-12 06:49:44.000000 tlcGIS-0.0.3/src/tlcGIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-12 06:49:44.000000 tlcGIS-0.0.3/src/tlcGIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 06:49:44.000000 tlcGIS-0.0.3/src/tlcGIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-12 06:49:44.000000 tlcGIS-0.0.3/src/tlcGIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-12 06:49:44.000000 tlcGIS-0.0.3/src/tlcGIS.egg-info/top_level.txt
```

### Comparing `tlcGIS-0.0.2/LICENSE` & `tlcGIS-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tlcGIS-0.0.2/PKG-INFO` & `tlcGIS-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlcGIS
-Version: 0.0.2
+Version: 0.0.3
 Summary: gis coordinate transform tools
 Author-email: Bankxi <1259564569@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tlcGIS-0.0.2/src/tlcGIS/wct.py` & `tlcGIS-0.0.3/src/tlcGIS/wct.py`

 * *Files identical despite different names*

### Comparing `tlcGIS-0.0.2/src/tlcGIS.egg-info/PKG-INFO` & `tlcGIS-0.0.3/src/tlcGIS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlcGIS
-Version: 0.0.2
+Version: 0.0.3
 Summary: gis coordinate transform tools
 Author-email: Bankxi <1259564569@qq.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

