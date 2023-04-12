# Comparing `tmp/example-pkg-hh-0.0.1.tar.gz` & `tmp/example_pkg_hh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example-pkg-hh-0.0.1.tar", last modified: Wed Apr 12 08:56:17 2023, max compression
+gzip compressed data, was "example_pkg_hh-0.0.2.tar", last modified: Wed Apr 12 09:12:55 2023, max compression
```

## Comparing `example-pkg-hh-0.0.1.tar` & `example_pkg_hh-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 08:56:17.095168 example-pkg-hh-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-12 08:42:42.000000 example-pkg-hh-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      420 2023-04-12 08:56:17.094152 example-pkg-hh-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-12 08:41:29.000000 example-pkg-hh-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 08:56:17.091153 example-pkg-hh-0.0.1/example_pkg/
--rw-rw-rw-   0        0        0       20 2023-04-12 08:53:29.000000 example-pkg-hh-0.0.1/example_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 08:56:17.094152 example-pkg-hh-0.0.1/example_pkg_hh.egg-info/
--rw-rw-rw-   0        0        0      420 2023-04-12 08:56:16.000000 example-pkg-hh-0.0.1/example_pkg_hh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-12 08:56:17.000000 example-pkg-hh-0.0.1/example_pkg_hh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 08:56:16.000000 example-pkg-hh-0.0.1/example_pkg_hh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 08:56:16.000000 example-pkg-hh-0.0.1/example_pkg_hh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 08:56:17.095168 example-pkg-hh-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-04-12 08:55:36.000000 example-pkg-hh-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:12:55.556219 example_pkg_hh-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-12 08:42:42.000000 example_pkg_hh-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      420 2023-04-12 09:12:55.556219 example_pkg_hh-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-12 08:41:29.000000 example_pkg_hh-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:12:55.553218 example_pkg_hh-0.0.2/example_pkg_hh/
+-rw-rw-rw-   0        0        0       20 2023-04-12 08:53:29.000000 example_pkg_hh-0.0.2/example_pkg_hh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:12:55.555218 example_pkg_hh-0.0.2/example_pkg_hh.egg-info/
+-rw-rw-rw-   0        0        0      420 2023-04-12 09:12:55.000000 example_pkg_hh-0.0.2/example_pkg_hh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-04-12 09:12:55.000000 example_pkg_hh-0.0.2/example_pkg_hh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:12:55.000000 example_pkg_hh-0.0.2/example_pkg_hh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 09:12:55.000000 example_pkg_hh-0.0.2/example_pkg_hh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:12:55.557222 example_pkg_hh-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-04-12 09:12:35.000000 example_pkg_hh-0.0.2/setup.py
```

### Comparing `example-pkg-hh-0.0.1/LICENSE` & `example_pkg_hh-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `example-pkg-hh-0.0.1/setup.py` & `example_pkg_hh-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
-  name="example-pkg-hh",
-  version="0.0.1",
+  name="example_pkg_hh",
+  version="0.0.2",
   author="ironlionwg",
   author_email="author@example.com",
   description="A small example package",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

