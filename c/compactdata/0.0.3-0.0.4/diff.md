# Comparing `tmp/compactdata-0.0.3.tar.gz` & `tmp/compactdata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compactdata-0.0.3.tar", max compression
+gzip compressed data, was "compactdata-0.0.4.tar", max compression
```

## Comparing `compactdata-0.0.3.tar` & `compactdata-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-03-28 11:58:20.750185 compactdata-0.0.3/LICENSE
--rw-r--r--   0        0        0       77 2023-03-28 11:58:20.750237 compactdata-0.0.3/README.md
--rw-r--r--   0        0        0     2818 2023-03-28 12:00:33.219542 compactdata-0.0.3/compactdata/__init__.py
--rw-r--r--   0        0        0      668 2023-03-28 12:00:33.218612 compactdata-0.0.3/compactdata/decoder.py
--rw-r--r--   0        0        0    14672 2023-03-28 12:00:33.221564 compactdata-0.0.3/compactdata/encoder.py
--rw-r--r--   0        0        0     5097 2023-03-28 12:00:33.222197 compactdata-0.0.3/compactdata/escapes.py
--rwxr-xr-x   0        0        0     1892 2023-03-28 12:00:33.221801 compactdata-0.0.3/compactdata/grammar_rules.py
--rw-r--r--   0        0        0     5152 2023-03-28 12:00:33.219117 compactdata-0.0.3/compactdata/parsetab.py
--rwxr-xr-x   0        0        0     1101 2023-03-28 12:00:33.222422 compactdata-0.0.3/compactdata/token_definitions.py
--rw-r--r--   0        0        0      592 2023-03-28 12:06:23.869805 compactdata-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 compactdata-0.0.3/setup.py
--rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 compactdata-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-28 11:58:20.750185 compactdata-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3114 2023-03-28 12:27:49.401856 compactdata-0.0.4/README.md
+-rw-r--r--   0        0        0     2852 2023-03-31 01:53:09.664390 compactdata-0.0.4/compactdata/__init__.py
+-rw-r--r--   0        0        0     4312 2023-04-11 08:57:31.150330 compactdata-0.0.4/compactdata/char_constants.py
+-rw-r--r--   0        0        0      617 2023-03-31 01:53:09.613163 compactdata-0.0.4/compactdata/decoder.py
+-rw-r--r--   0        0        0    15104 2023-03-31 01:53:09.805959 compactdata-0.0.4/compactdata/encoder.py
+-rw-r--r--   0        0        0     2653 2023-04-11 09:09:24.043352 compactdata-0.0.4/compactdata/escapes.py
+-rw-r--r--   0        0        0      102 2023-03-31 01:53:09.180510 compactdata-0.0.4/compactdata/exceptions.py
+-rwxr-xr-x   0        0        0     2022 2023-03-30 15:38:40.709005 compactdata-0.0.4/compactdata/grammar_rules.py
+-rwxr-xr-x   0        0        0     1104 2023-03-31 01:58:54.416502 compactdata-0.0.4/compactdata/token_definitions.py
+-rw-r--r--   0        0        0     1158 2023-04-11 08:37:50.600151 compactdata-0.0.4/compactdata/unescapes.py
+-rw-r--r--   0        0        0      739 2023-04-12 12:35:59.847086 compactdata-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 compactdata-0.0.4/setup.py
+-rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 compactdata-0.0.4/PKG-INFO
```

### Comparing `compactdata-0.0.3/LICENSE` & `compactdata-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `compactdata-0.0.3/compactdata/__init__.py` & `compactdata-0.0.4/compactdata/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
-from compactdata.decoder import CompactDataDecodeError, create_parser, get_lexer_and_parser
-from compactdata.encoder import CompactDataEncodeError, CompactDataEncoder
+from compactdata.decoder import create_parser, get_lexer_and_parser
+from compactdata.encoder import CompactDataEncoder
+from compactdata.exceptions import CompactDataDecodeError, CompactDataEncodeError
 
 logger = logging.getLogger(__name__)
 
 _default_encoder = CompactDataEncoder(
     skipkeys=False,
     ensure_ascii=True,
     check_circular=True,
```

