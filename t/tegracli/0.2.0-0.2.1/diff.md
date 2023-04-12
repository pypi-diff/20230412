# Comparing `tmp/tegracli-0.2.0.tar.gz` & `tmp/tegracli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tegracli-0.2.0.tar", max compression
+gzip compressed data, was "tegracli-0.2.1.tar", max compression
```

## Comparing `tegracli-0.2.0.tar` & `tegracli-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.0/LICENSE
--rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.0/README.md
--rw-r--r--   0        0        0     1322 2023-04-12 14:06:28.899428 tegracli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.0/tegracli/__init__.py
--rw-r--r--   0        0        0     5026 2023-04-12 14:05:59.583449 tegracli-0.2.0/tegracli/dispatch.py
--rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.0/tegracli/group.py
--rw-r--r--   0        0        0    12827 2023-04-12 14:05:59.587449 tegracli-0.2.0/tegracli/main.py
--rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.0/tegracli/types.py
--rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.0/tegracli/utilities.py
--rw-r--r--   0        0        0     9481 1970-01-01 00:00:00.000000 tegracli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-10-24 15:55:29.200116 tegracli-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8456 2023-04-12 14:05:59.583449 tegracli-0.2.1/README.md
+-rw-r--r--   0        0        0     1322 2023-04-12 16:01:08.273768 tegracli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-04-11 13:51:38.330956 tegracli-0.2.1/tegracli/__init__.py
+-rw-r--r--   0        0        0     5336 2023-04-12 16:01:00.081752 tegracli-0.2.1/tegracli/dispatch.py
+-rw-r--r--   0        0        0     4578 2023-02-03 16:03:39.618393 tegracli-0.2.1/tegracli/group.py
+-rw-r--r--   0        0        0    12732 2023-04-12 16:01:00.081752 tegracli-0.2.1/tegracli/main.py
+-rw-r--r--   0        0        0      246 2023-02-03 16:03:39.618393 tegracli-0.2.1/tegracli/types.py
+-rw-r--r--   0        0        0     1578 2023-03-01 08:59:14.495867 tegracli-0.2.1/tegracli/utilities.py
+-rw-r--r--   0        0        0     9481 1970-01-01 00:00:00.000000 tegracli-0.2.1/PKG-INFO
```

### Comparing `tegracli-0.2.0/LICENSE` & `tegracli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.0/README.md` & `tegracli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.0/pyproject.toml` & `tegracli-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tegracli"
-version = "0.2.0"
+version = "0.2.1"
 description = "A research-focused Telegram CLI application"
 authors = ["Philipp Kessling <p.kessling@leibniz-hbi.de>", "Felix Münch <f.muench@lebniz-hbi.de>"]
 readme  = "README.md"
 license = "MIT"
 repository  = "https://github.com/Leibniz-HBI/tegracli"
 homepage = "https://pypi.org/project/tegracli/"
 classifiers = [
```

### Comparing `tegracli-0.2.0/tegracli/dispatch.py` & `tegracli-0.2.1/tegracli/dispatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Dispatch functions that request data from Telethon and MTProto."""
 import datetime
+import sys
 import time
 from functools import partial
 from io import TextIOWrapper
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import telethon
 import ujson
 from loguru import logger as log
 from telethon import TelegramClient
-from telethon.errors import FloodWaitError
+from telethon.errors import ChannelPrivateError, FloodWaitError, UserDeactivatedError
 
 from .types import MessageHandler
 from .utilities import str_dict
 
 # pylint: disable=I1101  # c-extensions-no-member; we know it's there and that's why we don't
 # want to see it
 
@@ -25,16 +26,22 @@
     """Dispatch a TG-method with callback.
 
     Args:
         client: the client to use.
         params: the parameters to pass to the method.
         callback: the callback to pass data to.
     """
-    async for message in client.iter_messages(wait_time=10, **params):
-        await callback(message)
+    try:
+        async for message in client.iter_messages(wait_time=10, **params):
+            await callback(message)
+    except UserDeactivatedError:
+        log.error("User account has been deactivated by Telegram. Stopping now.")
+        sys.exit(127)
+    except ChannelPrivateError:
+        log.error(f"Entity {params['entity']} is private. Skipping.")
 
 
 async def dispatch_get(users, client: TelegramClient, params: Dict):
     """Get the message history of a specified set of users."""
     for user in users:
         done = False
         while done is False:
```

### Comparing `tegracli-0.2.0/tegracli/group.py` & `tegracli-0.2.1/tegracli/group.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.0/tegracli/main.py` & `tegracli-0.2.1/tegracli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,19 @@
         if post_id is None:
             continue
         if channel not in channel_registry:
             channel_registry[channel] = [post_id]
         else:
             channel_registry[channel].append(post_id)
     with client:
-        for channel, post_ids in channel_registry.items():
-            client.loop.run_until_complete(
-                dispatch_hydrate(channel, post_ids, output_file, client)
-            )
+        with click.progressbar(channel_registry.items()) as channel_iter:
+            for channel, post_ids in channel_iter:
+                client.loop.run_until_complete(
+                    dispatch_hydrate(channel, post_ids, output_file, client)
+                )
 
 
 @cli.command()
 @click.option(
     "--limit", "-l", type=int, default=-1, help="Number of messages to retrieve."
 )
 @click.option(
@@ -331,25 +332,22 @@
     min_id = conf.get_last_message_for(member)
     if min_id is not None:
         _params["min_id"] = min_id
 
     log.debug(f"Request with the following parameters: {_params}")
 
     # request data from telethon and write to disk
-    try:
-        with (Path(conf.name) / (member + ".jsonl")).open("a") as member_file:
-            client.loop.run_until_complete(
-                dispatch_iter_messages(
-                    client,
-                    params=_params,
-                    callback=partial(handle_message, file=member_file, injects=None),
-                )
+    with (Path(conf.name) / (member + ".jsonl")).open("a") as member_file:
+        client.loop.run_until_complete(
+            dispatch_iter_messages(
+                client,
+                params=_params,
+                callback=partial(handle_message, file=member_file, injects=None),
             )
-    except telethon.errors.ChannelPrivateError:
-        log.error(f"channel {profile.get('username') or ''} is private. Skipping.")
+        )
 
 
 def run_group(client: TelegramClient, groups: Tuple[str]):
     """Runs the required operations for the specified groups."""
     cwd = Path()
 
     # iterate groups
```

### Comparing `tegracli-0.2.0/tegracli/utilities.py` & `tegracli-0.2.1/tegracli/utilities.py`

 * *Files identical despite different names*

### Comparing `tegracli-0.2.0/PKG-INFO` & `tegracli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tegracli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A research-focused Telegram CLI application
 Home-page: https://pypi.org/project/tegracli/
 License: MIT
 Author: Philipp Kessling
 Author-email: p.kessling@leibniz-hbi.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

