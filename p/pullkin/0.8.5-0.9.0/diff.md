# Comparing `tmp/pullkin-0.8.5.tar.gz` & `tmp/pullkin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pullkin-0.8.5.tar", last modified: Sat Feb 19 23:23:38 2022, max compression
+gzip compressed data, was "pullkin-0.9.0.tar", last modified: Sun Mar 13 16:17:58 2022, max compression
```

## Comparing `pullkin-0.8.5.tar` & `pullkin-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:38.638944 pullkin-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (116)    15549 2022-02-19 23:23:32.000000 pullkin-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3205 2022-02-19 23:23:38.638944 pullkin-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2338 2022-02-19 23:23:32.000000 pullkin-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:38.634944 pullkin-0.8.5/pullkin/
--rw-r--r--   0 runner    (1001) docker     (116)       62 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11940 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/aioclient.py
--rw-r--r--   0 runner    (1001) docker     (116)     5850 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     9008 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/client_base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:38.638944 pullkin-0.8.5/pullkin/models/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1150 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:38.638944 pullkin-0.8.5/pullkin/proto/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2968 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/proto/android_checkin_proto.py
--rw-r--r--   0 runner    (1001) docker     (116)     8773 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/proto/checkin_proto.py
--rw-r--r--   0 runner    (1001) docker     (116)     8499 2022-02-19 23:23:32.000000 pullkin-0.8.5/pullkin/proto/mcs_proto.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:38.634944 pullkin-0.8.5/pullkin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3205 2022-02-19 23:23:38.000000 pullkin-0.8.5/pullkin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      503 2022-02-19 23:23:38.000000 pullkin-0.8.5/pullkin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-19 23:23:38.000000 pullkin-0.8.5/pullkin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      135 2022-02-19 23:23:38.000000 pullkin-0.8.5/pullkin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-02-19 23:23:38.000000 pullkin-0.8.5/pullkin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-19 23:23:38.638944 pullkin-0.8.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     1319 2022-02-19 23:23:32.000000 pullkin-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:38.638944 pullkin-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-19 23:23:32.000000 pullkin-0.8.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      285 2022-02-19 23:23:32.000000 pullkin-0.8.5/tests/test_registration.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:58.190332 pullkin-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)    15549 2022-03-13 16:17:54.000000 pullkin-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     3533 2022-03-13 16:17:58.190332 pullkin-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2666 2022-03-13 16:17:54.000000 pullkin-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:58.190332 pullkin-0.9.0/pullkin/
+-rw-r--r--   0 runner    (1001) docker     (116)       62 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12433 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/aioclient.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5862 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9268 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/client_base.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:58.190332 pullkin-0.9.0/pullkin/models/
+-rw-r--r--   0 runner    (1001) docker     (116)      194 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      761 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/models/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1150 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:58.190332 pullkin-0.9.0/pullkin/proto/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2968 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/proto/android_checkin_proto.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8773 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/proto/checkin_proto.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8499 2022-03-13 16:17:54.000000 pullkin-0.9.0/pullkin/proto/mcs_proto.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:58.190332 pullkin-0.9.0/pullkin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3533 2022-03-13 16:17:57.000000 pullkin-0.9.0/pullkin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      613 2022-03-13 16:17:58.000000 pullkin-0.9.0/pullkin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-13 16:17:57.000000 pullkin-0.9.0/pullkin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      157 2022-03-13 16:17:58.000000 pullkin-0.9.0/pullkin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2022-03-13 16:17:58.000000 pullkin-0.9.0/pullkin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-03-13 16:17:58.190332 pullkin-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1320 2022-03-13 16:17:54.000000 pullkin-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:58.190332 pullkin-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-03-13 16:17:54.000000 pullkin-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      856 2022-03-13 16:17:54.000000 pullkin-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)      228 2022-03-13 16:17:54.000000 pullkin-0.9.0/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1013 2022-03-13 16:17:54.000000 pullkin-0.9.0/tests/test_receiving.py
+-rw-r--r--   0 runner    (1001) docker     (116)      430 2022-03-13 16:17:54.000000 pullkin-0.9.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (116)      262 2022-03-13 16:17:54.000000 pullkin-0.9.0/tests/testdata.py
```

### Comparing `pullkin-0.8.5/LICENSE` & `pullkin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pullkin-0.8.5/PKG-INFO` & `pullkin-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pullkin
-Version: 0.8.5
+Version: 0.9.0
 Summary: Like Pushkin, but subscribe to GCM/FCM and receive notifications
 Home-page: https://github.com/WhiteApfel/pullkin
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: Mozilla Public License 2.0
 Keywords: fcm gcm push notification receive firebase google
 Platform: UNKNOWN
