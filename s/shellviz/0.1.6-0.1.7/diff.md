# Comparing `tmp/shellviz-0.1.6.tar.gz` & `tmp/shellviz-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellviz-0.1.6.tar", max compression
+gzip compressed data, was "shellviz-0.1.7.tar", max compression
```

## Comparing `shellviz-0.1.6.tar` & `shellviz-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1060 2023-04-12 06:44:46.797833 shellviz-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-04-12 06:44:46.797887 shellviz-0.1.6/README.md
--rw-r--r--   0        0        0      328 2023-04-12 07:00:13.423040 shellviz-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1377 2023-04-12 07:00:06.750786 shellviz-0.1.6/shellviz/__init__.py
--rw-r--r--   0        0        0      289 1970-01-01 00:00:00.000000 shellviz-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-12 06:44:46.797833 shellviz-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-04-12 06:44:46.797887 shellviz-0.1.7/README.md
+-rw-r--r--   0        0        0      327 2023-04-12 07:08:22.319609 shellviz-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1377 2023-04-12 07:00:06.750786 shellviz-0.1.7/shellviz/__init__.py
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 shellviz-0.1.7/PKG-INFO
```

### Comparing `shellviz-0.1.6/LICENSE.txt` & `shellviz-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shellviz-0.1.6/shellviz/__init__.py` & `shellviz-0.1.7/shellviz/__init__.py`

 * *Files identical despite different names*

