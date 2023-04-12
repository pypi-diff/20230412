# Comparing `tmp/socketio_notfier-0.1.0.tar.gz` & `tmp/socketio_notfier-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketio_notfier-0.1.0.tar", max compression
+gzip compressed data, was "socketio_notfier-1.0.0.tar", max compression
```

## Comparing `socketio_notfier-0.1.0.tar` & `socketio_notfier-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      416 2023-04-06 14:05:45.889255 socketio_notfier-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-06 13:42:50.726345 socketio_notfier-0.1.0/README.md
--rw-r--r--   0        0        0       28 2023-04-06 13:38:33.184365 socketio_notfier-0.1.0/socketio_notifier/__init__.py
--rw-r--r--   0        0        0      681 2023-04-06 14:03:55.726842 socketio_notfier-0.1.0/socketio_notifier/notifier.py
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 socketio_notfier-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      416 2023-04-12 17:46:12.936906 socketio_notfier-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-06 13:42:50.726345 socketio_notfier-1.0.0/README.md
+-rw-r--r--   0        0        0       28 2023-04-06 13:38:33.184365 socketio_notfier-1.0.0/socketio_notifier/__init__.py
+-rw-r--r--   0        0        0      765 2023-04-12 17:44:52.387504 socketio_notfier-1.0.0/socketio_notifier/notifier.py
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 socketio_notfier-1.0.0/PKG-INFO
```

### Comparing `socketio_notfier-0.1.0/socketio_notifier/notifier.py` & `socketio_notfier-1.0.0/socketio_notifier/notifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,11 +15,14 @@
 
     @sio.event
     async def disconnect():
         print('Desconectado do servidor')
 
     await sio.connect(f'http://{server_address}:{port}')
     await my_message()
-    await sio.wait()
+
+    # Aguarda 1 segundo antes de desconectar
+    await asyncio.sleep(1)
+    await sio.disconnect()
 
 def notify(message, server_address, port, event_name):
-    asyncio.run(enviar_mensagem(message, server_address, port, event_name))
+    asyncio.run(enviar_mensagem(message, server_address, port, event_name))
```

