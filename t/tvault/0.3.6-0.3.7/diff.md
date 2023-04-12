# Comparing `tmp/tvault-0.3.6-py3-none-any.whl.zip` & `tmp/tvault-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10364 bytes, number of entries: 11
+Zip file size: 10385 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     2981 b- defN 23-Apr-12 04:50 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     8055 b- defN 23-Apr-11 08:27 tvault/parse_utils.py
--rw-r--r--  2.0 unx    14096 b- defN 23-Apr-12 06:30 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-12 06:30 tvault-0.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-12 06:30 tvault-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 06:30 tvault-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-12 06:30 tvault-0.3.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 06:30 tvault-0.3.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-12 06:30 tvault-0.3.6.dist-info/RECORD
-11 files, 32374 bytes uncompressed, 8924 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx    14234 b- defN 23-Apr-12 06:33 tvault/torchvault.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-12 06:33 tvault-0.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-12 06:33 tvault-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 06:33 tvault-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-12 06:33 tvault-0.3.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 06:33 tvault-0.3.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-12 06:33 tvault-0.3.7.dist-info/RECORD
+11 files, 32512 bytes uncompressed, 8945 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.3.6.dist-info/LICENSE
+Filename: tvault-0.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.3.6.dist-info/METADATA
+Filename: tvault-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.3.6.dist-info/WHEEL
+Filename: tvault-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.3.6.dist-info/entry_points.txt
+Filename: tvault-0.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: tvault-0.3.6.dist-info/top_level.txt
+Filename: tvault-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.3.6.dist-info/RECORD
+Filename: tvault-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/torchvault.py

```diff
@@ -346,23 +346,26 @@
         # find model log with most tags.
         table = []
         for e in target_models:
             if len(list(e.keys())) > len(table):
                 table = list(e.keys())
 
         # table should be sorted here
+        sorted_table_out = ["HASH", "MODEL-IDX"]
         sorted_table = ["HASH", "MODEL-IDX"]
         for e in table:
             if e.startswith("tag-"):
-                sorted_table.append(e.split("tag-")[1])
+                sorted_table_out.append(e.split("tag-")[1])
+                sorted_table.append(e)
         sorted_table.append("RESULT")
+        sorted_table_out.append("RESULT")
 
         # table contains model_log keys with most tags
         # should represent [hash, model idx, tag1, tag2, tag3, result] order.
-        tab = PrettyTable(sorted_table)
+        tab = PrettyTable(sorted_table_out)
         for e in target_models:
             row = []
             for k in sorted_table:
                 if k in e.keys():
                     row.append(e[k])
                 else:
                     row.append("")
```

## Comparing `tvault-0.3.6.dist-info/LICENSE` & `tvault-0.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tvault-0.3.6.dist-info/RECORD` & `tvault-0.3.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 tvault/__init__.py,sha256=TVz2_IMPP6K1W2KqqPjHxLze_PoVvz2yTPZRQJ_8UDg,2981
 tvault/model_diff.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tvault/model_log.py,sha256=ZD1LeL1wBRKQEZaAfZEcjYP7w76yeD0eMRAnI-fBOiA,4789
 tvault/parse_utils.py,sha256=rxESYl0qdIlmi4xFQo7G7IPI4sofHOXBduYjibFb50o,8055
-tvault/torchvault.py,sha256=57HW3nq-1F2gSYcP5sXkgyOYXX-UoJ7rzWAGMBeFqcM,14096
-tvault-0.3.6.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
-tvault-0.3.6.dist-info/METADATA,sha256=UQ8wWfCQhJTggjSyYZdYkuZLCCQ-yZlcJDLhQdImjYk,380
-tvault-0.3.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-tvault-0.3.6.dist-info/entry_points.txt,sha256=wdQKlmNgZH12ukkn44_90k6m4AgiW-MzRTo14Cf2RSc,53
-tvault-0.3.6.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
-tvault-0.3.6.dist-info/RECORD,,
+tvault/torchvault.py,sha256=PbYFE_sunNO-sJRYIZyDW2zrKZy9M9G6xwRfdfZYv1U,14234
+tvault-0.3.7.dist-info/LICENSE,sha256=WMAFuHtOPuSTgn-WJtxM1LLEDLfqaKQes7X7VhOaaOU,1067
+tvault-0.3.7.dist-info/METADATA,sha256=OPy8i2jYU-U7Rr0sVDYoaKpQtySBj5Nt2PBYkUUNQnc,380
+tvault-0.3.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+tvault-0.3.7.dist-info/entry_points.txt,sha256=wdQKlmNgZH12ukkn44_90k6m4AgiW-MzRTo14Cf2RSc,53
+tvault-0.3.7.dist-info/top_level.txt,sha256=Z1ZnwpooKsyvyYmlAXuGVOIRK1hO7QkkDVaneY85JDI,7
+tvault-0.3.7.dist-info/RECORD,,
```

