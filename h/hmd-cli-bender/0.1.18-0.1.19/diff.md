# Comparing `tmp/hmd_cli_bender-0.1.18-py3-none-any.whl.zip` & `tmp/hmd_cli_bender-0.1.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5251 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Apr-12 12:54 hmd_cli_bender/__init__.py
--rw-rw-rw-  2.0 unx     3035 b- defN 23-Apr-12 12:54 hmd_cli_bender/controller.py
--rw-rw-rw-  2.0 unx     8741 b- defN 23-Apr-12 12:54 hmd_cli_bender/hmd_cli_bender.py
--rw-rw-rw-  2.0 unx     1409 b- defN 23-Apr-12 12:54 hmd_cli_bender-0.1.18.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-12 12:54 hmd_cli_bender-0.1.18.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 23-Apr-12 12:54 hmd_cli_bender-0.1.18.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      584 b- defN 23-Apr-12 12:54 hmd_cli_bender-0.1.18.dist-info/RECORD
-7 files, 13876 bytes uncompressed, 4205 bytes compressed:  69.7%
+Zip file size: 5264 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Apr-12 13:27 hmd_cli_bender/__init__.py
+-rw-rw-rw-  2.0 unx     3035 b- defN 23-Apr-12 13:27 hmd_cli_bender/controller.py
+-rw-rw-rw-  2.0 unx     8792 b- defN 23-Apr-12 13:27 hmd_cli_bender/hmd_cli_bender.py
+-rw-rw-rw-  2.0 unx     1409 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      584 b- defN 23-Apr-12 13:27 hmd_cli_bender-0.1.19.dist-info/RECORD
+7 files, 13927 bytes uncompressed, 4218 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_bender/controller.py
 Comment: 
 
 Filename: hmd_cli_bender/hmd_cli_bender.py
 Comment: 
 
-Filename: hmd_cli_bender-0.1.18.dist-info/METADATA
+Filename: hmd_cli_bender-0.1.19.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_bender-0.1.18.dist-info/WHEEL
+Filename: hmd_cli_bender-0.1.19.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_bender-0.1.18.dist-info/top_level.txt
+Filename: hmd_cli_bender-0.1.19.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_bender-0.1.18.dist-info/RECORD
+Filename: hmd_cli_bender-0.1.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_bender/hmd_cli_bender.py

```diff
@@ -43,14 +43,15 @@
                     "TRANSFORM_INSTANCE_CONTEXT": json.dumps(
                         transform_instance_context
                     ),
                     "HMD_ENVIRONMENT": environment,
                     "HMD_REGION": region,
                     "HMD_ACCOUNT": account,
                     "HMD_CUSTOMER_CODE": customer_code,
+                    "HMD_HOME": "/root/hmd_home",
                     "INCLUDE": include,
                     "TEST_SUITE": test_suite,
                     "HMD_REPO_PATH": os.path.join(repo_path, "test"),
                     "PIP_CACHE_DIR": "/root/pip_cache",
                 },
                 "volumes": [
                     {
```

## Comparing `hmd_cli_bender-0.1.18.dist-info/METADATA` & `hmd_cli_bender-0.1.19.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-bender
-Version: 0.1.18
+Version: 0.1.19
 Summary: CLI for bender transform
 Home-page: UNKNOWN
 Author: Kate Walls
 Author-email: kate.walls@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: aws-secretsmanager-caching (==1.1.1.5)
```

## Comparing `hmd_cli_bender-0.1.18.dist-info/RECORD` & `hmd_cli_bender-0.1.19.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 hmd_cli_bender/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hmd_cli_bender/controller.py,sha256=Eo50412FUTICy-y65ApoggfFZmbKqFvQTzybAr_WNys,3035
-hmd_cli_bender/hmd_cli_bender.py,sha256=cYIgAIUJ-vaHdlMVCrGTfF4fhkmQfNd_Vb8jIb_kYiU,8741
-hmd_cli_bender-0.1.18.dist-info/METADATA,sha256=eeSkPih12m2rhBd6qQs78std8bkZekqMhpPy-o4rd-c,1409
-hmd_cli_bender-0.1.18.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_cli_bender-0.1.18.dist-info/top_level.txt,sha256=OWC5szsUfz-kr4tapErLRRy-BlKVNrdTSRKhNslM16U,15
-hmd_cli_bender-0.1.18.dist-info/RECORD,,
+hmd_cli_bender/hmd_cli_bender.py,sha256=kcVCjeZqDPAW3tSSlioj25AC1WB32NWlj4H3c64XM9I,8792
+hmd_cli_bender-0.1.19.dist-info/METADATA,sha256=ry4ZRQCWjsZsuMDYv2NpS0SwdC5EaYqD_Ez2DsIeG2I,1409
+hmd_cli_bender-0.1.19.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_cli_bender-0.1.19.dist-info/top_level.txt,sha256=OWC5szsUfz-kr4tapErLRRy-BlKVNrdTSRKhNslM16U,15
+hmd_cli_bender-0.1.19.dist-info/RECORD,,
```

