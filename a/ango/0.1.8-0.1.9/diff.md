# Comparing `tmp/ango-0.1.8-py3-none-any.whl.zip` & `tmp/ango-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8521 bytes, number of entries: 10
+Zip file size: 8526 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-23 13:16 ango/__init__.py
 -rw-rw-r--  2.0 unx     1304 b- defN 23-Jan-23 13:16 ango/plugin_logger.py
 -rw-rw-r--  2.0 unx     4419 b- defN 23-Jan-23 13:16 ango/plugins.py
--rw-rw-r--  2.0 unx    14478 b- defN 23-Jan-25 11:31 ango/sdk.py
+-rw-rw-r--  2.0 unx    14516 b- defN 23-Jan-25 12:56 ango/sdk.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-23 13:16 ango/models/__init__.py
 -rw-rw-r--  2.0 unx     5421 b- defN 23-Jan-23 13:16 ango/models/label_category.py
--rw-rw-r--  2.0 unx     1909 b- defN 23-Jan-25 11:50 ango-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jan-25 11:50 ango-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jan-25 11:50 ango-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      737 b- defN 23-Jan-25 11:50 ango-0.1.8.dist-info/RECORD
-10 files, 28365 bytes uncompressed, 7277 bytes compressed:  74.3%
+-rw-rw-r--  2.0 unx     1909 b- defN 23-Jan-25 12:57 ango-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jan-25 12:57 ango-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jan-25 12:57 ango-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      737 b- defN 23-Jan-25 12:57 ango-0.1.9.dist-info/RECORD
+10 files, 28403 bytes uncompressed, 7282 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: ango/models/__init__.py
 Comment: 
 
 Filename: ango/models/label_category.py
 Comment: 
 
-Filename: ango-0.1.8.dist-info/METADATA
+Filename: ango-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: ango-0.1.8.dist-info/WHEEL
+Filename: ango-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: ango-0.1.8.dist-info/top_level.txt
+Filename: ango-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ango-0.1.8.dist-info/RECORD
+Filename: ango-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ango/sdk.py

```diff
@@ -154,15 +154,15 @@
         integration_exists = False
         for t1 in integrations_list:
             if id in t1 and t1[id] == integration_id:
                 integration_exists = True
         return integration_exists
 
     def upload_files(self, project_id: str, file_paths: List, integration_id: str = None, batches: List[str] = None):
-        if not self.__check_integration(project_id, integration_id):
+        if integration_id and not self.__check_integration(project_id, integration_id):
             raise "Integration ID is Invalid!"
         assets = []
         for path in tqdm(file_paths):
             uid = uuid.uuid4().hex
             data = ""
             external_id = ""
             if isinstance(path, str):
@@ -191,15 +191,15 @@
             'apikey': self.api_key
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
         return response.json()
 
     def upload_files_cloud(self, project_id: str, assets, integration_id: str = None, batches: List[str] = None):
-        if not self.__check_integration(project_id, integration_id):
+        if integration_id and not self.__check_integration(project_id, integration_id):
             raise "Integration ID is Invalid!"
         url = "%s/v2/project/%s/cloud" % (self.host, project_id)
         if batches:
             tags = self.__getTags(project_id, batches)
             url += "?tags=%s" % json.dumps(tags)
 
         if integration_id:
```

## Comparing `ango-0.1.8.dist-info/METADATA` & `ango-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