### Comparing `compactdata-0.0.3/compactdata/decoder.py` & `compactdata-0.0.4/compactdata/decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import logging
 
-from compactdata.grammar_rules import *  # noqa
-from compactdata.token_definitions import *  # noqa
 from ply import lex as lex
 from ply import yacc as yacc
 
-logger = logging.getLogger(__name__)
-
+from compactdata.grammar_rules import *  # noqa
+from compactdata.token_definitions import *  # noqa
 
-class CompactDataDecodeError(Exception):
-    pass
+logger = logging.getLogger(__name__)
 
 
 def create_parser(debug: bool = False):
     lexer = lex.lex(debug=debug, debuglog=logger)
     parser = yacc.yacc(debug=debug, debuglog=logger)
     return lexer, parser
```

### Comparing `compactdata-0.0.3/compactdata/encoder.py` & `compactdata-0.0.4/compactdata/encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -270,35 +270,37 @@
                 # see comment above for int
                 yield buf + _floatstr(value)
             else:
                 yield buf
                 if isinstance(value, (list, tuple)):
                     chunks = _iterencode_list(value, _current_indent_level)
                 elif isinstance(value, dict):
-                    chunks = _iterencode_dict(value, _current_indent_level)
+                    chunks = _iterencode_dict(value, _current_indent_level, can_be_orphan_pair=True)
                 else:
                     chunks = _iterencode(value, _current_indent_level)
                 yield from chunks
         if newline_indent is not None:
             _current_indent_level -= 1
             yield "\n" + _indent * _current_indent_level
         yield "]"
         if markers is not None:
             del markers[marker_id]
 
-    def _iterencode_dict(dct, _current_indent_level):
+    def _iterencode_dict(dct, _current_indent_level, can_be_orphan_pair=False, top_level=False):
         if not dct:
             yield "()"
             return
         if markers is not None:
             marker_id = id(dct)
             if marker_id in markers:
                 raise ValueError("Circular reference detected")
             markers[marker_id] = dct
-        yield "("
+        orphan_pair = can_be_orphan_pair and len(dct) == 1
+        if not orphan_pair and not top_level:
+            yield "("
         if _indent is not None:
             _current_indent_level += 1
             newline_indent = "\n" + _indent * _current_indent_level
             item_separator = _item_separator + newline_indent
             yield newline_indent
         else:
             newline_indent = None
@@ -355,15 +357,16 @@
                     chunks = _iterencode_dict(value, _current_indent_level)
                 else:
                     chunks = _iterencode(value, _current_indent_level)
                 yield from chunks
         if newline_indent is not None:
             _current_indent_level -= 1
             yield "\n" + _indent * _current_indent_level
-        yield ")"
+        if not orphan_pair and not top_level:
+            yield ")"
         if markers is not None:
             del markers[marker_id]
 
     def _iterencode(o, _current_indent_level):
         if isinstance(o, str):
             yield _encoder(o, _escape_char, _quote_char, _shortest)
         elif o is None:
@@ -389,12 +392,14 @@
                     raise ValueError("Circular reference detected")
                 markers[marker_id] = o
             o = _default(o)
             yield from _iterencode(o, _current_indent_level)
             if markers is not None:
                 del markers[marker_id]
 
-    return _iterencode
-
+    def _top_level_iterencode(o, _current_indent_level):
+        if isinstance(o, dict):
+            yield from _iterencode_dict(o, _current_indent_level, top_level=True)
+        else:
+            yield from _iterencode(o, _current_indent_level)
 
-class CompactDataEncodeError(Exception):
-    pass
+    return _top_level_iterencode
```

### Comparing `compactdata-0.0.3/compactdata/grammar_rules.py` & `compactdata-0.0.4/compactdata/grammar_rules.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from compactdata.unescapes import decode_string
+
 def p_compactdata(p):
     """compactdata : top_level_map
     | value"""
     p[0] = p[1]
 
 
 def p_top_level_map(p):
