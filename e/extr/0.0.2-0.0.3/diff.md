# Comparing `tmp/extr-0.0.2.tar.gz` & `tmp/extr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-0.0.2.tar", last modified: Tue Apr 11 09:40:32 2023, max compression
+gzip compressed data, was "extr-0.0.3.tar", last modified: Wed Apr 12 10:53:28 2023, max compression
```

## Comparing `extr-0.0.2.tar` & `extr-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.624062 extr-0.0.2/
--rw-rw-rw-   0        0        0     2422 2023-04-11 09:40:32.613041 extr-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1586 2023-04-11 09:38:34.000000 extr-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 09:40:32.627345 extr-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-04-11 09:40:00.000000 extr-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.482951 extr-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.556188 extr-0.0.2/src/extr/
--rw-rw-rw-   0        0        0      226 2023-04-10 13:22:29.000000 extr-0.0.2/src/extr/__init__.py
--rw-rw-rw-   0        0        0     1526 2023-04-10 13:35:41.000000 extr-0.0.2/src/extr/entities.py
--rw-rw-rw-   0        0        0      158 2023-04-08 19:56:35.000000 extr-0.0.2/src/extr/iterutils.py
--rw-rw-rw-   0        0        0     1034 2023-04-10 13:02:05.000000 extr-0.0.2/src/extr/models.py
--rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.2/src/extr/regex.py
--rw-rw-rw-   0        0        0     1166 2023-04-10 13:13:58.000000 extr-0.0.2/src/extr/relations.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:40:32.610035 extr-0.0.2/src/extr.egg-info/
--rw-rw-rw-   0        0        0     2422 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 09:40:32.000000 extr-0.0.2/src/extr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.633602 extr-0.0.3/
+-rw-rw-rw-   0        0        0     2422 2023-04-12 10:53:28.633602 extr-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1586 2023-04-11 09:38:34.000000 extr-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:53:28.654589 extr-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-04-12 10:52:32.000000 extr-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.460178 extr-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.549514 extr-0.0.3/src/extr/
+-rw-rw-rw-   0        0        0      236 2023-04-12 10:21:01.000000 extr-0.0.3/src/extr/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-04-12 10:52:20.000000 extr-0.0.3/src/extr/entities.py
+-rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.3/src/extr/iterutils.py
+-rw-rw-rw-   0        0        0     1780 2023-04-12 10:52:00.000000 extr-0.0.3/src/extr/models.py
+-rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.3/src/extr/regex.py
+-rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.3/src/extr/relations.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:53:28.625555 extr-0.0.3/src/extr.egg-info/
+-rw-rw-rw-   0        0        0     2422 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-12 10:53:28.000000 extr-0.0.3/src/extr.egg-info/top_level.txt
```

### Comparing `extr-0.0.2/PKG-INFO` & `extr-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
```

### Comparing `extr-0.0.2/README.md` & `extr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `extr-0.0.2/src/extr/entities.py` & `extr-0.0.3/src/extr/entities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from typing import List
+from typing import List, cast
 
 from .regex import RegExLabel
 from .iterutils import flatten
-from .models import Entity, EntityAnnotationResults
+from .models import Entity, EntityAnnotationResults, Location
 
 
 class EntityExtractor:
     def __init__(self, regex_labels: List[RegExLabel]) -> None:
         self._regex_labels = regex_labels
 
     def get_entities(self, text: str) -> List[Entity]:
         def handler(regex_label: RegExLabel):
             return (
-                Entity(label, match.group(), *match.span())
+                Entity(label, match.group(), Location(*match.span()))
                 for label, match in regex_label.findall(text)
             )
 
-        found_labels = sorted(
-            flatten(map(handler, self._regex_labels)),
+        ## sort descending
+        all_found_labels = sorted(
+            cast(List[Entity], flatten(map(handler, self._regex_labels))),
             key=lambda entity: (entity.end, -entity.start),
             reverse=True
         )
 
-        if len(found_labels) == 0:
+        if len(all_found_labels) == 0:
             return []
 
-        labels = found_labels[:1]
-        for curr_label in found_labels[1:]:
+        labels = all_found_labels[:1]
+        for curr_label in all_found_labels[1:]:
             prev_label = labels[-1]
-            if curr_label.start >= prev_label.start or curr_label.end > prev_label.start:
+
+            if curr_label.location.is_in(prev_label.location):
                 continue
 
             labels.append(curr_label)
 
         return labels
 
 class EntityAnnotator:
     def annotate(self, text: str, entities: List[Entity]) -> EntityAnnotationResults:
         annotated_text = text[:]
         for identifer, entity in enumerate(entities):
             entity.identifer = identifer + 1
             annotated_text = annotated_text[:entity.start] + str(entity) + annotated_text[entity.end:]
 
         return EntityAnnotationResults(text, annotated_text, entities)
-
```

### Comparing `extr-0.0.2/src/extr/regex.py` & `extr-0.0.3/src/extr/regex.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.2/src/extr/relations.py` & `extr-0.0.3/src/extr/relations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Generator
+from typing import List, Generator, cast
 
 import re
 from .regex import RegExLabel
 from .entities import EntityAnnotationResults
 from .iterutils import flatten
 from .models import Relation
 
@@ -27,8 +27,8 @@
 
         def handler(relationship_label: RegExLabel) -> Generator[Relation, None, None]:
             return (
                 create_relation(label, match)
                 for label, match in relationship_label.findall(entity_annotation_results.annotated_text)
             )
 
-        return flatten(map(handler, self._relation_labels))
+        return cast(List[Relation], flatten(map(handler, self._relation_labels)))
```

### Comparing `extr-0.0.2/src/extr.egg-info/PKG-INFO` & `extr-0.0.3/src/extr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Extr - NLP
         
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
```

