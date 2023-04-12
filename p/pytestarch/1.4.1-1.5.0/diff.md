# Comparing `tmp/pytestarch-1.4.1.tar.gz` & `tmp/pytestarch-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestarch-1.4.1.tar", max compression
+gzip compressed data, was "pytestarch-1.5.0.tar", max compression
```

## Comparing `pytestarch-1.4.1.tar` & `pytestarch-1.5.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11311 2023-04-09 18:39:45.177121 pytestarch-1.4.1/LICENSE
--rwxr-xr-x   0        0        0     1646 2023-04-09 18:39:45.177121 pytestarch-1.4.1/README.md
--rw-r--r--   0        0        0     1541 2023-04-09 18:39:45.177121 pytestarch-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      555 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/dependency_to_rule_converter.py
--rw-r--r--   0        0        0     8085 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_parser.py
--rw-r--r--   0        0        0     4024 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_rule.py
--rw-r--r--   0        0        0      126 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/exceptions.py
--rw-r--r--   0        0        0      215 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/diagram_extension/parsed_dependencies.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/__init__.py
--rw-r--r--   0        0        0     8432 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/breadth_first_searches.py
--rw-r--r--   0        0        0     7786 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_architecture.py
--rw-r--r--   0        0        0     2939 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_graph.py
--rw-r--r--   0        0        0      696 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_structures.py
--rw-r--r--   0        0        0      123 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/exceptions.py
--rw-r--r--   0        0        0     3531 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/module_name_converter.py
--rw-r--r--   0        0        0    11036 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/networkxgraph.py
--rw-r--r--   0        0        0     1893 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/types.py
--rw-r--r--   0        0        0      612 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure/utils.py
--rw-r--r--   0        0        0      171 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/__init__.py
--rw-r--r--   0        0        0      378 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/config.py
--rw-r--r--   0        0        0     2214 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/converter.py
--rw-r--r--   0        0        0       80 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/exceptions.py
--rw-r--r--   0        0        0     1088 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/file_filter.py
--rw-r--r--   0        0        0     1450 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_filter.py
--rw-r--r--   0        0        0     1895 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_types.py
--rw-r--r--   0        0        0     1323 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py
--rw-r--r--   0        0        0     2842 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/parser.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/graph_generation/__init__.py
--rw-r--r--   0        0        0     4553 2023-04-09 18:39:45.177121 pytestarch-1.4.1/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py
--rwxr-xr-x   0        0        0     3770 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/pytestarch.py
--rw-r--r--   0        0        0    25816 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/LANGUAGE_DEFINTION.md
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/__init__.py
--rw-r--r--   0        0        0     8156 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/base_language.py
--rw-r--r--   0        0        0       85 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/exceptions.py
--rw-r--r--   0        0        0     7699 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/layered_architecture_rule.py
--rw-r--r--   0        0        0      914 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/multiple_rule_applier.py
--rw-r--r--   0        0        0    12304 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/query_language/rule.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/error_message/__init__.py
--rw-r--r--   0        0        0    20878 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/error_message/message_generator.py
--rw-r--r--   0        0        0       82 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/__init__.py
--rw-r--r--   0        0        0     2517 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py
--rw-r--r--   0        0        0    11661 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py
--rw-r--r--   0        0        0     1691 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/module_requirement.py
--rw-r--r--   0        0        0     9989 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_matcher.py
--rw-r--r--   0        0        0    17861 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py
--rw-r--r--   0        0        0      802 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violations.py
--rw-r--r--   0        0        0        0 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/utils/__init__.py
--rw-r--r--   0        0        0      576 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/utils/decorators.py
--rw-r--r--   0        0        0     1489 2023-04-09 18:39:45.181121 pytestarch-1.4.1/src/pytestarch/utils/partial_match_to_regex_converter.py
--rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 pytestarch-1.4.1/setup.py
--rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 pytestarch-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11311 2023-04-12 19:51:05.188330 pytestarch-1.5.0/LICENSE
+-rwxr-xr-x   0        0        0     1645 2023-04-12 19:51:05.188330 pytestarch-1.5.0/README.md
+-rw-r--r--   0        0        0     1541 2023-04-12 19:51:05.192330 pytestarch-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/diagram_extension/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/diagram_extension/dependency_to_rule_converter.py
+-rw-r--r--   0        0        0     8085 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/diagram_extension/diagram_parser.py
+-rw-r--r--   0        0        0     4024 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/diagram_extension/diagram_rule.py
+-rw-r--r--   0        0        0      126 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/diagram_extension/exceptions.py
+-rw-r--r--   0        0        0      215 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/diagram_extension/parsed_dependencies.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/__init__.py
+-rw-r--r--   0        0        0     8458 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/breadth_first_searches.py
+-rw-r--r--   0        0        0     9067 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/evaluable_architecture.py
+-rw-r--r--   0        0        0     3144 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/evaluable_graph.py
+-rw-r--r--   0        0        0      696 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/evaluable_structures.py
+-rw-r--r--   0        0        0      123 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/exceptions.py
+-rw-r--r--   0        0        0     3755 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/module_name_converter.py
+-rw-r--r--   0        0        0    11036 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/networkxgraph.py
+-rw-r--r--   0        0        0     1893 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/types.py
+-rw-r--r--   0        0        0      872 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure/utils.py
+-rw-r--r--   0        0        0      171 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/__init__.py
+-rw-r--r--   0        0        0      378 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/config.py
+-rw-r--r--   0        0        0     2214 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/converter.py
+-rw-r--r--   0        0        0       80 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/exceptions.py
+-rw-r--r--   0        0        0     1088 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/file_filter.py
+-rw-r--r--   0        0        0     1450 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/import_filter.py
+-rw-r--r--   0        0        0     1895 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/import_types.py
+-rw-r--r--   0        0        0     1323 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py
+-rw-r--r--   0        0        0     2842 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/parser.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/graph_generation/__init__.py
+-rw-r--r--   0        0        0     4553 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py
+-rwxr-xr-x   0        0        0     3770 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/pytestarch.py
+-rw-r--r--   0        0        0    25816 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/query_language/LANGUAGE_DEFINTION.md
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/query_language/__init__.py
+-rw-r--r--   0        0        0     8700 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/query_language/base_language.py
+-rw-r--r--   0        0        0       85 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/query_language/exceptions.py
+-rw-r--r--   0        0        0     7735 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/query_language/layered_architecture_rule.py
+-rw-r--r--   0        0        0      914 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/query_language/multiple_rule_applier.py
+-rw-r--r--   0        0        0    12418 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/query_language/rule.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/error_message/__init__.py
+-rw-r--r--   0        0        0    20445 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/error_message/message_generator.py
+-rw-r--r--   0        0        0       82 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/__init__.py
+-rw-r--r--   0        0        0     2517 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py
+-rw-r--r--   0        0        0    11661 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py
+-rw-r--r--   0        0        0     1733 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/module_requirement.py
+-rw-r--r--   0        0        0    10070 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/rule_matcher.py
+-rw-r--r--   0        0        0    17889 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py
+-rw-r--r--   0        0        0      748 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/rule_violations.py
+-rw-r--r--   0        0        0        0 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/utils/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/utils/decorators.py
+-rw-r--r--   0        0        0     1489 2023-04-12 19:51:05.192330 pytestarch-1.5.0/src/pytestarch/utils/partial_match_to_regex_converter.py
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 pytestarch-1.5.0/setup.py
+-rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 pytestarch-1.5.0/PKG-INFO
```

### Comparing `pytestarch-1.4.1/LICENSE` & `pytestarch-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/README.md` & `pytestarch-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from pytestarch import Rule
 
 rule = Rule() \
         .modules_that() \
         .are_named("src.moduleB") \
         .should_not() \
         .be_imported_by_modules_that() \
-        .are_sub_modules_of("src.moduleA") \
+        .are_sub_modules_of("src.moduleA") 
 ```
 
 This rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module
 that is a submodule of "src.moduleA", excluding "src.moduleA" itself.
 
 3) Evaluate your code against this rule
```

