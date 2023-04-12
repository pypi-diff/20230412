# Comparing `tmp/eth_abi_lite-3.1.0.tar.gz` & `tmp/eth_abi_lite-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth_abi_lite-3.1.0.tar", last modified: Sun Apr  9 06:14:57 2023, max compression
+gzip compressed data, was "eth_abi_lite-3.2.0.tar", last modified: Wed Apr 12 18:46:27 2023, max compression
```

## Comparing `eth_abi_lite-3.1.0.tar` & `eth_abi_lite-3.2.0.tar`

### file list

```diff
@@ -1,51 +1,61 @@
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.186220 eth_abi_lite-3.1.0/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1090 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/LICENSE
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      148 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/MANIFEST.in
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     5150 2023-04-09 06:14:57.186089 eth_abi_lite-3.1.0/PKG-INFO
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     4188 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/README.md
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1036 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/pyproject.toml
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       13 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/requirements-docs.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       38 2023-04-09 06:14:57.186259 eth_abi_lite-3.1.0/setup.cfg
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     2469 2023-04-09 06:12:23.000000 eth_abi_lite-3.1.0/setup.py
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.179434 eth_abi_lite-3.1.0/src/
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.182379 eth_abi_lite-3.1.0/src/eth_abi_lite/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      314 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/__init__.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      396 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/abi.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     4847 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/base.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     5824 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/codec.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       57 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/constants.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    16875 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/decoding.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    20309 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/encoding.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     2932 2023-04-01 17:42:17.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/exceptions.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    12233 2023-04-01 17:42:38.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/grammar.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      313 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/packed.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)        0 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/py.typed
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    19140 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/registry.py
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.183831 eth_abi_lite-3.1.0/src/eth_abi_lite/tools/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       65 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/tools/__init__.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     5806 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/tools/_strategies.py
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.184377 eth_abi_lite-3.1.0/src/eth_abi_lite/utils/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)        0 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/utils/__init__.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     2089 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/utils/numeric.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      437 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/utils/padding.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      435 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_abi_lite/utils/string.py
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.183489 eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     5150 2023-04-09 06:14:57.000000 eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/PKG-INFO
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1196 2023-04-09 06:14:57.000000 eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/SOURCES.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)        1 2023-04-09 06:14:57.000000 eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/dependency_links.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)        1 2023-04-01 17:27:12.000000 eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/not-zip-safe
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      686 2023-04-09 06:14:57.000000 eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/requires.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       44 2023-04-09 06:14:57.000000 eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/top_level.txt
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.184535 eth_abi_lite-3.1.0/src/eth_typing_lite/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      394 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_typing_lite/__init__.py
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:14:57.185910 eth_abi_lite-3.1.0/src/eth_utils_lite/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      215 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/__init__.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     2088 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/abi.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     4245 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/address.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     5362 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/conversions.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      333 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/crypto.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     3895 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/decorators.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      199 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/encoding.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1812 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/functional.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1876 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/hexadecimal.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1065 2023-04-01 17:26:55.000000 eth_abi_lite-3.1.0/src/eth_utils_lite/types.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.805963 eth_abi_lite-3.2.0/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1090 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/LICENSE
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      148 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/MANIFEST.in
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     5150 2023-04-12 18:46:27.805836 eth_abi_lite-3.2.0/PKG-INFO
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     4188 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/README.md
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1036 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/pyproject.toml
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       13 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/requirements-docs.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       38 2023-04-12 18:46:27.806000 eth_abi_lite-3.2.0/setup.cfg
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     2468 2023-04-12 18:30:19.000000 eth_abi_lite-3.2.0/setup.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.798076 eth_abi_lite-3.2.0/src/
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.800739 eth_abi_lite-3.2.0/src/eth_abi_lite/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      314 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      396 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/abi.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     4847 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/base.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     5824 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/codec.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       57 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/constants.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    16875 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/decoding.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    20309 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/encoding.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     2932 2023-04-01 17:42:17.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/exceptions.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    12233 2023-04-01 17:42:38.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/grammar.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      313 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/packed.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)        0 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/py.typed
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    19140 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/registry.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.802186 eth_abi_lite-3.2.0/src/eth_abi_lite/tools/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       65 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/tools/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     5806 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/tools/_strategies.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.802762 eth_abi_lite-3.2.0/src/eth_abi_lite/utils/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)        0 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/utils/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     2089 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/utils/numeric.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      437 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/utils/padding.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      435 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_abi_lite/utils/string.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.801797 eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     5150 2023-04-12 18:46:27.000000 eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/PKG-INFO
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1448 2023-04-12 18:46:27.000000 eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)        1 2023-04-12 18:46:27.000000 eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)        1 2023-04-01 17:27:12.000000 eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/not-zip-safe
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      652 2023-04-12 18:46:27.000000 eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/requires.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       71 2023-04-12 18:46:27.000000 eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/top_level.txt
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.802930 eth_abi_lite-3.2.0/src/eth_typing_lite/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      394 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_typing_lite/__init__.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.804462 eth_abi_lite-3.2.0/src/eth_utils_lite/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      215 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     2088 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/abi.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     4245 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/address.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     5362 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/conversions.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      333 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/crypto.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     3895 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/decorators.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      199 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/encoding.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1812 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/functional.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1876 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/hexadecimal.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1065 2023-04-01 17:26:55.000000 eth_abi_lite-3.2.0/src/eth_utils_lite/types.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.805342 eth_abi_lite-3.2.0/src/parsimonious_lite/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      436 2023-04-12 18:26:42.000000 eth_abi_lite-3.2.0/src/parsimonious_lite/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     3773 2023-04-12 18:31:26.000000 eth_abi_lite-3.2.0/src/parsimonious_lite/exceptions.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    16532 2023-04-12 18:32:03.000000 eth_abi_lite-3.2.0/src/parsimonious_lite/expressions.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    19461 2023-04-12 18:31:36.000000 eth_abi_lite-3.2.0/src/parsimonious_lite/grammar.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    13192 2023-04-12 18:31:21.000000 eth_abi_lite-3.2.0/src/parsimonious_lite/nodes.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1166 2023-04-12 18:31:30.000000 eth_abi_lite-3.2.0/src/parsimonious_lite/utils.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-12 18:46:27.805619 eth_abi_lite-3.2.0/src/six_lite/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       24 2023-04-12 18:35:51.000000 eth_abi_lite-3.2.0/src/six_lite/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    34658 2023-04-12 18:37:42.000000 eth_abi_lite-3.2.0/src/six_lite/six_lite.py
```

### Comparing `eth_abi_lite-3.1.0/LICENSE` & `eth_abi_lite-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/PKG-INFO` & `eth_abi_lite-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth_abi_lite
-Version: 3.1.0
+Version: 3.2.0
 Summary: eth_abi_lite is a lite fork of `eth_abi`, aiming to support EVM abi encode/decode functionality without external dependencies on `eth_utils`, `eth_typing`, `toolz`, or `cytoolz`
 Home-page: https://github.com/sslivkoff/eth-abi-lite
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eth_abi_lite-3.1.0/README.md` & `eth_abi_lite-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/pyproject.toml` & `eth_abi_lite-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/setup.py` & `eth_abi_lite-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,36 +50,36 @@
 
 with open('./README.md') as readme:
     long_description = readme.read()
 
 
 setup(
     name='eth_abi_lite',
-    version='3.1.0',
+    version='3.2.0',
     description="""eth_abi_lite is a lite fork of `eth_abi`, aiming to support EVM abi encode/decode functionality without external dependencies on `eth_utils`, `eth_typing`, `toolz`, or `cytoolz`""",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sslivkoff/eth-abi-lite',
     include_package_data=True,
-    install_requires=[
-        'parsimonious-lite>=0.11.0,<0.12.0',
-    ],
+    install_requires=[],
     python_requires='>=3.7, <4',
     extras_require=extras_require,
     py_modules=['eth_abi_lite'],
     license="MIT",
     zip_safe=False,
     keywords='ethereum',
     package_dir={"": 'src'},
     packages=[
         'eth_abi_lite',
         'eth_abi_lite.tools',
         'eth_abi_lite.utils',
         'eth_utils_lite',
         'eth_typing_lite',
+        'parsimonious_lite',
+        'six_lite',
     ],
     package_data={'eth_abi_lite': ['py.typed']},
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
```

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/base.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/base.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/codec.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/codec.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/decoding.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/decoding.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/encoding.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/encoding.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/exceptions.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/grammar.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/grammar.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/registry.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/registry.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/tools/_strategies.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite/utils/numeric.py` & `eth_abi_lite-3.2.0/src/eth_abi_lite/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/PKG-INFO` & `eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-abi-lite
-Version: 3.1.0
+Version: 3.2.0
 Summary: eth_abi_lite is a lite fork of `eth_abi`, aiming to support EVM abi encode/decode functionality without external dependencies on `eth_utils`, `eth_typing`, `toolz`, or `cytoolz`
 Home-page: https://github.com/sslivkoff/eth-abi-lite
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/SOURCES.txt` & `eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -34,8 +34,16 @@
 src/eth_utils_lite/address.py
 src/eth_utils_lite/conversions.py
 src/eth_utils_lite/crypto.py
 src/eth_utils_lite/decorators.py
 src/eth_utils_lite/encoding.py
 src/eth_utils_lite/functional.py
 src/eth_utils_lite/hexadecimal.py
-src/eth_utils_lite/types.py
+src/eth_utils_lite/types.py
+src/parsimonious_lite/__init__.py
+src/parsimonious_lite/exceptions.py
+src/parsimonious_lite/expressions.py
+src/parsimonious_lite/grammar.py
+src/parsimonious_lite/nodes.py
+src/parsimonious_lite/utils.py
+src/six_lite/__init__.py
+src/six_lite/six_lite.py
```

### Comparing `eth_abi_lite-3.1.0/src/eth_abi_lite.egg-info/requires.txt` & `eth_abi_lite-3.2.0/src/eth_abi_lite.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-parsimonious-lite<0.12.0,>=0.11.0
 
 [dev]
 bumpversion<1,>=0.5.3
 pytest-watch<5,>=4.1.0
 wheel
 twine
 ipython
```

### Comparing `eth_abi_lite-3.1.0/src/eth_utils_lite/abi.py` & `eth_abi_lite-3.2.0/src/eth_utils_lite/abi.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_utils_lite/address.py` & `eth_abi_lite-3.2.0/src/eth_utils_lite/address.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_utils_lite/conversions.py` & `eth_abi_lite-3.2.0/src/eth_utils_lite/conversions.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_utils_lite/decorators.py` & `eth_abi_lite-3.2.0/src/eth_utils_lite/decorators.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_utils_lite/functional.py` & `eth_abi_lite-3.2.0/src/eth_utils_lite/functional.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_utils_lite/hexadecimal.py` & `eth_abi_lite-3.2.0/src/eth_utils_lite/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `eth_abi_lite-3.1.0/src/eth_utils_lite/types.py` & `eth_abi_lite-3.2.0/src/eth_utils_lite/types.py`

 * *Files identical despite different names*

