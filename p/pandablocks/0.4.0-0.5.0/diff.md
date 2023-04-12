# Comparing `tmp/pandablocks-0.4.0.tar.gz` & `tmp/pandablocks-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PandABlocks-client/PandABlocks-client/dist/tmpqq8370mu/pandablocks-0.4.0.tar", last modified: Thu Mar 23 09:24:26 2023, max compression
+gzip compressed data, was "/home/runner/work/PandABlocks-client/PandABlocks-client/dist/tmpg6038ak2/pandablocks-0.5.0.tar", last modified: Wed Apr 12 12:16:32 2023, max compression
```

## Comparing `pandablocks-0.4.0.tar` & `pandablocks-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:24:26.000000 pandablocks-0.4.0/
--rw-rw-r--   0 runner    (1001) docker     (123)     4091 2023-03-23 09:24:26.000000 pandablocks-0.4.0/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (123)     2890 2023-03-23 09:23:40.000000 pandablocks-0.4.0/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks/
--rw-rw-r--   0 runner    (1001) docker     (123)       76 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)      122 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     5568 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/_control.py
--rw-rw-r--   0 runner    (1001) docker     (123)      961 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/_exchange.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3820 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks/_version_git.py
--rw-rw-r--   0 runner    (1001) docker     (123)     5652 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/asyncio.py
--rw-rw-r--   0 runner    (1001) docker     (123)     4416 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/blocking.py
--rw-rw-r--   0 runner    (1001) docker     (123)     4575 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/cli.py
--rw-rw-r--   0 runner    (1001) docker     (123)    30188 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/commands.py
--rw-rw-r--   0 runner    (1001) docker     (123)    16410 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/connections.py
--rw-rw-r--   0 runner    (1001) docker     (123)     7911 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/hdf.py
--rw-rw-r--   0 runner    (1001) docker     (123)     8017 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/responses.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks/saves/
--rw-rw-r--   0 runner    (1001) docker     (123)    15831 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pandablocks/saves/tutorial.sav
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks.egg-info/
--rw-rw-r--   0 runner    (1001) docker     (123)     4091 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (123)      573 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1001) docker     (123)        1 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1001) docker     (123)       53 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1001) docker     (123)       59 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks.egg-info/requires.txt
--rw-rw-r--   0 runner    (1001) docker     (123)       12 2023-03-23 09:24:26.000000 pandablocks-0.4.0/pandablocks.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      172 2023-03-23 09:23:40.000000 pandablocks-0.4.0/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (123)     1519 2023-03-23 09:24:26.000000 pandablocks-0.4.0/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (123)      500 2023-03-23 09:23:40.000000 pandablocks-0.4.0/setup.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:32.000000 pandablocks-0.5.0/
+-rw-rw-r--   0 runner    (1001) docker     (123)     4091 2023-04-12 12:16:32.000000 pandablocks-0.5.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (123)     2890 2023-04-12 12:15:47.000000 pandablocks-0.5.0/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks/
+-rw-rw-r--   0 runner    (1001) docker     (123)       76 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      122 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     5568 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/_control.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      961 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/_exchange.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3820 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks/_version_git.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     6386 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/asyncio.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     4416 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/blocking.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     4575 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/cli.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    30188 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/commands.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    16410 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/connections.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     7911 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/hdf.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     8017 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/responses.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks/saves/
+-rw-rw-r--   0 runner    (1001) docker     (123)    15831 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pandablocks/saves/tutorial.sav
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks.egg-info/
+-rw-rw-r--   0 runner    (1001) docker     (123)     4091 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (123)      573 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)       53 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)       59 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)       12 2023-04-12 12:16:32.000000 pandablocks-0.5.0/pandablocks.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      172 2023-04-12 12:15:47.000000 pandablocks-0.5.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (123)     1519 2023-04-12 12:16:32.000000 pandablocks-0.5.0/setup.cfg
+-rw-rw-r--   0 runner    (1001) docker     (123)      500 2023-04-12 12:15:47.000000 pandablocks-0.5.0/setup.py
```

### Comparing `pandablocks-0.4.0/PKG-INFO` & `pandablocks-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandablocks
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python client to control and data ports of the PandABlocks TCP server
 Home-page: https://github.com/PandABlocks/PandABlocks-client
 Author: Tom Cobb
 Author-email: tom.cobb@diamond.ac.uk
 License: Apache License 2.0
 Description: PandABlocks Python Client
         =========================
```

### Comparing `pandablocks-0.4.0/README.rst` & `pandablocks-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/_control.py` & `pandablocks-0.5.0/pandablocks/_control.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/_exchange.py` & `pandablocks-0.5.0/pandablocks/_exchange.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/_version_git.py` & `pandablocks-0.5.0/pandablocks/_version_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # versiongit-1.0 (https://github.com/dls-controls/versiongit)
 import os
 import re
 import sys
 from subprocess import STDOUT, CalledProcessError, check_output
 
 # These will be filled in if git archive is run or by setup.py cmdclasses