### Comparing `pytestarch-1.4.1/pyproject.toml` & `pytestarch-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyTestArch"
-version = "1.4.1"
+version = "1.5.0"
 description = "Test framework for software architecture based on imports between modules"
 authors = ["zyskarch <zyskarch@gmail.com>"]
 maintainers = ["zyskarch <zyskarch@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 documentation = "https://zyskarch.github.io/pytestarch/"
 repository = "https://github.com/zyskarch/pytestarch"
```

### Comparing `pytestarch-1.4.1/src/pytestarch/__init__.py` & `pytestarch-1.5.0/src/pytestarch/__init__.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/diagram_extension/dependency_to_rule_converter.py` & `pytestarch-1.5.0/src/pytestarch/diagram_extension/dependency_to_rule_converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_parser.py` & `pytestarch-1.5.0/src/pytestarch/diagram_extension/diagram_parser.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/diagram_extension/diagram_rule.py` & `pytestarch-1.5.0/src/pytestarch/diagram_extension/diagram_rule.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure/breadth_first_searches.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure/breadth_first_searches.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 from typing import List, Set
 
-from pytestarch.eval_structure.evaluable_architecture import Module, StrictDependency
+from pytestarch.eval_structure.evaluable_architecture import Dependency, ModuleFilter
 from pytestarch.eval_structure.evaluable_structures import AbstractGraph, AbstractNode
-from pytestarch.eval_structure.utils import get_excluded_nodes, get_node, to_modules
+from pytestarch.eval_structure.utils import get_node, get_parent_nodes, to_modules
 
 
 def get_dependency_between_modules(
-    graph: AbstractGraph, dependent: Module, dependent_upon: Module
-) -> List[StrictDependency]:
+    graph: AbstractGraph, dependent: ModuleFilter, dependent_upon: ModuleFilter
+) -> List[Dependency]:
     dependent_node = get_node(dependent)
     dependent_upon_nodes = get_all_submodules_of(graph, dependent_upon)
 
-    nodes_to_exclude = get_excluded_nodes([dependent, dependent_upon])
+    nodes_to_exclude = get_parent_nodes([dependent, dependent_upon])
 
     nodes_to_check = [dependent_node]
     checked_nodes = set()
 
     dependencies = []
 
     while nodes_to_check:
@@ -40,16 +40,16 @@
                 and child not in nodes_to_exclude
             ):
                 dependencies.append(tuple(to_modules([node, child])))
     return dependencies  # type: ignore
 
 
 def any_dependency_to_module_other_than(  # noqa: C901
-    graph: AbstractGraph, dependent: Module, dependent_upons: Set[Module]
-) -> List[StrictDependency]:
+    graph: AbstractGraph, dependent: ModuleFilter, dependent_upons: Set[ModuleFilter]
+) -> List[Dependency]:
     # nodes to exclude are nodes that once reached will not have their submodules analysed next
     nodes_to_exclude = set()
     for dependent_upon in dependent_upons:
         if dependent_upon == dependent:
             continue
         nodes_to_exclude.update(get_all_submodules_of(graph, dependent_upon))
 
@@ -105,16 +105,16 @@
                 else:
                     nodes_to_check.append(child)
 
     return nodes_fulfilling_criteria  # type: ignore
 
 
 def any_other_dependency_to_module_than(  # noqa: C901
-    graph: AbstractGraph, dependents: Set[Module], dependent_upon: Module
-) -> List[StrictDependency]:
+    graph: AbstractGraph, dependents: Set[ModuleFilter], dependent_upon: ModuleFilter
+) -> List[Dependency]:
     # submodules of the dependent upon module do not count as an import that is not the dependent upon module
     # submodules of and including the dependent do not count as allowed imports
 
     # nodes to exclude are nodes that once reached will not have their submodules analysed next
     nodes_to_exclude = set()
     for dependent in dependents:
         if dependent == dependent_upon:
@@ -173,15 +173,17 @@
 
                 if parent not in nodes_to_exclude:
                     nodes_to_check.append(parent)
 
     return nodes_fulfilling_criteria  # type: ignore
 
 
-def get_all_submodules_of(graph: AbstractGraph, module: Module) -> Set[AbstractNode]:
+def get_all_submodules_of(
+    graph: AbstractGraph, module: ModuleFilter
+) -> Set[AbstractNode]:
     """Returns all submodules of a given module.
 
     Args:
         module: module to retrieve submodules of
 
     Returns:
         all submodules, including the module itself
```

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_architecture.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure/evaluable_architecture.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,56 +9,63 @@
 from pytestarch.eval_structure.exceptions import LayerMismatch
 
 Layer = str
 ModuleName = str
 
 
 class LayerMapping:
-    def __init__(self, layer_mapping: Dict[Layer, List[Module]]) -> None:
-        self._layer_mapping = layer_mapping
-        self._module_mapping = {
+    def __init__(
+        self, layer_mapping_for_module_filters: Dict[Layer, List[ModuleFilter]]
+    ) -> None:
+        self._layer_mapping_for_module_filters = layer_mapping_for_module_filters
+        self._module_filter_mapping = {
             module: layer
-            for layer, modules in layer_mapping.items()
+            for layer, modules in layer_mapping_for_module_filters.items()
             for module in modules
         }
 
-        self._sorted_module_names = sorted(
-            map(lambda module: module.name, self._module_mapping.keys())
+        self._sorted_module_filter_names = sorted(
+            map(lambda module: module.name, self._module_filter_mapping.keys())
         )
 
-    def get_modules(self, layer: Layer) -> List[Module]:
-        return self._layer_mapping[layer]
+    def get_module_filters(self, layer: Layer) -> List[ModuleFilter]:
+        return self._layer_mapping_for_module_filters[layer]
 
     def get_layer(self, module: Module) -> Optional[Layer]:
         """Attempts to find the layer the given module belongs to. If the module does not appear in the
         layer definition itself, it is checked whether the module is a submodule of one of the modules in the layer
         definition. If so, the layer of the parent module is returned. Otherwise, None is returned.
         This assumes that if a module is in layer X, all of its submodules are as well.
         """
         if not module.name:
             return None
 
-        layer_candidate = self._module_mapping.get(module, None)
+        layer_candidate = self._module_filter_mapping.get(module, None)
 
         if layer_candidate is not None:
             return layer_candidate
 
         idx_of_module = (
-            bisect(self._sorted_module_names, module.name) - 1
+            bisect(self._sorted_module_filter_names, module.name) - 1
         )  # -1 since idx is after the insertion point
 
         candidate_parent_modules = []
         while idx_of_module >= 0:
-            parent_module_candidate = self._sorted_module_names[idx_of_module]
+            parent_module_candidate = self._sorted_module_filter_names[idx_of_module]
             if module.name.startswith(parent_module_candidate):
-                candidate_parent_modules.append(Module(name=parent_module_candidate))
+                candidate_parent_modules.append(
+                    ModuleFilter(name=parent_module_candidate)
+                )
             idx_of_module -= 1
 
         candidate_layers = set(
-            map(lambda module: self._module_mapping[module], candidate_parent_modules)
+            map(
+                lambda module: self._module_filter_mapping[module],
+                candidate_parent_modules,
+            )
         )
 
         if len(candidate_layers) > 1:
             raise LayerMismatch(
                 f"Multiple possible parent modules found for module {module.name}."
             )
 
@@ -68,50 +75,79 @@
             return candidate_layers.pop()
 
     def get_layer_for_module_name(self, module_name: str) -> Optional[Layer]:
         return self.get_layer(Module(name=module_name))
 
     @property
     def all_layers(self) -> Iterable[Layer]:
-        return self._layer_mapping.keys()
+        return self._layer_mapping_for_module_filters.keys()
 
 
 @dataclass(frozen=True)
-class Module:
-    """Represents a python module.
+class ModuleFilter:
+    """Represents a way to identify a python module in the dependency graph.
     The module can either be identified by its name or by the name of a parent module.
 
     Attributes:
         name: full name of the module
         parent_module: full name of the parent module
         regex: if True, the name represents a regex pattern that matches potentially multiple modules
+
+    Either name or parent_module can be specified, but not both.
     """
 
     name: Optional[str] = None
     parent_module: Optional[str] = None
     regex: bool = False
 
 
-StrictDependency = Tuple[Module, Module]
+@dataclass(frozen=True)
+class Module:
+    """Represents an actual python module found in the dependency graph."""
+
+    name: str
+
+    @property
+    def is_single_module(self) -> bool:
+        return True
+
+
+@dataclass(frozen=True)
+class ModuleGroup(Module):
+    """Represents a group of actual python module found in the dependency graph.
+    This is only needed if a group of modules is specified via their parent module's name, and only for not explicitly
+    requested dependencies. For these, the original module filter is not converted to actual modules, as this would
+    clutter the return type and the user output.
+    Instead, this filter will be converted to a module group.
+
+    The name is the name of the parent module of all modules in this group.
+    """
+
+    name: str
+
+    @property
+    def is_single_module(self) -> bool:
+        return False
+
+
+Dependency = Tuple[Module, Module]
 # key: user-requested dependency
 # values: list of exact modules that show this dependency
-ExplicitlyRequestedDependenciesByBaseModules = Dict[
-    StrictDependency, List[StrictDependency]
-]
+ExplicitlyRequestedDependenciesByBaseModules = Dict[Dependency, List[Dependency]]
 # key: module that either has dependencies or that others are dependent on that were not explicitly requested
 # via the rule the user has specified
 # value: importer and importee that were not found
