# Comparing `tmp/airlabs-0.0.2.tar.gz` & `tmp/airlabs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airlabs-0.0.2.tar", last modified: Wed Apr 12 00:11:00 2023, max compression
+gzip compressed data, was "airlabs-0.0.3.tar", last modified: Wed Apr 12 00:21:21 2023, max compression
```

## Comparing `airlabs-0.0.2.tar` & `airlabs-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.086203 airlabs-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-04-11 20:29:40.000000 airlabs-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       57 2023-04-11 20:29:40.000000 airlabs-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1946 2023-04-12 00:11:00.085176 airlabs-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1461 2023-04-11 23:56:33.000000 airlabs-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 00:11:00.086203 airlabs-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-04-12 00:10:38.000000 airlabs-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.075202 airlabs-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.082213 airlabs-0.0.2/src/airlabs/
--rw-rw-rw-   0        0        0       27 2023-04-11 20:29:40.000000 airlabs-0.0.2/src/airlabs/__init__.py
--rw-rw-rw-   0        0        0     9455 2023-04-11 23:44:56.000000 airlabs-0.0.2/src/airlabs/endpoints.py
--rw-rw-rw-   0        0        0      460 2023-04-11 23:30:26.000000 airlabs-0.0.2/src/airlabs/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-12 00:11:00.084209 airlabs-0.0.2/src/airlabs.egg-info/
--rw-rw-rw-   0        0        0     1946 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 00:11:00.000000 airlabs-0.0.2/src/airlabs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       76 2023-04-12 00:10:33.000000 airlabs-0.0.2/versions.md
+drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.981094 airlabs-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-11 20:29:40.000000 airlabs-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-04-11 20:29:40.000000 airlabs-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1419 2023-04-12 00:21:21.980097 airlabs-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      943 2023-04-12 00:20:26.000000 airlabs-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 00:21:21.981094 airlabs-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-04-12 00:20:39.000000 airlabs-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.971121 airlabs-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.977105 airlabs-0.0.3/src/airlabs/
+-rw-rw-rw-   0        0        0       27 2023-04-11 20:29:40.000000 airlabs-0.0.3/src/airlabs/__init__.py
+-rw-rw-rw-   0        0        0     9455 2023-04-11 23:44:56.000000 airlabs-0.0.3/src/airlabs/endpoints.py
+-rw-rw-rw-   0        0        0      460 2023-04-11 23:30:26.000000 airlabs-0.0.3/src/airlabs/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 00:21:21.979099 airlabs-0.0.3/src/airlabs.egg-info/
+-rw-rw-rw-   0        0        0     1419 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 00:21:21.000000 airlabs-0.0.3/src/airlabs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      109 2023-04-12 00:20:51.000000 airlabs-0.0.3/versions.md
```

### Comparing `airlabs-0.0.2/LICENSE` & `airlabs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airlabs-0.0.2/setup.py` & `airlabs-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="airlabs",
-    version="0.0.2",
+    version="0.0.3",
     description="Python wrapper for AirLabs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/calebyhan/AirLabs",
     author="Caleb Han",
     author_email="calebhantech@gmail.com",
     license="MIT",
```

### Comparing `airlabs-0.0.2/src/airlabs/endpoints.py` & `airlabs-0.0.3/src/airlabs/endpoints.py`

 * *Files identical despite different names*

