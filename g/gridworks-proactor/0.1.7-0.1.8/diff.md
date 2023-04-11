# Comparing `tmp/gridworks_proactor-0.1.7.tar.gz` & `tmp/gridworks_proactor-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_proactor-0.1.7.tar", max compression
+gzip compressed data, was "gridworks_proactor-0.1.8.tar", max compression
```

## Comparing `gridworks_proactor-0.1.7.tar` & `gridworks_proactor-0.1.8.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0     1070 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/LICENSE
--rw-r--r--   0        0        0     2615 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/README.md
--rw-r--r--   0        0        0     2357 2023-04-10 19:05:06.120349 gridworks_proactor-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2119 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/src/gwproactor/__init__.py
--rw-r--r--   0        0        0     1610 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/src/gwproactor/config/__init__.py
--rw-r--r--   0        0        0     4109 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/src/gwproactor/config/logging.py
--rw-r--r--   0        0        0      373 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/src/gwproactor/config/mqtt.py
--rw-r--r--   0        0        0     3107 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/src/gwproactor/config/paths.py
--rw-r--r--   0        0        0      596 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/src/gwproactor/config/proactor_settings.py
--rw-r--r--   0        0        0    16041 2023-04-10 19:04:53.880566 gridworks_proactor-0.1.7/src/gwproactor/link_state.py
--rw-r--r--   0        0        0     5557 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/logger.py
--rw-r--r--   0        0        0     4184 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/logging_setup.py
--rw-r--r--   0        0        0     7718 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/message.py
--rw-r--r--   0        0        0    11137 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/mqtt.py
--rw-r--r--   0        0        0    13287 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/persister.py
--rw-r--r--   0        0        0    35518 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/proactor_implementation.py
--rw-r--r--   0        0        0     3448 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/proactor_interface.py
--rw-r--r--   0        0        0     2645 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/problems.py
--rw-r--r--   0        0        0        0 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/py.typed
--rw-r--r--   0        0        0     3714 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/stats.py
--rw-r--r--   0        0        0     9207 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/sync_thread.py
--rw-r--r--   0        0        0     6070 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor/watchdog.py
--rw-r--r--   0        0        0     1053 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/__init__.py
--rw-r--r--   0        0        0     6615 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/clean.py
--rw-r--r--   0        0        0     6895 2023-04-10 19:05:06.120349 gridworks_proactor-0.1.7/src/gwproactor_test/comm_test_helper.py
--rw-r--r--   0        0        0    20076 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/config/hardware-layout.json
--rw-r--r--   0        0        0      807 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/__init__.py
--rw-r--r--   0        0        0      187 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/child/__init__.py
--rw-r--r--   0        0        0      401 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/child/config.py
--rw-r--r--   0        0        0     2558 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/child/dummy.py
--rw-r--r--   0        0        0      195 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/names.py
--rw-r--r--   0        0        0      193 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/parent/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/parent/config.py
--rw-r--r--   0        0        0     2199 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/dummies/parent/dummy.py
--rw-r--r--   0        0        0     2388 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/logger_guard.py
--rw-r--r--   0        0        0     9437 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/proactor_recorder.py
--rw-r--r--   0        0        0    47268 2023-04-10 19:05:06.120349 gridworks_proactor-0.1.7/src/gwproactor_test/proactor_test_collections.py
--rw-r--r--   0        0        0     2936 2023-04-10 19:04:53.884565 gridworks_proactor-0.1.7/src/gwproactor_test/wait.py
--rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.7/setup.py
--rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2615 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/README.md
+-rw-r--r--   0        0        0     2357 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2119 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/__init__.py
+-rw-r--r--   0        0        0     1610 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/__init__.py
+-rw-r--r--   0        0        0     4109 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/logging.py
+-rw-r--r--   0        0        0      373 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/mqtt.py
+-rw-r--r--   0        0        0     3107 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/paths.py
+-rw-r--r--   0        0        0      596 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/config/proactor_settings.py
+-rw-r--r--   0        0        0      107 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/link_state.py
+-rw-r--r--   0        0        0     1351 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/__init__.py
+-rw-r--r--   0        0        0     2763 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/acks.py
+-rw-r--r--   0        0        0      514 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/asyncio_timer_manager.py
+-rw-r--r--   0        0        0    16041 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/link_state.py
+-rw-r--r--   0        0        0     2220 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/message_times.py
+-rw-r--r--   0        0        0     1487 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/links/timer_interface.py
+-rw-r--r--   0        0        0     5557 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/logger.py
+-rw-r--r--   0        0        0     4184 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/logging_setup.py
+-rw-r--r--   0        0        0     7718 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/message.py
+-rw-r--r--   0        0        0    11137 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/mqtt.py
+-rw-r--r--   0        0        0    13287 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/persister.py
+-rw-r--r--   0        0        0    32266 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor/proactor_implementation.py
+-rw-r--r--   0        0        0     3448 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/proactor_interface.py
+-rw-r--r--   0        0        0     2645 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/problems.py
+-rw-r--r--   0        0        0        0 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/py.typed
+-rw-r--r--   0        0        0     3714 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/stats.py
+-rw-r--r--   0        0        0     9207 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/sync_thread.py
+-rw-r--r--   0        0        0     6070 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor/watchdog.py
+-rw-r--r--   0        0        0     1053 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor_test/__init__.py
+-rw-r--r--   0        0        0     6615 2023-04-11 22:28:21.174231 gridworks_proactor-0.1.8/src/gwproactor_test/clean.py
+-rw-r--r--   0        0        0     6895 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/comm_test_helper.py
+-rw-r--r--   0        0        0    20076 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/config/hardware-layout.json
+-rw-r--r--   0        0        0      807 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/config.py
+-rw-r--r--   0        0        0     2558 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/dummy.py
+-rw-r--r--   0        0        0      195 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/names.py
+-rw-r--r--   0        0        0      193 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/config.py
+-rw-r--r--   0        0        0     2199 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/dummy.py
+-rw-r--r--   0        0        0     2388 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/logger_guard.py
+-rw-r--r--   0        0        0     9073 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor_test/proactor_recorder.py
+-rw-r--r--   0        0        0    47333 2023-04-11 22:28:33.794414 gridworks_proactor-0.1.8/src/gwproactor_test/proactor_test_collections.py
+-rw-r--r--   0        0        0     2936 2023-04-11 22:28:21.178231 gridworks_proactor-0.1.8/src/gwproactor_test/wait.py
+-rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.8/setup.py
+-rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.8/PKG-INFO
```

### Comparing `gridworks_proactor-0.1.7/LICENSE` & `gridworks_proactor-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/README.md` & `gridworks_proactor-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/pyproject.toml` & `gridworks_proactor-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-proactor"
-version = "0.1.7"
+version = "0.1.8"
 description = "Gridworks Proactor"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-proactor"
 repository = "https://github.com/thegridelectric/gridworks-proactor"
 documentation = "https://gridworks-proactor.readthedocs.io"
