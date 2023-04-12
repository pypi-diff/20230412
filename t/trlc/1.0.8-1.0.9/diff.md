# Comparing `tmp/trlc-1.0.8.tar.gz` & `tmp/trlc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trlc-1.0.8.tar", last modified: Tue Feb  7 11:56:21 2023, max compression
+gzip compressed data, was "dist/trlc-1.0.9.tar", last modified: Wed Mar  1 11:00:03 2023, max compression
```

## Comparing `trlc-1.0.8.tar` & `trlc-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-07 11:56:21.000000 trlc-1.0.8/
--rw-r--r--   0 florian   (1000) florian   (1000)     3128 2023-02-07 11:56:21.000000 trlc-1.0.8/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1790 2022-12-07 10:31:49.000000 trlc-1.0.8/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-02-07 11:56:21.000000 trlc-1.0.8/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     1399 2022-12-05 12:42:52.000000 trlc-1.0.8/setup.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-07 11:56:21.000000 trlc-1.0.8/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.0.8/trlc/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    77508 2023-01-18 12:30:34.000000 trlc-1.0.8/trlc/ast.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6958 2022-12-14 13:45:21.000000 trlc-1.0.8/trlc/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)    13829 2023-02-07 11:53:43.000000 trlc-1.0.8/trlc/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1000 2022-12-05 12:42:52.000000 trlc-1.0.8/trlc/lint.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1003 2022-12-05 12:42:52.000000 trlc-1.0.8/trlc/math.py
--rw-r--r--   0 florian   (1000) florian   (1000)    39434 2023-02-04 13:18:54.000000 trlc-1.0.8/trlc/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)    12920 2023-02-07 11:53:43.000000 trlc-1.0.8/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-02-07 11:54:08.000000 trlc-1.0.8/trlc/version.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-07 11:56:21.000000 trlc-1.0.8/trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     3128 2023-02-07 11:56:21.000000 trlc-1.0.8/trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      299 2023-02-07 11:56:21.000000 trlc-1.0.8/trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-02-07 11:56:21.000000 trlc-1.0.8/trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       41 2023-02-07 11:56:21.000000 trlc-1.0.8/trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-02-07 11:56:21.000000 trlc-1.0.8/trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-01 11:00:03.000000 trlc-1.0.9/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3406 2023-03-01 11:00:03.000000 trlc-1.0.9/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1875 2023-03-01 10:58:12.000000 trlc-1.0.9/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)      103 2023-03-01 11:00:03.000000 trlc-1.0.9/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2135 2023-02-21 07:05:56.000000 trlc-1.0.9/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-01 11:00:03.000000 trlc-1.0.9/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)      815 2022-12-05 12:42:52.000000 trlc-1.0.9/trlc/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    78894 2023-03-01 10:58:12.000000 trlc-1.0.9/trlc/ast.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6958 2022-12-14 13:45:21.000000 trlc-1.0.9/trlc/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    14323 2023-03-01 10:58:12.000000 trlc-1.0.9/trlc/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1000 2022-12-05 12:42:52.000000 trlc-1.0.9/trlc/lint.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1003 2022-12-05 12:42:52.000000 trlc-1.0.9/trlc/math.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    40651 2023-03-01 10:58:12.000000 trlc-1.0.9/trlc/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    12920 2023-02-07 11:53:43.000000 trlc-1.0.9/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1004 2023-03-01 10:58:55.000000 trlc-1.0.9/trlc/version.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-03-01 11:00:03.000000 trlc-1.0.9/trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3406 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      299 2023-03-01 11:00:03.000000 trlc-1.0.9/trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       41 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        5 2023-03-01 11:00:02.000000 trlc-1.0.9/trlc.egg-info/top_level.txt
```

### Comparing `trlc-1.0.8/PKG-INFO` & `trlc-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
 Project-URL: Source Code, https://github.com/bmw-software-engineering/trlc
 Description: # Treat Requirements Like Code (TRLC)
         TRLC is a domain-specific language developed at BMW for writing (and
         linking) requirements with meta-data.
         
         The repository contains:
         
