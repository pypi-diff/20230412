# Comparing `tmp/tvault-0.3.4-py3-none-any.whl.zip` & `tmp/tvault-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10358 bytes, number of entries: 11
--rw-r--r--  2.0 unx     2977 b- defN 23-Apr-12 04:48 tvault/__init__.py
+Zip file size: 10359 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     2981 b- defN 23-Apr-12 04:50 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     8055 b- defN 23-Apr-11 08:27 tvault/parse_utils.py
 -rw-r--r--  2.0 unx    14094 b- defN 23-Apr-12 04:43 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-12 04:48 tvault-0.3.4.dist-info/RECORD
-11 files, 32368 bytes uncompressed, 8918 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-12 04:50 tvault-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-12 04:50 tvault-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 04:50 tvault-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-12 04:50 tvault-0.3.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-12 04:50 tvault-0.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-12 04:50 tvault-0.3.5.dist-info/RECORD
+11 files, 32372 bytes uncompressed, 8919 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.3.4.dist-info/LICENSE
+Filename: tvault-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.3.4.dist-info/METADATA
+Filename: tvault-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.3.4.dist-info/WHEEL
+Filename: tvault-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.3.4.dist-info/entry_points.txt
+Filename: tvault-0.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: tvault-0.3.4.dist-info/top_level.txt
+Filename: tvault-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.3.4.dist-info/RECORD
+Filename: tvault-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/__init__.py

```diff
@@ -35,15 +35,15 @@
 
 def add_result(result=0, sha="", log_dir="./model_log"):
     vault = TorchVault(log_dir)
     vault.add_result(sha, result)
 
 
 # tags should be a dictionary of key, value pairs
-def log_all(model, tags="", result=-1, optimizer=None, log_dir="./model_log", model_dir="./"):
+def log_all(model, tags=dict(), result=-1, optimizer=None, log_dir="./model_log", model_dir="./"):
     vault = TorchVault(log_dir, model_dir)
     vault.log_model(model)
     if optimizer is not None:
         vault.log_optimizer(optimizer)
     for tag_type, tag in tags.items():
         vault.add_tag("", tag_type, tag)
     if result is not -1:
```

## Comparing `tvault-0.3.4.dist-info/LICENSE` & `tvault-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