```

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/__init__.py` & `gridworks_proactor-0.1.8/src/gwproactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/config/__init__.py` & `gridworks_proactor-0.1.8/src/gwproactor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/config/logging.py` & `gridworks_proactor-0.1.8/src/gwproactor/config/logging.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/config/paths.py` & `gridworks_proactor-0.1.8/src/gwproactor/config/paths.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/config/proactor_settings.py` & `gridworks_proactor-0.1.8/src/gwproactor/config/proactor_settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/link_state.py` & `gridworks_proactor-0.1.8/src/gwproactor/links/link_state.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/logger.py` & `gridworks_proactor-0.1.8/src/gwproactor/logger.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/logging_setup.py` & `gridworks_proactor-0.1.8/src/gwproactor/logging_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/message.py` & `gridworks_proactor-0.1.8/src/gwproactor/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/mqtt.py` & `gridworks_proactor-0.1.8/src/gwproactor/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/persister.py` & `gridworks_proactor-0.1.8/src/gwproactor/persister.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/proactor_implementation.py` & `gridworks_proactor-0.1.8/src/gwproactor/proactor_implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 """Proactor implementation"""
 
 import asyncio
-import enum
-import functools
 import json
 import sys
-import time
 import traceback
-from dataclasses import dataclass
-from dataclasses import field
 from typing import Any
 from typing import Awaitable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
@@ -36,17 +31,20 @@
 from paho.mqtt.client import MQTTMessageInfo
 from result import Err
 from result import Ok
 from result import Result
 
 from gwproactor import ProactorSettings
 from gwproactor import config
-from gwproactor.config.proactor_settings import MQTT_LINK_POLL_SECONDS
-from gwproactor.link_state import LinkStates
-from gwproactor.link_state import Transition
+from gwproactor.links import AckManager
+from gwproactor.links import AckWaitInfo
+from gwproactor.links import AsyncioTimerManager
+from gwproactor.links import LinkStates
+from gwproactor.links import MessageTimes
+from gwproactor.links import Transition
 from gwproactor.logger import ProactorLogger
 from gwproactor.message import DBGCommands
 from gwproactor.message import DBGEvent
 from gwproactor.message import DBGPayload
 from gwproactor.message import Message
 from gwproactor.message import MQTTConnectFailPayload
 from gwproactor.message import MQTTConnectPayload
@@ -67,108 +65,46 @@
 from gwproactor.proactor_interface import Runnable
 from gwproactor.proactor_interface import ServicesInterface
 from gwproactor.problems import Problems
 from gwproactor.stats import ProactorStats
 from gwproactor.watchdog import WatchdogManager
 
 
-@dataclass
-class AckWaitInfo:
-    message_id: str
-    timer_handle: asyncio.TimerHandle
-    client_name: str
-    context: Any = None
-
-
-class AckWaitSummary(enum.Enum):
-    acked = "acked"
-    timeout = "timeout"
-    connection_failure = "connection_failure"
-
-
-@dataclass
-class AckWaitResult:
-    summary: AckWaitSummary
-    wait_info: AckWaitInfo
-
-    def __bool__(self) -> bool:
-        return self.ok()
-
-    def ok(self) -> bool:
-        return self.summary == AckWaitSummary.acked
-
-
-import_time = time.time()
-
-
-@dataclass
-class MessageTimes:
-    last_send: float = field(default_factory=time.time)
-    last_recv: float = field(default_factory=time.time)
-
-    def next_ping_second(self, link_poll_seconds: float) -> float:
-        return self.last_send + link_poll_seconds
-
-    def seconds_until_next_ping(self, link_poll_seconds: float) -> float:
-        return self.next_ping_second(link_poll_seconds) - time.time()
-
-    def time_to_send_ping(self, link_poll_seconds: float) -> bool:
-        return time.time() > self.next_ping_second(link_poll_seconds)
-
-    def get_str(
-        self, link_poll_seconds: float = MQTT_LINK_POLL_SECONDS, relative: bool = True
-    ) -> str:
-        if relative:
-            adjust = import_time
-        else:
-            adjust = 0
-        return (
-            f"n:{time.time() - adjust:5.2f}  lps:{link_poll_seconds:5.2f}  "
-            f"ls:{self.last_send - adjust:5.2f}  lr:{self.last_recv - adjust:5.2f}  "
-            f"nps:{self.next_ping_second(link_poll_seconds) - adjust:5.2f}  "
-            f"snp:{self.next_ping_second(link_poll_seconds):5.2f}  "
-            f"tsp:{int(self.time_to_send_ping(link_poll_seconds))}"
-        )
-
-    def __str__(self) -> str:
-        return self.get_str()
-
-
 class Proactor(ServicesInterface, Runnable):
 
     PERSISTER_ENCODING = "utf-8"
 
     _name: str
     _settings: ProactorSettings
     _logger: ProactorLogger
     _stats: ProactorStats
     _event_persister: PersisterInterface
     _loop: Optional[asyncio.AbstractEventLoop] = None
     _receive_queue: Optional[asyncio.Queue] = None
     _mqtt_clients: MQTTClients
     _mqtt_codecs: Dict[str, MQTTCodec]
     _link_states: LinkStates
-    _link_message_times: dict[str, MessageTimes]
-    _acks: dict[str, AckWaitInfo]
+    _link_message_times: MessageTimes
+    _link_acks: AckManager
     _communicators: Dict[str, CommunicatorInterface]
     _stop_requested: bool
     _tasks: List[asyncio.Task]
     _watchdog: WatchdogManager
 
     def __init__(self, name: str, settings: ProactorSettings):
         self._name = name
         self._settings = settings
         self._logger = ProactorLogger(**settings.logging.qualified_logger_names())
         self._stats = self.make_stats()
         self._event_persister = self.make_event_persister(settings)
         self._mqtt_clients = MQTTClients()
         self._mqtt_codecs = dict()
         self._link_states = LinkStates()
-        self._link_message_times = dict()
-        self._acks = dict()
+        self._link_message_times = MessageTimes()
+        self._link_acks = AckManager(AsyncioTimerManager(), self._process_ack_timeout)
         self._communicators = dict()
         self._tasks = []
         self._stop_requested = False
         self._watchdog = WatchdogManager(10, self)
         self.add_communicator(self._watchdog)
 
     @classmethod
@@ -257,99 +193,64 @@
     ):
         self._mqtt_clients.add_client(
             name, client_config, upstream=upstream, primary_peer=primary_peer
         )
         if codec is not None:
             self._mqtt_codecs[name] = codec
         self._link_states.add(name)
-        self._link_message_times[name] = MessageTimes()
+        self._link_message_times.add_link(name)
         self._stats.add_link(name)
 
     async def _send_ping(self, client: str):
         while not self._stop_requested:
-            message_times = self._link_message_times[client]
+            message_times = self._link_message_times.get_copy(client)
             link_state = self._link_states[client]
             if (
                 message_times.time_to_send_ping(self.settings.mqtt_link_poll_seconds)
                 and link_state.active_for_send()
             ):
                 self._publish_message(client, PingMessage(Src=self.publication_name))
             await asyncio.sleep(
                 message_times.seconds_until_next_ping(
                     self.settings.mqtt_link_poll_seconds
                 )
             )
 
-    def _start_ack_timer(
-        self,
-        client_name: str,
-        message_id: str,
-        context: Any = None,
-        delay: Optional[float] = None,
-    ) -> None:
-        if delay is None:
-            delay = 5
-        self._acks[message_id] = AckWaitInfo(
-            message_id,
-            asyncio.get_running_loop().call_later(
-                delay,
-                functools.partial(self._process_ack_timeout, message_id),
-            ),
-            client_name=client_name,
-            context=context,
+    def _process_ack_timeout(self, wait_info: AckWaitInfo) -> None:
+        self._logger.message_enter(
+            "++Proactor._process_ack_timeout %s", wait_info.message_id
         )
-
-    def _cancel_ack_timer(self, message_id: str) -> Optional[AckWaitInfo]:
-        self._logger.path("++cancel_ack_timer %s", message_id)
         path_dbg = 0
-        wait_info = self._acks.pop(message_id, None)
-        if wait_info is not None:
+        self.stats.link(wait_info.link_name).timeouts += 1
+        result = self._link_states.process_ack_timeout(wait_info.link_name)
+        if result.is_ok():
             path_dbg |= 0x00000001
-            wait_info.timer_handle.cancel()
-
-        self._logger.path("--cancel_ack_timer path:0x%08X", path_dbg)
-        return wait_info
-
-    def _process_ack_timeout(self, message_id: str):
-        self._logger.message_enter("++Proactor._process_ack_timeout %s", message_id)
-        wait_info = self._acks.get(message_id, None)
-        if wait_info is not None:
-            self.stats.link(wait_info.client_name).timeouts += 1
-        self._process_ack_result(message_id, AckWaitSummary.timeout)
-        self._logger.message_exit("--Proactor._process_ack_timeout")
-
-    def _apply_ack_timeout(self, transition: Transition) -> Ok:
-        self._logger.path("++Proactor._apply_ack_timeout")
-        path_dbg = 0
-        if transition.deactivated():
-            path_dbg |= 0x00000001
-            self.generate_event(ResponseTimeoutEvent(PeerName=transition.link_name))
-            self._logger.comm_event(str(transition))
-            self._derived_recv_deactivated(transition)
-            for message_id in list(self._acks.keys()):
+            if result.value.deactivated():
                 path_dbg |= 0x00000002
-                self._process_ack_result(message_id, AckWaitSummary.connection_failure)
-        self._logger.path("--Proactor._apply_ack_timeout path:0x%08X", path_dbg)
-        return Ok()
+                self.generate_event(
+                    ResponseTimeoutEvent(PeerName=result.value.link_name)
+                )
+                self._logger.comm_event(str(result.value))
+                self._derived_recv_deactivated(result.value)
+                self._link_acks.cancel_ack_timers(wait_info.link_name)
+        else:
+            path_dbg |= 0x00000004
+            self._report_error(result.err(), msg="Proactor._process_ack_timeout")
+        self._logger.message_exit(
+            "--Proactor._process_ack_timeout path:0x%08X", path_dbg
+        )
 
-    def _process_ack_result(self, message_id: str, reason: AckWaitSummary):
-        self._logger.path("++Proactor._process_ack_result  %s", message_id)
+    def _process_ack(self, link_name: str, message_id: str):
+        self._logger.path("++Proactor._process_ack  %s", message_id)
         path_dbg = 0
-        wait_info = self._cancel_ack_timer(message_id)
-        if wait_info is not None:
+        wait_info = self._link_acks.cancel_ack_timer(link_name, message_id)
+        if wait_info is not None and message_id in self._event_persister:
             path_dbg |= 0x00000001
-            if reason == AckWaitSummary.timeout:
-                path_dbg |= 0x00000002
-                self._link_states.process_ack_timeout(wait_info.client_name).and_then(
-                    self._apply_ack_timeout
-                ).or_else(self._report_error)
-            elif reason == AckWaitSummary.acked and message_id in self._event_persister:
-                path_dbg |= 0x00000004
-                self._event_persister.clear(message_id)
-        self._logger.path("--Proactor._process_ack_result path:0x%08X", path_dbg)
+            self._event_persister.clear(message_id)
+        self._logger.path("--Proactor._process_ack path:0x%08X", path_dbg)
 
     def _process_dbg(self, dbg: DBGPayload):
         self._logger.path("++_process_dbg")
         path_dbg = 0
         count_dbg = 0
         for logger_name in ["message_summary", "lifecycle", "comm_event"]:
             requested_level = getattr(dbg.Levels, logger_name)
@@ -392,18 +293,18 @@
     ) -> MQTTMessageInfo:
         topic = message.mqtt_topic()
         payload = self._mqtt_codecs[client].encode(message)
         self._logger.message_summary(
             "OUT mqtt    ", message.Header.Src, topic, message.Payload
         )
         if message.Header.AckRequired:
-            if message.Header.MessageId in self._acks:
-                self._cancel_ack_timer(message.Header.MessageId)
-            self._start_ack_timer(client, message.Header.MessageId, context)
-        self._link_message_times[client].last_send = time.time()
+            self._link_acks.start_ack_timer(
+                client, message.Header.MessageId, context=context
+            )
+        self._link_message_times.update_send(client)
         return self._mqtt_clients.publish(client, topic, payload, qos)
 
     def _publish_upstream(
         self, payload, qos: QOS = QOS.AtMostOnce, **message_args: Any
     ) -> MQTTMessageInfo:
         message = Message(Src=self.publication_name, Payload=payload, **message_args)
         return self._publish_message(
@@ -458,16 +359,16 @@
         except:
             self._logger.exception(f"ERROR stopping proactor")
 
     def start_tasks(self):
         self._tasks = [
             asyncio.create_task(self.process_messages(), name="process_messages"),
         ]
-        for link in self._link_message_times:
-            self._tasks.append(asyncio.create_task(self._send_ping(link)))
+        for link_name in self._link_message_times.link_names():
+            self._tasks.append(asyncio.create_task(self._send_ping(link_name)))
         self._start_derived_tasks()
 
     def _start_derived_tasks(self):
         pass
 
     def _derived_process_message(self, message: Message):
         pass
@@ -608,17 +509,17 @@
                     self.name,
                     mqtt_receipt_message.Payload.message.topic,
                     decoded_message.Payload,
                 )
                 match self._link_states.process_mqtt_message(mqtt_receipt_message):
                     case Ok(transition):
                         path_dbg |= 0x00000004
-                        self._link_message_times[
+                        self._link_message_times.update_recv(
                             mqtt_receipt_message.Payload.client_name
-                        ].last_recv = time.time()
+                        )
                         if transition:
                             self._logger.comm_event(transition)
                         if transition.recv_activated():
                             path_dbg |= 0x00000008
                             self._recv_activated(transition)
                         elif transition.recv_deactivated():
                             path_dbg |= 0x00000010
@@ -628,16 +529,17 @@
                         self._report_error(
                             error,
                             "_process_mqtt_message/_link_states.process_mqtt_message",
                         )
                 match decoded_message.Payload:
                     case Ack():
                         path_dbg |= 0x00000040
-                        self._process_ack_result(
-                            decoded_message.Payload.AckMessageID, AckWaitSummary.acked
+                        self._process_ack(
+                            mqtt_receipt_message.Payload.client_name,
+                            decoded_message.Payload.AckMessageID,
                         )
                     case Ping():
                         path_dbg |= 0x00000080
                     case DBGPayload():
                         path_dbg |= 0x00000100
                         self._process_dbg(decoded_message.Payload)
                     case _:
@@ -704,18 +606,15 @@
                 self.generate_event(
                     MQTTDisconnectEvent(PeerName=message.Payload.client_name)
                 )
                 self._logger.comm_event(transition)
                 if transition.recv_deactivated():
                     result = self._derived_recv_deactivated(transition)
                 if transition.recv_deactivated() or transition.send_deactivated():
-                    for message_id in list(self._acks.keys()):
-                        self._process_ack_result(
-                            message_id, AckWaitSummary.connection_failure
-                        )
+                    self._link_acks.cancel_ack_timers(message.Payload.client_name)
             case Err(error):
                 result = Err(error)
         return result
 
     def _process_mqtt_connect_fail(
         self, message: Message[MQTTConnectFailPayload]
     ) -> Result[bool, BaseException]:
```

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/proactor_interface.py` & `gridworks_proactor-0.1.8/src/gwproactor/proactor_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/problems.py` & `gridworks_proactor-0.1.8/src/gwproactor/problems.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/stats.py` & `gridworks_proactor-0.1.8/src/gwproactor/stats.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/sync_thread.py` & `gridworks_proactor-0.1.8/src/gwproactor/sync_thread.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor/watchdog.py` & `gridworks_proactor-0.1.8/src/gwproactor/watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/__init__.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/clean.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/clean.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/comm_test_helper.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/comm_test_helper.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/config/hardware-layout.json` & `gridworks_proactor-0.1.8/src/gwproactor_test/config/hardware-layout.json`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/dummies/__init__.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/dummies/child/dummy.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/child/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/dummies/parent/config.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/dummies/parent/dummy.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/dummies/parent/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/logger_guard.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/logger_guard.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/proactor_recorder.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/proactor_recorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,14 @@
 def make_recorder_class(
     proactor_type: Type[ProactorT],
 ) -> Callable[..., RecorderInterface]:
     class Recorder(proactor_type):
 
         subacks_paused: bool
         pending_subacks: list[Message]
-        ack_timeout_seconds: float = 5.0
         acks_paused: bool
         needs_ack: list[_PausedAck]
         mqtt_messages_dropped: bool
 
         def __init__(self, name: str, settings: ProactorSettings, **kwargs_):
             super().__init__(name=name, settings=settings, **kwargs_)
             self.subacks_paused = False
@@ -212,27 +211,16 @@
             s = str(self.stats)
             s += f"\nsubacks_paused: {self.subacks_paused}  pending_subacks: {len(self.pending_subacks)}\n"
             s += "Link states:\n"
             for link_name in self.stats.links:
                 s += f"  {link_name:10s}  {self._link_states.link_state(link_name).value}\n"
             return s
 
-        def _start_ack_timer(
-            self: ProactorT,
-            client_name: str,
-            message_id: str,
-            context: Any = None,
-            delay: Optional[float] = None,
-        ) -> None:
-            if delay is None:
-                delay = self.ack_timeout_seconds
-            # noinspection PyProtectedMember
-            super()._start_ack_timer(
-                client_name, message_id, context=context, delay=delay
-            )
+        def set_ack_timeout_seconds(self, timeout_seconds: float):
+            self._link_acks._default_delay_seconds = timeout_seconds
 
         def summarize(self: ProactorT):
             self._logger.info(self.summary_str())
 
         def ping_peer(self):
             self._publish_message(
                 self.primary_peer_client, PingMessage(Src=self.publication_name)
```

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/proactor_test_collections.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/proactor_test_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Type
 
 import pytest
 from gwproto import MQTTTopic
 from paho.mqtt.client import MQTT_ERR_CONN_LOST
 
 from gwproactor.config import MQTTClient