-NotExplicitlyRequestedDependenciesByBaseModule = Dict[Module, List[StrictDependency]]
+NotExplicitlyRequestedDependenciesByBaseModule = Dict[Module, List[Dependency]]
 
 
 class EvaluableArchitecture(Protocol):
     def get_dependencies(
         self,
-        dependents: Union[Module, list[Module]],
-        dependent_upons: Union[Module, list[Module]],
+        dependents: Union[ModuleFilter, list[ModuleFilter]],
+        dependent_upons: Union[ModuleFilter, list[ModuleFilter]],
     ) -> ExplicitlyRequestedDependenciesByBaseModules:
         """Returns tuple of importer and importee per dependent and depending module if the dependent module is indeed
         depending on the dependent_upon module. In short: find all dependencies between dependent and dependent_upons.
 
         Submodules of dependent and dependent upon are taken into account.
         If X.A depends on Y, then X also depends on Y, as X.A is part of X.
         If X depends on Y.Z, then it also depends on Y.
@@ -127,16 +163,16 @@
             Importer and importee per pair of dependent and dependent_upon module if there are any
             that are sub modules of dependent and dependent_upon respectively.
         """
         raise NotImplementedError()
 
     def any_dependencies_from_dependents_to_modules_other_than_dependent_upons(
         self,
-        dependents: List[Module],
-        dependent_upons: List[Module],
+        dependents: List[ModuleFilter],
+        dependent_upons: List[ModuleFilter],
     ) -> NotExplicitlyRequestedDependenciesByBaseModule:
         """Returns list of depending modules per dependent module if the dependent module has any
         dependency to a module other than the dependent_upon modules
         or any of their submodules.
 
         If a dependent module is defined via a parent module, this parent module is not taken into account.
         If a dependent upon module is defined via a parent module, this parent module counts as an 'other' dependency.
@@ -150,16 +186,16 @@
         Returns:
             All modules other than dependent_upon on which dependent module as any dependency per dependent module
         """
         raise NotImplementedError()
 
     def any_other_dependencies_on_dependent_upons_than_from_dependents(
         self,
-        dependents: List[Module],
-        dependent_upons: List[Module],
+        dependents: List[ModuleFilter],
+        dependent_upons: List[ModuleFilter],
     ) -> NotExplicitlyRequestedDependenciesByBaseModule:
         """Returns list of depending modules per dependent_upon module if any module other than the dependent
         module and its submodules has any dependency to the
         dependent_upon module.
         If the dependent module is defined via a parent module, this parent module is taken into account. This means
         that if the dependent module's parent module has a dependency to the dependent upon module, this will be contained
         in the returned list.
```

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_graph.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure/evaluable_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,80 +10,83 @@
     any_dependency_to_module_other_than,
     any_other_dependency_to_module_than,
     get_dependency_between_modules,
 )
 from pytestarch.eval_structure.evaluable_architecture import (
     EvaluableArchitecture,
     ExplicitlyRequestedDependenciesByBaseModules,
-    Module,
+    ModuleFilter,
     NotExplicitlyRequestedDependenciesByBaseModule,
 )
 from pytestarch.eval_structure.evaluable_structures import AbstractGraph
+from pytestarch.eval_structure.utils import filter_to_module
 
 
 class EvaluableArchitectureGraph(EvaluableArchitecture):
     """Abstract implementation of an evaluable object that is based on a graph structure."""
 
     def __init__(self, graph: AbstractGraph) -> None:
         self._graph = graph
 
     def get_dependencies(
         self,
-        dependents: List[Module],
-        dependent_upons: List[Module],
+        dependents: List[ModuleFilter],
+        dependent_upons: List[ModuleFilter],
     ) -> ExplicitlyRequestedDependenciesByBaseModules:
         result = {}
 
         # remove any duplicates
         dependents = set(dependents)
         dependent_upons = set(dependent_upons)
 
         for dependent, dependent_upon in product(dependents, dependent_upons):
             dependency = get_dependency_between_modules(
                 self._graph, dependent, dependent_upon
             )
-            result[(dependent, dependent_upon)] = dependency
+            result[
+                (filter_to_module(dependent), filter_to_module(dependent_upon))
+            ] = dependency
 
         return result
 
     def any_dependencies_from_dependents_to_modules_other_than_dependent_upons(
         self,
-        dependents: List[Module],
-        dependent_upons: List[Module],
+        dependents: List[ModuleFilter],
+        dependent_upons: List[ModuleFilter],
     ) -> NotExplicitlyRequestedDependenciesByBaseModule:
         # remove any duplicates
         dependents = set(dependents)
         dependent_upons = set(dependent_upons)
 
         result = {}
 
         for dependent in dependents:
             dependencies = any_dependency_to_module_other_than(
                 self._graph, dependent, dependent_upons
             )
-            result[dependent] = dependencies
+            result[filter_to_module(dependent)] = dependencies
 
         return result
 
     def any_other_dependencies_on_dependent_upons_than_from_dependents(
         self,
-        dependents: List[Module],
-        dependent_upons: List[Module],
+        dependents: List[ModuleFilter],
+        dependent_upons: List[ModuleFilter],
     ) -> NotExplicitlyRequestedDependenciesByBaseModule:
         # remove any duplicates
         dependents = set(dependents)
         dependent_upons = set(dependent_upons)
 
         result = {}
 
         for dependent_upon in dependent_upons:
             dependencies = any_other_dependency_to_module_than(
                 self._graph, dependents, dependent_upon
             )
-            result[dependent_upon] = dependencies
+            result[filter_to_module(dependent_upon)] = dependencies
 
         return result
 
     def visualize(self, **kwargs: Any) -> None:
         self._graph.draw(**kwargs)
 
     @property
```

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure/evaluable_structures.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure/evaluable_structures.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure/module_name_converter.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure/module_name_converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,88 +2,89 @@
 
 import re
 from collections import defaultdict
 from typing import Dict, List, Tuple
 
 from pytestarch import EvaluableArchitecture
 from pytestarch.eval_structure.breadth_first_searches import get_all_submodules_of
-from pytestarch.eval_structure.evaluable_architecture import Module
+from pytestarch.eval_structure.evaluable_architecture import Module, ModuleFilter
 from pytestarch.eval_structure.exceptions import ImpossibleMatch
 
 
 class ModuleNameConverter:
     """Converts module names specified via regex pattern to module names based on which modules in the architecture
     match the regex pattern."""
 
     @classmethod
     def convert(
-        cls, modules: List[Module], arch: EvaluableArchitecture
-    ) -> Tuple[List[Module], Dict[str, List[Module]]]:
+        cls, modules: List[ModuleFilter], arch: EvaluableArchitecture
+    ) -> Tuple[List[ModuleFilter], Dict[str, List[Module]]]:
         """Converts each regex pattern that serves to identify module names into actual modules that match this pattern.
 
         Args:
             - modules: list of modules, some of which may need converting since their names are regex patterns
             - arch: architecture that contains actual modules
 
         Returns:
-            - list of modules, now without any regex patterns.
+            - list of module filters, now without any regex patterns. Will be used for later dependency graph queries.
             - mapping between a regex pattern and the actual modules it was replaced by
         """
         (
             modules_that_need_converting,
             other_modules,
         ) = cls._split_modules_by_presence_of_regex_pattern(modules)
 
         never_matched = {module.name for module in modules_that_need_converting}
 
-        converted_modules = set()
+        converted_module_filters = set()
         conversion_mapping = defaultdict(list)
         matching_submodules = set()
 
         module_names_that_need_to_be_matched = list(
             map(lambda module: module.name, modules_that_need_converting)
         )
 
         for actually_present_module in arch.modules:
             for module_to_match in module_names_that_need_to_be_matched:
                 if cls._name_matches_pattern(module_to_match, actually_present_module):
                     converted_module = Module(name=actually_present_module)
+                    converted_module_filter = ModuleFilter(name=actually_present_module)
 
-                    converted_modules.add(converted_module)
+                    converted_module_filters.add(converted_module_filter)
                     conversion_mapping[module_to_match].append(converted_module)
 
                     if module_to_match in never_matched:
                         never_matched.remove(module_to_match)
 
                     submodules_of_match = get_all_submodules_of(
-                        arch._graph, converted_module
+                        arch._graph, converted_module_filter
                     )
                     submodules_of_match.remove(
                         actually_present_module
                     )  # should not count as its own submodule here
                     matching_submodules.update(submodules_of_match)
 
         if never_matched:
             raise ImpossibleMatch(
                 f'No modules found that match: {", ".join(never_matched)}'
             )
 
-        return list(converted_modules) + other_modules, conversion_mapping
+        return list(converted_module_filters) + other_modules, conversion_mapping
 
     @classmethod
     def _name_matches_pattern(cls, pattern_to_match: str, name: str) -> bool:
         pattern = re.compile(pattern_to_match)
         match = re.match(pattern, name)
 
         return match is not None
 
     @classmethod
     def _split_modules_by_presence_of_regex_pattern(
-        cls, modules: List[Module]
-    ) -> Tuple[List[Module], List[Module]]:
+        cls, modules: List[ModuleFilter]
+    ) -> Tuple[List[ModuleFilter], List[ModuleFilter]]:
         modules_with_regex_name_pattern = []
         other_modules = []
 
         for module in modules:
             if module.regex:
                 modules_with_regex_name_pattern.append(module)
             else:
```

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure/networkxgraph.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure/networkxgraph.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure/types.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure/types.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/converter.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/file_filter.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/file_filter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_filter.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/import_filter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/import_types.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/import_types.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/importee_module_calculator.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/file_import/parser.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure_generation/file_import/parser.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py` & `pytestarch-1.5.0/src/pytestarch/eval_structure_generation/graph_generation/graph_generator.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/pytestarch.py` & `pytestarch-1.5.0/src/pytestarch/pytestarch.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/query_language/LANGUAGE_DEFINTION.md` & `pytestarch-1.5.0/src/pytestarch/query_language/LANGUAGE_DEFINTION.md`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/query_language/base_language.py` & `pytestarch-1.5.0/src/pytestarch/query_language/base_language.py`

 * *Files 7% similar despite different names*

```diff
@@ -111,15 +111,18 @@
         pass
 
     @abstractmethod
     def have_name_matching(
         self,
         regex: str,
     ) -> ModuleSpecificationSuccessor:
-        """If multiple rule subjects are specified, this has the same effect as defining a rule per rule subject."""
+        """Note that regex expressions can have unexpected results if predicates apply to modules, but not their submodules.
+        This is often the case for regex expressions with negations. Refer to the documentation of the module import feature for more details.
+        If multiple rule subjects are specified, this has the same effect as defining a rule per rule subject.
+        """
         pass
 
 
 class RuleObject(ModuleSpecification[RuleApplier], ABC):
     pass
 
 
@@ -183,14 +186,16 @@
     @abstractmethod
     def have_modules_with_names_matching(
         self,
         regex: str,
     ) -> Union[LayerName, BaseLayeredArchitecture]:
         """If a module is defined as belonging to layer X, then its submodules are also assumed to be part of layer X.
         Note that no attempt will be made to ensure that the regex patterns for different layers are mutually exclusive.
