# Comparing `tmp/midas-data-util-0.2.0.tar.gz` & `tmp/midas-data-util-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-data-util-0.2.0.tar", last modified: Wed Apr 12 07:09:23 2023, max compression
+gzip compressed data, was "midas-data-util-0.2.1.tar", last modified: Wed Apr 12 07:13:11 2023, max compression
```

## Comparing `midas-data-util-0.2.0.tar` & `midas-data-util-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:09:23.833403 midas-data-util-0.2.0/
--rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      520 2023-04-12 07:09:23.831408 midas-data-util-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.0/README.md
--rw-rw-rw-   0        0        0      623 2023-04-12 07:05:51.000000 midas-data-util-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 07:09:23.833403 midas-data-util-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 07:09:23.765343 midas-data-util-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 07:09:23.789238 midas-data-util-0.2.0/src/midas/
--rw-rw-rw-   0        0        0     3334 2023-04-12 07:05:51.000000 midas-data-util-0.2.0/src/midas/__init__.py
--rw-rw-rw-   0        0        0     5725 2023-04-12 05:16:53.000000 midas-data-util-0.2.0/src/midas/data_encoder.py
--rw-rw-rw-   0        0        0    11344 2023-04-12 07:05:28.000000 midas-data-util-0.2.0/src/midas/event.py
--rw-rw-rw-   0        0        0     9405 2023-04-12 06:08:18.000000 midas-data-util-0.2.0/src/midas/playfab.py
--rw-rw-rw-   0        0        0     4285 2023-04-12 06:34:39.000000 midas-data-util-0.2.0/src/midas/session.py
--rw-rw-rw-   0        0        0     3410 2023-04-12 06:24:36.000000 midas-data-util-0.2.0/src/midas/user.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:09:23.830411 midas-data-util-0.2.0/src/midas_data_util.egg-info/
--rw-rw-rw-   0        0        0      520 2023-04-12 07:09:23.000000 midas-data-util-0.2.0/src/midas_data_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-12 07:09:23.000000 midas-data-util-0.2.0/src/midas_data_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:09:23.000000 midas-data-util-0.2.0/src/midas_data_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-12 07:09:23.000000 midas-data-util-0.2.0/src/midas_data_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 07:09:23.000000 midas-data-util-0.2.0/src/midas_data_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.539327 midas-data-util-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-04-12 07:13:11.538330 midas-data-util-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.1/README.md
+-rw-rw-rw-   0        0        0      623 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 07:13:11.539327 midas-data-util-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.482960 midas-data-util-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.510398 midas-data-util-0.2.1/src/midas/
+-rw-rw-rw-   0        0        0     3337 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/__init__.py
+-rw-rw-rw-   0        0        0     5726 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/data_encoder.py
+-rw-rw-rw-   0        0        0    11347 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/event.py
+-rw-rw-rw-   0        0        0     9405 2023-04-12 06:08:18.000000 midas-data-util-0.2.1/src/midas/playfab.py
+-rw-rw-rw-   0        0        0     4287 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/session.py
+-rw-rw-rw-   0        0        0     3412 2023-04-12 07:12:36.000000 midas-data-util-0.2.1/src/midas/user.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:13:11.537333 midas-data-util-0.2.1/src/midas_data_util.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-12 07:13:11.000000 midas-data-util-0.2.1/src/midas_data_util.egg-info/top_level.txt
```

### Comparing `midas-data-util-0.2.0/LICENSE` & `midas-data-util-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.0/PKG-INFO` & `midas-data-util-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.0
+Version: 0.2.1
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `midas-data-util-0.2.0/pyproject.toml` & `midas-data-util-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas-data-util"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"lxml~=4.9.2", 
 	"pandas~=2.0.0",
 	"adal~=1.2.7",
```

### Comparing `midas-data-util-0.2.0/src/midas/__init__.py` & `midas-data-util-0.2.1/src/midas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 from pandas import DataFrame
 from typing import Any
-from event import Event, get_events_from_df
-from session import Session, SessionDumpData,  get_sessions_from_events, get_survival_rate
-from user import User, UserDumpData, get_users_from_session_list
+from .event import Event, get_events_from_df
+from .session import Session, SessionDumpData,  get_sessions_from_events, get_survival_rate
+from .user import User, UserDumpData, get_users_from_session_list
 
 def dump(objects: list[Event] | list[Session] | list[User]):
 	untyped_objects: Any = objects
 	object_count = len(objects)
 	if type(objects[0]) == Event:
 		event_list: list[Event] = untyped_objects
 		event_data_list: list[Any] = []
```

### Comparing `midas-data-util-0.2.0/src/midas/data_encoder.py` & `midas-data-util-0.2.1/src/midas/data_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from pandas import DataFrame
 from typing import Any, TypedDict, Union
-from playfab import RawRowData
+from .playfab import RawRowData
 
 class PlayFabEnvironmentData(TypedDict):
 	Vertical: str
 	Cloud: str
 	Application: str
 	Commit: str
```

### Comparing `midas-data-util-0.2.0/src/midas/event.py` & `midas-data-util-0.2.1/src/midas/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
 import json
 from uuid import uuid4
 from pandas import DataFrame
 from datetime import datetime
 from typing import Any
-from playfab import get_datetime_from_playfab_str, get_playfab_str_from_datetime
-from data_encoder import DecodedRowData as RowData
-from data_encoder import VersionData, EventData, BaseStateTree
+from .playfab import get_datetime_from_playfab_str, get_playfab_str_from_datetime
+from .data_encoder import DecodedRowData as RowData
+from .data_encoder import VersionData, EventData, BaseStateTree
 
 SID_GEN_REFIX = "!generated"
 
 def get_if_session_id_generated(session_id: str) -> bool:
 	pattern = session_id[0:len(SID_GEN_REFIX)]
 	result = pattern == SID_GEN_REFIX
 	# print(f"is_gen: {result} since {pattern} is start of {session_id}")
```

### Comparing `midas-data-util-0.2.0/src/midas/playfab.py` & `midas-data-util-0.2.1/src/midas/playfab.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.0/src/midas/session.py` & `midas-data-util-0.2.1/src/midas/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from copy import deepcopy
 from datetime import datetime
 from typing import Any, TypedDict
-from playfab import get_playfab_str_from_datetime
-from event import Event
+from .playfab import get_playfab_str_from_datetime
+from .event import Event
 
 class SessionDumpData(TypedDict):
 	session_id: str
 	user_id: str
 	timestamp: str
 	version_text: str
 	index: int
```

### Comparing `midas-data-util-0.2.0/src/midas/user.py` & `midas-data-util-0.2.1/src/midas/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime as dt
 import copy
 from datetime import datetime
 from typing import Any, TypedDict
-from session import Session
-from playfab import get_playfab_str_from_datetime
+from .session import Session
+from .playfab import get_playfab_str_from_datetime
 
 class UserDumpData(TypedDict):
 	user_id: str
 	timestamp: str
 	index: int
 	session_count: int
 	net_revenue: int
```

### Comparing `midas-data-util-0.2.0/src/midas_data_util.egg-info/PKG-INFO` & `midas-data-util-0.2.1/src/midas_data_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.0
+Version: 0.2.1
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