-from gwproactor.link_state import StateName
+from gwproactor.links import StateName
 from gwproactor.message import DBGPayload
 from gwproactor_test.comm_test_helper import CommTestHelper
 from gwproactor_test.dummies import DummyChildSettings
 from gwproactor_test.wait import await_for
 
 
 @pytest.mark.asyncio
@@ -892,15 +892,15 @@
                 lambda: parent_link.in_state(StateName.awaiting_peer),
                 3,
                 "ERROR waiting for parent to connect to broker",
                 err_str_f=parent.summary_str,
             )
 
             # start child
-            child.ack_timeout_seconds = 0.1
+            child.set_ack_timeout_seconds(0.1)
             assert stats.timeouts == 0
             h.start_child()
             await await_for(
                 lambda: link.in_state(StateName.awaiting_peer),
                 3,
                 "ERROR waiting for child to connect to broker",
                 err_str_f=parent.summary_str,
@@ -932,15 +932,17 @@
                 err_str_f=child.summary_str,
             )
 
             # Timeout while active
             # (active -> response_timeout -> awaiting_peer)
             parent.pause_acks()
             child.ping_peer()
-            exp_timeouts = stats.timeouts + len(child._acks)
+            exp_timeouts = stats.timeouts + len(
+                child._link_acks._acks[child.upstream_client]
+            )
             await await_for(
                 lambda: stats.timeouts == exp_timeouts,
                 1,
                 "ERROR waiting for child to timeout",
                 err_str_f=child.summary_str,
             )
             assert link.state == StateName.awaiting_peer