@@ -55,18 +57,18 @@
 
 def p_orphan_pair(p):
     """orphan_pair : pair"""
     p[0] = dict([p[1]])
 
 
 def p_value(p):
-    """value : QUOTED_STRING
-    | GRAVE_STRING
+    """value : quoted_string
+    | grave_string
+    | unquoted_string
     | reserved
-    | unquoted_value
     | map
     | array"""
     p[0] = p[1]
 
 
 def p_reserved(p):
     """reserved : NULL
@@ -76,28 +78,31 @@
         p[0] = None
     elif p[1] == "true":
         p[0] = True
     elif p[1] == "false":
         p[0] = False
 
 
-# use type inference for unquoted values
-def p_unquoted_value(p):
-    """unquoted_value : UNQUOTED_VALUE"""
-    try:
-        p[0] = int(p[1])
-    except ValueError:
-        try:
-            p[0] = float(p[1])
-        except ValueError:
-            p[0] = p[1]
+def p_unquoted_string(p):
+    """unquoted_string : UNQUOTED_STRING"""
+    p[0] = decode_string(p[1], quote_char="")
+
+
+def p_quoted_string(p):
+    """quoted_string : QUOTED_STRING"""
+    p[0] = decode_string(p[1], quote_char='"')
+
+
+def p_grave_string(p):
+    """grave_string : GRAVE_STRING"""
+    p[0] = decode_string(p[1], quote_char="`")
 
 
 def p_key(p):
-    """key : UNQUOTED_VALUE
+    """key : UNQUOTED_STRING
     | QUOTED_STRING
     | GRAVE_STRING"""
     p[0] = p[1]
 
 
 # Error handling rule
 def p_error(p):
```

### Comparing `compactdata-0.0.3/compactdata/token_definitions.py` & `compactdata-0.0.4/compactdata/token_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "false": "FALSE",
 }
 
 # Define the tokens
 tokens = [
     "QUOTED_STRING",
     "GRAVE_STRING",
-    "UNQUOTED_VALUE",
+    "UNQUOTED_STRING",
     "LPAREN",
     "RPAREN",
     "LBRACKET",
     "RBRACKET",
     "EQUALS",
     "SEMICOLON",
 ] + list(reserved.values())
@@ -37,17 +37,17 @@
 
 def t_QUOTED_STRING(t):
     r'"(?:[\\~][\\~"/bfnrt]|[\\~]u[0-9a-fA-F]{4}|[^\\"~])*"'
     t.value = t.value[1:-1]  # Remove quotes from value
     return t
 
 
-def t_UNQUOTED_VALUE(t):
+def t_UNQUOTED_STRING(t):
     r'(?:[\\~][\\~`"/bfnrt\[\]\(\);=]|\\u[0-9a-fA-F]{4}|[^\\`"~\[\]\(\);=])+'
-    t.type = reserved.get(t.value, "UNQUOTED_VALUE")
+    t.type = reserved.get(t.value, "UNQUOTED_STRING")
     return t
 
 
 # Error handling rule
 def t_error(t):
     raise Exception(f"Invalid character: {t.value[0]}")
     # t.lexer.skip(1)
```

### Comparing `compactdata-0.0.3/pyproject.toml` & `compactdata-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 [tool.poetry]
 name = "compactdata"
-version = "0.0.3"
-description = "Python package for CompactData encoding and decoding"
+version = "0.0.4"
+description = "A parser for the CompactData serialisation format."
 authors = ["NUM Technology <developer@num.uk>"]
 readme = "README.md"
 packages = [{include = "compactdata"}]
 license = "MIT"
 homepage = "https://compactdata.org"
 repository = "https://github.com/NUMtechnology/compactdata-python"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NUMtechnology/compactdata-python/issues"
 
 [tool.poetry.dependencies]
-python = "^3.0"
+python = "^3.6"
 ply = "^3.11"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

