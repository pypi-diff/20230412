# Comparing `tmp/rstream-0.5.0.tar.gz` & `tmp/rstream-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstream-0.5.0.tar", max compression
+gzip compressed data, was "rstream-0.6.0.tar", max compression
```

## Comparing `rstream-0.5.0.tar` & `rstream-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-03-08 12:45:40.073873 rstream-0.5.0/LICENSE
--rw-r--r--   0        0        0     3743 2023-03-08 12:45:40.073873 rstream-0.5.0/README.md
--rw-r--r--   0        0        0      660 2023-03-08 12:45:40.073873 rstream-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      575 2023-03-08 12:45:40.073873 rstream-0.5.0/rstream/__init__.py
--rw-r--r--   0        0        0      651 2023-03-08 12:45:40.073873 rstream-0.5.0/rstream/amqp.py
--rw-r--r--   0        0        0    17226 2023-03-08 12:45:40.073873 rstream-0.5.0/rstream/client.py
--rw-r--r--   0        0        0     2117 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/connection.py
--rw-r--r--   0        0        0      928 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/constants.py
--rw-r--r--   0        0        0     8080 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/consumer.py
--rw-r--r--   0        0        0     5638 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/encoding.py
--rw-r--r--   0        0        0     1364 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/exceptions.py
--rw-r--r--   0        0        0    10736 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/producer.py
--rw-r--r--   0        0        0    12569 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/schema.py
--rw-r--r--   0        0        0      705 2023-03-08 12:45:40.077873 rstream-0.5.0/rstream/utils.py
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 rstream-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-12 12:26:02.281874 rstream-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5442 2023-04-12 12:26:02.281874 rstream-0.6.0/README.md
+-rw-r--r--   0        0        0      660 2023-04-12 12:26:02.281874 rstream-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-04-12 12:26:02.281874 rstream-0.6.0/rstream/__init__.py
+-rw-r--r--   0        0        0      651 2023-04-12 12:26:02.281874 rstream-0.6.0/rstream/amqp.py
+-rw-r--r--   0        0        0    17432 2023-04-12 12:26:02.281874 rstream-0.6.0/rstream/client.py
+-rw-r--r--   0        0        0     2117 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/connection.py
+-rw-r--r--   0        0        0      928 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/constants.py
+-rw-r--r--   0        0        0     8080 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/consumer.py
+-rw-r--r--   0        0        0     5638 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/encoding.py
+-rw-r--r--   0        0        0     1364 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/exceptions.py
+-rw-r--r--   0        0        0    12802 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/producer.py
+-rw-r--r--   0        0        0    12768 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/schema.py
+-rw-r--r--   0        0        0      705 2023-04-12 12:26:02.285874 rstream-0.6.0/rstream/utils.py
+-rw-r--r--   0        0        0     6073 1970-01-01 00:00:00.000000 rstream-0.6.0/PKG-INFO
```

### Comparing `rstream-0.5.0/LICENSE` & `rstream-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rstream-0.5.0/README.md` & `rstream-0.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -77,14 +77,56 @@
             list_messages.append(amqp_message)
 
         await producer.send_batch('mystream',  list_messages) 
 
 asyncio.run(publish())
 ```
 
+### Publishing with confirmation
+
+The Send method takes as parameter an handle function that will be called asynchronously when the message sent will be notified from the server to have been published.
+
+In this case the example will work like this:
+
+
+```python
+import asyncio
+from rstream import Producer, AMQPMessage, ConfirmationStatus
+
+def _on_publish_confirm_client(confirmation: ConfirmationStatus) -> None:
+
+     if confirmation.is_confirmed == True:
+        print("message id: " + str(confirmation.message_id) + " is confirmed")
+     else:
+         print("message id: " + str(confirmation.message_id) + " is not confirmed")
+
+
+async def publish():
+    async with Producer('localhost', username='guest', password='guest') as producer:
+        await producer.create_stream('mystream')
+
+        for i in range(100):
+            amqp_message = AMQPMessage(
+                body='hello: {}'.format(i),
+            )
+            await producer.send('mystream', amqp_message, on_publish_confirm=_on_publish_confirm_client) 
+
+asyncio.run(publish())
+```
+
+Same is valid also for send_batch.
+
+Please note that the publish confirmation callbacks are internally managed by the client and they are triggered in the Producer class.
+This means that when the Producer will terminate its scope and lifetime you will not be able to receive the remaining notifications if any.
+Depending on your scenario, you could add a synchronization mechanism (like an asyncio condition) to wait till all the notifications 
+have been received or you could use an asyncio.wait to give time for the callbacks to be invoked by the client.
+
+
+With `send_wait` instead will wait until the confirmation from the server is received.
+
 ### Consuming messages:
 
 ```python
 import asyncio
 import signal
 from rstream import Consumer, amqp_decoder, AMQPMessage
