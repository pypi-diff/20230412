# Comparing `tmp/xlsx_evaluate-0.4.8.tar.gz` & `tmp/xlsx_evaluate-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlsx_evaluate-0.4.8.tar", max compression
+gzip compressed data, was "xlsx_evaluate-0.5.0.tar", max compression
```

## Comparing `xlsx_evaluate-0.4.8.tar` & `xlsx_evaluate-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1423 2023-01-30 21:15:33.550364 xlsx_evaluate-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     3251 2023-01-30 21:15:32.778354 xlsx_evaluate-0.4.8/readme.md
--rw-r--r--   0        0        0      525 2023-01-30 21:15:33.550364 xlsx_evaluate-0.4.8/xlsx_evaluate/__init__.py
--rw-r--r--   0        0        0     7521 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/ast_nodes.py
--rw-r--r--   0        0        0     3815 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/evaluator.py
--rw-r--r--   0        0        0    12747 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/date.py
--rw-r--r--   0        0        0     6974 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/engineering.py
--rw-r--r--   0        0        0     9474 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/financial.py
--rw-r--r--   0        0        0    14671 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/func_xltypes.py
--rw-r--r--   0        0        0     2426 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/information.py
--rw-r--r--   0        0        0     2812 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/logical.py
--rw-r--r--   0        0        0     2807 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/lookup.py
--rw-r--r--   0        0        0    18251 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/math.py
--rw-r--r--   0        0        0     2612 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/operator.py
--rw-r--r--   0        0        0     4113 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/statistics.py
--rw-r--r--   0        0        0     6904 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/text.py
--rw-r--r--   0        0        0      640 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/utils.py
--rw-r--r--   0        0        0     3809 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/xl.py
--rw-r--r--   0        0        0     1595 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/xlcriteria.py
--rw-r--r--   0        0        0     2078 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/functions/xlerrors.py
--rw-r--r--   0        0        0    13020 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/model.py
--rw-r--r--   0        0        0    11358 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/parser.py
--rw-r--r--   0        0        0     2116 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/patch.py
--rw-r--r--   0        0        0     1388 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/reader.py
--rw-r--r--   0        0        0    20971 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/tokenizer.py
--rw-r--r--   0        0        0     2944 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/utils.py
--rw-r--r--   0        0        0     3378 2023-01-30 21:15:32.786353 xlsx_evaluate-0.4.8/xlsx_evaluate/xltypes.py
--rw-r--r--   0        0        0     4261 1970-01-01 00:00:00.000000 xlsx_evaluate-0.4.8/setup.py
--rw-r--r--   0        0        0     4316 1970-01-01 00:00:00.000000 xlsx_evaluate-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1423 2023-04-12 11:15:23.090756 xlsx_evaluate-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3251 2023-04-12 11:15:22.242735 xlsx_evaluate-0.5.0/readme.md
+-rw-r--r--   0        0        0      525 2023-04-12 11:15:23.090756 xlsx_evaluate-0.5.0/xlsx_evaluate/__init__.py
+-rw-r--r--   0        0        0     7521 2023-04-12 11:15:22.250735 xlsx_evaluate-0.5.0/xlsx_evaluate/ast_nodes.py
+-rw-r--r--   0        0        0     3815 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/evaluator.py
+-rw-r--r--   0        0        0    12747 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/date.py
+-rw-r--r--   0        0        0     6974 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/engineering.py
+-rw-r--r--   0        0        0     9474 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/financial.py
+-rw-r--r--   0        0        0    14671 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/func_xltypes.py
+-rw-r--r--   0        0        0     2426 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/information.py
+-rw-r--r--   0        0        0     3255 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/logical.py
+-rw-r--r--   0        0        0     2807 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/lookup.py
+-rw-r--r--   0        0        0    18251 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/math.py
+-rw-r--r--   0        0        0     2612 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/operator.py
+-rw-r--r--   0        0        0     4113 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/statistics.py
+-rw-r--r--   0        0        0     6904 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/text.py
+-rw-r--r--   0        0        0      640 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/utils.py
+-rw-r--r--   0        0        0     3809 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/xl.py
+-rw-r--r--   0        0        0     1595 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/xlcriteria.py
+-rw-r--r--   0        0        0     2078 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/functions/xlerrors.py
+-rw-r--r--   0        0        0    13020 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/model.py
+-rw-r--r--   0        0        0    11358 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/parser.py
+-rw-r--r--   0        0        0     2116 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/patch.py
+-rw-r--r--   0        0        0     1388 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/reader.py
+-rw-r--r--   0        0        0    20971 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/tokenizer.py
+-rw-r--r--   0        0        0     2944 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/utils.py
+-rw-r--r--   0        0        0     3378 2023-04-12 11:15:22.254736 xlsx_evaluate-0.5.0/xlsx_evaluate/xltypes.py
+-rw-r--r--   0        0        0     4316 1970-01-01 00:00:00.000000 xlsx_evaluate-0.5.0/PKG-INFO
```

### Comparing `xlsx_evaluate-0.4.8/pyproject.toml` & `xlsx_evaluate-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xlsx_evaluate"
-version = "0.4.8"
+version = "0.5.0"
 description = "Calculate XLSX formulas"
 authors = ["Victor <lyferov@yandex.ru>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/devind-team/xlsx_evaluate"
 repository = "https://github.com/devind-team/xlsx_evaluate"
 keywords = ["openpyxlsx", "xlsx", "formulas", "evaluate"]
```

### Comparing `xlsx_evaluate-0.4.8/readme.md` & `xlsx_evaluate-0.5.0/readme.md`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/__init__.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,8 @@
     lookup,
     math,
     operator,
     statistics,
     text
 )
 
-__version__ = '0.4.8'
+__version__ = '0.5.0'
```

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/ast_nodes.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/ast_nodes.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/evaluator.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/evaluator.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/date.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/date.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/engineering.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/engineering.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/financial.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/financial.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/func_xltypes.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/func_xltypes.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/information.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/information.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/logical.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/logical.py`

 * *Files 14% similar despite different names*

```diff
@@ -93,7 +93,23 @@
 @xl.validate_args
 def NOT(logical: func_xltypes.XlExpr) -> func_xltypes.XlBoolean:
     """Return inverse of boolean representation of value.
 
     https://support.microsoft.com/en-us/office/not-function-9cfc6011-a054-40c7-a140-cd4ba2d87d77
     """
     return not bool(logical())
+
+
+@xl.register()
+@xl.validate_args
+def IFERROR(
+        logical_test: func_xltypes.XlExpr,
+        value_if_error: func_xltypes.XlExpr,
+):
+    """Return value if not error and another value if an error has occurred.
+
+    https://support.microsoft.com/en-us/office/iferror-function-c526fd07-caeb-47b8-8bb6-63f3e417f611
+    """
+    val = logical_test()
+    if isinstance(val, xlerrors.ExcelError):
+        return value_if_error()
+    return val
```

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/lookup.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/lookup.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/math.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/math.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/operator.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/operator.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/statistics.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/statistics.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/text.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/text.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/utils.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/utils.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/xl.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/xl.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/xlcriteria.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/xlcriteria.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/functions/xlerrors.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/functions/xlerrors.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/model.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/model.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/parser.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/parser.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/patch.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/patch.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/reader.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/reader.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/tokenizer.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/tokenizer.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/utils.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/xlsx_evaluate/xltypes.py` & `xlsx_evaluate-0.5.0/xlsx_evaluate/xltypes.py`

 * *Files identical despite different names*

### Comparing `xlsx_evaluate-0.4.8/PKG-INFO` & `xlsx_evaluate-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlsx-evaluate
-Version: 0.4.8
+Version: 0.5.0
 Summary: Calculate XLSX formulas
 Home-page: https://github.com/devind-team/xlsx_evaluate
 License: MIT
 Keywords: openpyxlsx,xlsx,formulas,evaluate
 Author: Victor
 Author-email: lyferov@yandex.ru
 Requires-Python: >=3.9
```

