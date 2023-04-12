# Comparing `tmp/infra_flow-1.0.11-py3-none-any.whl.zip` & `tmp/infra_flow-1.0.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3246 bytes, number of entries: 9
+Zip file size: 3212 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 08:03 infra_enver/__init__.py
--rw-r--r--  2.0 unx      319 b- defN 23-Apr-11 13:06 infra_enver/cache.py
+-rw-r--r--  2.0 unx      249 b- defN 23-Apr-12 12:10 infra_enver/cache.py
 -rw-r--r--  2.0 unx       75 b- defN 23-Apr-11 13:02 infra_enver/config.py
 -rw-r--r--  2.0 unx     2556 b- defN 23-Apr-11 13:06 infra_enver/infra_enver.py
 -rw-r--r--  2.0 unx       47 b- defN 23-Apr-11 08:03 infra_enver/infra_enver_exceptions.py
--rw-r--r--  2.0 unx      597 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      717 b- defN 23-Apr-11 13:10 infra_flow-1.0.11.dist-info/RECORD
-9 files, 4415 bytes uncompressed, 1998 bytes compressed:  54.7%
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-12 12:12 infra_flow-1.0.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:12 infra_flow-1.0.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-12 12:12 infra_flow-1.0.12.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      717 b- defN 23-Apr-12 12:12 infra_flow-1.0.12.dist-info/RECORD
+9 files, 4345 bytes uncompressed, 1964 bytes compressed:  54.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: infra_enver/infra_enver.py
 Comment: 
 
 Filename: infra_enver/infra_enver_exceptions.py
 Comment: 
 
-Filename: infra_flow-1.0.11.dist-info/METADATA
+Filename: infra_flow-1.0.12.dist-info/METADATA
 Comment: 
 
-Filename: infra_flow-1.0.11.dist-info/WHEEL
+Filename: infra_flow-1.0.12.dist-info/WHEEL
 Comment: 
 
-Filename: infra_flow-1.0.11.dist-info/top_level.txt
+Filename: infra_flow-1.0.12.dist-info/top_level.txt
 Comment: 
 
-Filename: infra_flow-1.0.11.dist-info/RECORD
+Filename: infra_flow-1.0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## infra_enver/cache.py

```diff
@@ -1,14 +1,11 @@
 import json
 import redis
 import typing as t
-import time
 
 
 def get_value(db: redis.Redis, key: str) -> t.Any:
-    for _ in range(10):
-        value = db.get(key)
-        if value is not None:
-            return json.loads(value.decode("utf-8"))
-        time.sleep(1)
+    value = db.get(key)
+    if value is not None:
+        return json.loads(value.decode("utf-8"))
 
     raise KeyError(f"redis key <{key}> not exists")
```

## Comparing `infra_flow-1.0.11.dist-info/METADATA` & `infra_flow-1.0.12.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infra-flow
-Version: 1.0.11
+Version: 1.0.12
 Summary: Infra Enver
 Author: Daniil Vladimirov
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pydantic
 Requires-Dist: redis
```

## Comparing `infra_flow-1.0.11.dist-info/RECORD` & `infra_flow-1.0.12.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 infra_enver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-infra_enver/cache.py,sha256=wOsmvTuabakBVhGPT21JsZw4cy0yRojAZikNBSbQNxc,319
+infra_enver/cache.py,sha256=balw5fg5SnHsFno8FqjkNeJf_3eIxq7oud3KE39cpvE,249
 infra_enver/config.py,sha256=VZWFJ-yCa5Xri7bmLm1cW4SjboRRH-1SW5Unjoubwi8,75
 infra_enver/infra_enver.py,sha256=Y62nrV9YppVg2-yOJfyrKtQeJoDGqxd9cKsxSxBgOL4,2556
 infra_enver/infra_enver_exceptions.py,sha256=wt8Xw2eIHLm74SVp4yr7etiZzPEMamngK3bL8zjaNZ0,47
-infra_flow-1.0.11.dist-info/METADATA,sha256=IW_ib8amXQhGL4VLPYuQ16mzVi9SUp6QfRYxBNMTBD4,597
-infra_flow-1.0.11.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-infra_flow-1.0.11.dist-info/top_level.txt,sha256=8z-lPdgvjFG_G_2YBOauqYB4bAV7wVa0SZBX6EU4gcU,12
-infra_flow-1.0.11.dist-info/RECORD,,
+infra_flow-1.0.12.dist-info/METADATA,sha256=HiZoP1y1mYMNq8nyiPssb8gIJ9ORFklAllsQBNdCrmM,597
+infra_flow-1.0.12.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+infra_flow-1.0.12.dist-info/top_level.txt,sha256=8z-lPdgvjFG_G_2YBOauqYB4bAV7wVa0SZBX6EU4gcU,12
+infra_flow-1.0.12.dist-info/RECORD,,
```