```

### Comparing `rstream-0.5.0/pyproject.toml` & `rstream-0.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rstream"
-version = "0.5.0"
+version = "0.6.0"
 description = "A python client for RabbitMQ Streams"
 authors = ["George Fortunatov <qweeeze@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/qweeze/rstream"
 repository = "https://github.com/qweeze/rstream"
 license = "MIT"
```

### Comparing `rstream-0.5.0/rstream/__init__.py` & `rstream-0.6.0/rstream/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+# Copyright 2023 VMware, Inc. All Rights Reserved.
+# SPDX-License-Identifier: MIT
+
 from importlib import metadata
 
 try:
     __version__ = metadata.version(__package__)
     __license__ = metadata.metadata(__package__)["license"]
 except metadata.PackageNotFoundError:
     __version__ = "dev"
     __license__ = None
 
 del metadata
 
 from .amqp import AMQPMessage, amqp_decoder  # noqa: E402
 from .constants import OffsetType  # noqa: E402
 from .consumer import Consumer  # noqa: E402
-from .producer import Producer, RawMessage  # noqa: E402
+from .producer import (  # noqa: E402
+    ConfirmationStatus,
+    Producer,
+    RawMessage,
+)
 
 __all__ = [
     "AMQPMessage",
     "amqp_decoder",
     "Consumer",
     "RawMessage",
     "Producer",
     "OffsetType",
+    "ConfirmationStatus",
 ]
```

### Comparing `rstream-0.5.0/rstream/amqp.py` & `rstream-0.6.0/rstream/amqp.py`

 * *Files identical despite different names*

### Comparing `rstream-0.5.0/rstream/client.py` & `rstream-0.6.0/rstream/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright 2023 VMware, Inc. All Rights Reserved.
+# SPDX-License-Identifier: MIT
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import ssl
 import time
 from collections import defaultdict
@@ -137,19 +140,19 @@
 
         fut: asyncio.Future[schema.Frame] = asyncio.Future()
         _key = frame_cls.key, corr_id
         self._waiters[_key].add(fut)
         fut.add_done_callback(self._waiters[_key].discard)
         return utils.TimeoutWrapper(fut, timeout)
 
-    async def sync_request(self, frame: schema.Frame, resp_schema: Type[FT]) -> FT:
+    async def sync_request(self, frame: schema.Frame, resp_schema: Type[FT], raise_exception=True) -> FT:
         waiter = self.wait_frame(resp_schema, frame.corr_id)
         await self.send_frame(frame)
         resp = await waiter
-        resp.check_response_code()
+        resp.check_response_code(raise_exception=raise_exception)
         return resp
 
     async def start(self) -> None:
         logger.info("Starting client %s:%s", self.host, self.port)
         assert self._conn is None
         self._conn = Connection(self.host, self.port, self._ssl_context)
         await self._conn.open()
@@ -420,14 +423,15 @@
             schema.DeclarePublisher(
                 self._corr_id_seq.next(),
                 publisher_id=publisher_id,
                 stream=stream,
                 reference=reference,
             ),
             resp_schema=schema.DeclarePublisherResponse,
+            raise_exception=False,
         )
 
     async def delete_publisher(self, publisher_id: int) -> None:
         await self.sync_request(
             schema.DeletePublisher(
                 self._corr_id_seq.next(),
                 publisher_id=publisher_id,
@@ -439,14 +443,15 @@
         resp = await self.sync_request(
             schema.QueryPublisherSequence(
                 self._corr_id_seq.next(),
                 publisher_ref=reference,
                 stream=stream,
             ),
             resp_schema=schema.QueryPublisherSequenceResponse,
+            raise_exception=False,
         )
         return resp.sequence
 
     async def publish(self, messages: list[schema.Message], publisher_id: int) -> None:
         await self.send_frame(
             schema.Publish(
                 publisher_id=publisher_id,
```

### Comparing `rstream-0.5.0/rstream/connection.py` & `rstream-0.6.0/rstream/connection.py`

 * *Files identical despite different names*

### Comparing `rstream-0.5.0/rstream/constants.py` & `rstream-0.6.0/rstream/constants.py`

 * *Files identical despite different names*

### Comparing `rstream-0.5.0/rstream/consumer.py` & `rstream-0.6.0/rstream/consumer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.5.0/rstream/encoding.py` & `rstream-0.6.0/rstream/encoding.py`

 * *Files identical despite different names*

### Comparing `rstream-0.5.0/rstream/exceptions.py` & `rstream-0.6.0/rstream/exceptions.py`

 * *Files identical despite different names*

### Comparing `rstream-0.5.0/rstream/producer.py` & `rstream-0.6.0/rstream/producer.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,21 +4,33 @@
 from __future__ import annotations
 
 import asyncio
 import ssl
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import partial
-from typing import Any, NoReturn, Optional, TypeVar
+from typing import (
+    Annotated,
+    Any,
+    Awaitable,
+    Callable,
+    Generic,
+    NoReturn,
+    Optional,
+    TypeVar,
+    Union,
+)
 
 from . import exceptions, schema, utils
 from .amqp import _MessageProtocol
 from .client import Addr, Client, ClientPool
 
 MessageT = TypeVar("MessageT", _MessageProtocol, bytes)
+MT = TypeVar("MT")
+CB = Annotated[Callable[[MT], Union[None, Awaitable[None]]], "Message callback type"]
 
 
 @dataclass
 class _Publisher:
     id: int
     reference: str
     stream: str
@@ -31,14 +43,27 @@
     data: bytes
     publishing_id: Optional[int] = None
 
     def __bytes__(self) -> bytes:
         return self.data
 
 
+@dataclass
+class _MessageNotification(Generic[MessageT]):
+    message: MessageT
+    callback: Optional[CB[ConfirmationStatus]] = None
+
+
+@dataclass
+class ConfirmationStatus:
+    message_id: int
+    is_confirmed: bool = False
+    response_code: int = 0
+
+
 class Producer:
     def __init__(
         self,
         host: str,
         port: int = 5552,
         *,
         ssl_context: Optional[ssl.SSLContext] = None,
@@ -62,15 +87,17 @@
             heartbeat=heartbeat,
             load_balancer_mode=load_balancer_mode,
             max_retries=max_retries,
         )
         self._default_client: Optional[Client] = None
         self._clients: dict[str, Client] = {}
         self._publishers: dict[str, _Publisher] = {}
-        self._waiting_for_confirm: dict[str, dict[asyncio.Future[None], set[int]]] = defaultdict(dict)
+        self._waiting_for_confirm: dict[
+            str, dict[asyncio.Future[None] | CB[ConfirmationStatus], set[int]]
+        ] = defaultdict(dict)
         self._lock = asyncio.Lock()
         # dictionary [stream][list] of buffered messages to send asynchronously
         self._buffered_messages: dict[str, list] = defaultdict(list)
         self._buffered_messages_lock = asyncio.Lock()
         self.task: asyncio.Task[NoReturn] | None = None
         # Delay After sending the messages on _buffered_messages list
         self._default_batch_publishing_delay = default_batch_publishing_delay
@@ -166,36 +193,42 @@
         return publisher
 
     async def send_batch(
         self,
         stream: str,
         batch: list[MessageT],
         publisher_name: Optional[str] = None,
+        on_publish_confirm: Optional[CB[ConfirmationStatus]] = None,
     ) -> list[int]:
 
-        return await self._send_batch(stream, batch, sync=False, publisher_name=publisher_name)
+        wrapped_batch = []
+        for item in batch:
+            wrapped_item = _MessageNotification(item, on_publish_confirm)
+            wrapped_batch.append(wrapped_item)
+
+        return await self._send_batch(stream, wrapped_batch, sync=False, publisher_name=publisher_name)
 
     async def _send_batch(
         self,
         stream: str,
-        batch: list[MessageT],
+        batch: list[_MessageNotification],
         sync: bool = True,
         publisher_name: Optional[str] = None,
     ) -> list[int]:
         if len(batch) == 0:
             raise ValueError("Empty batch")
 
         async with self._lock:
             publisher = await self._get_or_create_publisher(stream, publisher_name=publisher_name)
 
         messages = []
 
         for item in batch:
 
-            msg = RawMessage(item) if isinstance(item, bytes) else item
+            msg = RawMessage(item.message) if isinstance(item.message, bytes) else item.message
 
             if msg.publishing_id is None:
                 msg.publishing_id = publisher.sequence.next()
 
             messages.append(
                 schema.Message(
                     publishing_id=msg.publishing_id,
@@ -208,30 +241,35 @@
                 publisher_id=publisher.id,
                 messages=messages,
             ),
         )
 
         publishing_ids = [m.publishing_id for m in messages]
 
-        if sync:
+        if item.callback is not None:
+            self._waiting_for_confirm[publisher.reference][item.callback] = set(publishing_ids)
+        elif sync:
             future: asyncio.Future[None] = asyncio.Future()
             self._waiting_for_confirm[publisher.reference][future] = set(publishing_ids)
             await future
 
         return publishing_ids
 
     async def send_wait(
         self,
         stream: str,
         message: MessageT,
         publisher_name: Optional[str] = None,
     ) -> int:
+
+        wrapped_message: _MessageNotification = _MessageNotification(message, None)
+
         publishing_ids = await self._send_batch(
             stream,
-            [message],
+            [wrapped_message],
             sync=True,
             publisher_name=publisher_name,
         )
         return publishing_ids[0]
 
     def _timer_completed(self, context):
 
@@ -242,26 +280,28 @@
         return 0
 
     async def send(
         self,
         stream: str,
         message: MessageT,
         publisher_name: Optional[str] = None,
+        on_publish_confirm: Optional[CB[ConfirmationStatus]] = None,
     ):
 
         # start the background thread to send buffered messages
         if self.task is None:
             self.task = asyncio.create_task(self._timer())
             self.task.add_done_callback(self._timer_completed)
 
         async with self._lock:
             await self._get_or_create_publisher(stream, publisher_name=publisher_name)
 
+        wrapped_message = _MessageNotification(message, on_publish_confirm)
         async with self._buffered_messages_lock:
-            self._buffered_messages[stream].append(message)
+            self._buffered_messages[stream].append(wrapped_message)
 
         await asyncio.sleep(0)
 
     # After the timeout send the messages in _buffered_messages in batches
     async def _timer(self):
 
         while True:
@@ -273,44 +313,63 @@
 
         async with self._buffered_messages_lock:
             if len(self._buffered_messages[stream]):
                 await self._send_batch(stream, self._buffered_messages[stream], sync=False)
                 self._buffered_messages[stream].clear()
 
     def _on_publish_confirm(self, frame: schema.PublishConfirm, publisher: _Publisher) -> None:
+
         if frame.publisher_id != publisher.id:
             return
 
         waiting = self._waiting_for_confirm[publisher.reference]
-        for fut in list(waiting):
-            ids = waiting[fut]
+        for confirmation in list(waiting):
+            ids = waiting[confirmation]
+            ids_to_call = ids.intersection(frame.publishing_ids)
+
+            for id in ids_to_call:
+                if not isinstance(confirmation, asyncio.Future):
+                    confirmation_status: ConfirmationStatus = ConfirmationStatus(id, True)
+                    confirmation(confirmation_status)
             ids.difference_update(frame.publishing_ids)
             if not ids:
-                fut.set_result(None)
-                del waiting[fut]
+                del waiting[confirmation]
+                if isinstance(confirmation, asyncio.Future):
+                    confirmation.set_result(None)
 
     def _on_publish_error(self, frame: schema.PublishError, publisher: _Publisher) -> None:
+
         if frame.publisher_id != publisher.id:
             return
 
         waiting = self._waiting_for_confirm[publisher.reference]
         for error in frame.errors:
             exc = exceptions.ServerError.from_code(error.response_code)
-            for fut in list(waiting):
-                ids = waiting[fut]
+            for confirmation in list(waiting):
+                ids = waiting[confirmation]
                 if error.publishing_id in ids:
-                    fut.set_exception(exc)
-                    del waiting[fut]
+                    if not isinstance(confirmation, asyncio.Future):
+                        confirmation_status = ConfirmationStatus(
+                            error.publishing_id, False, error.response_code
+                        )
+                        confirmation(confirmation_status)
+                        ids.remove(error.publishing_id)
+
+                if not ids:
+                    del waiting[confirmation]
+                    if isinstance(confirmation, asyncio.Future):
+                        confirmation.set_exception(exc)
 
     async def create_stream(
         self,
         stream: str,
         arguments: Optional[dict[str, Any]] = None,
         exists_ok: bool = False,
     ) -> None:
+
         try:
             await self.default_client.create_stream(stream, arguments)
         except exceptions.StreamAlreadyExists:
             if not exists_ok:
                 raise
 
     async def delete_stream(self, stream: str, missing_ok: bool = False) -> None:
```

### Comparing `rstream-0.5.0/rstream/schema.py` & `rstream-0.6.0/rstream/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright 2023 VMware, Inc. All Rights Reserved.
+# SPDX-License-Identifier: MIT
+
 import zlib
 from dataclasses import dataclass, field
 from typing import ClassVar, Optional, Type, cast
 
 from .constants import Key, OffsetType, T
 from .exceptions import ServerError
 
@@ -25,17 +28,17 @@
             return cast(int, correlation_id)
         return None
 
     def __init_subclass__(cls, is_response: bool = False) -> None:
         assert cls.key is not NotImplemented
         registry[(is_response, cls.key)] = cls
 
-    def check_response_code(self) -> None:
+    def check_response_code(self, raise_exception: bool = True) -> None:
         code: int = getattr(self, "response_code", 0)
-        if code > 1:
+        if code > 1 and raise_exception is True:
             raise ServerError.from_code(code)
 
 
 @dataclass
 class Property(Struct):
     key: str = field(metadata={"type": T.string})
     value: str = field(metadata={"type": T.string})
@@ -231,18 +234,18 @@
 @dataclass
 class MetadataResponse(Frame, is_response=True):
     key = Key.Metadata
     correlation_id: int = field(metadata={"type": T.uint32})
     brokers: list[Broker]
     metadata: list[StreamMetadata]
 
-    def check_response_code(self) -> None:
+    def check_response_code(self, raise_exception: bool = True) -> None:
         for item in self.metadata:
             code = item.response_code
-            if code > 1:
+            if code > 1 and raise_exception is True:
                 raise ServerError.from_code(code)
 
 
 @dataclass
 class MetadataInfo(Struct):
     code: int = field(metadata={"type": T.uint16})
     stream: str = field(metadata={"type": T.string})
```

### Comparing `rstream-0.5.0/rstream/utils.py` & `rstream-0.6.0/rstream/utils.py`

 * *Files identical despite different names*