-GIT_REFS = 'tag: 0.4.0'
-GIT_SHA1 = '5dc0999'
+GIT_REFS = 'tag: 0.5.0'
+GIT_SHA1 = '8729a25'
 
 # Git describe gives us sha1, last version-like tag, and commits since then
 CMD = "git describe --tags --dirty --always --long --match=[0-9]*[-.][0-9]*"
 
 
 def get_version_from_git(path=None):
     """Try to parse version from git describe, fallback to git archive tags"""
```

### Comparing `pandablocks-0.4.0/pandablocks/asyncio.py` & `pandablocks-0.5.0/pandablocks/asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,25 @@
         return self._reader
 
     @property
     def writer(self) -> StreamWriter:
         assert self._writer, "connect() not called yet"
         return self._writer
 
-    async def write_and_drain(self, data: bytes):
+    async def write_and_drain(self, data: bytes, timeout: Optional[float] = None):
         writer = self.writer
         writer.write(data)
-        await writer.drain()
+
+        # Cannot simply await the drain, as if the remote end has disconnected
+        # then the drain will never complete as the OS cannot clear its send buffer.
+        _, pending = await asyncio.wait([writer.drain()], timeout=timeout)
+        if len(pending):
+            for task in pending:
+                task.cancel()
+            raise asyncio.TimeoutError("Timeout writing data")
 
     async def connect(self, host: str, port: int):
         self._reader, self._writer = await asyncio.open_connection(host, port)
 
     async def close(self):
         writer = self.writer
         self._reader = None
@@ -66,14 +73,21 @@
         """Connect to the control port, and be ready to handle commands"""
         await self._ctrl_stream.connect(self._host, 8888),
 
         self._ctrl_task = asyncio.create_task(
             self._ctrl_read_forever(self._ctrl_stream.reader)
         )
 
+    def is_connected(self):
+        """True if there is a currently active connection.
+        NOTE: This does not indicate if the remote end is still connected."""
+        if self._ctrl_task and not self._ctrl_task.done():
+            return True
+        return False
+
     async def close(self):
         """Close the control connection, and wait for completion"""
         assert self._ctrl_task, "connect() not called yet"
         self._ctrl_task.cancel()
         await self._ctrl_stream.close()
 
     async def __aenter__(self) -> "AsyncioClient":
@@ -91,26 +105,26 @@
                 await self._ctrl_stream.write_and_drain(to_send)
                 for command, response in self._ctrl_connection.responses():
                     queue = self._ctrl_queues.pop(id(command))
                     queue.put_nowait(response)
             except Exception:
                 logging.exception(f"Error handling '{received.decode()}'")
 
-    async def send(self, command: Command[T]) -> T:
+    async def send(self, command: Command[T], timeout: Optional[float] = None) -> T:
         """Send a command to control port of the PandA, returning its response.
 
         Args:
             command: The `Command` to send
         """
         queue: asyncio.Queue[T] = asyncio.Queue()
         # Need to use the id as non-frozen dataclasses don't hash
         self._ctrl_queues[id(command)] = queue
         to_send = self._ctrl_connection.send(command)
-        await self._ctrl_stream.write_and_drain(to_send)
-        response = await queue.get()
+        await self._ctrl_stream.write_and_drain(to_send, timeout)
+        response = await asyncio.wait_for(queue.get(), timeout)
         if isinstance(response, Exception):
             raise response
         else:
             return response
 
     async def data(
         self,
```

### Comparing `pandablocks-0.4.0/pandablocks/blocking.py` & `pandablocks-0.5.0/pandablocks/blocking.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/cli.py` & `pandablocks-0.5.0/pandablocks/cli.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/commands.py` & `pandablocks-0.5.0/pandablocks/commands.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/connections.py` & `pandablocks-0.5.0/pandablocks/connections.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/hdf.py` & `pandablocks-0.5.0/pandablocks/hdf.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/responses.py` & `pandablocks-0.5.0/pandablocks/responses.py`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks/saves/tutorial.sav` & `pandablocks-0.5.0/pandablocks/saves/tutorial.sav`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/pandablocks.egg-info/PKG-INFO` & `pandablocks-0.5.0/pandablocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandablocks
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python client to control and data ports of the PandABlocks TCP server
 Home-page: https://github.com/PandABlocks/PandABlocks-client
 Author: Tom Cobb
 Author-email: tom.cobb@diamond.ac.uk
 License: Apache License 2.0
 Description: PandABlocks Python Client
         =========================
```

### Comparing `pandablocks-0.4.0/pandablocks.egg-info/SOURCES.txt` & `pandablocks-0.5.0/pandablocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandablocks-0.4.0/setup.cfg` & `pandablocks-0.5.0/setup.cfg`

 * *Files identical despite different names*

