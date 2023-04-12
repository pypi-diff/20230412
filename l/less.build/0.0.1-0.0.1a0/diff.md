# Comparing `tmp/less.build-0.0.1.tar.gz` & `tmp/less.build-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "less.build-0.0.1.tar", last modified: Sat Feb  4 06:57:35 2023, max compression
+gzip compressed data, was "less.build-0.0.1a0.tar", last modified: Wed Apr 12 21:47:05 2023, max compression
```

## Comparing `less.build-0.0.1.tar` & `less.build-0.0.1a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-02-04 06:57:35.312931 less.build-0.0.1/
--rw-r--r--   0 sam        (501) staff       (20)       11 2023-02-04 06:55:50.000000 less.build-0.0.1/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)        0 2023-02-04 06:55:50.000000 less.build-0.0.1/MANIFEST.in
--rw-r--r--   0 sam        (501) staff       (20)      471 2023-02-04 06:57:35.312812 less.build-0.0.1/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)       28 2023-02-04 06:56:59.000000 less.build-0.0.1/README.md
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-02-04 06:57:35.312664 less.build-0.0.1/less.build.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)      471 2023-02-04 06:57:35.000000 less.build-0.0.1/less.build.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      222 2023-02-04 06:57:35.000000 less.build-0.0.1/less.build.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2023-02-04 06:57:35.000000 less.build-0.0.1/less.build.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)        7 2023-02-04 06:57:35.000000 less.build-0.0.1/less.build.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2023-02-04 06:57:35.000000 less.build-0.0.1/less.build.egg-info/top_level.txt
--rw-r--r--   0 sam        (501) staff       (20)      631 2023-02-04 06:56:14.000000 less.build-0.0.1/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)       38 2023-02-04 06:57:35.312964 less.build-0.0.1/setup.cfg
--rw-r--r--   0 sam        (501) staff       (20)       50 2023-02-04 06:55:50.000000 less.build-0.0.1/setup.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-04-12 21:47:05.473506 less.build-0.0.1a0/
+-rw-r--r--   0 sam        (501) staff       (20)       11 2023-02-18 06:45:16.000000 less.build-0.0.1a0/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)        0 2023-02-18 06:45:16.000000 less.build-0.0.1a0/MANIFEST.in
+-rw-r--r--   0 sam        (501) staff       (20)      473 2023-04-12 21:47:05.473191 less.build-0.0.1a0/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)       27 2023-02-18 06:45:16.000000 less.build-0.0.1a0/README.md
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-04-12 21:47:05.472793 less.build-0.0.1a0/less.build.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)      473 2023-04-12 21:47:05.000000 less.build-0.0.1a0/less.build.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      222 2023-04-12 21:47:05.000000 less.build-0.0.1a0/less.build.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2023-04-12 21:47:05.000000 less.build-0.0.1a0/less.build.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)        7 2023-04-12 21:47:05.000000 less.build-0.0.1a0/less.build.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2023-04-12 21:47:05.000000 less.build-0.0.1a0/less.build.egg-info/top_level.txt
+-rw-r--r--   0 sam        (501) staff       (20)      639 2023-04-12 21:44:39.000000 less.build-0.0.1a0/pyproject.toml
+-rw-r--r--   0 sam        (501) staff       (20)       38 2023-04-12 21:47:05.473554 less.build-0.0.1a0/setup.cfg
+-rw-r--r--   0 sam        (501) staff       (20)       50 2023-02-18 06:45:16.000000 less.build-0.0.1a0/setup.py
```

### Comparing `less.build-0.0.1/pyproject.toml` & `less.build-0.0.1a0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "less.build"
-version = "0.0.1"
+version = "0.0.1-alpha0"
 description = "Coming soon"
 readme = "README.md"
 authors = [{ name = "Elide", email = "libs@elide.dev" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -19,11 +19,11 @@
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
-Homepage = "https://elide.dev"
+Homepage = "https://less.build"
 
 [project.scripts]
 # nothing at this time
```

