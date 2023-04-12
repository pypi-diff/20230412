# Comparing `tmp/lupin-danquin-0.0.1.dev5.tar.gz` & `tmp/lupin-danquin-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev5.tar", last modified: Wed Apr 12 09:47:23 2023, max compression
+gzip compressed data, was "lupin-danquin-0.0.1.dev6.tar", last modified: Wed Apr 12 09:52:09 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev5.tar` & `lupin-danquin-0.0.1.dev6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.323485 lupin-danquin-0.0.1.dev5/
--rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev5/LICENCE
--rw-rw-rw-   0        0        0       67 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev5/MANIFEST.in
--rw-rw-rw-   0        0        0      573 2023-04-12 09:47:23.323485 lupin-danquin-0.0.1.dev5/PKG-INFO
--rw-rw-rw-   0        0        0     1010 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.293865 lupin-danquin-0.0.1.dev5/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-12 09:47:23.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.313050 lupin-danquin-0.0.1.dev5/lupin_danquin/assets/
--rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/assets/BeginingOfFile.md
--rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/assets/EndOfFile.md
--rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/check_coding_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.319486 lupin-danquin-0.0.1.dev5/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/application.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.320486 lupin-danquin-0.0.1.dev5/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0     2206 2023-04-12 08:36:50.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.322484 lupin-danquin-0.0.1.dev5/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     2940 2023-04-12 09:46:49.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     2509 2023-04-12 08:32:27.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/run.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.323485 lupin-danquin-0.0.1.dev5/lupin_danquin/templates/
--rw-rw-rw-   0        0        0     2801 2023-04-11 15:18:48.000000 lupin-danquin-0.0.1.dev5/lupin_danquin/templates/val3_documentation_md.j2
-drwxrwxrwx   0        0        0        0 2023-04-12 09:47:23.311050 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-12 09:47:23.000000 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-12 09:47:23.000000 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:47:23.000000 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-12 09:47:23.000000 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-04-12 09:47:23.000000 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 09:47:23.000000 lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      906 2023-04-12 09:47:23.327995 lupin-danquin-0.0.1.dev5/setup.cfg
--rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.369083 lupin-danquin-0.0.1.dev6/
+-rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev6/LICENCE
+-rw-rw-rw-   0        0        0       67 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev6/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2023-04-12 09:52:09.369083 lupin-danquin-0.0.1.dev6/PKG-INFO
+-rw-rw-rw-   0        0        0     1010 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.337541 lupin-danquin-0.0.1.dev6/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-12 09:52:09.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.355569 lupin-danquin-0.0.1.dev6/lupin_danquin/assets/
+-rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/assets/BeginingOfFile.md
+-rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/assets/EndOfFile.md
+-rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/check_coding_rules.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.363568 lupin-danquin-0.0.1.dev6/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/application.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.365074 lupin-danquin-0.0.1.dev6/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     2206 2023-04-12 08:36:50.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.367082 lupin-danquin-0.0.1.dev6/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     2948 2023-04-12 09:51:31.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     2509 2023-04-12 08:32:27.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.368081 lupin-danquin-0.0.1.dev6/lupin_danquin/templates/
+-rw-rw-rw-   0        0        0     2801 2023-04-11 15:18:48.000000 lupin-danquin-0.0.1.dev6/lupin_danquin/templates/val3_documentation_md.j2
+drwxrwxrwx   0        0        0        0 2023-04-12 09:52:09.353054 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-12 09:52:09.000000 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-12 09:52:09.000000 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:52:09.000000 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-12 09:52:09.000000 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-12 09:52:09.000000 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 09:52:09.000000 lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-04-12 09:52:09.375593 lupin-danquin-0.0.1.dev6/setup.cfg
+-rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev6/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev5/LICENCE` & `lupin-danquin-0.0.1.dev6/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/PKG-INFO` & `lupin-danquin-0.0.1.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev5
+Version: 0.0.1.dev6
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev5/README.md` & `lupin-danquin-0.0.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/assets/BeginingOfFile.md` & `lupin-danquin-0.0.1.dev6/lupin_danquin/assets/BeginingOfFile.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/check_coding_rules.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/check_coding_rules.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/core/application.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/core/global_variable.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/core/local_variable.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/core/parameter.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/core/program.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/core/tools/utils.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,8 +78,8 @@
         except (TemplateError, TemplateRuntimeError) as e:
             die(msg=f"Error rendering Jinja2 template: {e}")
 
         with codecs.open(
             "./val3_documentation.md", "w", encoding="utf-8"
         ) as f:
             f.write(content)
-        info(msg="Documentation generated")
+        info(msg="val3_documentation.md generated")
```

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/run.py` & `lupin-danquin-0.0.1.dev6/lupin_danquin/run.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin/templates/val3_documentation_md.j2` & `lupin-danquin-0.0.1.dev6/lupin_danquin/templates/val3_documentation_md.j2`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev5
+Version: 0.0.1.dev6
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev5/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-0.0.1.dev6/lupin_danquin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev5/setup.cfg` & `lupin-danquin-0.0.1.dev6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 312e 6465 7635 0d0a 6465 7363 7269 7074  1.dev5..descript
+00000030: 312e 6465 7636 0d0a 6465 7363 7269 7074  1.dev6..descript
 00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
 00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
 00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
 00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
 00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
 000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords =
```