@@ -20,15 +20,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pullkin
 
 [![CodeFactor](https://www.codefactor.io/repository/github/whiteapfel/pullkin/badge/master)](https://www.codefactor.io/repository/github/whiteapfel/pullkin/overview/master)
 [![Build Status](https://app.travis-ci.com/WhiteApfel/Pullkin.svg?branch=master)](https://app.travis-ci.com/WhiteApfel/Pullkin)
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FWhiteApfel%2FPullkin.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FWhiteApfel%2FPullkin?ref=badge_shield)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pullkin)
 ![GitHub](https://img.shields.io/github/license/whiteapfel/pullkin)
 ![GitHub last commit](https://img.shields.io/github/last-commit/whiteapfel/pullkin)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pullkin)
 
 Like Pushkin, but subscribe to FCM (GCM) and receive notifications
 
@@ -59,21 +58,28 @@
 ```shell
 pip install pullkin
 ```
 
 ### How to use
 
 ```python
+import json
+import os.path
 import asyncio
 
 from pullkin import AioPullkin
-from pullkin.models.message import Message
+from pullkin.models import Message, AppCredentials
 
+SENDER_ID = '<<SENDER_ID>>'
 pullkin = AioPullkin()
 
+if not os.path.exists('.persistent_ids.txt'):
+        with open('.persistent_ids.txt', 'w+') as f:
+            ...
+
 with open(".persistent_ids.txt", "r") as f:
     received_persistent_ids = [x.strip() for x in f]
 
 
 @pullkin.on_notification()
 async def on_notification(obj, message: Message, data_message):
     idstr = data_message.persistent_id + "\n"
@@ -82,13 +88,20 @@
             return
     with open(".persistent_ids.txt", "a") as f:
         f.write(idstr)
     print(message.notification)
 
 
 async def main():
-    await pullkin.listen_forever()
+    if not os.path.exists('.pullkin_app_credentials'):
+        with open('.pullkin_app_credentials', 'w+') as f:
+            credentials = pullkin.register(SENDER_ID)
+            f.write(json.dumps(credentials.dict()))
+    else:
+        with open('.pullkin_app_credentials', 'r') as f:
+            pullkin.credentials = AppCredentials(**json.loads(f.read()))
+    await pullkin.run()
 
 
 asyncio.run(main())
 ```
```

### Comparing `pullkin-0.8.5/README.md` & `pullkin-0.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Pullkin
 
 [![CodeFactor](https://www.codefactor.io/repository/github/whiteapfel/pullkin/badge/master)](https://www.codefactor.io/repository/github/whiteapfel/pullkin/overview/master)
 [![Build Status](https://app.travis-ci.com/WhiteApfel/Pullkin.svg?branch=master)](https://app.travis-ci.com/WhiteApfel/Pullkin)
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FWhiteApfel%2FPullkin.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FWhiteApfel%2FPullkin?ref=badge_shield)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pullkin)
 ![GitHub](https://img.shields.io/github/license/whiteapfel/pullkin)
 ![GitHub last commit](https://img.shields.io/github/last-commit/whiteapfel/pullkin)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pullkin)
 
 Like Pushkin, but subscribe to FCM (GCM) and receive notifications
 
@@ -37,21 +36,28 @@
 ```shell
 pip install pullkin
 ```
 
 ### How to use
 
 ```python
+import json
+import os.path
 import asyncio
 
 from pullkin import AioPullkin
-from pullkin.models.message import Message
+from pullkin.models import Message, AppCredentials
 
+SENDER_ID = '<<SENDER_ID>>'
 pullkin = AioPullkin()
 
+if not os.path.exists('.persistent_ids.txt'):
+        with open('.persistent_ids.txt', 'w+') as f:
+            ...
+
 with open(".persistent_ids.txt", "r") as f:
     received_persistent_ids = [x.strip() for x in f]
 
 
 @pullkin.on_notification()
 async def on_notification(obj, message: Message, data_message):
     idstr = data_message.persistent_id + "\n"
@@ -60,12 +66,19 @@
             return
     with open(".persistent_ids.txt", "a") as f:
         f.write(idstr)
     print(message.notification)
 
 
 async def main():
-    await pullkin.listen_forever()
+    if not os.path.exists('.pullkin_app_credentials'):
+        with open('.pullkin_app_credentials', 'w+') as f:
+            credentials = pullkin.register(SENDER_ID)
+            f.write(json.dumps(credentials.dict()))
+    else:
+        with open('.pullkin_app_credentials', 'r') as f:
+            pullkin.credentials = AppCredentials(**json.loads(f.read()))
+    await pullkin.run()
 
 
 asyncio.run(main())
 ```
```

### Comparing `pullkin-0.8.5/pullkin/aioclient.py` & `pullkin-0.9.0/pullkin/aioclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 import inspect
 import json
 import struct
 import traceback
 from asyncio import StreamReader, StreamWriter
 from base64 import urlsafe_b64decode
 from binascii import hexlify
-from typing import Callable, Optional, Union, AsyncGenerator
+from typing import AsyncGenerator, Callable, Optional, Union
 
 import cryptography.hazmat.primitives.serialization as serialization
 import http_ece
 from cryptography.hazmat.backends import default_backend
 from loguru import logger
 
 from pullkin.client_base import PullkinBase
-from pullkin.proto.mcs_proto import *
 from pullkin.models.message import Message
+from pullkin.proto.mcs_proto import *  # noqa: F403
 
 logger.disable("pullkin")
 
 
 class AioPullkin(PullkinBase):
     def __init__(self):
         super().__init__()
         self.__reader: Optional[StreamReader] = None
         self.__writer: Optional[StreamWriter] = None
-        self.credentials: dict = {}
         self.persistent_ids: list = []
         self.callback: Callable = None
         self.on_notification_handlers: list = []
         self.once = True
+        self._started = False
 
-    def on_notification(self, filter: Callable = lambda *a, **k: True):
+    def on_notification(self, handler_filter: Callable = lambda *a, **k: True):
         """
         Decorator
 
         Registers a new callback with filter rule to trigger this callback
 
         First param to be passed into filter or callback: some object. Now is empty dict.
         Later you will be able to passed your object
@@ -57,22 +57,22 @@
                 await asyncio.sleep(2)
                 print("=-)")
 
         """
 
         def decorator(callback):
             self.on_notification_handlers.append(
-                {"callback": callback, "filter": filter}
+                {"callback": callback, "filter": handler_filter}
             )
             return callback
 
         return decorator
 
     def register_on_notification_handler(
-        self, filter: Callable = None, callback: Callable = None
+        self, handler_filter: Callable = None, callback: Callable = None
     ):
         """
         Function
 
         Registers a new callback with filter rule to trigger this callback
 
         filter: rule for calling thit callback
@@ -95,15 +95,17 @@
             async def on_normal(obj: dict, notification: Notification, message: Message):
                 print(f"#{message.id} @{message.sent})
                 print(notification")
                 await asyncio.sleep(2)
                 print("=-)")
 
         """
-        self.on_notification_handlers.append({"callback": callback, "filter": filter})
+        self.on_notification_handlers.append(
+            {"callback": callback, "filter": handler_filter}
+        )
 
     async def __run_on_notification_callbacks(self, obj, notification, data_message):
         x = 0
         for handler in self.on_notification_handlers:
             if handler["filter"](obj, notification, data_message):
                 if inspect.iscoroutinefunction(handler["callback"]):
                     await handler["callback"](obj, notification, data_message)
@@ -116,24 +118,23 @@
             if self.callback:
                 if inspect.iscoroutinefunction(self.callback):
                     await self.callback(obj, notification, data_message)
                 else:
                     self.callback(obj, notification, data_message)
 
         if not x:
-            logger.debug('No one callback was called')
+            logger.debug("No one callback was called")
 
-    @classmethod
-    async def aioregister(cls, sender_id):
+    async def aioregister(self, sender_id):
         """
         Async version. Register "app" for receive pushed
 
         Returns "app"-credential in dict for receive "personal" push by token
         """
-        return await cls._register(sender_id)
+        return await self._register(sender_id)
 
     async def __open_connection(self) -> None:
         import ssl
 
         ssl_ctx = ssl.create_default_context()
         self.__reader, self.__writer = await asyncio.open_connection(
             self.PUSH_HOST, self.PUSH_PORT, ssl=ssl_ctx
@@ -156,25 +157,25 @@
             res |= (b & 0x7F) << shift
             if (b & 0x80) == 0:
                 break
             shift += 7
         return res
 
     async def __aiosend(self, packet) -> None:
-        logger.debug(f"Send")
+        logger.debug("Send")
         header = bytearray([self.MCS_VERSION, self.PACKET_BY_TAG.index(type(packet))])
         logger.debug(f"Packet:\n'{packet}'")
         payload = packet.SerializeToString()
         buf = bytes(header) + self._encode_varint32(len(payload)) + payload
         logger.debug(f"HEX buffer:\n`{hexlify(buf)}`")
         self.__writer.write(buf)
         await self.__writer.drain()
 
     async def __aiorecv(self, first=False) -> Optional[PullkinBase.packet_union]:
-        logger.debug(f"Receive")
+        logger.debug("Receive")
         if first:
             version, tag = struct.unpack("BB", await self.__aioread(2))
             logger.debug(f"Version {version}")
             if version < self.MCS_VERSION and version != 38:
                 raise RuntimeError(f"Protocol version {version} unsupported")
         else:
             (tag,) = struct.unpack("B", await self.__aioread(1))
@@ -189,15 +190,15 @@
             payload.parse(buf)
             logger.debug(f"Payload:\n`{payload}`")
             return payload
         return None
 
     async def __aiolisten_once(
         self,
-    ) -> None:
+    ) -> Message:
         load_der_private_key = serialization.load_der_private_key
 
         p = await self.__aiorecv()
         if type(p) is not DataMessageStanza:
             return
         if self._is_deleted_message(p):
             return
@@ -206,49 +207,51 @@
         logger.debug(f"crypto-key: {crypto_key}, salt: {salt}")
         if not (salt and crypto_key):
             return
         crypto_key = crypto_key[3:]  # strip dh=
         salt = salt[5:]  # strip salt=
         crypto_key = urlsafe_b64decode(crypto_key.encode("ascii"))
         salt = urlsafe_b64decode(salt.encode("ascii"))
-        der_data = self.credentials["keys"]["private"]
+        der_data = self.credentials.keys.private
         der_data = urlsafe_b64decode(der_data.encode("ascii") + b"========")
-        secret = self.credentials["keys"]["secret"]
+        secret = self.credentials.keys.secret
         secret = urlsafe_b64decode(secret.encode("ascii") + b"========")
         privkey = load_der_private_key(
             der_data, password=None, backend=default_backend()
         )
         decrypted = http_ece.decrypt(
             p.raw_data,
             salt=salt,
             private_key=privkey,
             dh=crypto_key,
             version="aesgcm",
             auth_secret=secret,
         )
         notification = Message(json.loads(decrypted.decode("utf-8")))
         await self.__run_on_notification_callbacks({}, notification, p)
+        return notification
 
-    async def __aiolisten_start(self) -> None:
-        await self.gcm_check_in(**self.credentials["gcm"])
+    async def _aiolisten_start(self) -> None:
+        await self.gcm_check_in(self.credentials.gcm)
         req = LoginRequest()
         req.adaptive_heartbeat = False
         req.auth_service = 2
-        req.auth_token = self.credentials["gcm"]["securityToken"]
+        req.auth_token = self.credentials.gcm.securityToken
         req.id = "chrome-91.0.3234.0"
         req.domain = "mcs.android.com"
-        req.device_id = "android-%x" % int(self.credentials["gcm"]["androidId"])
+        req.device_id = "android-%x" % int(self.credentials.gcm.androidId)
         req.network_type = 1
-        req.resource = self.credentials["gcm"]["androidId"]
-        req.user = self.credentials["gcm"]["androidId"]
+        req.resource = self.credentials.gcm.androidId
+        req.user = self.credentials.gcm.androidId
         req.use_rmq2 = True
         req.setting.append(Setting(name="new_vc", value="1"))
         req.received_persistent_id.extend(self.persistent_ids)
         await self.__aiosend(req)
         await self.__aiorecv(first=True)
+        self._started = True
 
     async def __aiolisten_coroutine(self) -> AsyncGenerator:
         while True:
             yield await self.__aiolisten_once()
 
     async def listen_coroutine(self) -> AsyncGenerator:
         """
@@ -271,43 +274,55 @@
 
             # <some code>
 
         :return: coroutine
         """
         if not (self.__reader or self.__writer):
             await self.__open_connection()
-        await self.__aiolisten_start()
+        await self._aiolisten_start()
         coroutine = self.__aiolisten_coroutine()
         return coroutine
 
-    async def listen_forever(self, timer: Union[int, float] = 0.05) -> None:
-        """
-        Listens for push notifications
-
-        Runs an endless loop for reading notifications and distributing among callbacks based on filter results
+    async def _wait_start(self):
+        while not all([self._started, self.__reader, self.__writer]):
+            await asyncio.sleep(0.1)
 
-        :param timer: timer in seconds between receive iteration
-        :type timer: ``int`` or ``float``, optional, default ``0.05``
-        """
+    async def _run_listener(self, timer: Union[int, float] = 0.05) -> None:
         if not (self.__reader or self.__writer):
             await self.__open_connection()
 
-        await self.__aiolisten_start()
+        await self._aiolisten_start()
         coroutine = self.__aiolisten_coroutine()
         try:
             while self.__reader and self.__writer:
                 await coroutine.asend(None)
                 await asyncio.sleep(timer)
-        except Exception as e:
+        except Exception:
             print(traceback.format_exc())
         finally:
             if self.__writer:
                 self.__writer.close()
                 await self.__writer.wait_closed()
 
+    async def run(self, timer: Union[int, float] = 0.05) -> None:
+        """
+        Listens for push notifications
+
+        Runs an endless loop for reading notifications and distributing among callbacks based on filter results
+
+        :param timer: timer in seconds between receive iteration
+        :type timer: ``int`` or ``float``, optional, default ``0.05``
+        """
+
+        asyncio.ensure_future(self._run_listener(timer))
+        try:
+            await asyncio.wait(self._wait_start(), timeout=10)
+        except asyncio.exceptions.TimeoutError:
+            print("Timeout start listener 10s")
+
     async def close(self):
         try:
             if self._http_client:
                 await self._http_client.aclose()
                 self._http_client = None
             if self.__writer:
                 self.__writer.close()
```

### Comparing `pullkin-0.8.5/pullkin/client.py` & `pullkin-0.9.0/pullkin/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 from base64 import urlsafe_b64decode
 from binascii import hexlify
 
 from loguru import logger
 
 from pullkin.client_base import PullkinBase
-from pullkin.proto.mcs_proto import *
+from pullkin.proto.mcs_proto import *  # noqa: F403
 
 logger.disable("pullkin")
 
 
 class Pullkin(PullkinBase):
     def __init__(self):
         super().__init__()
@@ -33,30 +33,30 @@
             res |= (b & 0x7F) << shift
             if (b & 0x80) == 0:
                 break
             shift += 7
         return res
 
     def __send(self, s, packet):
-        logger.debug(f"Send")
+        logger.debug("Send")
         header = bytearray([self.MCS_VERSION, self.PACKET_BY_TAG.index(type(packet))])
         logger.debug(f"Packet:\n`{packet}`")
         payload = packet.SerializeToString()
         buf = bytes(header) + self._encode_varint32(len(payload)) + payload
         logger.debug(f"HEX buffer:\n`{hexlify(buf)}`")
         n = len(buf)
         total = 0
         while total < n:
             sent = s.send(buf[total:])
             if sent == 0:
                 raise RuntimeError("socket connection broken")
             total += sent
 
     def __recv(self, s, first=False):
-        logger.debug(f"Receive")
+        logger.debug("Receive")
         if first:
             version, tag = struct.unpack("BB", self.__read(s, 2))
             logger.debug(f"Version {version}")
             if version < self.MCS_VERSION and version != 38:
                 raise RuntimeError("protocol version {} unsupported".format(version))
         else:
             (tag,) = struct.unpack("B", self.__read(s, 1))
```

### Comparing `pullkin-0.8.5/pullkin/client_base.py` & `pullkin-0.9.0/pullkin/client_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import asyncio
 import json
 import os
 import time
 from base64 import urlsafe_b64encode
-from typing import Union
+from typing import Optional, Union
 from urllib.parse import urlencode
 
 import nest_asyncio
 from httpx import AsyncClient, Request
 from loguru import logger
 from oscrypto.asymmetric import generate_pair
 
+from pullkin.models import AppCredentials, AppCredentialsGcm
 from pullkin.proto.android_checkin_proto import AndroidCheckinProto, ChromeBuildProto
 from pullkin.proto.checkin_proto import AndroidCheckinRequest, AndroidCheckinResponse
-from pullkin.proto.mcs_proto import *
+from pullkin.proto.mcs_proto import *  # noqa: F403
 
 nest_asyncio.apply()
 logger.disable("pullkin")
 
 
 class PullkinBase:
     unicode = str
@@ -66,14 +67,15 @@
         IqStanza,
         DataMessageStanza,
         StreamErrorStanza,
     ]
 
     def __init__(self):
         self._http_client = None
+        self.credentials: AppCredentials = None
 
     @property
     def http_client(self):
         if not self._http_client:
             self._http_client = AsyncClient()
         return self._http_client
 
@@ -85,22 +87,22 @@
     async def _do_request(self, req, retries=5):
         for _ in range(retries):
             try:
                 resp = await self.http_client.send(req, follow_redirects=True)
                 resp_data = resp.content
                 logger.debug(f"Response:\n{resp_data}")
                 return resp_data
-            except ValueError as e:
+            except ValueError:
                 ...
             except Exception as e:
                 logger.opt(exception=e).error("Error during request:")
                 time.sleep(1)
         raise ConnectionError(f"Error during request: {e}")
 
-    async def gcm_check_in(self, androidId=None, securityToken=None, **_):
+    async def gcm_check_in(self, credentials: Optional[AppCredentialsGcm] = None):
         """
         perform check-in request
 
         androidId, securityToken can be provided if we already did the initial
         check-in
 
         returns dict with androidId, securityToken and more
@@ -114,26 +116,25 @@
         checkin.type = 3
         checkin.chrome_build.from_dict(chrome.to_dict())
 
         payload = AndroidCheckinRequest()
         payload.user_serial_number = 0
         payload.checkin.from_dict(checkin.to_dict())
         payload.version = 3
-        if androidId:
-            payload.id = int(androidId)
-        if securityToken:
-            payload.security_token = int(securityToken)
+        if credentials:
+            payload.id = int(credentials.androidId)
+            payload.security_token = int(credentials.securityToken)
 
         logger.debug(f"Payload:\n{payload}")
         req = self.http_client.build_request(
             method="POST",
             url=self.CHECKIN_URL,
             headers={"Content-Type": "application/x-protobuf"},
             content=payload.SerializeToString(),
-            timeout=5
+            timeout=5,
         )
         resp_data = await self._do_request(req)
         resp = AndroidCheckinResponse()
         resp.parse(resp_data)
         logger.debug(f"Response:\n{resp}")
         return resp.to_dict()
 
@@ -185,15 +186,15 @@
             token = resp_data.decode("utf-8").split("=")[1]
             chkfields = {k: chk[k] for k in ["androidId", "securityToken"]}
             res = {"token": token, "appId": appId}
             res.update(chkfields)
             return res
         return None
 
-    async def fcm_register(self, sender_id, token, retries=5):
+    async def fcm_register(self, sender_id: Union[str, int], token, retries=5):
         """
         generates key pair and obtains a fcm token
 
         sender_id: sender id as an integer
         token: the subscription token in the dict returned by gcm_register
 
         returns {"keys": keys, "fcm": {...}}
@@ -211,43 +212,44 @@
         logger.debug(b64encode(private.asn1.dump()))
         keys = {
             "public": self.urlsafe_base64(public.asn1.dump()[26:]),
             "private": self.urlsafe_base64(private.asn1.dump()),
             "secret": self.urlsafe_base64(os.urandom(16)),
         }
         body = {
-            "authorized_entity": sender_id,
+            "authorized_entity": int(sender_id),
             "endpoint": "{}/{}".format(self.FCM_ENDPOINT, token),
             "encryption_key": keys["public"],
             "encryption_auth": keys["secret"],
         }
         logger.debug(f"Data:\n{body}")
         req = Request(method="POST", url=self.FCM_SUBSCRIBE, data=body)
         resp_data = await self._do_request(req, retries)
         return {"keys": keys, "fcm": json.loads(resp_data.decode("utf-8"))}
 
-    async def _register(self, sender_id):
+    async def _register(self, sender_id: Union[str, int]):
         """register gcm and fcm tokens for sender_id"""
         app_id = "1:302251869498:android:90c5cd74bae68792813c03"
         subscription = await self.gcm_register(appId=app_id)
         logger.debug(f"GCM subscription data: {subscription}")
         fcm = await self.fcm_register(sender_id=sender_id, token=subscription["token"])
         logger.debug(f"FCM subscription data: {fcm}")
         res = {"gcm": subscription}
         res.update(fcm)
         return res
 
-    def register(self, sender_id):
+    def register(self, sender_id: Union[str, int]):
         """
         Sync version. Register "app" for receive pushed
 
         Returns "app"-credential in dict for receive "personal" push by token
         """
         res = asyncio.get_event_loop().run_until_complete(self._register(sender_id))
-        return res
+        self.credentials = AppCredentials(**res)
+        return AppCredentials(**res)
 
     @classmethod
     def _encode_varint32(cls, x):
         res = bytearray([])
         while x != 0:
             b = x & 0x7F
             x >>= 7
```

### Comparing `pullkin-0.8.5/pullkin/models/message.py` & `pullkin-0.9.0/pullkin/models/message.py`

 * *Files identical despite different names*

### Comparing `pullkin-0.8.5/pullkin/proto/android_checkin_proto.py` & `pullkin-0.9.0/pullkin/proto/android_checkin_proto.py`

 * *Files identical despite different names*

### Comparing `pullkin-0.8.5/pullkin/proto/checkin_proto.py` & `pullkin-0.9.0/pullkin/proto/checkin_proto.py`

 * *Files identical despite different names*

### Comparing `pullkin-0.8.5/pullkin/proto/mcs_proto.py` & `pullkin-0.9.0/pullkin/proto/mcs_proto.py`

 * *Files identical despite different names*

### Comparing `pullkin-0.8.5/pullkin.egg-info/PKG-INFO` & `pullkin-0.9.0/pullkin.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pullkin
-Version: 0.8.5
+Version: 0.9.0
 Summary: Like Pushkin, but subscribe to GCM/FCM and receive notifications
 Home-page: https://github.com/WhiteApfel/pullkin
 Author: WhiteApfel
 Author-email: white@pfel.ru
 License: Mozilla Public License 2.0
 Keywords: fcm gcm push notification receive firebase google
 Platform: UNKNOWN
@@ -20,15 +20,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pullkin
 
 [![CodeFactor](https://www.codefactor.io/repository/github/whiteapfel/pullkin/badge/master)](https://www.codefactor.io/repository/github/whiteapfel/pullkin/overview/master)
 [![Build Status](https://app.travis-ci.com/WhiteApfel/Pullkin.svg?branch=master)](https://app.travis-ci.com/WhiteApfel/Pullkin)
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FWhiteApfel%2FPullkin.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FWhiteApfel%2FPullkin?ref=badge_shield)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pullkin)
 ![GitHub](https://img.shields.io/github/license/whiteapfel/pullkin)
 ![GitHub last commit](https://img.shields.io/github/last-commit/whiteapfel/pullkin)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pullkin)
 
 Like Pushkin, but subscribe to FCM (GCM) and receive notifications
 
@@ -59,21 +58,28 @@
 ```shell
 pip install pullkin
 ```
 
 ### How to use
 
 ```python
+import json
+import os.path
 import asyncio
 
 from pullkin import AioPullkin
-from pullkin.models.message import Message
+from pullkin.models import Message, AppCredentials
 
+SENDER_ID = '<<SENDER_ID>>'
 pullkin = AioPullkin()
 
+if not os.path.exists('.persistent_ids.txt'):
+        with open('.persistent_ids.txt', 'w+') as f:
+            ...
+
 with open(".persistent_ids.txt", "r") as f:
     received_persistent_ids = [x.strip() for x in f]
 
 
 @pullkin.on_notification()
 async def on_notification(obj, message: Message, data_message):
     idstr = data_message.persistent_id + "\n"
@@ -82,13 +88,20 @@
             return
     with open(".persistent_ids.txt", "a") as f:
         f.write(idstr)
     print(message.notification)
 
 
 async def main():
-    await pullkin.listen_forever()
+    if not os.path.exists('.pullkin_app_credentials'):
+        with open('.pullkin_app_credentials', 'w+') as f:
+            credentials = pullkin.register(SENDER_ID)
+            f.write(json.dumps(credentials.dict()))
+    else:
+        with open('.pullkin_app_credentials', 'r') as f:
+            pullkin.credentials = AppCredentials(**json.loads(f.read()))
+    await pullkin.run()
 
 
 asyncio.run(main())
 ```
```

### Comparing `pullkin-0.8.5/setup.py` & `pullkin-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,9 +33,9 @@
     packages=find_packages("."),
     description="Like Pushkin, but subscribe to GCM/FCM and receive notifications",
     long_description=push_receiver_readme,
     long_description_content_type="text/markdown",
     license="Mozilla Public License 2.0",
     classifiers=pullkin_classifiers,
     keywords="fcm gcm push notification receive firebase google",
-    install_requires=requirements()
+    install_requires=requirements(),
 )
```

