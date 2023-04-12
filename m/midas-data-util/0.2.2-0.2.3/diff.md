# Comparing `tmp/midas-data-util-0.2.2.tar.gz` & `tmp/midas-data-util-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-data-util-0.2.2.tar", last modified: Wed Apr 12 07:17:49 2023, max compression
+gzip compressed data, was "midas-data-util-0.2.3.tar", last modified: Wed Apr 12 12:05:58 2023, max compression
```

## Comparing `midas-data-util-0.2.2.tar` & `midas-data-util-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.802185 midas-data-util-0.2.2/
--rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      520 2023-04-12 07:17:49.801187 midas-data-util-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.2/README.md
--rw-rw-rw-   0        0        0      623 2023-04-12 07:17:12.000000 midas-data-util-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 07:17:49.802185 midas-data-util-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.761383 midas-data-util-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.777341 midas-data-util-0.2.2/src/midas/
--rw-rw-rw-   0        0        0     2631 2023-04-12 07:17:33.000000 midas-data-util-0.2.2/src/midas/__init__.py
--rw-rw-rw-   0        0        0     5845 2023-04-12 07:16:48.000000 midas-data-util-0.2.2/src/midas/data_encoder.py
--rw-rw-rw-   0        0        0    11347 2023-04-12 07:12:36.000000 midas-data-util-0.2.2/src/midas/event.py
--rw-rw-rw-   0        0        0     9405 2023-04-12 06:08:18.000000 midas-data-util-0.2.2/src/midas/playfab.py
--rw-rw-rw-   0        0        0     4287 2023-04-12 07:12:36.000000 midas-data-util-0.2.2/src/midas/session.py
--rw-rw-rw-   0        0        0     3412 2023-04-12 07:12:36.000000 midas-data-util-0.2.2/src/midas/user.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:17:49.798194 midas-data-util-0.2.2/src/midas_data_util.egg-info/
--rw-rw-rw-   0        0        0      520 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 07:17:49.000000 midas-data-util-0.2.2/src/midas_data_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.192146 midas-data-util-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-04-12 12:05:58.191078 midas-data-util-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.3/README.md
+-rw-rw-rw-   0        0        0      623 2023-04-12 12:05:24.000000 midas-data-util-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 12:05:58.192146 midas-data-util-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.082965 midas-data-util-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.140814 midas-data-util-0.2.3/src/midas/
+-rw-rw-rw-   0        0        0     2631 2023-04-12 07:17:33.000000 midas-data-util-0.2.3/src/midas/__init__.py
+-rw-rw-rw-   0        0        0     5845 2023-04-12 07:16:48.000000 midas-data-util-0.2.3/src/midas/data_encoder.py
+-rw-rw-rw-   0        0        0    11528 2023-04-12 11:59:47.000000 midas-data-util-0.2.3/src/midas/event.py
+-rw-rw-rw-   0        0        0     9405 2023-04-12 06:08:18.000000 midas-data-util-0.2.3/src/midas/playfab.py
+-rw-rw-rw-   0        0        0     4327 2023-04-12 12:04:40.000000 midas-data-util-0.2.3/src/midas/session.py
+-rw-rw-rw-   0        0        0     3448 2023-04-12 12:05:02.000000 midas-data-util-0.2.3/src/midas/user.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:05:58.189085 midas-data-util-0.2.3/src/midas_data_util.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 12:05:58.000000 midas-data-util-0.2.3/src/midas_data_util.egg-info/top_level.txt
```

### Comparing `midas-data-util-0.2.2/LICENSE` & `midas-data-util-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.2/PKG-INFO` & `midas-data-util-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.2
+Version: 0.2.3
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `midas-data-util-0.2.2/pyproject.toml` & `midas-data-util-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas-data-util"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"lxml~=4.9.2", 
 	"pandas~=2.0.0",
 	"adal~=1.2.7",
```

### Comparing `midas-data-util-0.2.2/src/midas/__init__.py` & `midas-data-util-0.2.3/src/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.2/src/midas/data_encoder.py` & `midas-data-util-0.2.3/src/midas/data_encoder.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.2/src/midas/event.py` & `midas-data-util-0.2.3/src/midas/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import copy
+from copy import deepcopy
 import json
 from uuid import uuid4
 from pandas import DataFrame
 from datetime import datetime
 from typing import Any
 from .playfab import get_datetime_from_playfab_str, get_playfab_str_from_datetime
 from .data_encoder import DecodedRowData as RowData
@@ -38,24 +38,29 @@
 	if is_build_included:
 		build = version["Build"]
 		version_text+=f"-{build}"
 
 	return version_text
 
 class EventDumpData:
-	state_data: BaseStateTree
 	name: str
-	timestamp: str
 	event_id: str
-	session_id: str | None
-	user_id: str
+	timestamp: str
+	seconds_since_previous_event: None | float
+	seconds_since_session_start: float
 	version_text: str
+	revenue: int
+	session_id: str
+	user_id: str
+	place_id: str
+	version: VersionData
 	index: int
-	first_event_found: bool
+	is_studio: bool
 	is_sequential: bool
+	state_date: BaseStateTree
 
 class Event: 
 	name: str
 	event_id: str
 	timestamp: datetime
 	seconds_since_previous_event: None | float
 	seconds_since_session_start: float
