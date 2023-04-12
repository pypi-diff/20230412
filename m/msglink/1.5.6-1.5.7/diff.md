# Comparing `tmp/msglink-1.5.6.tar.gz` & `tmp/msglink-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msglink-1.5.6.tar", last modified: Wed Mar 15 12:41:34 2023, max compression
+gzip compressed data, was "msglink-1.5.7.tar", last modified: Wed Apr 12 12:56:59 2023, max compression
```

## Comparing `msglink-1.5.6.tar` & `msglink-1.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 12:41:34.454550 msglink-1.5.6/
--rw-rw-rw-   0        0        0     7814 2018-01-22 14:20:08.000000 msglink-1.5.6/LICENSE.txt
--rw-rw-rw-   0        0        0      224 2023-03-15 12:41:34.453487 msglink-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0        8 2018-01-22 14:19:01.000000 msglink-1.5.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-15 12:41:34.451126 msglink-1.5.6/msglink/
--rw-rw-rw-   0        0        0      114 2022-02-15 10:03:50.000000 msglink-1.5.6/msglink/__init__.py
--rw-rw-rw-   0        0        0     5063 2020-05-12 14:30:40.000000 msglink-1.5.6/msglink/packets.py
--rw-rw-rw-   0        0        0    13590 2023-03-15 12:40:51.000000 msglink-1.5.6/msglink/protocol.py
--rw-rw-rw-   0        0        0        0 2022-03-04 14:45:43.000000 msglink-1.5.6/msglink/py.typed
--rw-rw-rw-   0        0        0    10525 2023-02-03 15:51:54.000000 msglink-1.5.6/msglink/router.py
-drwxrwxrwx   0        0        0        0 2023-03-15 12:41:34.453487 msglink-1.5.6/msglink.egg-info/
--rw-rw-rw-   0        0        0      224 2023-03-15 12:41:34.000000 msglink-1.5.6/msglink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-03-15 12:41:34.000000 msglink-1.5.6/msglink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 12:41:34.000000 msglink-1.5.6/msglink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-15 12:41:34.000000 msglink-1.5.6/msglink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 12:41:34.454550 msglink-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      290 2023-03-15 12:41:04.000000 msglink-1.5.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:56:59.625486 msglink-1.5.7/
+-rwxrwxrwx   0 root         (0) root         (0)     7814 2023-02-03 15:46:02.000000 msglink-1.5.7/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)      176 2023-04-12 12:56:59.619381 msglink-1.5.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-02-03 15:46:02.000000 msglink-1.5.7/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:56:59.385249 msglink-1.5.7/msglink/
+-rwxrwxrwx   0 root         (0) root         (0)      114 2023-02-03 15:46:02.000000 msglink-1.5.7/msglink/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5063 2023-02-03 15:46:02.000000 msglink-1.5.7/msglink/packets.py
+-rwxrwxrwx   0 root         (0) root         (0)    13590 2023-03-16 09:33:42.000000 msglink-1.5.7/msglink/protocol.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-02-03 15:46:02.000000 msglink-1.5.7/msglink/py.typed
+-rwxrwxrwx   0 root         (0) root         (0)    10652 2023-04-06 12:34:43.000000 msglink-1.5.7/msglink/router.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 12:56:59.573094 msglink-1.5.7/msglink.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      176 2023-04-12 12:56:58.000000 msglink-1.5.7/msglink.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      249 2023-04-12 12:56:58.000000 msglink-1.5.7/msglink.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-12 12:56:58.000000 msglink-1.5.7/msglink.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-04-12 12:56:58.000000 msglink-1.5.7/msglink.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-12 12:56:59.628334 msglink-1.5.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      290 2023-04-06 12:35:44.000000 msglink-1.5.7/setup.py
```

### Comparing `msglink-1.5.6/LICENSE.txt` & `msglink-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msglink-1.5.6/msglink/packets.py` & `msglink-1.5.7/msglink/packets.py`

 * *Files identical despite different names*

### Comparing `msglink-1.5.6/msglink/protocol.py` & `msglink-1.5.7/msglink/protocol.py`

 * *Files identical despite different names*

### Comparing `msglink-1.5.6/msglink/router.py` & `msglink-1.5.7/msglink/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,14 +232,15 @@
             return
 
         # need to make new authentication attempt
         # (_auth_result either None or failed)
         log.info(f"[msglink] authenticating to {self._server}")
         self._auth_future = asyncio.Future()
         self._protocol.send_auth_request(self._role, self._password, self._info)
+
         await self._auth_future
 
     async def _reconnect_loop(self):
         while self._running:
             try:
                 await self._try_connect_msglink()
                 await self._try_authenticate()
@@ -254,14 +255,16 @@
 
         for cr in self._channel_readers:
             cr.queue.put_nowait(None)
 
     # msglink callbacks =================================================================
     def on_connect_close(self):
         log.info(f"[msglink] connection to {self._server}:{self._port} was closed")
+        if self._auth_future is not None and not self._auth_future.done():
+            self._auth_future.set_result(False)
         self._established = False
         self._connected_peers.clear()
         self._all_disconnected()
         self._auth_future = None
 
     def on_auth_fail(self):
         log.warning(f"[msglink] authentication failed for role '{self._role}' at server {self._server}")
```

