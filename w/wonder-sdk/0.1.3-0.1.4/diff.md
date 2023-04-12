# Comparing `tmp/wonder-sdk-0.1.3.tar.gz` & `tmp/wonder-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-sdk-0.1.3.tar", last modified: Wed Apr 12 12:05:29 2023, max compression
+gzip compressed data, was "wonder-sdk-0.1.4.tar", last modified: Wed Apr 12 12:13:11 2023, max compression
```

## Comparing `wonder-sdk-0.1.3.tar` & `wonder-sdk-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:05:29.012332 wonder-sdk-0.1.3/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.3/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:05:29.012205 wonder-sdk-0.1.3/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 12:05:29.012375 wonder-sdk-0.1.3/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 12:05:13.000000 wonder-sdk-0.1.3/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:05:29.011471 wonder-sdk-0.1.3/wonder_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     4433 2023-04-12 12:04:56.000000 wonder-sdk-0.1.3/wonder_sdk/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)     1044 2023-04-12 12:03:33.000000 wonder-sdk-0.1.3/wonder_sdk/config.py
--rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.3/wonder_sdk/health.py
--rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.3/wonder_sdk/logger.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:05:29.012052 wonder-sdk-0.1.3/wonder_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 12:05:28.000000 wonder-sdk-0.1.3/wonder_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:13:11.768364 wonder-sdk-0.1.4/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2023-04-12 11:52:01.000000 wonder-sdk-0.1.4/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:13:11.768246 wonder-sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2023-04-12 12:13:11.768410 wonder-sdk-0.1.4/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      250 2023-04-12 12:13:07.000000 wonder-sdk-0.1.4/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:13:11.767530 wonder-sdk-0.1.4/wonder_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     4481 2023-04-12 12:13:02.000000 wonder-sdk-0.1.4/wonder_sdk/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)     1044 2023-04-12 12:03:33.000000 wonder-sdk-0.1.4/wonder_sdk/config.py
+-rw-r--r--   0 basri      (501) staff       (20)      520 2023-04-12 09:13:42.000000 wonder-sdk-0.1.4/wonder_sdk/health.py
+-rw-r--r--   0 basri      (501) staff       (20)      563 2023-04-12 11:36:48.000000 wonder-sdk-0.1.4/wonder_sdk/logger.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2023-04-12 12:13:11.768086 wonder-sdk-0.1.4/wonder_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      168 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      238 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       11 2023-04-12 12:13:11.000000 wonder-sdk-0.1.4/wonder_sdk.egg-info/top_level.txt
```

### Comparing `wonder-sdk-0.1.3/LICENCE` & `wonder-sdk-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.3/wonder_sdk/__init__.py` & `wonder-sdk-0.1.4/wonder_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 
         db = self.get_firestore_client()
         doc_ref = db.collection(collection_name).document(document_name)
         doc = doc_ref.get()
         return doc.to_dict()
 
     # PUB/SUB
-    def subscribe_to_pubsub(self, max_messages: int, callback, timeout=None):
+    def subscribe_to_pubsub(self, callback, max_messages=None, timeout=None):
         subscriber = pubsub_v1.SubscriberClient()
         subscription_path = subscriber.subscription_path(self._config.project_id, self._config.subscription_name)
-        flow_control = pubsub_v1.types.FlowControl(max_messages=max_messages)
+        flow_control = pubsub_v1.types.FlowControl(max_messages=max_messages if max_messages else self._config.process_count)
 
         def on_message(message):
             try:
                 callback(message)
                 message.ack()
             except e:
                 self.logger.error(f'Callback function raised exception: {e}')
```

### Comparing `wonder-sdk-0.1.3/wonder_sdk/config.py` & `wonder-sdk-0.1.4/wonder_sdk/config.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.3/wonder_sdk/health.py` & `wonder-sdk-0.1.4/wonder_sdk/health.py`

 * *Files identical despite different names*

### Comparing `wonder-sdk-0.1.3/wonder_sdk/logger.py` & `wonder-sdk-0.1.4/wonder_sdk/logger.py`

 * *Files identical despite different names*

