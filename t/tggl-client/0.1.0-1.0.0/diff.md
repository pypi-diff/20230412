# Comparing `tmp/tggl_client-0.1.0.tar.gz` & `tmp/tggl_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tggl_client-0.1.0.tar", last modified: Wed Apr 12 18:14:45 2023, max compression
+gzip compressed data, was "tggl_client-1.0.0.tar", last modified: Fri Apr  7 19:27:03 2023, max compression
```

## Comparing `tggl_client-0.1.0.tar` & `tggl_client-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-12 18:14:45.735509 tggl_client-0.1.0/
--rw-r--r--   0 nick       (501) staff       (20)      111 2023-04-12 18:14:45.735410 tggl_client-0.1.0/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)       38 2023-04-12 18:14:45.735547 tggl_client-0.1.0/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)      230 2023-04-12 17:56:52.000000 tggl_client-0.1.0/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-12 18:14:45.735243 tggl_client-0.1.0/tggl_client.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)      111 2023-04-12 18:14:45.000000 tggl_client-0.1.0/tggl_client.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      148 2023-04-12 18:14:45.000000 tggl_client-0.1.0/tggl_client.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-12 18:14:45.000000 tggl_client-0.1.0/tggl_client.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-12 18:14:45.000000 tggl_client-0.1.0/tggl_client.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-07 19:27:03.898436 tggl_client-1.0.0/
+-rw-r--r--   0 nick       (501) staff       (20)      111 2023-04-07 19:27:03.898338 tggl_client-1.0.0/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)       38 2023-04-07 19:27:03.898473 tggl_client-1.0.0/setup.cfg
+-rw-r--r--   0 nick       (501) staff       (20)      254 2023-04-07 19:23:06.000000 tggl_client-1.0.0/setup.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-07 19:27:03.898174 tggl_client-1.0.0/tggl_client.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)      111 2023-04-07 19:27:03.000000 tggl_client-1.0.0/tggl_client.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      182 2023-04-07 19:27:03.000000 tggl_client-1.0.0/tggl_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-07 19:27:03.000000 tggl_client-1.0.0/tggl_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)        9 2023-04-07 19:27:03.000000 tggl_client-1.0.0/tggl_client.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-07 19:27:03.000000 tggl_client-1.0.0/tggl_client.egg-info/top_level.txt
```

