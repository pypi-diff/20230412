# Comparing `tmp/macrometa-target-collection-0.0.49.tar.gz` & `tmp/macrometa-target-collection-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.49.tar", last modified: Wed Apr 12 15:15:23 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.50.tar", last modified: Wed Apr 12 16:23:47 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.49.tar` & `macrometa-target-collection-0.0.50.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:23.051548 macrometa-target-collection-0.0.49/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 15:14:57.000000 macrometa-target-collection-0.0.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 15:15:23.051548 macrometa-target-collection-0.0.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 15:14:57.000000 macrometa-target-collection-0.0.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:23.051548 macrometa-target-collection-0.0.49/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 15:14:57.000000 macrometa-target-collection-0.0.49/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13116 2023-04-12 15:14:57.000000 macrometa-target-collection-0.0.49/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:15:23.051548 macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 15:15:23.000000 macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 15:15:23.000000 macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:15:23.000000 macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 15:15:23.000000 macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 15:15:23.000000 macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 15:15:23.000000 macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 15:14:57.000000 macrometa-target-collection-0.0.49/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 15:15:23.051548 macrometa-target-collection-0.0.49/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:23:47.259015 macrometa-target-collection-0.0.50/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 16:23:47.263015 macrometa-target-collection-0.0.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:23:47.259015 macrometa-target-collection-0.0.50/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13371 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:23:47.259015 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 16:23:47.263015 macrometa-target-collection-0.0.50/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.49/LICENSE` & `macrometa-target-collection-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.49/PKG-INFO` & `macrometa-target-collection-0.0.50/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.49
+Version: 0.0.50
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.49/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.50/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.49/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.50/macrometa_target_collection/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,38 +83,45 @@
         sys.stdout.flush()
 
 
 def try_upsert(collection: StandardCollection, record_batch: RecordBatch, force=False):
     if record_batch.length() >= record_batch.max_batch_size or force:
         to_insert = record_batch.flush()
         to_update = []
-        for i, r in enumerate(collection.insert_many(to_insert)):
+        records_array = remove_time_extracted(to_insert)
+
+        for i, r in enumerate(collection.insert_many(records_array)):
             if type(r) is DocumentInsertError:
                 to_update.append(to_insert[i])
             else:
                 # Update ingested_documents and ingested_bytes metrics
                 ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
                 # Update ingest_lag metric
                 diff = datetime.utcnow() - datetime.strptime(to_insert[i]["time_extracted"], "%Y-%m-%dT%H:%M:%S.%fZ")
                 ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
 
         if len(to_update) > 0:
-            for i, r in enumerate(collection.update_many(to_update)):
+            records_array = remove_time_extracted(to_update)
+            for i, r in enumerate(collection.update_many(records_array)):
                 if type(r) is DocumentInsertError:
                     # Increment ingest_errors metric
                     ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     print(f'Failed to insert/update record: {to_update[i]}. {r}')
                 else:
                     # Update ingest_lag metric
                     diff = datetime.utcnow() - datetime.strptime(to_update[i]["time_extracted"], "%Y-%m-%dT%H:%M:%S.%fZ")
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
         record_batch.last_executed_time = utils.now()
 
 
+def remove_time_extracted(records):
+    return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
+
+
 def try_delete(collection: StandardCollection, _key: str):
     try:
         collection.delete(_key)
     except Exception as e:
         # Increment ingest_errors metric
         ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         logger.warn(f'Failed to delete record with _key: {_key}. {e}')
@@ -277,15 +284,15 @@
     event_loop = setup_batch_task(collection, record_batch)
     input_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
     state = persist_messages(collection, input_messages, record_batch)
 
     # There can still be records in the `record_batch` which is not processed,
     # So, we have to force process it one last time before the workflow terminates.
     try_upsert(collection, record_batch, force=True)
-    
+
     # Wait for Prometheus to scrape the metrics
     logger.info("Waiting for metrics scrape...")
     while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total", f"workflow=\"{workflow_label}\""):
         time.sleep(15)
     logger.info("Metrics scrape complete. Exiting...")
 
     emit_state(state)
```

### Comparing `macrometa-target-collection-0.0.49/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.49
+Version: 0.0.50
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.49/pyproject.toml` & `macrometa-target-collection-0.0.50/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.49"
+version = "0.0.50"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