+        Also note that regex expressions can have unexpected results if predicates apply to modules, but not their submodules.
+        This is often the case for regex expressions with negations. Refer to the documentation of the module import feature for more details.
         """
         pass
 
 
 class LayerName(ABC):
     """Offers functionality to specify the name of a yet to be defined layer."""
```

### Comparing `pytestarch-1.4.1/src/pytestarch/query_language/layered_architecture_rule.py` & `pytestarch-1.5.0/src/pytestarch/query_language/layered_architecture_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from functools import partial
 from typing import List, Tuple, Type, Union
 
 from pytestarch import EvaluableArchitecture, Rule
-from pytestarch.eval_structure.evaluable_architecture import LayerMapping, Module
+from pytestarch.eval_structure.evaluable_architecture import LayerMapping, ModuleFilter
 from pytestarch.query_language.base_language import (
     AccessSpecification,
     BaseLayeredArchitecture,
     LayerBase,
     LayerBehaviorSpecification,
     LayerDefinition,
     LayerName,
@@ -112,22 +112,22 @@
     def __str__(self) -> str:
         layers = [
             f"Layer {layer}: [{', '.join(map(lambda m: m.name, modules))}]"
             for layer, modules in self._modules_by_layer_name.items()
         ]
         return f'Layered Architecture: {"; ".join(layers)}'
 
-    def __getitem__(self, layer: str) -> List[Module]:
+    def __getitem__(self, layer: str) -> List[ModuleFilter]:
         return self._modules_by_layer_name[layer]
 
-    def _to_module_objects(self, modules: List[str]) -> List[Module]:
-        return [Module(name=module) for module in modules]
+    def _to_module_objects(self, modules: List[str]) -> List[ModuleFilter]:
+        return [ModuleFilter(name=module) for module in modules]
 
-    def _from_regex_to_module_objects(self, regex: str) -> List[Module]:
-        return [Module(name=regex, regex=True)]
+    def _from_regex_to_module_objects(self, regex: str) -> List[ModuleFilter]:
+        return [ModuleFilter(name=regex, regex=True)]
 
 
 class LayerRule(
     RuleApplier,
     LayerRuleBase,
     LayerRuleSubject,
     LayerRuleObject,
```

### Comparing `pytestarch-1.4.1/src/pytestarch/query_language/multiple_rule_applier.py` & `pytestarch-1.5.0/src/pytestarch/query_language/multiple_rule_applier.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/query_language/rule.py` & `pytestarch-1.5.0/src/pytestarch/query_language/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, replace
 from typing import Callable, List, Optional, Tuple, Union
 
 from pytestarch import EvaluableArchitecture
-from pytestarch.eval_structure.evaluable_architecture import Module
+from pytestarch.eval_structure.evaluable_architecture import ModuleFilter
 from pytestarch.query_language.base_language import (
     BehaviorSpecification,
     DependencySpecification,
     RuleApplier,
     RuleBase,
     RuleObject,
     RuleSubject,
@@ -26,16 +26,16 @@
 from pytestarch.utils.partial_match_to_regex_converter import (
     convert_partial_match_to_regex,
 )
 
 
 @dataclass
 class RuleConfiguration:
-    modules_to_check: Optional[List[Module]] = None
-    modules_to_check_against: Optional[List[Module]] = None
+    modules_to_check: Optional[List[ModuleFilter]] = None
+    modules_to_check_against: Optional[List[ModuleFilter]] = None
     should: bool = False
     should_only: bool = False
     should_not: bool = False
     except_present: bool = False
     import_: bool = None
     rule_object_anything: bool = False
 
@@ -59,52 +59,54 @@
         ] = DefaultRuleMatcher,
     ) -> None:
         self._rule_matcher_class = rule_matcher_class
         self._modules_to_check_to_be_specified_next = None
         self._configuration = RuleConfiguration()
 
     @property
-    def rule_subjects(self) -> Optional[List[Module]]:
+    def rule_subjects(self) -> Optional[List[ModuleFilter]]:
         return self._configuration.modules_to_check
 
     def modules_that(self) -> RuleSubject:
         self._modules_to_check_to_be_specified_next = True
         return self
 
     def are_sub_modules_of(
         self, modules: Union[str, List[str]]
     ) -> BehaviorSpecification:
-        self._set_modules(modules, lambda name: Module(parent_module=name))
+        self._set_modules(modules, lambda name: ModuleFilter(parent_module=name))
         return self
 
     def are_named(self, names: Union[str, List[str]]) -> BehaviorSpecification:
-        self._set_modules(names, lambda name: Module(name=name))
+        self._set_modules(names, lambda name: ModuleFilter(name=name))
         return self
 
     @deprecated
     def have_name_containing(
         self, partial_names: Union[str, List[str]]
     ) -> BehaviorSpecification:
         self._set_modules(
             partial_names,
-            lambda name: Module(name=convert_partial_match_to_regex(name), regex=True),
+            lambda name: ModuleFilter(
+                name=convert_partial_match_to_regex(name), regex=True
+            ),
         )
         return self
 
     def have_name_matching(
         self,
         regex: str,
     ) -> BehaviorSpecification:
-        self._set_modules(regex, lambda name: Module(name=name, regex=True))
+        self._set_modules(regex, lambda name: ModuleFilter(name=name, regex=True))
         return self
 
     def _set_modules(
         self,
         module_names: Union[str, List[str]],
-        create_module_fn: Callable[[str], Module],
+        create_module_fn: Callable[[str], ModuleFilter],
     ) -> None:
         if self._modules_to_check_to_be_specified_next is None:
             raise ImproperlyConfigured("Specify a RuleSubject or RuleObject first.")
 
         if isinstance(module_names, str):
             module_names = [module_names]
 
@@ -117,24 +119,24 @@
     def _add_modules(self, modules: List[Tuple[str, bool]]) -> BehaviorSpecification:
         module_names = []
         module_creation_fn = []
 
         for module, name_is_regex in modules:
             module_names.append(module)
             module_creation_fn.append(
-                lambda name: Module(name=name, regex=name_is_regex)
+                lambda name: ModuleFilter(name=name, regex=name_is_regex)
             )
 
         self._append_modules(module_names, module_creation_fn)
         return self
 
     def _append_modules(
         self,
         module_names: List[str],
-        create_module_fns: List[Callable[[str], Module]],
+        create_module_fns: List[Callable[[str], ModuleFilter]],
     ) -> None:
         modules = [fn(n) for n, fn in zip(module_names, create_module_fns)]
         if self._modules_to_check_to_be_specified_next:
             if self._configuration.modules_to_check is None:
                 self._configuration.modules_to_check = []
 
             self._configuration.modules_to_check.extend(modules)
@@ -236,20 +238,20 @@
             f"{method_name} "
             f'{"import" if self._configuration.import_ else "be imported by"} '
             f'{"modules except " if self._configuration.except_present else ""}'
             f"{object_message}"
             f'"{combined_rule_objects}".'
         )
 
-    def _combine_names(self, modules: list[Module]) -> str:
+    def _combine_names(self, modules: list[ModuleFilter]) -> str:
         return ", ".join(
             sorted(map(lambda module: self._get_module_name(module), modules))
         )
 
-    def _get_module_name(self, module: Module) -> str:
+    def _get_module_name(self, module: ModuleFilter) -> str:
         return module.name if module.name is not None else module.parent_module
 
     def _assert_required_configuration_present(self) -> None:
         behavior_missing = not any(
             [
                 self._configuration.should,
                 self._configuration.should_only,
@@ -316,15 +318,15 @@
             modules_to_check_against=modules_to_check_without_parent_and_submodule_combinations,
             except_present=True,
         )
 
     @classmethod
     def _get_modules_to_check_without_parent_and_submodule_combinations(
         cls, configuration: RuleConfiguration
-    ) -> Optional[List[Module]]:
+    ) -> Optional[List[ModuleFilter]]:
         # if modules_to_check contain a module and its submodule, this can throw off the breadth first search conducted
         # on the dependency graph - and also, this setup does not really make sense
         if configuration.modules_to_check is None:
             return None
 
         module_names = sorted(
             map(lambda module: module.name, configuration.modules_to_check)
```

### Comparing `pytestarch-1.4.1/src/pytestarch/rule_assessment/error_message/message_generator.py` & `pytestarch-1.5.0/src/pytestarch/rule_assessment/error_message/message_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Converts a RuleViolations object into a human-readable format."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Dict, List, Optional, Set, Tuple
+from typing import Dict, Iterable, List, Optional, Set, Tuple
 
 from pytestarch.eval_structure.evaluable_architecture import (
+    Dependency,
     LayerMapping,
     Module,
-    StrictDependency,
 )
 from pytestarch.rule_assessment.rule_check.rule_violations import RuleViolations
 
 LAYER_FIRST_LETTER = "l"
 LAYER_FIRST_LETTER_CAPITAL = "L"
 
 IMPORT = "import"
@@ -161,15 +161,15 @@
         self, rule_violations: RuleViolations
     ) -> List[RuleViolatedMessage]:
         return self._create_no_import_between_original_subject_and_objects_message(
             rule_violations.should_violations
         )
 
     def _create_no_import_between_original_subject_and_objects_message(
-        self, rule_violations: List[StrictDependency]
+        self, rule_violations: Iterable[Dependency]
     ) -> List[RuleViolatedMessage]:
         messages = []
 
         (
             rule_objects_for_rule_subject,
             violating_rule_subjects,
         ) = self._get_violating_rule_subjects_and_objects(rule_violations)
@@ -203,26 +203,26 @@
         combined_rule_object = ", ".join(rule_objects)
         if combined_rule_object:
             messages.append(
                 RuleViolatedMessage(rule_subject, rule_verb, combined_rule_object)
             )
 
     def _get_violating_rule_subjects_and_objects(
-        self, rule_violation_dependency_names: List[StrictDependency]
+        self, rule_violation_dependencies: Iterable[Dependency]
     ) -> Tuple[Dict[Module, List[Module]], Set[Module]]:
         violating_rule_subjects = set()
         rule_objects_for_rule_subject = defaultdict(list)
-        for rule_subject, rule_object in rule_violation_dependency_names:
+        for rule_subject, rule_object in rule_violation_dependencies:
             violating_rule_subjects.add(rule_subject)
             rule_objects_for_rule_subject[rule_subject].append(rule_object)
 
         return rule_objects_for_rule_subject, violating_rule_subjects
 
     def _convert_to_names(
-        self, violating_dependencies: List[StrictDependency]
+        self, violating_dependencies: List[Dependency]
     ) -> List[Tuple[str, str]]:
         return [
             (dependency[0].name, dependency[1].name)
             for dependency in violating_dependencies
         ]
 
     def _create_should_only_import_violated_messages(
@@ -250,15 +250,15 @@
     ) -> List[RuleViolatedMessage]:
         return self._create_other_violating_dependencies_message(
             rule_violations.should_only_violations_by_forbidden_import
         )
 
     def _create_other_violating_dependencies_message(
         self,
-        violating_dependencies: List[StrictDependency],
+        violating_dependencies: Iterable[Dependency],
     ) -> List[RuleViolatedMessage]:
         # messages are always of the type "module x imports module y"
         messages = []
 
         verb_prefix = self._get_verb_prefix(negated=False, subject_singular=True)
         suffix = self._get_verb_suffix(subject_singular=True)
         rule_verb = self._concatenate_verb(
@@ -294,15 +294,15 @@
         self, rule_violations: RuleViolations
     ) -> List[RuleViolatedMessage]:
         return self._create_no_import_other_than_between_original_subject_and_objects_message(
             rule_violations.should_except_violations
         )
 
     def _create_no_import_other_than_between_original_subject_and_objects_message(
-        self, rule_violations: List[StrictDependency]
+        self, rule_violations: Iterable[Dependency]
     ) -> List[RuleViolatedMessage]:
         messages = []
 
         (
             rule_objects_for_rule_subject,
             violating_rule_subjects,
         ) = self._get_violating_rule_subjects_and_objects(rule_violations)
@@ -380,35 +380,22 @@
     def _create_should_not_import_except_violated_messages(
         self, rule_violations: RuleViolations
     ) -> List[RuleViolatedMessage]:
         return self._create_other_violating_dependencies_message(
             rule_violations.should_not_except_violations
         )
 
-    def _generate_rule_xbject_names_and_count(
-        self, original_rule_xbjects: List[Module]
-    ) -> Tuple[List[str], Dict[str, bool]]:
-        names = []
-        is_singular = {}
-
-        for rule_object in original_rule_xbjects:
-            module_name = self._get_module_name(rule_object)
-            names.append(module_name)
-            is_singular[module_name] = self._is_singular_module(rule_object)
-
-        return names, is_singular
-
     def _get_module_name(self, module: Module) -> str:
-        return module.name if module.name is not None else module.parent_module
+        return module.name
 
     def _is_singular_module(self, module: Module) -> bool:
-        return module.name is not None
+        return module.is_single_module
 
     def _get_verb_prefix(self, negated: bool, subject_singular: bool) -> str:
-        return PREFIX_MAPPING[(self._import_rule, negated, subject_singular)]
+        return PREFIX_MAPPING[(self._import_rule, negated, subject_singular)]  # type: ignore
 
     def _concatenate_verb(self, verb: str, prefix: str = "", suffix="") -> str:
         return f"{prefix}{verb}{suffix}"
 
     def _get_rule_object(self, rule_object: Module) -> str:
         module_qualifier = (
             ""
@@ -426,15 +413,15 @@
 
         return f'{prefix}"{self._get_module_name(rule_subject)}"'
 
     def _get_quoted_name(self, name: str) -> str:
         return f'"{name}"'
 
     def _get_rule_subject_and_object_of_dependency(
-        self, dependency: StrictDependency
+        self, dependency: Dependency
     ) -> Tuple[str, str]:
         rule_subject_name = self._get_module_name(dependency[0])
         rule_object_name = self._get_module_name(dependency[1])
 
         rule_subject_name_formatted = self._get_quoted_name(rule_subject_name)
         rule_object_name_formatted = self._get_quoted_name(rule_object_name)
 
@@ -479,15 +466,15 @@
 
         if layer is None:
             return " (no layer)"
         else:
             return f" (layer {self._get_quoted_name(layer)})"
 
     def _create_no_import_between_original_subject_and_objects_message(
-        self, rule_violations: List[StrictDependency]
+        self, rule_violations: List[Dependency]
     ) -> List[RuleViolatedMessage]:
         messages = []
 
         (
             rule_object_layers_for_rule_subject_layer,
             violating_rule_subject_layers,
         ) = self._get_violating_rule_subject_and_objects_layers(rule_violations)
@@ -514,32 +501,36 @@
             self._add_combined_rule_objects(
                 messages, rule_object_layers, rule_subject_layer_formatted, rule_verb
             )
 
         return messages
 
     def _get_violating_rule_subject_and_objects_layers(
-        self, rule_violation_dependency_names: List[StrictDependency]
+        self, rule_violation_dependencies: List[Dependency]
     ) -> Tuple[Dict[str, Set[str]], Set[str]]:
         violating_rule_subject_layers = set()
         rule_object_layers_for_rule_subject_layer = defaultdict(set)
 
-        for rule_subject, rule_object in rule_violation_dependency_names:
-            rule_subject_layer = self._layer_mapping.get_layer(rule_subject)
-            rule_object_layer = self._layer_mapping.get_layer(rule_object)
+        for rule_subject, rule_object in rule_violation_dependencies:
+            rule_subject_layer = self._layer_mapping.get_layer_for_module_name(
+                rule_subject.name
+            )
+            rule_object_layer = self._layer_mapping.get_layer_for_module_name(
+                rule_object.name
+            )
 
             violating_rule_subject_layers.add(rule_subject_layer)
             rule_object_layers_for_rule_subject_layer[rule_subject_layer].add(
                 rule_object_layer
             )
 
         return rule_object_layers_for_rule_subject_layer, violating_rule_subject_layers
 
     def _create_no_import_other_than_between_original_subject_and_objects_message(
-        self, rule_violations: List[StrictDependency]
+        self, rule_violations: List[Dependency]
     ) -> List[RuleViolatedMessage]:
         messages = []
 
         (
             rule_object_layers_for_rule_subject,
             violating_rule_subject_layers,
         ) = self._get_violating_rule_subject_and_objects_layers(rule_violations)
```

### Comparing `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py` & `pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/behavior_requirement.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py` & `pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/layer_rule_violation_detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import Any, Dict, List, Optional, Set
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 from pytestarch.eval_structure.evaluable_architecture import (
+    Dependency,
     ExplicitlyRequestedDependenciesByBaseModules,
     Layer,
     LayerMapping,
     Module,
     NotExplicitlyRequestedDependenciesByBaseModule,
-    StrictDependency,
 )
 from pytestarch.rule_assessment.rule_check.behavior_requirement import (
     BehaviorRequirement,
 )
 from pytestarch.rule_assessment.rule_check.module_requirement import ModuleRequirement
 from pytestarch.rule_assessment.rule_check.rule_violation_detector import (
     RuleViolationBaseDetector,
@@ -38,30 +38,30 @@
 
     def _should_not_requirement_violations(
         self,
         explicitly_requested_dependencies_should_not_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_should_not_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(explicitly_requested_dependencies)
 
     def _should_requirement_violations(
         self,
         explicitly_requested_dependencies_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_should_be_present
         ):
             return set()
 
         return self._get_abstract_dependencies_without_any_realisations(
@@ -70,15 +70,15 @@
 
     def _should_only_requirement_violations_by_no_import(
         self,
         explicitly_requested_dependencies_and_no_other_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_and_no_other_should_be_present
         ):
             return set()
 
         return self._get_abstract_dependencies_without_any_realisations(
@@ -87,30 +87,30 @@
 
     def _should_only_requirement_violations_by_not_explicitly_requested_dependency(
         self,
         explicitly_requested_dependencies_and_no_other_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_and_no_other_should_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(not_explicitly_requested_dependencies)
 
     def _should_except_requirement_violations(
         self,
         at_least_one_not_explicitly_requested_dependency_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not at_least_one_not_explicitly_requested_dependency_should_be_present
         ):
             return set()
 
         return self._get_any_missing_dependencies_in_user_specified_order(
@@ -119,15 +119,15 @@
 
     def _should_only_except_requirement_violations_due_to_no_other_imports(
         self,
         explicitly_requested_dependency_should_not_but_others_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not explicitly_requested_dependency_should_not_but_others_should_be_present
         ):
             return set()
 
         return self._get_any_missing_dependencies_in_user_specified_order(
@@ -136,53 +136,51 @@
 
     def _should_only_except_requirement_violations_due_to_explicit_dependency_present(
         self,
         explicitly_requested_dependency_should_not_but_others_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependency_should_not_but_others_should_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(explicitly_requested_dependencies)
 
     def _should_not_except_requirement_violations(
         self,
         not_explicitly_requested_dependencies_should_not_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not not_explicitly_requested_dependencies_should_not_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(not_explicitly_requested_dependencies)
 
     def _get_abstract_dependencies_without_any_realisations(
         self,
-        explicitly_requested_dependencies: Dict[
-            StrictDependency, List[StrictDependency]
-        ],
-    ) -> Set[StrictDependency]:
+        explicitly_requested_dependencies: Dict[Dependency, List[Dependency]],
+    ) -> Set[Dependency]:
         """If there is any explicitly requested dependency for each rule object, an empty list will be returned. If there is none at all for at least one rule object,
         all dependencies will be returned."""
         explicitly_requested_dependencies_by_layers = (
             self._group_explicitly_requested_dependencies_by_layers(
                 explicitly_requested_dependencies
             )
         )
 
-        result = set()
+        result: Set[Tuple[Module, Module]] = set()  # type: ignore
 
         for layer in self._layer_to_module_mapping.all_layers:
             explicitly_requested_dependencies_for_layer = (
                 explicitly_requested_dependencies_by_layers[layer]
             )
 
             if not explicitly_requested_dependencies_for_layer:
@@ -203,58 +201,55 @@
                 }
             )
         return result
 
     def _get_any_missing_dependencies_in_user_specified_order(
         self,
         not_explicitly_requested_dependencies: NotExplicitlyRequestedDependenciesByBaseModule,
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         """If no not explicitly requested dependency is present, all possible not present dependencies will be
         returned. If there is one dependency per rule subject, an empty list will be returned.
         """
-        dependencies = []
-
         if any(
             len(not_explicitly_requested_dependencies_of_module) > 0
             for not_explicitly_requested_dependencies_of_module in not_explicitly_requested_dependencies.values()
         ):
             return set()
 
-        self._append_missing_dependencies(
-            dependencies, not_explicitly_requested_dependencies
+        dependencies = self._append_missing_dependencies(
+            not_explicitly_requested_dependencies
         )
 
         return {
             self._get_rule_subject_and_object_in_user_specified_order(dependency)
             for dependency in dependencies
         }
 
     def _append_missing_dependencies(
         self,
-        dependencies: List[StrictDependency],
         not_explicitly_requested_dependencies: NotExplicitlyRequestedDependenciesByBaseModule,
-    ) -> None:
+    ) -> List[Dependency]:
+        dependencies = []
+
         for (
             module_with_missing_dependencies
         ) in not_explicitly_requested_dependencies.keys():
             if self._module_requirement.rule_specified_with_importer_as_rule_subject:
-                for (
-                    other_module
-                ) in self._module_requirement.importees_as_specified_by_user:
+                for other_module in self._get_importee_modules_as_specified_by_user():
                     dependencies.append(
                         (module_with_missing_dependencies, other_module)
                     )
             else:
-                for (
-                    other_module
-                ) in self._module_requirement.importees_as_specified_by_user:
+                for other_module in self._get_importee_modules_as_specified_by_user():
                     dependencies.append(
                         (other_module, module_with_missing_dependencies)
                     )
 
+        return dependencies
+
     def _group_explicitly_requested_dependencies_by_layers(
         self,
         explicitly_requested_dependencies: ExplicitlyRequestedDependenciesByBaseModules,
     ) -> Dict[Layer, ExplicitlyRequestedDependenciesByBaseModules]:
         result = defaultdict(dict)
 
         for (
@@ -266,33 +261,39 @@
             )
             layer = self._get_layer_for_module(relevant_module_for_layer)
 
             result[layer][abstract_dependency] = concrete_dependencies
 
         return result
 
-    def _get_module_relevant_for_layer(self, dependency: StrictDependency) -> Module:
+    def _get_module_relevant_for_layer(self, dependency: Dependency) -> Module:
         if self._module_requirement.rule_specified_with_importer_as_rule_subject:
             return dependency[1]
 
         return dependency[0]
 
     def _get_layer_for_module(self, module: Module) -> Layer:
-        return self._layer_to_module_mapping.get_layer(module)
+        return self._layer_to_module_mapping.get_layer_for_module_name(module.name)
 
     def _get_realised_dependencies(
-        self, explicitly_requested_dependencies: Dict[Any, List[StrictDependency]]
-    ) -> Set[StrictDependency]:
+        self, explicitly_requested_dependencies: Dict[Any, List[Dependency]]
+    ) -> Set[Dependency]:
         """Removes all dependencies between modules of the same layer, as these are one logical unit."""
         violating_dependencies = super()._get_realised_dependencies(
             explicitly_requested_dependencies
         )
 
         violating_dependencies_in_different_layers = set()
         for dependency in violating_dependencies:
-            rule_subject_layer = self._layer_to_module_mapping.get_layer(dependency[0])
-            rule_object_layer = self._layer_to_module_mapping.get_layer(dependency[1])
+            rule_subject_layer = (
+                self._layer_to_module_mapping.get_layer_for_module_name(
+                    dependency[0].name
+                )
+            )
+            rule_object_layer = self._layer_to_module_mapping.get_layer_for_module_name(
+                dependency[1].name
+            )
 
             if rule_subject_layer != rule_object_layer:
                 violating_dependencies_in_different_layers.add(dependency)
 
         return violating_dependencies_in_different_layers
```

### Comparing `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/module_requirement.py` & `pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/module_requirement.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import List
 
-from pytestarch.eval_structure.evaluable_architecture import Module
+from pytestarch.eval_structure.evaluable_architecture import ModuleFilter
 
 
 class ModuleRequirement:
     """Stores information about which module is supposed to be checked against which module."""
 
     def __init__(
         self,
-        importers: List[Module],
-        importees: List[Module],
+        importers: List[ModuleFilter],
+        importees: List[ModuleFilter],
         importer_specified_as_rule_subject: bool,
     ) -> None:
         self._importer_as_specified_by_user = importers
         self._importees_as_specified_by_user = importees
 
         self._importers = importers
         self._importees = importees
@@ -25,27 +25,27 @@
         if self.rule_specified_with_importer_as_rule_object:
             self._importers, self._importees = (
                 self._importees,
                 self._importers,
             )
 
     @property
-    def importers(self) -> List[Module]:
+    def importers(self) -> List[ModuleFilter]:
         return self._importers
 
     @property
-    def importees(self) -> List[Module]:
+    def importees(self) -> List[ModuleFilter]:
         return self._importees
 
     @property
-    def importers_as_specified_by_user(self) -> list[Module]:
+    def importers_as_specified_by_user(self) -> list[ModuleFilter]:
         return self._importer_as_specified_by_user
 
     @property
-    def importees_as_specified_by_user(self) -> List[Module]:
+    def importees_as_specified_by_user(self) -> List[ModuleFilter]:
         return self._importees_as_specified_by_user
 
     @property
     def rule_specified_with_importer_as_rule_object(self) -> bool:
         # True if rule is of format "is imported by"
         return not self._importer_specified_as_rule_subject
```

### Comparing `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_matcher.py` & `pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/rule_matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,26 +152,28 @@
         self._updated_module_requirement = ModuleRequirement(
             converted_importers,
             converted_importees,
             self._module_requirement.rule_specified_with_importer_as_rule_subject,
         )
 
     def _create_module_name_regex_conversion_mapping(self) -> Dict[str, List[Module]]:
+        """Maps between a regex and the actual modules it represents."""
+
         result = {
             key: values for key, values in self._conversion_mapping_importers.items()
         }
 
         for key, values in self._conversion_mapping_importees.items():
             if key not in result:
                 result[key] = values
             else:
                 existing_values = set(result[key])
                 existing_values.update(set(values))
 
-                result[key] = list[existing_values]
+                result[key] = list(existing_values)
 
         return result
 
 
 class DefaultRuleMatcher(RuleMatcher):
     """To be used for rules that operate on modules, such as "module X should not import module Y."""
 
