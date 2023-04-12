# Comparing `tmp/geneve-0.1.1.tar.gz` & `tmp/geneve-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneve-0.1.1.tar", last modified: Wed Nov 16 13:02:23 2022, max compression
+gzip compressed data, was "geneve-0.2.0.tar", last modified: Wed Apr 12 16:34:49 2023, max compression
```

## Comparing `geneve-0.1.1.tar` & `geneve-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 13:02:23.362498 geneve-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    10143 2022-11-16 13:02:06.000000 geneve-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-11-16 13:02:23.362498 geneve-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 13:02:23.358498 geneve-0.1.1/geneve/
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    22063 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     6447 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/events_emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8668 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/events_emitter_eql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 13:02:23.362498 geneve-0.1.1/geneve/kql/
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5930 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/ast.py
--rw-r--r--   0 runner    (1001) docker     (121)     4251 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/dsl.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4818 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/eql2kql.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5093 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/kql.g
--rwxr-xr-x   0 runner    (1001) docker     (121)     3660 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/kql2eql.py
--rw-r--r--   0 runner    (1001) docker     (121)     4621 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    13262 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/kql/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 13:02:23.362498 geneve-0.1.1/geneve/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     5239 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5631 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/utils/ast_dag.py
--rw-r--r--   0 runner    (1001) docker     (121)     5064 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/utils/kibana.py
--rw-r--r--   0 runner    (1001) docker     (121)     2807 2022-11-16 13:02:06.000000 geneve-0.1.1/geneve/utils/shelllib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 13:02:23.362498 geneve-0.1.1/geneve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-11-16 13:02:23.000000 geneve-0.1.1/geneve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-16 13:02:23.000000 geneve-0.1.1/geneve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 13:02:23.000000 geneve-0.1.1/geneve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-16 13:02:23.000000 geneve-0.1.1/geneve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-16 13:02:23.000000 geneve-0.1.1/geneve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-11-16 13:02:06.000000 geneve-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-11-16 13:02:23.362498 geneve-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:34:49.989033 geneve-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-12 16:34:35.000000 geneve-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-04-12 16:34:49.989033 geneve-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-12 16:34:35.000000 geneve-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:34:49.981032 geneve-0.2.0/geneve/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/events_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/events_emitter_eql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:34:49.985033 geneve-0.2.0/geneve/kql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/dsl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4818 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/eql2kql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/kql.g
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3660 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/kql2eql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/kql/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:34:49.985033 geneve-0.2.0/geneve/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/group_as.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/group_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/type_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/type_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/type_geo_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/type_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/type_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/solver/type_long.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:34:49.985033 geneve-0.2.0/geneve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/utils/ast_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/utils/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/utils/hdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/utils/kibana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-12 16:34:35.000000 geneve-0.2.0/geneve/utils/shelllib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:34:49.985033 geneve-0.2.0/geneve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-04-12 16:34:49.000000 geneve-0.2.0/geneve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 16:34:49.000000 geneve-0.2.0/geneve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:34:49.000000 geneve-0.2.0/geneve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 16:34:49.000000 geneve-0.2.0/geneve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:34:49.000000 geneve-0.2.0/geneve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-12 16:34:35.000000 geneve-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 16:34:49.989033 geneve-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:34:49.989033 geneve-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28910 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36283 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_emitter_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_emitter_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_group_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_shelllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-12 16:34:35.000000 geneve-0.2.0/tests/test_utils.py
```

### Comparing `geneve-0.1.1/LICENSE.txt` & `geneve-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/__init__.py` & `geneve-0.2.0/geneve/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from .events_emitter import *  # noqa: F401, F403
 