@@ -64,14 +69,15 @@
 	session_id: str
 	user_id: str
 	place_id: str
 	version: VersionData
 	index: int
 	is_studio: bool
 	is_sequential: bool
+	state_date: BaseStateTree
 
 	def __init__(
 		self, 
 		row_data: RowData
 	):
 		
 		self.name = row_data["EventName"]
@@ -106,28 +112,29 @@
 	def __lt__(self, other):
 		t1 = self.index
 		t2 = other.index
 		return t1 < t2
 
 	def dump(self) -> EventDumpData:
 		event_dump_date: Any = {
-			"state_data": copy.deepcopy(self.state_data),
 			"name": self.name,
+			"event_id": self.event_id,
 			"timestamp": get_playfab_str_from_datetime(self.timestamp),
 			"seconds_since_previous_event": self.seconds_since_previous_event,
 			"seconds_since_session_start": self.seconds_since_session_start,
+			"version_text": self.version_text,
 			"revenue": self.revenue,
-			"place_id": self.place_id,
-			"event_id": self.event_id,
-			"user_id": self.user_id,
 			"session_id": self.session_id,
-			"version_text": self.version_text,
-			"version": copy.deepcopy(self.version),
+			"user_id": self.user_id,
+			"place_id": self.place_id,
+			"version": deepcopy(self.version),
 			"index": self.index,
+			"is_studio": self.is_studio,
 			"is_sequential": self.is_sequential,
+			"state_date": deepcopy(self.state_data),
 		}
 		return event_dump_date
 
 def fill_down(current_data: dict | None, prev_data: dict | None):
 		if current_data == None:
 			current_data = {}
 
@@ -137,15 +144,15 @@
 			return current_data
 
 		assert prev_data
 
 		for key in prev_data:
 			val = prev_data[key]
 			if not key in current_data:
-				current_data[key] = copy.deepcopy(prev_data[key])
+				current_data[key] = deepcopy(prev_data[key])
 
 				return current_data
 
 			if type(val) == dict:
 				fill_down(current_data[key], prev_data[key])
 			else:
 				current_data[key] = val
```

### Comparing `midas-data-util-0.2.2/src/midas/playfab.py` & `midas-data-util-0.2.3/src/midas/playfab.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.2/src/midas/session.py` & `midas-data-util-0.2.3/src/midas/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 from typing import Any, TypedDict
 from .playfab import get_playfab_str_from_datetime
 from .event import Event
 
 class SessionDumpData(TypedDict):
 	session_id: str
 	user_id: str
+	is_studio: bool
 	timestamp: str
 	version_text: str
-	index: int
-	event_count: int
-	revenue: int
 	is_singular_version: bool
 	duration: float
+	revenue: int
+	index: int
 
 class Session: 
 	session_id: str
 	user_id: str
 	is_studio: bool
 	events: list[Event]
 	timestamp: datetime
 	version_text: str
 	is_singular_version: bool
+	duration: float
+	revenue: int
+	index: int
 
 	def __init__(
 		self, 
 		events: list[Event]
 	):
 		# sort list
 		events = sorted(events, key=lambda event: event.timestamp)
@@ -61,21 +64,21 @@
 		t2 = other.timestamp
 		return t1 < t2
 
 	def dump(self) -> SessionDumpData:
 		return {
 			"session_id": self.session_id,
 			"user_id": self.user_id,
+			"is_studio": self.is_studio,
 			"timestamp": get_playfab_str_from_datetime(self.timestamp),
 			"version_text": self.version_text,
 			"is_singular_version": self.is_singular_version,
-			"index": self.index,
-			"event_count": len(self.events),
-			"revenue": self.revenue,
 			"duration": self.duration,
+			"revenue": self.revenue,
+			"index": self.index
 		}
 
 def get_survival_rate(sessions: list[Session]) -> float:
 	missing_event_count = 0
 	found_event_count = 0
 	session_count = len(sessions)
 	print("getting event survival rate for ", session_count, "sessions")
```

### Comparing `midas-data-util-0.2.2/src/midas/user.py` & `midas-data-util-0.2.3/src/midas/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,28 +75,29 @@
 		self.index = -1
 
 	def __lt__(self, other):
 		t1 = self.timestamp
 		t2 = other.timestamp
 		return t1 < t2
 		
-	def dump(self):
-		return {
+	def dump(self) -> UserDumpData:
+		data: Any = {
 			"user_id": self.user_id,
 			"timestamp": get_playfab_str_from_datetime(self.timestamp),
 			"index": self.index,
 			"session_count": len(self.sessions),
 			"net_revenue": self.net_revenue,
 			"net_duration": self.net_duration,
 			"is_retained_on_d0": self.is_retained_on_d0,
 			"is_retained_on_d1": self.is_retained_on_d1,
 			"is_retained_on_d7": self.is_retained_on_d7,
 			"is_retained_on_d14": self.is_retained_on_d14,
 			"is_retained_on_d28": self.is_retained_on_d28,
 		}
+		return data
 
 def get_users_from_session_list(sessions: list[Session]):
 	
 	user_session_lists: dict[str, list[Session]] = {}
 	for session in sessions:
 		user_id = session.user_id
 		if not user_id in user_session_lists:
```

### Comparing `midas-data-util-0.2.2/src/midas_data_util.egg-info/PKG-INFO` & `midas-data-util-0.2.3/src/midas_data_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.2
+Version: 0.2.3
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

