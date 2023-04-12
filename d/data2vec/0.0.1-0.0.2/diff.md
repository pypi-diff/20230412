# Comparing `tmp/data2vec-0.0.1.tar.gz` & `tmp/data2vec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2vec-0.0.1.tar", last modified: Wed Apr 12 04:31:45 2023, max compression
+gzip compressed data, was "data2vec-0.0.2.tar", last modified: Wed Apr 12 14:07:30 2023, max compression
```

## Comparing `data2vec-0.0.1.tar` & `data2vec-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 xuehang    (501) staff       (20)        0 2023-04-12 04:31:45.350122 data2vec-0.0.1/
--rw-r--r--   0 xuehang    (501) staff       (20)     1069 2023-04-12 04:19:25.000000 data2vec-0.0.1/LICENSE
--rw-r--r--   0 xuehang    (501) staff       (20)      401 2023-04-12 04:31:45.350018 data2vec-0.0.1/PKG-INFO
--rw-r--r--   0 xuehang    (501) staff       (20)      279 2023-04-12 04:26:32.000000 data2vec-0.0.1/README.md
-drwxr-xr-x   0 xuehang    (501) staff       (20)        0 2023-04-12 04:31:45.349367 data2vec-0.0.1/data2vec/
--rw-r--r--   0 xuehang    (501) staff       (20)       34 2023-04-12 04:22:01.000000 data2vec-0.0.1/data2vec/__init__.py
--rw-r--r--   0 xuehang    (501) staff       (20)        0 2023-04-12 04:21:43.000000 data2vec-0.0.1/data2vec/img_to_vec.py
-drwxr-xr-x   0 xuehang    (501) staff       (20)        0 2023-04-12 04:31:45.349870 data2vec-0.0.1/data2vec.egg-info/
--rw-r--r--   0 xuehang    (501) staff       (20)      401 2023-04-12 04:31:45.000000 data2vec-0.0.1/data2vec.egg-info/PKG-INFO
--rw-r--r--   0 xuehang    (501) staff       (20)      229 2023-04-12 04:31:45.000000 data2vec-0.0.1/data2vec.egg-info/SOURCES.txt
--rw-r--r--   0 xuehang    (501) staff       (20)        1 2023-04-12 04:31:45.000000 data2vec-0.0.1/data2vec.egg-info/dependency_links.txt
--rw-r--r--   0 xuehang    (501) staff       (20)       51 2023-04-12 04:31:45.000000 data2vec-0.0.1/data2vec.egg-info/requires.txt
--rw-r--r--   0 xuehang    (501) staff       (20)        9 2023-04-12 04:31:45.000000 data2vec-0.0.1/data2vec.egg-info/top_level.txt
--rw-r--r--   0 xuehang    (501) staff       (20)       38 2023-04-12 04:31:45.350159 data2vec-0.0.1/setup.cfg
--rw-r--r--   0 xuehang    (501) staff       (20)      638 2023-04-12 04:31:28.000000 data2vec-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:07:30.226873 data2vec-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-12 12:09:40.000000 data2vec-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-04-12 14:07:30.225871 data2vec-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-12 12:09:40.000000 data2vec-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 14:07:30.211675 data2vec-0.0.2/data2vec/
+-rw-rw-rw-   0        0        0       45 2023-04-12 12:09:40.000000 data2vec-0.0.2/data2vec/__init__.py
+-rw-rw-rw-   0        0        0     3224 2023-04-12 13:47:23.000000 data2vec-0.0.2/data2vec/img_to_vec.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:07:30.225871 data2vec-0.0.2/data2vec.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 14:07:30.000000 data2vec-0.0.2/data2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:07:30.226873 data2vec-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      925 2023-04-12 14:05:49.000000 data2vec-0.0.2/setup.py
```