@@ -986,15 +988,15 @@
             parent_stats = parent.stats.link(parent.primary_peer_client)
             parent_ping_topic = MQTTTopic.encode(
                 "gw", parent.publication_name, "gridworks-ping"
             )
 
             child = h.child
             child.suppress_status = True
-            child.ack_timeout_seconds = 0.1
+            child.set_ack_timeout_seconds(0.1)
             link = child._link_states.link(child.upstream_client)
             stats = child.stats.link(child.upstream_client)
             child_ping_topic = MQTTTopic.encode(
                 "gw", child.publication_name, "gridworks-ping"
             )
 
             # start parent and child
```

### Comparing `gridworks_proactor-0.1.7/src/gwproactor_test/wait.py` & `gridworks_proactor-0.1.8/src/gwproactor_test/wait.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.7/setup.py` & `gridworks_proactor-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
  'gwproactor_test.dummies': 'src/gwproactor_test/dummies',
  'gwproactor_test.dummies.child': 'src/gwproactor_test/dummies/child',
  'gwproactor_test.dummies.parent': 'src/gwproactor_test/dummies/parent'}
 
 packages = \
 ['gwproactor',
  'gwproactor.config',
+ 'gwproactor.links',
  'gwproactor_test',
  'gwproactor_test.dummies',
  'gwproactor_test.dummies.child',
  'gwproactor_test.dummies.parent']
 
 package_data = \
 {'': ['*'], 'gwproactor_test': ['config/*']}