-        * The language reference manual for TRLC.
+        * The [language reference
+          manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
+          for TRLC.
         
         * A pure Python reference implementation of TRLC.
         
         The implementation is not very fast, but designed to be pedantically
         correct in following the language definition.  Eventually it will also
         contain a powerful linter to find issues with types and check
         rules.
@@ -34,21 +36,21 @@
         * The API can be used to write other tools based on TRLC (for example
           a tool to render the requirements in HTML, a tool to diff
           requirements or perform an impact analysis, or a tool to perform
           software traceability, etc.)
         
         ## Documentation
         
-        * [Tutorial](TUTORIAL.md) (read this as a first introduction)
-        * [Release Notes](CHANGELOG.md) (read this to find out whats new)
+        * [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
+        * [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
         * [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
           (user guide for using the API)
-        * [Language Reference Manual](language-reference-manual/README.md)
+        * [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
           (for language lawyers)
-        * [License](LICENSE)
+        * [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
         
         ## Dependencies
         
         ### Run-time
         * Python3 >= 3.7
         
         ### Development tools
```

### Comparing `trlc-1.0.8/README.md` & `trlc-1.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Treat Requirements Like Code (TRLC)
 TRLC is a domain-specific language developed at BMW for writing (and
 linking) requirements with meta-data.
 
 The repository contains:
 
-* The language reference manual for TRLC.
+* The [language reference
+  manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
+  for TRLC.
 
 * A pure Python reference implementation of TRLC.
 
 The implementation is not very fast, but designed to be pedantically
 correct in following the language definition.  Eventually it will also
 contain a powerful linter to find issues with types and check
 rules.
@@ -27,15 +29,15 @@
 
 ## Documentation
 
 * [Tutorial](TUTORIAL.md) (read this as a first introduction)
 * [Release Notes](CHANGELOG.md) (read this to find out whats new)
 * [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
   (user guide for using the API)
-* [Language Reference Manual](language-reference-manual/README.md)
+* [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
   (for language lawyers)
 * [License](LICENSE)
 
 ## Dependencies
 
 ### Run-time
 * Python3 >= 3.7
```

### Comparing `trlc-1.0.8/setup.py` & `trlc-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 #!/usr/bin/env python3
 
+import re
 import sys
 import setuptools
 
 from trlc import version
 
+gh_root = "https://github.com"
+gh_project = "bmw-software-engineering/trlc"
+
 with open("README.md", "r") as fd:
     long_description = fd.read()
 
-gh_root = "https://github.com"
-gh_project = "bmw-software-engineering/trlc"
+# For the readme to look right on PyPI we need to translate any
+# relative links to absolute links to github.
+fixes = []
+for match in re.finditer(r"\[(.*)\]\((.*)\)", long_description):
+    if not match.group(2).startswith("http"):
+        fixes.append((match.span(0)[0], match.span(0)[1],
+                      "[%s](%s/%s/blob/main/%s)" % (match.group(1),
+                                                    gh_root,
+                                                    gh_project,
+                                                    match.group(2))))
+
+for begin, end, text in reversed(fixes):
+    long_description = (long_description[:begin] +
+                        text +
+                        long_description[end:])
 
 project_urls = {
     "Bug Tracker"   : "%s/%s/issues" % (gh_root, gh_project),
     "Documentation" : "%s/pages/%s/" % (gh_root, gh_project),
     "Source Code"   : "%s/%s"        % (gh_root, gh_project),
 }
```

### Comparing `trlc-1.0.8/trlc/__init__.py` & `trlc-1.0.9/trlc/__init__.py`

 * *Files identical despite different names*

### Comparing `trlc-1.0.8/trlc/ast.py` & `trlc-1.0.9/trlc/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         assert typ is None or isinstance(typ, Type)
         assert (typ is None) == (value is None)
 
         self.location = location
         self.value    = value
         self.typ      = typ
 
+    def __eq__(self, other):
+        return self.value == other.value
+
     def __repr__(self):  # pragma: no cover
         return "Value(%s)" % self.value
 
     def resolve_references(self, mh):
         assert isinstance(mh, Message_Handler)
 
         if isinstance(self.value, Record_Reference):
@@ -263,14 +266,16 @@
     COMP_GEQ = auto()
 
     STRING_CONTAINS   = auto()
     STRING_STARTSWITH = auto()
     STRING_ENDSWITH   = auto()
     STRING_REGEX      = auto()
 
+    ARRAY_CONTAINS = auto()
+
     PLUS      = auto()
     MINUS     = auto()
     TIMES     = auto()
     DIVIDE    = auto()
     REMAINDER = auto()
 
     POWER = auto()
@@ -836,14 +841,15 @@
     * Binary_Operator.COMP_LEQ (e.g. ``1 <= 2``)
     * Binary_Operator.COMP_GT (e.g. ``a > b``)
     * Binary_Operator.COMP_GEQ (e.g. ``a >= b``)
     * Binary_Operator.STRING_CONTAINS (e.g. ``"foo" in "foobar"``)
     * Binary_Operator.STRING_STARTSWITH (e.g. ``startswith("foo", "f")``)
     * Binary_Operator.STRING_ENDSWITH (e.g. ``endswith("foo", "o")``)
     * Binary_Operator.STRING_REGEX (e.g. ``matches("foo", ".o.``)
+    * Binary_Operator.ARRAY_CONTAINS (e.g. ``42 in arr``)
     * Binary_Operator.PLUS (e.g. ``42 + b`` or ``"foo" + bar``)
     * Binary_Operator.MINUS (e.g. ``a - 1``)
     * Binary_Operator.TIMES (e.g. ``2 * x``)
     * Binary_Operator.DIVIDE (e.g. ``x / 2``)
     * Binary_Operator.REMAINDER (e.g. ``x % 2``)
     * Binary_Operator.POWER (e.g. ``x ** 2``)
     * Binary_Operator.INDEX (e.g. ``foo[2]``)
@@ -903,14 +909,18 @@
         elif operator in (Binary_Operator.STRING_CONTAINS,
                           Binary_Operator.STRING_STARTSWITH,
                           Binary_Operator.STRING_ENDSWITH,
                           Binary_Operator.STRING_REGEX):
             self.n_lhs.ensure_type(mh, Builtin_String)
             self.n_rhs.ensure_type(mh, Builtin_String)
 
+        elif operator == Binary_Operator.ARRAY_CONTAINS:
+            self.n_rhs.ensure_type(mh, Array_Type)
+            self.n_lhs.ensure_type(mh, self.n_rhs.typ.element_type.__class__)
+
         elif operator == Binary_Operator.PLUS:
             if isinstance(self.n_lhs.typ, Builtin_Integer):
                 self.n_rhs.ensure_type(mh, Builtin_Integer)
             else:
                 self.n_lhs.ensure_type(mh, Builtin_String)
                 self.n_rhs.ensure_type(mh, Builtin_String)
 
@@ -945,14 +955,15 @@
             Binary_Operator.COMP_EQ         : "==",
             Binary_Operator.COMP_NEQ        : "!=",
             Binary_Operator.COMP_LT         : "<",
             Binary_Operator.COMP_LEQ        : "<=",
             Binary_Operator.COMP_GT         : ">",
             Binary_Operator.COMP_GEQ        : ">=",
             Binary_Operator.STRING_CONTAINS : "in",
+            Binary_Operator.ARRAY_CONTAINS  : "in",
             Binary_Operator.PLUS            : "+",
             Binary_Operator.MINUS           : "-",
             Binary_Operator.TIMES           : "*",
             Binary_Operator.DIVIDE          : "/",
             Binary_Operator.REMAINDER       : "%",
             Binary_Operator.POWER           : "**",
         }
@@ -1082,14 +1093,21 @@
             assert isinstance(v_lhs.value, str)
             assert isinstance(v_rhs.value, str)
             return Value(location = self.location,
                          value    = re.match(v_rhs.value,
                                              v_lhs.value) is not None,
                          typ      = self.typ)
 
+        elif self.operator == Binary_Operator.ARRAY_CONTAINS:
+            assert isinstance(v_rhs.value, list)
+
+            return Value(location = self.location,
+                         value    = v_lhs in v_rhs.value,
+                         typ      = self.typ)
+
         elif self.operator == Binary_Operator.PLUS:
             assert isinstance(v_lhs.value, (int, str))
             assert isinstance(v_rhs.value, (int, str))
             return Value(location = self.location,
                          value    = v_lhs.value + v_rhs.value,
                          typ      = self.typ)
 
@@ -1384,15 +1402,15 @@
 
 class Quantified_Expression(Expression):
     """A quantified expression
 
     For example::
 
       (forall x in array_component => x > 0)
-              ^1   ^2                 ^^^^^3
+       ^4     ^1   ^2                 ^^^^^3
 
     A quantified expression introduces and binds a
     :class:`Quantified_Variable` (see 1) from a specified source (see
     2). When the body (see 3) is evaluated, the name of 1 is bound to
     each component of the source in turn.
 
     :attribute n_var: The quantified variable (see 1)
@@ -1400,35 +1418,51 @@
 
     :attribute n_source: The array to iterate over (see 2)
     :type: Name_Reference
 
     :attribute n_expr: The body of the quantifier (see 3)
     :type: Expression
 
+    :attribute universal: True means forall, false means exists (see 4)
+    :type: Boolean
+
     """
-    def __init__(self, mh, location, typ, n_variable, n_source, n_expr):
+    def __init__(self, mh, location,
+                 typ,
+                 universal,
+                 n_variable,
+                 n_source,
+                 n_expr):
         super().__init__(location, typ)
+        assert isinstance(typ, Builtin_Boolean)
+        assert isinstance(universal, bool)
         assert isinstance(n_variable, Quantified_Variable)
         assert isinstance(n_expr, Expression)
         assert isinstance(n_source, Name_Reference)
-        assert isinstance(typ, Builtin_Boolean)
-        self.n_var    = n_variable
-        self.n_expr   = n_expr
-        self.n_source = n_source
+        self.universal = universal
+        self.n_var     = n_variable
+        self.n_expr    = n_expr
+        self.n_source  = n_source
         self.n_expr.ensure_type(mh, Builtin_Boolean)
 
     def dump(self, indent=0):  # pragma: no cover
-        self.write_indent(indent, "Quantified expression")
+        if self.universal:
+            self.write_indent(indent, "Universal quantified expression")
+        else:
+            self.write_indent(indent, "Existential quantified expression")
         self.n_var.dump(indent + 1)
         self.n_expr.dump(indent + 1)
 
     def to_string(self):
-        return "(forall %s in %s => %s)" % (self.n_var.name,
-                                            self.n_source.to_string(),
-                                            self.n_expr.to_string())
+        return "(%s %s in %s => %s)" % ("forall"
+                                        if self.universal
+                                        else "exists",
+                                        self.n_var.name,
+                                        self.n_source.to_string(),
+                                        self.n_expr.to_string())
 
     def evaluate(self, mh, context):
         assert isinstance(mh, Message_Handler)
         assert context is None or isinstance(context, dict)
 
         if context is None:
             new_ctx = {}
@@ -1446,27 +1480,31 @@
                      "must not be null" %
                      (self.n_source.to_string(),
                       self.to_string(),
                       self.location.to_string(False)))
         else:
             assert isinstance(array_values, Array_Aggregate)
 
-        ok = True
+        rv  = self.universal
         loc = self.location
         for binding in array_values.value:
             new_ctx[self.n_var.name] = binding
             result = self.n_expr.evaluate(mh, new_ctx)
             assert isinstance(result.value, bool)
-            if not result.value:
-                ok  = False
+            if self.universal and not result.value:
+                rv  = False
+                loc = binding.location
+                break
+            elif not self.universal and result.value:
+                rv  = True
                 loc = binding.location
                 break
 
         return Value(location = loc,
-                     value    = ok,
+                     value    = rv,
                      typ      = self.typ)
 
 
 ##############################################################################
 # AST Nodes (Entities)
 ##############################################################################
```

### Comparing `trlc-1.0.8/trlc/errors.py` & `trlc-1.0.9/trlc/errors.py`

 * *Files identical despite different names*

### Comparing `trlc-1.0.8/trlc/lexer.py` & `trlc-1.0.9/trlc/lexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,15 +99,16 @@
         tlen = self.end_pos + 1 - self.start_pos
 
         return [line,
                 " " * offset + "^" * min(tlen, maxtrail)]
 
 
 class Token:
-    KIND = frozenset(["IDENTIFIER",
+    KIND = frozenset(["COMMENT",
+                      "IDENTIFIER",
                       "BUILTIN",
                       "KEYWORD",
                       "BRA", "KET",
                       "S_BRA", "S_KET",
                       "C_BRA", "C_KET",
                       "COMMA",
                       "DOT",
@@ -117,15 +118,16 @@
                       "ARROW",
                       "INTEGER",
                       "STRING"])
 
     def __init__(self, location, kind, value=None):
         assert isinstance(location, Location)
         assert kind in Token.KIND
-        if kind in ("IDENTIFIER", "BUILTIN", "KEYWORD", "OPERATOR", "STRING"):
+        if kind in ("COMMENT", "IDENTIFIER", "BUILTIN",
+                    "KEYWORD", "OPERATOR", "STRING"):
             assert isinstance(value, str)
         elif kind == "INTEGER":
             assert isinstance(value, int)
         else:
             assert value is None
 
         self.location = location
@@ -139,18 +141,19 @@
             return "%s_Token(%s)" % (self.kind, self.value)
 
 
 class Lexer:
     KEYWORDS = frozenset(["abs",
                           "and",
                           "checks",
-                          "enum",
                           "else",
                           "elsif",
+                          "enum",
                           "error",
+                          "exists",
                           "extends",
                           "false",
                           "fatal",
                           "forall",
                           "if",
                           "implies",
                           "import",
@@ -188,18 +191,22 @@
         self.file_name = file_name
 
     def token(self):
         assert False
 
 
 class Python_Lexer(Lexer):
-    def __init__(self, mh, file_name):
+    def __init__(self, mh, file_name, file_content=None):
         super().__init__(mh, file_name)
-        with open(file_name, "r", encoding="UTF-8") as fd:
-            self.file_content = fd.read()
+        if file_content:
+            self.file_content = file_content
+        else:
+            with open(file_name, "r", encoding="UTF-8") as fd:
+                self.file_content = fd.read()
+
         self.file_length  = len(self.file_content)
 
         self.lexpos = -2
         self.line_no = 0
         self.col_no  = 0
         self.cc = None
         self.nc = None
@@ -240,37 +247,37 @@
         return Source_Reference(lexer      = self,
                                 start_line = self.line_no,
                                 start_col  = self.col_no,
                                 start_pos  = self.lexpos,
                                 end_pos    = self.lexpos)
 
     def token(self):
-        # Skip whitespace and comments
-        while True:
-            while self.nc and self.nc.isspace():
-                self.advance()
-            if self.nc is None:
-                return None
+        # Skip whitespace and move to the next char
+        while self.nc and self.nc.isspace():
             self.advance()
-
-            if self.cc == "/" and self.nc == "/":
-                while self.cc and self.cc != "\n":
-                    self.advance()
-            elif self.cc == "/" and self.nc == "*":
-                while self.nc and not (self.cc == "*" and self.nc == "/"):
-                    self.advance()
-                self.advance()
-            else:
-                break
+        if self.nc is None:
+            return None
+        self.advance()
 
         start_pos  = self.lexpos
         start_line = self.line_no
         start_col  = self.col_no
 
-        if self.is_alpha(self.cc):
+        if self.cc == "/" and self.nc == "/":
+            kind = "COMMENT"
+            while self.cc and self.nc != "\n":
+                self.advance()
+
+        elif self.cc == "/" and self.nc == "*":
+            kind = "COMMENT"
+            while self.nc and not (self.cc == "*" and self.nc == "/"):
+                self.advance()
+            self.advance()
+
+        elif self.is_alpha(self.cc):
             kind = "IDENTIFIER"
             while self.nc and (self.is_alnum(self.nc) or
                                self.nc == "_" or
                                self.nc == ":"):
                 self.advance()
 
         elif self.cc in Lexer.PUNCTUATION:
@@ -400,14 +407,24 @@
                 value = value.replace('\\"', '"')
             else:
                 value = triple_quoted_string_value(value)
 
         elif kind == "INTEGER":
             value = int(sref.text())
 
+        elif kind == "COMMENT":
+            value = sref.text()
+            if value.startswith("//"):
+                value = value[2:].strip()
+            else:
+                value = value[2:]
+                if value.endswith("*/"):
+                    value = value[:-2]
+                value = value.strip()
+
         else:
             value = None
 
         return Token(sref, kind, value)
 
 
 def create_lexer(mh, file_name):
```

### Comparing `trlc-1.0.8/trlc/lint.py` & `trlc-1.0.9/trlc/lint.py`

 * *Files identical despite different names*

### Comparing `trlc-1.0.8/trlc/math.py` & `trlc-1.0.9/trlc/math.py`

 * *Files identical despite different names*

### Comparing `trlc-1.0.8/trlc/parser.py` & `trlc-1.0.9/trlc/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,42 +26,49 @@
 
 
 class Parser:
     COMPARISON_OPERATOR = ("==", "!=", "<", "<=", ">", ">=")
     ADDING_OPERATOR = ("+", "-")
     MULTIPLYING_OPERATOR = ("*", "/", "%")
 
-    def __init__(self, mh, stab, file_name, lint_mode):
+    def __init__(self, mh, stab, file_name, lint_mode, lexer=None):
         assert isinstance(mh, Message_Handler)
         assert isinstance(stab, ast.Symbol_Table)
         assert isinstance(file_name, str)
         assert isinstance(lint_mode, bool)
         self.mh        = mh
         self.lint_mode = lint_mode
-        self.lexer     = create_lexer(mh, file_name)
+        if lexer:
+            self.lexer = lexer
+        else:
+            self.lexer = create_lexer(mh, file_name)
         self.stab      = stab
         self.pkg       = None
         self.raw_deps  = []
         self.deps      = []
         self.imports   = set()
 
         self.ct = None
-        self.nt = self.lexer.token()
+        self.nt = None
+        self.advance()
 
         self.builtin_bool = stab.table["Boolean"]
         self.builtin_int  = stab.table["Integer"]
         self.builtin_str  = stab.table["String"]
 
         self.section = []
         self.default_scope = ast.Scope()
         self.default_scope.push(self.stab)
 
     def advance(self):
         self.ct = self.nt
-        self.nt = self.lexer.token()
+        while True:
+            self.nt = self.lexer.token()
+            if self.nt is None or self.nt.kind != "COMMENT":
+                break
 
     def peek(self, kind):
         assert kind in Token.KIND
         return self.nt is not None and self.nt.kind == kind
 
     def peek_eof(self):
         return self.nt is None
@@ -346,23 +353,38 @@
                     mh       = self.mh,
                     location = t_in.location,
                     typ      = self.builtin_bool,
                     n_lhs    = n_lhs,
                     n_lower  = n_a,
                     n_upper  = n_b)
 
-            else:
+            elif isinstance(n_a.typ, ast.Builtin_String):
                 rv = ast.Binary_Expression(
                     mh       = self.mh,
                     location = t_in.location,
                     typ      = self.builtin_bool,
                     operator = ast.Binary_Operator.STRING_CONTAINS,
                     n_lhs    = n_lhs,
                     n_rhs    = n_a)
 
+            elif isinstance(n_a.typ, ast.Array_Type):
+                rv = ast.Binary_Expression(
+                    mh       = self.mh,
+                    location = t_in.location,
+                    typ      = self.builtin_bool,
+                    operator = ast.Binary_Operator.ARRAY_CONTAINS,
+                    n_lhs    = n_lhs,
+                    n_rhs    = n_a)
+
+            else:
+                self.mh.error(
+                    n_a.location,
+                    "membership test only defined for Strings and Arrays,"
+                    " not for %s" % n_a.typ.name)
+
             if t_not is not None:
                 rv = ast.Unary_Expression(
                     mh        = self.mh,
                     location  = t_not.location,
                     typ       = self.builtin_bool,
                     operator  = ast.Unary_Operator.LOGICAL_NOT,
                     n_operand = rv)
@@ -491,36 +513,45 @@
             self.match("INTEGER")
             return ast.Integer_Literal(self.ct, self.builtin_int)
 
         elif self.peek("STRING"):
             self.match("STRING")
             return ast.String_Literal(self.ct, self.builtin_str)
 
+        elif self.peek_kw("true") or self.peek_kw("false"):
+            self.match("KEYWORD")
+            return ast.Boolean_Literal(self.ct, self.builtin_bool)
+
         elif self.peek_kw("null"):
             self.match_kw("null")
             return ast.Null_Literal(self.ct)
 
         elif self.peek("BRA"):
             self.match("BRA")
-            if self.peek_kw("forall"):
+            if self.peek_kw("forall") or self.peek_kw("exists"):
                 rv = self.parse_quantified_expression(scope)
             elif self.peek_kw("if"):
                 rv = self.parse_conditional_expression(scope)
             else:
                 rv = self.parse_expression(scope)
             self.match("KET")
             return rv
 
         else:
             return self.parse_name(scope)
 
     def parse_quantified_expression(self, scope):
         assert isinstance(scope, ast.Scope)
 
-        self.match_kw("forall")
+        if self.peek_kw("forall"):
+            self.match_kw("forall")
+            universal = True
+        else:
+            self.match_kw("exists")
+            universal = False
         loc = self.ct.location
         self.match("IDENTIFIER")
         t_qv = self.ct
         if scope.contains(t_qv.value):
             pdef = scope.lookup(self.mh, t_qv)
             self.mh.error(t_qv.location,
                           "shadows %s %s from %s" %
@@ -545,14 +576,15 @@
         scope.push(new_table)
         n_expr = self.parse_expression(scope)
         scope.pop()
 
         return ast.Quantified_Expression(mh         = self.mh,
                                          location   = loc,
                                          typ        = self.builtin_bool,
+                                         universal  = universal,
                                          n_variable = n_var,
                                          n_source   = n_source,
                                          n_expr     = n_expr)
 
     def parse_conditional_expression(self, scope):
         assert isinstance(scope, ast.Scope)
```

### Comparing `trlc-1.0.8/trlc/trlc.py` & `trlc-1.0.9/trlc/trlc.py`

 * *Files identical despite different names*

### Comparing `trlc-1.0.8/trlc/version.py` & `trlc-1.0.9/trlc/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public
 # License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with TRLC. If not, see <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (1, 0, 8)
+VERSION_TUPLE = (1, 0, 9)
 VERSION_SUFFIX = ""
 
 TRLC_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "TRLC %s" % TRLC_VERSION
```

### Comparing `trlc-1.0.8/trlc.egg-info/PKG-INFO` & `trlc-1.0.9/trlc.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: trlc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Treat Requirements Like Code
 Home-page: https://github.com/bmw-software-engineering/trlc
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/trlc/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/trlc/
 Project-URL: Source Code, https://github.com/bmw-software-engineering/trlc
 Description: # Treat Requirements Like Code (TRLC)
         TRLC is a domain-specific language developed at BMW for writing (and
         linking) requirements with meta-data.
         
         The repository contains:
         
-        * The language reference manual for TRLC.
+        * The [language reference
+          manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
+          for TRLC.
         
         * A pure Python reference implementation of TRLC.
         
         The implementation is not very fast, but designed to be pedantically
         correct in following the language definition.  Eventually it will also
         contain a powerful linter to find issues with types and check
         rules.
@@ -34,21 +36,21 @@
         * The API can be used to write other tools based on TRLC (for example
           a tool to render the requirements in HTML, a tool to diff
           requirements or perform an impact analysis, or a tool to perform
           software traceability, etc.)
         
         ## Documentation
         
-        * [Tutorial](TUTORIAL.md) (read this as a first introduction)
-        * [Release Notes](CHANGELOG.md) (read this to find out whats new)
+        * [Tutorial](https://github.com/bmw-software-engineering/trlc/blob/main/TUTORIAL.md) (read this as a first introduction)
+        * [Release Notes](https://github.com/bmw-software-engineering/trlc/blob/main/CHANGELOG.md) (read this to find out whats new)
         * [Python API Documentation](https://bmw-software-engineering.github.io/trlc/)
           (user guide for using the API)
-        * [Language Reference Manual](language-reference-manual/README.md)
+        * [Language Reference Manual](https://bmw-software-engineering.github.io/trlc/lrm.html)
           (for language lawyers)
-        * [License](LICENSE)
+        * [License](https://github.com/bmw-software-engineering/trlc/blob/main/LICENSE)
         
         ## Dependencies
         
         ### Run-time
         * Python3 >= 3.7
         
         ### Development tools
```

