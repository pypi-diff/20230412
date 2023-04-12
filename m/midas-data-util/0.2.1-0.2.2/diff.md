# Comparing `tmp/midas-data-util-0.2.1.tar.gz` & `tmp/midas-data-util-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-data-util-0.2.1.tar", last modified: Wed Apr 12 07:13:11 2023, max compression
+gzip compressed data, was "midas-data-util-0.2.2.tar", last modified: Wed Apr 12 07:17:49 2023, max compression
```

## Comparing `midas-data-util-0.2.1.tar` & `midas-data-util-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.539327 midas-data-util-0.2.1/
--rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      520 2023-04-12 07:13:11.538330 midas-data-util-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.1/README.md
--rw-rw-rw-   0        0        0      623 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 07:13:11.539327 midas-data-util-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.482960 midas-data-util-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.510398 midas-data-util-0.2.1/src/midas/
--rw-rw-rw-   0        0        0     3337 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/__init__.py
--rw-rw-rw-   0        0        0     5726 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/data_encoder.py
--rw-rw-rw-   0        0        0    11347 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/event.py
--rw-rw-rw-   0        0        0     9405 2023-04-12 06:08:18.000000 midas-data-util-0.2.1/src/midas/playfab.py
--rw-rw-rw-   0        0        0     4287 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/session.py
--rw-rw-rw-   0        0        0     3412 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/user.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.537333 midas-data-util-0.2.1/src/midas_data_util.egg-info/
--rw-rw-rw-   0        0        0      520 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.802185 midas-data-util-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-04-12 07:17:49.801187 midas-data-util-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.2/README.md
+-rw-rw-rw-   0        0        0      623 2023-04-12 07:17:12.000000 midas-data-util-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 07:17:49.802185 midas-data-util-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.761383 midas-data-util-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.777341 midas-data-util-0.2.2/src/midas/
+-rw-rw-rw-   0        0        0     2631 2023-04-12 07:17:33.000000 midas-data-util-0.2.2/src/midas/__init__.py
+-rw-rw-rw-   0        0        0     5845 2023-04-12 07:16:48.000000 midas-data-util-0.2.2/src/midas/data_encoder.py
+-rw-rw-rw-   0        0        0    11347 2023-04-12 07:12:36.000000 midas-data-util-0.2.2/src/midas/event.py
+-rw-rw-rw-   0        0        0     9405 2023-04-12 06:08:18.000000 midas-data-util-0.2.2/src/midas/playfab.py
+-rw-rw-rw-   0        0        0     4287 2023-04-12 07:12:36.000000 midas-data-util-0.2.2/src/midas/session.py
+-rw-rw-rw-   0        0        0     3412 2023-04-12 07:12:36.000000 midas-data-util-0.2.2/src/midas/user.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.798194 midas-data-util-0.2.2/src/midas_data_util.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/top_level.txt
```

### Comparing `midas-data-util-0.2.1/LICENSE` & `midas-data-util-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.1/PKG-INFO` & `midas-data-util-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.1
+Version: 0.2.2
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `midas-data-util-0.2.1/pyproject.toml` & `midas-data-util-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas-data-util"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"lxml~=4.9.2", 
 	"pandas~=2.0.0",
 	"adal~=1.2.7",
```

### Comparing `midas-data-util-0.2.1/src/midas/data_encoder.py` & `midas-data-util-0.2.2/src/midas/data_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,16 +198,20 @@
 
 def decode_raw_df(raw_df: DataFrame, encoding_config: Any) -> DataFrame:
 	untyped_raw_df: Any = raw_df
 	raw_record_list: list[RawRowData] = untyped_raw_df.to_dict(orient="records")
 
 	decoded_record_list: list[DecodedRowData] = []
 	for raw_row_data in raw_record_list:
-		encoded_data_str = raw_row_data["EventData"].replace("'", "\"").replace("False", "false").replace("True", "true")
-		event_data: Any = json.loads(encoded_data_str)
+		event_data: Any = {}
+		if type(raw_row_data["EventData"]) == str:
+			encoded_data_str = raw_row_data["EventData"].replace("'", "\"").replace("False", "false").replace("True", "true")
+			event_data = json.loads(encoded_data_str)
+		else:
+			event_data = raw_row_data["EventData"]
 		encoded_state_data = event_data["State"]
 		decoded_state_data = decode(encoded_state_data, encoding_config)
 		event_data["State"] = decoded_state_data
 		decoded_row_data: DecodedRowData = {
 				"EventData": event_data,
 				"Timestamp": raw_row_data["Timestamp"],
 				"PlayFabUserId": raw_row_data["PlayFabUserId"],
```

### Comparing `midas-data-util-0.2.1/src/midas/event.py` & `midas-data-util-0.2.2/src/midas/event.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.1/src/midas/playfab.py` & `midas-data-util-0.2.2/src/midas/playfab.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.1/src/midas/session.py` & `midas-data-util-0.2.2/src/midas/session.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.1/src/midas/user.py` & `midas-data-util-0.2.2/src/midas/user.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.1/src/midas_data_util.egg-info/PKG-INFO` & `midas-data-util-0.2.2/src/midas_data_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.1
+Version: 0.2.2
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