-version = "0.1.1"
+version = "0.2.0"
```

### Comparing `geneve-0.1.1/geneve/config.py` & `geneve-0.2.0/geneve/config.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/events_emitter.py` & `geneve-0.2.0/geneve/events_emitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Functions for generating event documents that would trigger a given rule."""
 
-import random
 from collections import namedtuple
 from datetime import datetime, timedelta, timezone
 from itertools import chain
 
 from .events_emitter_eql import collect_constraints as collect_constraints_eql
 from .events_emitter_eql import get_ast_stats  # noqa: F401
-from .utils import deep_merge
+from .solver import emit_field
+from .utils import deep_merge, random
 
 __all__ = ("SourceEvents",)
 
 default_custom_schema = {
     "file.Ext.windows.zone_identifier": {
         "type": "long",
     },
@@ -95,29 +95,19 @@
         value = {"type": field_type}
         for part in reversed(field.split(".")):
             value = {"properties": {part: value}}
         deep_merge(mappings, value)
     return mappings
 
 
-def emit_field(field, value):
-    for part in reversed(field.split(".")):
-        value = {part: value}
-    return value
-
-
 def events_from_branch(branch, schema, timestamp, meta):
     events = []
-    for solution in branch.solve(schema):
-        doc = {}
-        for field, value in solution:
-            if value is not None:
-                deep_merge(doc, emit_field(field, value))
+    for doc in branch.solve(schema):
         if timestamp:
-            deep_merge(doc, emit_field("@timestamp", timestamp[0].isoformat(timespec="milliseconds")))
+            emit_field(doc, "@timestamp", timestamp[0].isoformat(timespec="milliseconds"))
             timestamp[0] += timedelta(milliseconds=1)
         events.append(Event(meta, doc))
     return events
 
 
 def events_from_root(root, schema, timestamp):
     return [events_from_branch(branch, schema, timestamp, root.meta) for branch in root]
```

### Comparing `geneve-0.1.1/geneve/events_emitter_eql.py` & `geneve-0.2.0/geneve/events_emitter_eql.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """Functions for collecting constraints from an EQL AST."""
 
 from itertools import chain, product
 from typing import Any, List, NoReturn, Tuple, Union
 
 import eql
 
-from .constraints import Branch, Constraints, Root
+from .constraints import Branch, Document, Root
 from .utils import TreeTraverser
 
 __all__ = ()
 
 traverser = TreeTraverser()
 
 
@@ -50,16 +50,16 @@
         cc_and_terms: cc_or_terms,
     }
     return operation if not negate else negation.get(operation, not operation)
 
 
 @traverser(eql.ast.Field)
 def cc_field(node: eql.ast.Field, value: str, negate: bool) -> Root:
-    c = Constraints(node.render(), _nope("==", negate), value)
-    return Root([Branch([c])])
+    doc = Document(node.render(), _nope("==", negate), value)
+    return Root([Branch([doc])])
 
 
 @traverser(eql.ast.Boolean)
 def cc_boolean(node: eql.ast.Boolean, negate: bool) -> Root:
     branches = []
     if _nope(node.value, negate):
         branches.append(Branch.Identity)
@@ -106,30 +106,30 @@
 @traverser(eql.ast.InSet)
 def cc_in_set(node: eql.ast.InSet, negate: bool) -> Root:
     if type(node.expression) != eql.ast.Field:
         raise NotImplementedError(f"Unsupported expression type: {type(node.expression)}")
     branches = []
     if negate:
         field = node.expression.render()
-        c = Constraints()
+        doc = Document()
         for term in node.container:
-            c.append_constraint(field, "!=", term.value)
-        branches.append(Branch([c]))
+            doc.append_constraint(field, "!=", term.value)
+        branches.append(Branch([doc]))
     else:
         for term in node.container:
             branches.extend(cc_field(node.expression, term.value, negate))
     return Root(branches)
 
 
 @traverser(eql.ast.Comparison)
 def cc_comparison(node: eql.ast.Comparison, negate: bool) -> Root:
     if type(node.left) != eql.ast.Field:
         raise NotImplementedError(f"Unsupported LHS type: {type(node.left)}")
-    c = Constraints(node.left.render(), _nope(node.comparator, negate), node.right.value)
-    return Root([Branch([c])])
+    doc = Document(node.left.render(), _nope(node.comparator, negate), node.right.value)
+    return Root([Branch([doc])])
 
 
 @traverser(eql.ast.EventQuery)
 def cc_event_query(node: eql.ast.EventQuery, negate: bool) -> Root:
     if negate:
         raise NotImplementedError(f"Negation of {type(node)} is not supported")
     if type(node.event_type) != str:
@@ -146,47 +146,47 @@
     if negate:
         raise NotImplementedError(f"Negation of {type(node)} is not supported")
     if node.pipes:
         raise NotImplementedError("Pipes are unsupported")
     return collect_constraints(node.first, negate)
 
 
-def cc_subquery_by(node: eql.ast.SubqueryBy, negate: bool) -> List[Tuple[Constraints, List[str]]]:
+def cc_subquery_by(node: eql.ast.SubqueryBy, negate: bool) -> List[Tuple[Document, List[str]]]:
     if negate:
         raise NotImplementedError(f"Negation of {type(node)} is not supported")
     if any(type(value) != eql.ast.Field for value in node.join_values):
         raise NotImplementedError(f"Unsupported join values: {node.join_values}")
     if node.fork:
         raise NotImplementedError(f"Unsupported fork: {node.fork}")
     join_fields = [field.render() for field in node.join_values]
-    return [[(c, join_fields) for c in branch] for branch in collect_constraints(node.query, negate)]
+    return [[(doc, join_fields) for doc in branch] for branch in collect_constraints(node.query, negate)]
 
 
-def cc_join_branch(seq: List[Tuple[Constraints, List[str]]]) -> Branch:
-    constraints = []
+def cc_join_branch(seq: List[Tuple[Document, List[str]]]) -> Branch:
+    docs = []
     join_rows = []
-    for c, join_fields in seq:
-        c = c.clone()
-        constraints.append(c)
-        join_rows.append([(field, c) for field in join_fields])
+    for doc, join_fields in seq:
+        doc = doc.clone()
+        docs.append(doc)
+        join_rows.append([(field, doc) for field in join_fields])
     for join_col in zip(*join_rows):
         field0 = None
-        for field, c in join_col:
+        for field, doc in join_col:
             field0 = field0 or field
-            constraints[0].append_constraint(field0, "join_value", (field, c))
-    return Branch(constraints)
+            docs[0].append_constraint(field0, "join_value", (field, doc))
+    return Branch(docs)
 
 
 @traverser(eql.ast.Sequence)
 def cc_sequence(node: eql.ast.Sequence, negate: bool) -> Root:
     if negate:
         raise NotImplementedError(f"Negation of {type(node)} is not supported")
     queries = [cc_subquery_by(query, negate) for query in node.queries]
     if node.close:
-        queries.append([[(c, []) for c in branch] for branch in collect_constraints(node.close, negate)])
+        queries.append([[(doc, []) for doc in branch] for branch in collect_constraints(node.close, negate)])
     return Root([cc_join_branch(chain(*branches)) for branches in chain(product(*queries))])
 
 
 @traverser(eql.ast.FunctionCall)
 def cc_function_call(node: eql.ast.FunctionCall, negate: bool) -> Root:
     if type(node.arguments[0]) is not eql.ast.Field:
         raise NotImplementedError(f"Unsupported argument type: {type(node.arguments[0])}")
@@ -204,16 +204,16 @@
     else:
         raise NotImplementedError(f"Unsupported function: {node.name}")
 
 
 def cc_function(node: eql.ast.FunctionCall, negate: bool, constraint_name: str) -> Root:
     field = node.arguments[0].render()
     constraint_name = constraint_name if not negate else f"not {constraint_name}"
-    c = Constraints(field, constraint_name, tuple(arg.value for arg in node.arguments[1:]))
-    return Root([Branch([c])])
+    doc = Document(field, constraint_name, tuple(arg.value for arg in node.arguments[1:]))
+    return Root([Branch([doc])])
 
 
 @traverser(eql.ast.BaseNode)
 @traverser(eql.ast.Expression)
 @traverser(eql.ast.EqlNode)
 @traverser(eql.ast.Literal)
 @traverser(eql.ast.String)
```

### Comparing `geneve-0.1.1/geneve/kql/__init__.py` & `geneve-0.2.0/geneve/kql/__init__.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/ast.py` & `geneve-0.2.0/geneve/kql/ast.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/dsl.py` & `geneve-0.2.0/geneve/kql/dsl.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/eql2kql.py` & `geneve-0.2.0/geneve/kql/eql2kql.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/errors.py` & `geneve-0.2.0/geneve/kql/errors.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/evaluator.py` & `geneve-0.2.0/geneve/kql/evaluator.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/kql.g` & `geneve-0.2.0/geneve/kql/kql.g`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/kql2eql.py` & `geneve-0.2.0/geneve/kql/kql2eql.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/optimizer.py` & `geneve-0.2.0/geneve/kql/optimizer.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/kql/parser.py` & `geneve-0.2.0/geneve/kql/parser.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/utils/__init__.py` & `geneve-0.2.0/geneve/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,72 +14,71 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Util functions."""
 
 import functools