@@ -29,15 +30,15 @@
  'xdg>=6.0.0,<7.0.0']
 
 extras_require = \
 {'tests': ['pytest>=7.2.0,<8.0.0', 'pytest-asyncio>=0.20.3,<0.21.0']}
 
 setup_kwargs = {
     'name': 'gridworks-proactor',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Gridworks Proactor',
     'long_description': "# Gridworks Proactor\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-proactor.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/gridworks-proactor.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-proactor)][pypi status]\n[![License](https://img.shields.io/pypi/l/gridworks-proactor)][license]\n\n[![Read the documentation at https://gridworks-proactor.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-proactor/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-proactor/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-proactor/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/gridworks-proactor/\n[read the docs]: https://gridworks-proactor.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-proactor/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-proactor\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Gridworks Proactor_ via [pip] from [PyPI]:\n\n```console\n$ pip install gridworks-proactor\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome. In order to develop, do this:\n\n```console\n$ poetry install --all-extras\n```\n\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Gridworks Proactor_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-proactor/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-proactor/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-proactor/blob/main/CONTRIBUTING.md\n[command-line reference]: https://gridworks-proactor.readthedocs.io/en/latest/usage.html\n",
     'author': 'Jessica Millar',
     'author_email': 'jmillar@gridworks-consulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegridelectric/gridworks-proactor',
```

### Comparing `gridworks_proactor-0.1.7/PKG-INFO` & `gridworks_proactor-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-proactor
-Version: 0.1.7
+Version: 0.1.8
 Summary: Gridworks Proactor
 Home-page: https://github.com/thegridelectric/gridworks-proactor
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

