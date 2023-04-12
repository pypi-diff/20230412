# Comparing `tmp/tremolo-0.0.80.tar.gz` & `tmp/tremolo-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.80.tar", last modified: Wed Apr  5 01:19:28 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.81.tar", last modified: Wed Apr 12 13:07:53 2023, max compression
```

## Comparing `tremolo-0.0.80.tar` & `tremolo-0.0.81.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-05 01:19:28.000000 tremolo-0.0.80/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-05 01:19:28.000000 tremolo-0.0.80/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     2202 2023-03-26 12:59:14.000000 tremolo-0.0.80/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-05 01:19:28.000000 tremolo-0.0.80/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-05 01:17:21.000000 tremolo-0.0.80/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-03-31 02:46:47.000000 tremolo-0.0.80/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      321 2023-03-27 13:02:24.000000 tremolo-0.0.80/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11735 2023-04-03 04:26:19.000000 tremolo-0.0.80/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-03-26 12:59:14.000000 tremolo-0.0.80/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-03 09:33:20.000000 tremolo-0.0.80/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1665 2023-03-30 23:13:21.000000 tremolo-0.0.80/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13415 2023-04-05 01:13:22.000000 tremolo-0.0.80/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     8527 2023-03-27 10:34:31.000000 tremolo-0.0.80/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-04 02:34:30.000000 tremolo-0.0.80/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-03-26 12:59:14.000000 tremolo-0.0.80/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     5466 2023-03-26 12:46:38.000000 tremolo-0.0.80/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-03-26 12:59:14.000000 tremolo-0.0.80/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-03 11:22:19.000000 tremolo-0.0.80/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13754 2023-03-31 04:29:34.000000 tremolo-0.0.80/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-05 01:19:28.000000 tremolo-0.0.80/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 13:07:53.000000 tremolo-0.0.81/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.81/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-12 13:07:53.000000 tremolo-0.0.81/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-12 13:07:35.000000 tremolo-0.0.81/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11735 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/connection_pool.py
+-rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13633 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     8527 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/http_response.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo/lib/parsed/
+-rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/parsed/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     5466 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/parsed/parse.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13754 2023-04-12 13:07:35.000000 tremolo-0.0.81/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:53.000000 tremolo-0.0.81/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-12 13:07:52.000000 tremolo-0.0.81/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.80/PKG-INFO` & `tremolo-0.0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.80
+Version: 0.0.81
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

