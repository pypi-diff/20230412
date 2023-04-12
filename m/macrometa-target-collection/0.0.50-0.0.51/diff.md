# Comparing `tmp/macrometa-target-collection-0.0.50.tar.gz` & `tmp/macrometa-target-collection-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.50.tar", last modified: Wed Apr 12 16:23:47 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.51.tar", last modified: Wed Apr 12 17:32:43 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.50.tar` & `macrometa-target-collection-0.0.51.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:23:47.259015 macrometa-target-collection-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 16:23:47.263015 macrometa-target-collection-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:23:47.259015 macrometa-target-collection-0.0.50/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13371 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:23:47.259015 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 16:23:47.000000 macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 16:23:18.000000 macrometa-target-collection-0.0.50/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 16:23:47.263015 macrometa-target-collection-0.0.50/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:32:43.553337 macrometa-target-collection-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 17:32:18.000000 macrometa-target-collection-0.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 17:32:43.553337 macrometa-target-collection-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 17:32:18.000000 macrometa-target-collection-0.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:32:43.553337 macrometa-target-collection-0.0.51/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 17:32:18.000000 macrometa-target-collection-0.0.51/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13435 2023-04-12 17:32:18.000000 macrometa-target-collection-0.0.51/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:32:43.553337 macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 17:32:43.000000 macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 17:32:43.000000 macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:32:43.000000 macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 17:32:43.000000 macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 17:32:43.000000 macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 17:32:43.000000 macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 17:32:18.000000 macrometa-target-collection-0.0.51/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 17:32:43.553337 macrometa-target-collection-0.0.51/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.50/LICENSE` & `macrometa-target-collection-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.50/PKG-INFO` & `macrometa-target-collection-0.0.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.50
+Version: 0.0.51
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.50/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.51/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.50/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.51/macrometa_target_collection/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,27 +93,27 @@
             if type(r) is DocumentInsertError:
                 to_update.append(to_insert[i])
             else:
                 # Update ingested_documents and ingested_bytes metrics
                 ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
                 # Update ingest_lag metric
-                diff = datetime.utcnow() - datetime.strptime(to_insert[i]["time_extracted"], "%Y-%m-%dT%H:%M:%S.%fZ")
+                diff = datetime.utcnow() - to_insert[i]["time_extracted"]
                 ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
 
         if len(to_update) > 0:
             records_array = remove_time_extracted(to_update)
             for i, r in enumerate(collection.update_many(records_array)):
                 if type(r) is DocumentInsertError:
                     # Increment ingest_errors metric
                     ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     print(f'Failed to insert/update record: {to_update[i]}. {r}')
                 else:
                     # Update ingest_lag metric
-                    diff = datetime.utcnow() - datetime.strptime(to_update[i]["time_extracted"], "%Y-%m-%dT%H:%M:%S.%fZ")
+                    diff = datetime.utcnow() - to_update[i]["time_extracted"]
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
         record_batch.last_executed_time = utils.now()
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
@@ -157,15 +157,15 @@
                 ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 logger.error(f"Failed parsing the json schema for stream: {stream}.")
                 raise e
 
             try:
                 rec = o['record']
                 if 'time_extracted' in o:
-                    rec["time_extracted"] = o["time_extracted"]
+                    rec["time_extracted"] = ensure_datetime(o["time_extracted"])
                 else:
                     rec["time_extracted"] = record_batch.last_executed_time
                 try:
                     kps = key_properties.get(stream)
                     _key = None
                     # Appending _ to keys inorder for preserving values of reserved keys in source data
                     reserved_keys = ['_key', '_id', '_rev']
@@ -230,25 +230,31 @@
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.warning("Unknown message type {} in message {}".format(o['type'], o))
 
     scrape_complete_flag.labels(workflow_label).inc()
     return state
 
 
+def ensure_datetime(time_extracted):
+    if isinstance(time_extracted, str):
+        return datetime.strptime(time_extracted, "%Y-%m-%dT%H:%M:%S.%fZ")
+    return time_extracted
+
+
 def setup_batch_task(collection: StandardCollection, record_batch: RecordBatch) -> AbstractEventLoop:
     event_loop = asyncio.new_event_loop()
     Thread(target=start_background_loop, args=(event_loop,), daemon=True).start()
     asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch), event_loop)
     return event_loop
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
     while True:
         await asyncio.sleep(record_batch.interval)
-        timedelta = datetime.utcnow() - datetime.strptime(record_batch.last_executed_time, "%Y-%m-%dT%H:%M:%S.%fZ")
+        timedelta = datetime.utcnow() - record_batch.last_executed_time
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
 
 
 def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
     asyncio.set_event_loop(loop)
```

### Comparing `macrometa-target-collection-0.0.50/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.51/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.50
+Version: 0.0.51
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.50/pyproject.toml` & `macrometa-target-collection-0.0.51/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.50"
+version = "0.0.51"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