-import os
 import shutil
 from contextlib import contextmanager
 from glob import glob
 from pathlib import Path
+from random import Random
 from tempfile import mkdtemp
 from types import SimpleNamespace
 from urllib.parse import urlparse
 
-root_dir = os.path.abspath(os.path.join(os.path.split(__file__)[0], "..", ".."))
+random = Random()
 
 
 @contextmanager
 def tempdir():
     tmpdir = mkdtemp()
     try:
-        yield tmpdir
+        yield Path(tmpdir)
     finally:
         shutil.rmtree(tmpdir)
 
 
 @contextmanager
-def resource(uri, basedir=None):
+def resource(uri, basedir=None, cachedir=None):
     import requests
 
     with tempdir() as tmpdir:
         uri_parts = urlparse(uri)
         if uri_parts.scheme.startswith("http"):
             uri_file = uri_parts.path.split("/")[-1]
-            local_file = os.path.join(tmpdir, uri_file)
+            uri_dir = Path(cachedir or tmpdir)
+            uri_dir.mkdir(parents=True, exist_ok=True, mode=0o700)
+            local_file = uri_dir / uri_file
             with open(local_file, "wb") as f:
                 f.write(requests.get(uri).content)
         elif uri_parts.scheme == "file":
-            if uri_parts.netloc:
-                local_file = os.path.join(basedir or os.getcwd(), uri_parts.netloc + uri_parts.path)
-            else:
-                local_file = uri_parts.path
+            local_file = Path(basedir or Path.cwd()) / (uri_parts.netloc + uri_parts.path)
         elif uri_parts.scheme == "":
