# Comparing `tmp/pagexml_tools-0.3.2.tar.gz` & `tmp/pagexml_tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagexml_tools-0.3.2.tar", max compression
+gzip compressed data, was "pagexml_tools-0.3.3.tar", max compression
```

## Comparing `pagexml_tools-0.3.2.tar` & `pagexml_tools-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1090 2023-02-16 14:56:00.647522 pagexml_tools-0.3.2/LICENSE
--rw-r--r--   0        0        0     3617 2023-03-14 15:54:03.335111 pagexml_tools-0.3.2/README.md
--rw-r--r--   0        0        0       22 2023-03-14 15:56:29.099000 pagexml_tools-0.3.2/pagexml/__init__.py
--rw-r--r--   0        0        0        0 2022-07-06 13:20:40.880517 pagexml_tools-0.3.2/pagexml/analysis/__init__.py
--rw-r--r--   0        0        0    23754 2023-03-14 15:54:03.352243 pagexml_tools-0.3.2/pagexml/analysis/layout_stats.py
--rw-r--r--   0        0        0     5201 2023-03-14 15:54:03.352545 pagexml_tools-0.3.2/pagexml/analysis/stats.py
--rw-r--r--   0        0        0    49127 2023-03-14 15:54:03.353422 pagexml_tools-0.3.2/pagexml/analysis/text_stats.py
--rw-r--r--   0        0        0    15944 2023-03-14 16:06:33.454463 pagexml_tools-0.3.2/pagexml/column_parser.py
--rw-r--r--   0        0        0        0 2022-07-06 13:20:40.881048 pagexml_tools-0.3.2/pagexml/helper/__init__.py
--rw-r--r--   0        0        0    12061 2023-03-14 16:35:08.831818 pagexml_tools-0.3.2/pagexml/helper/file_helper.py
--rw-r--r--   0        0        0    22113 2023-03-14 16:08:28.033909 pagexml_tools-0.3.2/pagexml/helper/pagexml_helper.py
--rw-r--r--   0        0        0    17353 2023-03-14 16:09:34.238525 pagexml_tools-0.3.2/pagexml/helper/text_helper.py
--rwxr-xr-x   0        0        0        0 2022-04-25 11:16:08.181810 pagexml_tools-0.3.2/pagexml/model/__init__.py
--rw-r--r--   0        0        0    38072 2023-03-14 15:54:03.355625 pagexml_tools-0.3.2/pagexml/model/physical_document_model.py
--rw-r--r--   0        0        0        2 2023-03-01 09:40:10.895404 pagexml_tools-0.3.2/pagexml/pagexml_tools.py
--rw-r--r--   0        0        0    20882 2023-03-14 16:35:08.827843 pagexml_tools-0.3.2/pagexml/parser.py
--rw-r--r--   0        0        0        0 2022-07-06 13:20:40.882557 pagexml_tools-0.3.2/pagexml/plotting/__init__.py
--rw-r--r--   0        0        0     1235 2023-03-01 09:40:10.838606 pagexml_tools-0.3.2/pagexml/plotting/plot_dist.py
--rw-r--r--   0        0        0      963 2023-03-01 13:10:44.524749 pagexml_tools-0.3.2/pagexml/transform/segmentation.py
--rw-r--r--   0        0        0     1312 2023-03-14 15:56:29.072515 pagexml_tools-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 pagexml_tools-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-02-16 14:56:00.647522 pagexml_tools-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3617 2023-03-14 15:54:03.335111 pagexml_tools-0.3.3/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 10:15:14.149186 pagexml_tools-0.3.3/pagexml/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-06 13:20:40.880517 pagexml_tools-0.3.3/pagexml/analysis/__init__.py
+-rw-r--r--   0        0        0    23754 2023-03-14 15:54:03.352243 pagexml_tools-0.3.3/pagexml/analysis/layout_stats.py
+-rw-r--r--   0        0        0     5201 2023-03-14 15:54:03.352545 pagexml_tools-0.3.3/pagexml/analysis/stats.py
+-rw-r--r--   0        0        0    49127 2023-03-14 15:54:03.353422 pagexml_tools-0.3.3/pagexml/analysis/text_stats.py
+-rw-r--r--   0        0        0    15944 2023-03-14 16:06:33.454463 pagexml_tools-0.3.3/pagexml/column_parser.py
+-rw-r--r--   0        0        0        0 2022-07-06 13:20:40.881048 pagexml_tools-0.3.3/pagexml/helper/__init__.py
+-rw-r--r--   0        0        0    12061 2023-03-14 16:35:08.831818 pagexml_tools-0.3.3/pagexml/helper/file_helper.py
+-rw-r--r--   0        0        0    22113 2023-03-14 16:08:28.033909 pagexml_tools-0.3.3/pagexml/helper/pagexml_helper.py
+-rw-r--r--   0        0        0    17353 2023-03-14 16:09:34.238525 pagexml_tools-0.3.3/pagexml/helper/text_helper.py
+-rwxr-xr-x   0        0        0        0 2022-04-25 11:16:08.181810 pagexml_tools-0.3.3/pagexml/model/__init__.py
+-rw-r--r--   0        0        0    38072 2023-03-14 15:54:03.355625 pagexml_tools-0.3.3/pagexml/model/physical_document_model.py
+-rw-r--r--   0        0        0    20899 2023-04-12 10:15:00.526775 pagexml_tools-0.3.3/pagexml/parser.py
+-rw-r--r--   0        0        0        0 2022-07-06 13:20:40.882557 pagexml_tools-0.3.3/pagexml/plotting/__init__.py
+-rw-r--r--   0        0        0     1235 2023-03-01 09:40:10.838606 pagexml_tools-0.3.3/pagexml/plotting/plot_dist.py
+-rw-r--r--   0        0        0      963 2023-03-01 13:10:44.524749 pagexml_tools-0.3.3/pagexml/transform/segmentation.py
+-rw-r--r--   0        0        0     1312 2023-04-12 10:15:14.122787 pagexml_tools-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4923 1970-01-01 00:00:00.000000 pagexml_tools-0.3.3/PKG-INFO
```

### Comparing `pagexml_tools-0.3.2/LICENSE` & `pagexml_tools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/README.md` & `pagexml_tools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/analysis/layout_stats.py` & `pagexml_tools-0.3.3/pagexml/analysis/layout_stats.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/analysis/stats.py` & `pagexml_tools-0.3.3/pagexml/analysis/stats.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/analysis/text_stats.py` & `pagexml_tools-0.3.3/pagexml/analysis/text_stats.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/column_parser.py` & `pagexml_tools-0.3.3/pagexml/column_parser.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/helper/file_helper.py` & `pagexml_tools-0.3.3/pagexml/helper/file_helper.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/helper/pagexml_helper.py` & `pagexml_tools-0.3.3/pagexml/helper/pagexml_helper.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/helper/text_helper.py` & `pagexml_tools-0.3.3/pagexml/helper/text_helper.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/model/physical_document_model.py` & `pagexml_tools-0.3.3/pagexml/model/physical_document_model.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/parser.py` & `pagexml_tools-0.3.3/pagexml/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         )
     except ValueError as err:
         message = f'Error parsing TextLine:\n{json.dumps(textline, indent=4)}\n{err}'
         raise ValueError(message)
 
 
 def parse_conf(text_element: dict) -> Union[float, None]:
-    if '@conf' in text_element:
+    if text_element and '@conf' in text_element:
         if text_element['@conf'] == '':
             return None
         else:
             return float(text_element['@conf'])
     else:
         return None
```

### Comparing `pagexml_tools-0.3.2/pagexml/plotting/plot_dist.py` & `pagexml_tools-0.3.3/pagexml/plotting/plot_dist.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pagexml/transform/segmentation.py` & `pagexml_tools-0.3.3/pagexml/transform/segmentation.py`

 * *Files identical despite different names*

### Comparing `pagexml_tools-0.3.2/pyproject.toml` & `pagexml_tools-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pagexml-tools"
-version = "0.3.2"
+version = "0.3.3"
 description = "Utility functions for reading PageXML files"
 authors = ["Marijn Koolen <marijn.koolen@huygens.knaw.nl>", "Bram Buitendijk <bram.buitendijk@di.huc.knaw.nl>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/knaw-huc/pagexml"
 repository = "https://github.com/knaw-huc/pagexml"
 classifiers = [
```

### Comparing `pagexml_tools-0.3.2/PKG-INFO` & `pagexml_tools-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagexml-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Utility functions for reading PageXML files
 Home-page: https://github.com/knaw-huc/pagexml
 License: MIT
 Author: Marijn Koolen
 Author-email: marijn.koolen@huygens.knaw.nl
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