### Comparing `tremolo-0.0.80/README.md` & `tremolo-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/setup.py` & `tremolo-0.0.81/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.80',
+    version='0.0.81',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.80/tremolo/http_server.py` & `tremolo-0.0.81/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/lib/connection_pool.py` & `tremolo-0.0.81/tremolo/lib/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/lib/http_exception.py` & `tremolo-0.0.81/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/lib/http_protocol.py` & `tremolo-0.0.81/tremolo/lib/http_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,70 +156,77 @@
             data = b'<ul><li>%s</li></ul>' % '</li><li>'.join(
                 traceback.TracebackException.from_exception(exc).format()
             ).encode(encoding=encoding)
         else:
             data = str(exc).encode(encoding=encoding)
 
         await response.send(
-            b'HTTP/%s %d %s\r\nContent-Type: %s\r\nContent-Length: %d\r\nConnection: close\r\nDate: %s\r\nServer: %s\r\n\r\n%s' % (
-            request.version, exc.code, exc.message.encode(encoding='latin-1'), exc.content_type.encode(encoding='latin-1'), len(data),
-            datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'), self._options['server_name'], data))
+            b'HTTP/%s %d %s\r\nContent-Type: %s\r\nContent-Length: %d\r\nConnection: close\r\n\
+            Date: %s\r\nServer: %s\r\n\r\n%s' % (request.version,
+                                                 exc.code,
+                                                 exc.message.encode(encoding='latin-1'),
+                                                 exc.content_type.encode(encoding='latin-1'),
+                                                 len(data),
+                                                 datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
+                                                 self._options['server_name'],
+                                                 data))
 
         response.close()
 
     async def _handle_request_header(self, data, header_size):
         self._data = None
 
-        if self._header.parse(data, header_size=header_size, excludes=[b'proxy']).is_request:
-            self._request = HTTPRequest(self)
-            self._response = HTTPResponse(self._request)
-
-            try:
-                if b'connection' in self._request.headers:
-                    if self._request.headers[b'connection'].lower().find(b'close') == -1:
-                        self._request.http_keepalive = True
-                elif self._request.version == b'1.1':
+        if not self._header.parse(data, header_size=header_size, excludes=[b'proxy']).is_request:
+            if self._queue[1] is not None:
+                self._queue[1].put_nowait(None)
+
+            self._options['logger'].info('bad request: not a request')
+            return
+
+        self._request = HTTPRequest(self)
+        self._response = HTTPResponse(self._request)
+
+        try:
+            if b'connection' in self._request.headers:
+                if self._request.headers[b'connection'].lower().find(b'close') == -1:
                     self._request.http_keepalive = True
+            elif self._request.version == b'1.1':
+                self._request.http_keepalive = True
 
-                if self._request.method in (b'POST', b'PUT', b'PATCH'):
-                    if b'content-type' in self._request.headers:
-                        self._request.content_type = self._request.headers[b'content-type'].lower()
-
-                    if b'transfer-encoding' in self._request.headers:
-                        if self._request.version == b'1.0':
-                            raise BadRequest
-
-                        self._request.transfer_encoding = self._request.headers[b'transfer-encoding'].lower()
-
-                    if b'content-length' in self._request.headers:
-                        if self._request.transfer_encoding.find(b'chunked') > -1:
-                            raise BadRequest
+            if self._request.method in (b'POST', b'PUT', b'PATCH'):
+                if b'content-type' in self._request.headers:
+                    self._request.content_type = self._request.headers[b'content-type'].lower()
 
-                        self._request.content_length = int(self._request.headers[b'content-length'])
-                    elif self._request.version == b'1.0':
+                if b'transfer-encoding' in self._request.headers:
+                    if self._request.version == b'1.0':
                         raise BadRequest
 
-                    if b'expect' in self._request.headers and self._request.headers[b'expect'].lower() == b'100-continue':
-                        self._request.http_continue = True
+                    self._request.transfer_encoding = self._request.headers[b'transfer-encoding'].lower()
 
-                    await self.put_to_queue(
-                        data[header_size + 4:], queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate']
-                    )
-
-                await self.header_received(self._request, self._response)
-            except Exception as exc:
-                if not isinstance(exc, HTTPException):
-                    exc = InternalServerError(cause=exc)
+                if b'content-length' in self._request.headers:
+                    if self._request.transfer_encoding.find(b'chunked') > -1:
+                        raise BadRequest
 
-                await self.handle_exception(exc, self._request, self._response)
-        else:
-            if self._queue[1] is not None:
-                self._queue[1].put_nowait(None)
+                    self._request.content_length = int(self._request.headers[b'content-length'])
+                elif self._request.version == b'1.0':
+                    raise BadRequest
+
+                if b'expect' in self._request.headers and self._request.headers[b'expect'].lower() == b'100-continue':
+                    self._request.http_continue = True
+
+                await self.put_to_queue(
+                    data[header_size + 4:], queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate']
+                )
+
+            await self.header_received(self._request, self._response)
+        except Exception as exc:
+            if not isinstance(exc, HTTPException):
+                exc = InternalServerError(cause=exc)
 
-            self._options['logger'].info('bad request: not a request')
+            await self.handle_exception(exc, self._request, self._response)
 
     def data_received(self, data):
         if self._data is not None:
             self._data.extend(data)
             header_size = self._data.find(b'\r\n\r\n')
 
             if -1 < header_size <= 8192:
```

### Comparing `tremolo-0.0.80/tremolo/lib/http_request.py` & `tremolo-0.0.81/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/lib/http_response.py` & `tremolo-0.0.81/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/lib/parsed/parse.py` & `tremolo-0.0.81/tremolo/lib/parsed/parse.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/lib/request.py` & `tremolo-0.0.81/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/lib/response.py` & `tremolo-0.0.81/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo/tremolo.py` & `tremolo-0.0.81/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.80/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.81/tremolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.80
+Version: 0.0.81
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