-            local_file = uri_parts.path
+            local_file = Path(basedir or Path.cwd()) / uri_parts.path
         else:
             raise ValueError(f"uri scheme not supported: {uri_parts.scheme}")
 
-        if os.path.isdir(local_file):
+        if local_file.is_dir():
             tmpdir = local_file
         else:
             shutil.unpack_archive(local_file, tmpdir)
-            if uri_parts.scheme.startswith("http"):
-                os.unlink(local_file)
+            if local_file.parent == tmpdir:
+                local_file.unlink()
 
         yield tmpdir
 
 
 @functools.lru_cache
 def load_schema(uri, path, basedir=None):
     from ruamel.yaml import YAML
 
     with resource(uri, basedir=basedir) as resource_dir:
-        filenames = glob(os.path.join(resource_dir, "*", path), recursive=True)
+        filenames = list(resource_dir.glob(f"*/{path}"))
         if len(filenames) < 1:
             raise ValueError(f"File not found in '{resource_dir}': '{path}'")
         if len(filenames) > 1:
             raise ValueError(f"Too many files: {filenames}")
 
         with open(filenames[0]) as f:
             yaml = YAML(typ="safe")
@@ -92,15 +91,15 @@
 
     if type(paths) == str:
         paths = (paths,)
 
     rules = []
     with resource(uri, basedir=basedir) as resource_dir:
         for path in paths:
-            for filename in glob(os.path.join(resource_dir, "*", path), recursive=True):
+            for filename in resource_dir.glob(f"*/{path}"):
                 with open(filename) as f:
                     rule = pytoml.load(f)["rule"]
                 rule["path"] = Path(".").joinpath(*Path(filename).relative_to(resource_dir).parts[1:])
                 rules.append(SimpleNamespace(**rule))
     return rules
```

### Comparing `geneve-0.1.1/geneve/utils/ast_dag.py` & `geneve-0.2.0/geneve/utils/ast_dag.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/utils/kibana.py` & `geneve-0.2.0/geneve/utils/kibana.py`

 * *Files identical despite different names*

### Comparing `geneve-0.1.1/geneve/utils/shelllib.py` & `geneve-0.2.0/geneve/utils/shelllib.py`

 * *Files identical despite different names*

