# Comparing `tmp/lupin-danquin-0.0.1.dev7.tar.gz` & `tmp/lupin-danquin-0.0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev7.tar", last modified: Wed Apr 12 10:47:07 2023, max compression
+gzip compressed data, was "lupin-danquin-0.0.1.dev8.tar", last modified: Wed Apr 12 10:49:45 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev7.tar` & `lupin-danquin-0.0.1.dev8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.216595 lupin-danquin-0.0.1.dev7/
--rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev7/LICENCE
--rw-rw-rw-   0        0        0       67 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev7/MANIFEST.in
--rw-rw-rw-   0        0        0      576 2023-04-12 10:47:07.216595 lupin-danquin-0.0.1.dev7/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-04-12 10:45:59.000000 lupin-danquin-0.0.1.dev7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.191652 lupin-danquin-0.0.1.dev7/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-12 10:47:07.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.206501 lupin-danquin-0.0.1.dev7/lupin_danquin/assets/
--rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/assets/BeginingOfFile.md
--rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/assets/EndOfFile.md
--rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/check_coding_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.212596 lupin-danquin-0.0.1.dev7/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/application.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.213595 lupin-danquin-0.0.1.dev7/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0     2206 2023-04-12 08:36:50.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.215597 lupin-danquin-0.0.1.dev7/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     2948 2023-04-12 09:51:31.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     2509 2023-04-12 08:32:27.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/run.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.215597 lupin-danquin-0.0.1.dev7/lupin_danquin/templates/
--rw-rw-rw-   0        0        0     2801 2023-04-11 15:18:48.000000 lupin-danquin-0.0.1.dev7/lupin_danquin/templates/val3_documentation_md.j2
-drwxrwxrwx   0        0        0        0 2023-04-12 10:47:07.205501 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      576 2023-04-12 10:47:07.000000 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-12 10:47:07.000000 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:47:07.000000 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-12 10:47:07.000000 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-04-12 10:47:07.000000 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 10:47:07.000000 lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      898 2023-04-12 10:47:07.221103 lupin-danquin-0.0.1.dev7/setup.cfg
--rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.781654 lupin-danquin-0.0.1.dev8/
+-rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev8/LICENCE
+-rw-rw-rw-   0        0        0       67 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev8/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2023-04-12 10:49:45.781654 lupin-danquin-0.0.1.dev8/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-04-12 10:45:59.000000 lupin-danquin-0.0.1.dev8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.755178 lupin-danquin-0.0.1.dev8/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.771301 lupin-danquin-0.0.1.dev8/lupin_danquin/assets/
+-rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/assets/BeginingOfFile.md
+-rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/assets/EndOfFile.md
+-rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/check_coding_rules.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.777300 lupin-danquin-0.0.1.dev8/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/application.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.778303 lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     2206 2023-04-12 08:36:50.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.780656 lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     2948 2023-04-12 09:51:31.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     2509 2023-04-12 08:32:27.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.780656 lupin-danquin-0.0.1.dev8/lupin_danquin/templates/
+-rw-rw-rw-   0        0        0     2801 2023-04-11 15:18:48.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/templates/val3_documentation_md.j2
+drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.769301 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-04-12 10:49:45.782655 lupin-danquin-0.0.1.dev8/setup.cfg
+-rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev8/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev7/LICENCE` & `lupin-danquin-0.0.1.dev8/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/PKG-INFO` & `lupin-danquin-0.0.1.dev8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev7
-Summary: # Documentation extraction
+Version: 0.0.1.dev8
+Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-danquin-0.0.1.dev7/README.md` & `lupin-danquin-0.0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/assets/BeginingOfFile.md` & `lupin-danquin-0.0.1.dev8/lupin_danquin/assets/BeginingOfFile.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/check_coding_rules.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/check_coding_rules.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/core/application.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/core/global_variable.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/core/local_variable.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/core/parameter.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/core/program.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/core/tools/utils.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/run.py` & `lupin-danquin-0.0.1.dev8/lupin_danquin/run.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin/templates/val3_documentation_md.j2` & `lupin-danquin-0.0.1.dev8/lupin_danquin/templates/val3_documentation_md.j2`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev7
-Summary: # Documentation extraction
+Version: 0.0.1.dev8
+Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-danquin-0.0.1.dev7/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev7/setup.cfg` & `lupin-danquin-0.0.1.dev8/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 312e 6465 7637 0d0a 6465 7363 7269 7074  1.dev7..descript
-00000040: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-00000050: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-00000060: 7269 7074 696f 6e20 3d20 5465 7374 2056  ription = Test V
-00000070: 414c 3320 636f 6465 2061 6e64 2067 656e  AL3 code and gen
-00000080: 6572 6174 6520 646f 6375 6d65 6e74 6174  erate documentat
-00000090: 696f 6e20 6672 6f6d 2069 740d 0a6b 6579  ion from it..key
-000000a0: 776f 7264 7320 3d20 646f 6375 6d65 6e74  words = document
-000000b0: 6174 696f 6e2c 2074 6573 7469 6e67 0d0a  ation, testing..
-000000c0: 6c69 6365 6e73 6520 3d20 4d49 5420 4c69  license = MIT Li
-000000d0: 6365 6e73 650d 0a63 6c61 7373 6966 6965  cense..classifie
-000000e0: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-000000f0: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
-00000100: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
-00000110: 6564 2041 7564 6965 6e63 6520 3a3a 2049  ed Audience :: I
-00000120: 6e66 6f72 6d61 7469 6f6e 2054 6563 686e  nformation Techn
-00000130: 6f6c 6f67 790d 0a09 546f 7069 6320 3a3a  ology...Topic ::
-00000140: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
-00000150: 706d 656e 7420 3a3a 2054 6573 7469 6e67  pment :: Testing
-00000160: 0d0a 0954 6f70 6963 203a 3a20 446f 6375  ...Topic :: Docu
-00000170: 6d65 6e74 6174 696f 6e0d 0a09 5072 6f67  mentation...Prog
-00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000001a0: 3130 0d0a 094c 6963 656e 7365 203a 3a20  10...License :: 
-000001b0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000001c0: 4d49 5420 4c69 6365 6e73 650d 0a0d 0a5b  MIT License....[
-000001d0: 6f70 7469 6f6e 735d 0d0a 7a69 705f 7361  options]..zip_sa
-000001e0: 6665 203d 2046 616c 7365 0d0a 696e 636c  fe = False..incl
-000001f0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-00000200: 203d 2054 7275 650d 0a70 6163 6b61 6765   = True..package
-00000210: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000220: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000230: 2e31 300d 0a69 6e73 7461 6c6c 5f72 6571  .10..install_req
-00000240: 7569 7265 7320 3d20 0d0a 0974 7970 6572  uires = ...typer
-00000250: 5b61 6c6c 5d3d 3d30 2e36 2e31 0d0a 0970  [all]==0.6.1...p
-00000260: 7974 686f 6e2d 646f 7465 6e76 3d3d 302e  ython-dotenv==0.
-00000270: 3231 2e30 0d0a 094a 696e 6a61 323d 3d33  21.0...Jinja2==3
-00000280: 2e31 2e32 0d0a 0d0a 5b6f 7074 696f 6e73  .1.2....[options
-00000290: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-000002a0: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
-000002b0: 3d20 0d0a 0964 616e 7120 3d20 6c75 7069  = ...danq = lupi
-000002c0: 6e5f 6461 6e71 7569 6e2e 7275 6e3a 636c  n_danquin.run:cl
-000002d0: 690d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  i....[options.ex
-000002e0: 7472 6173 5f72 6571 7569 7265 5d0d 0a74  tras_require]..t
-000002f0: 6573 7420 3d20 0d0a 0970 7974 6573 743d  est = ...pytest=
-00000300: 3d37 2e32 2e32 0d0a 0966 6c61 6b65 383d  =7.2.2...flake8=
-00000310: 3d36 2e30 2e30 0d0a 0d0a 5b6f 7074 696f  =6.0.0....[optio
-00000320: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000330: 5d0d 0a65 7863 6c75 6465 203d 200d 0a09  ]..exclude = ...
-00000340: 6c75 7069 6e5f 6461 6e71 7569 6e2e 7465  lupin_danquin.te
-00000350: 7374 732a 0d0a 0d0a 5b65 6767 5f69 6e66  sts*....[egg_inf
-00000360: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000370: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000380: 0d0a                                     ..
+00000030: 312e 6465 7638 0d0a 6465 7363 7269 7074  1.dev8..descript
+00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
+00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
+00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
+00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
+00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
+000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords = 
+000000b0: 646f 6375 6d65 6e74 6174 696f 6e2c 2074  documentation, t
+000000c0: 6573 7469 6e67 0d0a 6c69 6365 6e73 6520  esting..license 
+000000d0: 3d20 4d49 5420 4c69 6365 6e73 650d 0a63  = MIT License..c
+000000e0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000000f0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000100: 7573 203a 3a20 3320 2d20 416c 7068 610d  us :: 3 - Alpha.
+00000110: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+00000120: 6e63 6520 3a3a 2049 6e66 6f72 6d61 7469  nce :: Informati
+00000130: 6f6e 2054 6563 686e 6f6c 6f67 790d 0a09  on Technology...
+00000140: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000150: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+00000160: 2054 6573 7469 6e67 0d0a 0954 6f70 6963   Testing...Topic
+00000170: 203a 3a20 446f 6375 6d65 6e74 6174 696f   :: Documentatio
+00000180: 6e0d 0a09 5072 6f67 7261 6d6d 696e 6720  n...Programming 
+00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001a0: 6f6e 203a 3a20 332e 3130 0d0a 094c 6963  on :: 3.10...Lic
+000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000001d0: 6e73 650d 0a0d 0a5b 6f70 7469 6f6e 735d  nse....[options]
+000001e0: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
+000001f0: 7365 0d0a 696e 636c 7564 655f 7061 636b  se..include_pack
+00000200: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
+00000210: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000220: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+00000230: 6573 203d 203e 3d33 2e31 300d 0a69 6e73  es = >=3.10..ins
+00000240: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000250: 0d0a 0974 7970 6572 5b61 6c6c 5d3d 3d30  ...typer[all]==0
+00000260: 2e36 2e31 0d0a 0970 7974 686f 6e2d 646f  .6.1...python-do
+00000270: 7465 6e76 3d3d 302e 3231 2e30 0d0a 094a  tenv==0.21.0...J
+00000280: 696e 6a61 323d 3d33 2e31 2e32 0d0a 0d0a  inja2==3.1.2....
+00000290: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+000002a0: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
+000002b0: 7363 7269 7074 7320 3d20 0d0a 0964 616e  scripts = ...dan
+000002c0: 7120 3d20 6c75 7069 6e5f 6461 6e71 7569  q = lupin_danqui
+000002d0: 6e2e 7275 6e3a 636c 690d 0a0d 0a5b 6f70  n.run:cli....[op
+000002e0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+000002f0: 7569 7265 5d0d 0a74 6573 7420 3d20 0d0a  uire]..test = ..
+00000300: 0970 7974 6573 743d 3d37 2e32 2e32 0d0a  .pytest==7.2.2..
+00000310: 0966 6c61 6b65 383d 3d36 2e30 2e30 0d0a  .flake8==6.0.0..
+00000320: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000330: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
+00000340: 6465 203d 200d 0a09 6c75 7069 6e5f 6461  de = ...lupin_da
+00000350: 6e71 7569 6e2e 7465 7374 732a 0d0a 0d0a  nquin.tests*....
+00000360: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000370: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000380: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

