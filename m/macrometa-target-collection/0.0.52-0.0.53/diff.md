# Comparing `tmp/macrometa-target-collection-0.0.52.tar.gz` & `tmp/macrometa-target-collection-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.52.tar", last modified: Wed Apr 12 17:58:55 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.53.tar", last modified: Wed Apr 12 18:13:16 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.52.tar` & `macrometa-target-collection-0.0.53.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:55.234583 macrometa-target-collection-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 17:58:34.000000 macrometa-target-collection-0.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 17:58:55.234583 macrometa-target-collection-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 17:58:34.000000 macrometa-target-collection-0.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:55.234583 macrometa-target-collection-0.0.52/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 17:58:34.000000 macrometa-target-collection-0.0.52/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13856 2023-04-12 17:58:34.000000 macrometa-target-collection-0.0.52/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:58:55.234583 macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 17:58:55.000000 macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 17:58:55.000000 macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:58:55.000000 macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 17:58:55.000000 macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 17:58:55.000000 macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 17:58:55.000000 macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 17:58:34.000000 macrometa-target-collection-0.0.52/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 17:58:55.234583 macrometa-target-collection-0.0.52/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:13:16.749469 macrometa-target-collection-0.0.53/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13888 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.52/LICENSE` & `macrometa-target-collection-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.52/PKG-INFO` & `macrometa-target-collection-0.0.53/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.52
+Version: 0.0.53
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.52/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.53/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.52/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.53/macrometa_target_collection/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import jsonschema
 from adjust_precision_for_schema import adjust_decimal_precision_for_schema
 from c8 import C8Client, DocumentInsertError
 from c8.collection import StandardCollection
 from jsonschema import Draft4Validator
 from prometheus_client import Counter, Gauge, start_http_server
 from singer import get_logger
-from singer import utils
 
 logger = get_logger('macrometa_target_collection')
 
 DEFAULT_BATCH_SIZE_ROWS = 50
 DEFAULT_BATCH_FLUSH_INTERVAL = 60
 DEFAULT_MIN_BATCH_FLUSH_TIME_GAP = 60
 
@@ -48,15 +47,15 @@
 class RecordBatch:
     """Class wrapping the record batch in order to make it thread safe."""
 
     def __init__(self, config: dict):
         self._list = list()
         self._lock = Lock()
         self.interval = config.get('batch_flush_interval', DEFAULT_BATCH_FLUSH_INTERVAL)
-        self.last_executed_time = utils.now()
+        self.last_executed_time = datetime.now(timezone.utc)
         self.min_time_gap = config.get('batch_flush_min_time_gap', DEFAULT_MIN_BATCH_FLUSH_TIME_GAP)
         self.max_batch_size = config.get('batch_size_rows', DEFAULT_BATCH_SIZE_ROWS)
 
     def append(self, value) -> None:
         """Acquire the lock and add a record to the list."""
         with self._lock:
             self._list.append(value)
@@ -93,29 +92,29 @@
             if type(r) is DocumentInsertError:
                 to_update.append(to_insert[i])
             else:
                 # Update ingested_documents and ingested_bytes metrics
                 ingested_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 ingested_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(json.dumps(r)))
                 # Update ingest_lag metric
-                diff = datetime.utcnow() - ensure_datetime(to_insert[i]["time_extracted"])
+                diff = datetime.now(timezone.utc) - ensure_datetime(to_insert[i]["time_extracted"])
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
-                    diff = datetime.utcnow() - ensure_datetime(to_update[i]["time_extracted"])
+                    diff = datetime.now(timezone.utc) - ensure_datetime(to_update[i]["time_extracted"])
                     ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
-        record_batch.last_executed_time = utils.now()
+        record_batch.last_executed_time = datetime.now(timezone.utc)
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
 def try_delete(collection: StandardCollection, _key: str):
@@ -251,15 +250,15 @@
     asyncio.run_coroutine_threadsafe(process_batch(collection, record_batch), event_loop)
     return event_loop
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
     while True:
         await asyncio.sleep(record_batch.interval)
-        timedelta = datetime.utcnow() - ensure_datetime(record_batch.last_executed_time)
+        timedelta = datetime.now(timezone.utc) - ensure_datetime(record_batch.last_executed_time)
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
 
 
 def start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
     asyncio.set_event_loop(loop)
```

### Comparing `macrometa-target-collection-0.0.52/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.52
+Version: 0.0.53
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.52/pyproject.toml` & `macrometa-target-collection-0.0.53/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.52"
+version = "0.0.53"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