@@ -244,15 +246,15 @@
     @classmethod
     def _replace_regex_specified_modules_with_actual_modules(
         cls,
         layer: Layer,
         layer_mapping: LayerMapping,
         module_name_conversion_mapping: Dict[str, List[Module]],
     ) -> List[Module]:
-        modules_potentially_with_regexes = layer_mapping.get_modules(layer)
+        modules_potentially_with_regexes = layer_mapping.get_module_filters(layer)
 
         result = []
         for module in modules_potentially_with_regexes:
             if not module.regex:
                 result.append(module)
 
             else:
```

### Comparing `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py` & `pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/rule_violation_detector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Set
 
 from pytestarch.eval_structure.evaluable_architecture import (
+    Dependency,
     ExplicitlyRequestedDependenciesByBaseModules,
     NotExplicitlyRequestedDependenciesByBaseModule,
-    StrictDependency,
 )
+from pytestarch.eval_structure.utils import filter_to_module
 from pytestarch.rule_assessment.rule_check.behavior_requirement import (
     BehaviorRequirement,
 )
 from pytestarch.rule_assessment.rule_check.module_requirement import ModuleRequirement
 from pytestarch.rule_assessment.rule_check.rule_violations import RuleViolations
 
 
@@ -95,90 +96,90 @@
     @abstractmethod
     def _should_not_requirement_violations(
         self,
         explicitly_requested_dependencies_should_not_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     @abstractmethod
     def _should_requirement_violations(
         self,
         explicitly_requested_dependencies_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     @abstractmethod
     def _should_only_requirement_violations_by_no_import(
         self,
         explicitly_requested_dependencies_and_no_other_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     @abstractmethod
     def _should_only_requirement_violations_by_not_explicitly_requested_dependency(
         self,
         explicitly_requested_dependencies_and_no_other_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     @abstractmethod
     def _should_except_requirement_violations(
         self,
         at_least_one_not_explicitly_requested_dependency_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     @abstractmethod
     def _should_only_except_requirement_violations_due_to_no_other_imports(
         self,
         explicitly_requested_dependency_should_not_but_others_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     @abstractmethod
     def _should_only_except_requirement_violations_due_to_explicit_dependency_present(
         self,
         explicitly_requested_dependency_should_not_but_others_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     @abstractmethod
     def _should_not_except_requirement_violations(
         self,
         not_explicitly_requested_dependencies_should_not_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         pass
 
     def _get_realised_dependencies(
-        self, explicitly_requested_dependencies: Dict[Any, List[StrictDependency]]
-    ) -> Set[StrictDependency]:
+        self, explicitly_requested_dependencies: Dict[Any, List[Dependency]]
+    ) -> Set[Dependency]:
         violating_dependencies = explicitly_requested_dependencies.values()
 
         violating_dependencies_in_user_specified_rule_subject_object_order = set()
         for dependencies in violating_dependencies:
             for dependency in dependencies:
                 dependency_in_user_specified_order = (
                     self._get_rule_subject_and_object_in_user_specified_order(
@@ -189,16 +190,16 @@
                 violating_dependencies_in_user_specified_rule_subject_object_order.add(
                     dependency_in_user_specified_order
                 )
 
         return violating_dependencies_in_user_specified_rule_subject_object_order
 
     def _get_rule_subject_and_object_in_user_specified_order(
-        self, dependency: StrictDependency
-    ) -> StrictDependency:
+        self, dependency: Dependency
+    ) -> Dependency:
         if self._module_requirement.rule_specified_with_importer_as_rule_subject:
             return dependency
 
         return dependency[1], dependency[0]
 
     def _get_dependency_expectations(self) -> DependencyExpectation:
         return DependencyExpectation(
@@ -224,55 +225,61 @@
             ),
             explicitly_requested_dependencies_should_be_present=(
                 self._behavior_requirement.should
                 and not self._behavior_requirement.behavior_exception
             ),
         )
 
+    def _get_importee_modules_as_specified_by_user(self):
+        return [
+            filter_to_module(filter)
+            for filter in self._module_requirement.importees_as_specified_by_user
+        ]
+
 
 class RuleViolationDetector(RuleViolationBaseDetector):
     """Based on the behavior requirement and the dependencies that have actually been (not) found in the graph,
     this class decides whether any of the requirements have been violated and how.
 
     ExplicitlyRequestedDependenciesByBaseModules follow this structure:
     {(requested dependency, e.g. from A to B): [list of dependencies found that qualifiy as the requested dependency, e.g. A.a1 imports B, A.a2 imports B]}
 
     NotExplicitlyRequestedDependenciesByBaseModule on the other hand are structured like this:
     {Module for which not explicitly requested dependencies (either from or to this module) were found: [list of such dependencies]}.
 
-    The output is a rule violation object which for each type of rule contains a list of (rule subject, rule object) which violate the rule. These are ordered according
+    The output is a rule violation object which for each type of rule contains a list of (rule subject, rule object) modules which violate the rule. These are ordered according
     to the order the user used when specifying the rule, i.e. the rule subject is the original rule subject no matter if the rule is an import
     or be imported rule.
 
-    If multiple rule subjects have been specified, the rule needs to apply to each and every one of them in order not
+    If multiple rule subjects have been specified, the rule needs to apply to each one of them in order not
     to count as being violated.
     """
 
     def _should_not_requirement_violations(
         self,
         explicitly_requested_dependencies_should_not_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_should_not_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(explicitly_requested_dependencies)
 
     def _should_requirement_violations(
         self,
         explicitly_requested_dependencies_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_should_be_present
         ):
             return set()
 
         return self._get_abstract_dependencies_without_realisations(
@@ -281,15 +288,15 @@
 
     def _should_only_requirement_violations_by_no_import(
         self,
         explicitly_requested_dependencies_and_no_other_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_and_no_other_should_be_present
         ):
             return set()
 
         return self._get_abstract_dependencies_without_realisations(
@@ -298,30 +305,30 @@
 
     def _should_only_requirement_violations_by_not_explicitly_requested_dependency(
         self,
         explicitly_requested_dependencies_and_no_other_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not explicitly_requested_dependencies_and_no_other_should_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(not_explicitly_requested_dependencies)
 
     def _should_except_requirement_violations(
         self,
         at_least_one_not_explicitly_requested_dependency_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not at_least_one_not_explicitly_requested_dependency_should_be_present
         ):
             return set()
 
         return self._get_missing_dependencies_in_user_specified_order(
@@ -330,15 +337,15 @@
 
     def _should_only_except_requirement_violations_due_to_no_other_imports(
         self,
         explicitly_requested_dependency_should_not_but_others_should_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not explicitly_requested_dependency_should_not_but_others_should_be_present
         ):
             return set()
 
         return self._get_missing_dependencies_in_user_specified_order(
@@ -347,75 +354,71 @@
 
     def _should_only_except_requirement_violations_due_to_explicit_dependency_present(
         self,
         explicitly_requested_dependency_should_not_but_others_should_be_present: bool,
         explicitly_requested_dependencies: Optional[
             ExplicitlyRequestedDependenciesByBaseModules
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             explicitly_requested_dependencies is None
             or not explicitly_requested_dependency_should_not_but_others_should_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(explicitly_requested_dependencies)
 
     def _should_not_except_requirement_violations(
         self,
         not_explicitly_requested_dependencies_should_not_be_present: bool,
         not_explicitly_requested_dependencies: Optional[
             NotExplicitlyRequestedDependenciesByBaseModule
         ],
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         if (
             not_explicitly_requested_dependencies is None
             or not not_explicitly_requested_dependencies_should_not_be_present
         ):
             return set()
 
         return self._get_realised_dependencies(not_explicitly_requested_dependencies)
 
     def _get_abstract_dependencies_without_realisations(
-        self, explicitly_requested_dependencies: Dict[Any, List[StrictDependency]]
-    ) -> Set[StrictDependency]:
+        self, explicitly_requested_dependencies: Dict[Any, List[Dependency]]
+    ) -> Set[Dependency]:
         violating_dependencies = [
             abstract_dependency
             for abstract_dependency, concrete_dependency in explicitly_requested_dependencies.items()
             if len(concrete_dependency) == 0
         ]
         return {
             self._get_rule_subject_and_object_in_user_specified_order(dependency)
             for dependency in violating_dependencies
         }
 
     def _get_missing_dependencies_in_user_specified_order(
         self,
         not_explicitly_requested_dependencies: NotExplicitlyRequestedDependenciesByBaseModule,
-    ) -> Set[StrictDependency]:
+    ) -> Set[Dependency]:
         dependencies = []
 
         for (
             module_with_missing_dependencies,
             not_explicitly_requested_dependencies_of_module,
         ) in not_explicitly_requested_dependencies.items():
             if len(not_explicitly_requested_dependencies_of_module) > 0:
                 continue
 
             if self._module_requirement.rule_specified_with_importer_as_rule_subject:
-                for (
-                    other_module
-                ) in self._module_requirement.importees_as_specified_by_user:
+                for other_module in self._get_importee_modules_as_specified_by_user():
                     dependencies.append(
                         (module_with_missing_dependencies, other_module)
                     )
             else:
-                for (
-                    other_module
-                ) in self._module_requirement.importees_as_specified_by_user:
+                for other_module in self._get_importee_modules_as_specified_by_user():
                     dependencies.append(
                         (other_module, module_with_missing_dependencies)
                     )
 
         return {
             self._get_rule_subject_and_object_in_user_specified_order(dependency)
             for dependency in dependencies
```

### Comparing `pytestarch-1.4.1/src/pytestarch/rule_assessment/rule_check/rule_violations.py` & `pytestarch-1.5.0/src/pytestarch/rule_assessment/rule_check/rule_violations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, fields
 from typing import Set
 
-from pytestarch.eval_structure.evaluable_architecture import StrictDependency
+from pytestarch.eval_structure.evaluable_architecture import Dependency
 
 
 @dataclass
 class RuleViolations:
-    should_violations: Set[StrictDependency]
-    should_only_violations_by_forbidden_import: Set[StrictDependency]
-    should_only_violations_by_no_import: Set[StrictDependency]
-    should_not_violations: Set[StrictDependency]
-    should_except_violations: Set[StrictDependency]
-    should_only_except_violations_by_forbidden_import: Set[StrictDependency]
-    should_only_except_violations_by_no_import: Set[StrictDependency]
-    should_not_except_violations: Set[StrictDependency]
+    should_violations: Set[Dependency]
+    should_only_violations_by_forbidden_import: Set[Dependency]
+    should_only_violations_by_no_import: Set[Dependency]
+    should_not_violations: Set[Dependency]
+    should_except_violations: Set[Dependency]
+    should_only_except_violations_by_forbidden_import: Set[Dependency]
+    should_only_except_violations_by_no_import: Set[Dependency]
+    should_not_except_violations: Set[Dependency]
 
     def __bool__(self) -> bool:
         return any(self.__dict__[field.name] for field in fields(self))
```

### Comparing `pytestarch-1.4.1/src/pytestarch/utils/decorators.py` & `pytestarch-1.5.0/src/pytestarch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/src/pytestarch/utils/partial_match_to_regex_converter.py` & `pytestarch-1.5.0/src/pytestarch/utils/partial_match_to_regex_converter.py`

 * *Files identical despite different names*

### Comparing `pytestarch-1.4.1/setup.py` & `pytestarch-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 {'': ['*']}
 
 install_requires = \
 ['b2>=3.7.1,<4.0.0', 'matplotlib>=3.5.3,<4.0.0', 'networkx>=3.0,<4.0']
 
 setup_kwargs = {
     'name': 'pytestarch',
-    'version': '1.4.1',
+    'version': '1.5.0',
     'description': 'Test framework for software architecture based on imports between modules',
-    'long_description': '# Welcome to PyTestArch\n\nPyTestArch is an open source library that allows users to define architectural rules and test their code against them. It is \ngenerally inspired by [ArchUnit](https://www.archunit.org/).\n\n## Installation Guide\nPyTestArch is available via [PyPI](https://pypi.org/project/pytestarch/) and can be installed e.g. via pip: `pip install pytestarch`.\n\n## Usage Guide\nThree steps are required to test an architectural rule:\n\n1) Create an evaluable representation of the source code you want to test\n\n```\nfrom pytestarch import get_evaluable_architecture\n\nevaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")\n```\nThis will scan all python files under /home/dummy/project/src for imports and build an internal representation that can\nlater be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external \ndependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),\nyou could use a fixture for this evaluable object.\n\n2) Define an architectural rule\n```\nfrom pytestarch import Rule\n\nrule = Rule() \\\n        .modules_that() \\\n        .are_named("src.moduleB") \\\n        .should_not() \\\n        .be_imported_by_modules_that() \\\n        .are_sub_modules_of("src.moduleA") \\\n```\n\nThis rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module\nthat is a submodule of "src.moduleA", excluding "src.moduleA" itself.\n\n3) Evaluate your code against this rule\n\n```\nrule.assert_applies(evaluable)\n```\nThat\'s it!\n',
+    'long_description': '# Welcome to PyTestArch\n\nPyTestArch is an open source library that allows users to define architectural rules and test their code against them. It is \ngenerally inspired by [ArchUnit](https://www.archunit.org/).\n\n## Installation Guide\nPyTestArch is available via [PyPI](https://pypi.org/project/pytestarch/) and can be installed e.g. via pip: `pip install pytestarch`.\n\n## Usage Guide\nThree steps are required to test an architectural rule:\n\n1) Create an evaluable representation of the source code you want to test\n\n```\nfrom pytestarch import get_evaluable_architecture\n\nevaluable = get_evaluable_architecture("/home/dummy/project", "/home/dummy/project/src")\n```\nThis will scan all python files under /home/dummy/project/src for imports and build an internal representation that can\nlater be queried. The first parameter /home/dummy/project helps PyTestArch to differentiate between internal and external \ndependencies. This evaluable can be used for multiple architectural rule checks; if you are using [pytest](https://docs.pytest.org/en/7.1.x/),\nyou could use a fixture for this evaluable object.\n\n2) Define an architectural rule\n```\nfrom pytestarch import Rule\n\nrule = Rule() \\\n        .modules_that() \\\n        .are_named("src.moduleB") \\\n        .should_not() \\\n        .be_imported_by_modules_that() \\\n        .are_sub_modules_of("src.moduleA") \n```\n\nThis rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module\nthat is a submodule of "src.moduleA", excluding "src.moduleA" itself.\n\n3) Evaluate your code against this rule\n\n```\nrule.assert_applies(evaluable)\n```\nThat\'s it!\n',
     'author': 'zyskarch',
     'author_email': 'zyskarch@gmail.com',
     'maintainer': 'zyskarch',
     'maintainer_email': 'zyskarch@gmail.com',
     'url': 'https://github.com/zyskarch/pytestarch',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pytestarch-1.4.1/PKG-INFO` & `pytestarch-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestarch
-Version: 1.4.1
+Version: 1.5.0
 Summary: Test framework for software architecture based on imports between modules
 Home-page: https://github.com/zyskarch/pytestarch
 License: Apache-2.0
 Keywords: architecture,test
 Author: zyskarch
 Author-email: zyskarch@gmail.com
 Maintainer: zyskarch
@@ -60,15 +60,15 @@
 from pytestarch import Rule
 
 rule = Rule() \
         .modules_that() \
         .are_named("src.moduleB") \
         .should_not() \
         .be_imported_by_modules_that() \
-        .are_sub_modules_of("src.moduleA") \
+        .are_sub_modules_of("src.moduleA") 
 ```
 
 This rule represents the architectural requirements that a module named "src.moduleB" should not be imported by any module
 that is a submodule of "src.moduleA", excluding "src.moduleA" itself.
 
 3) Evaluate your code against this rule
```

