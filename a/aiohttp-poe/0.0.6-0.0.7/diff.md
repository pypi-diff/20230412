# Comparing `tmp/aiohttp_poe-0.0.6.tar.gz` & `tmp/aiohttp_poe-0.0.7.tar.gz`

## Comparing `aiohttp_poe-0.0.6.tar` & `aiohttp_poe-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/__main__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/base.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/types.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/samples/catbot.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/src/aiohttp_poe/samples/echo.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/.gitignore
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/__main__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/base.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/types.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/samples/catbot.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/src/aiohttp_poe/samples/echo.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aiohttp_poe-0.0.7/PKG-INFO
```

### Comparing `aiohttp_poe-0.0.6/src/aiohttp_poe/base.py` & `aiohttp_poe-0.0.7/src/aiohttp_poe/base.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.6/src/aiohttp_poe/types.py` & `aiohttp_poe-0.0.7/src/aiohttp_poe/types.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.6/src/aiohttp_poe/samples/catbot.py` & `aiohttp_poe-0.0.7/src/aiohttp_poe/samples/catbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,22 +73,27 @@
                 await asyncio.sleep(1)
         elif "square" in last_message:
             yield self.error_event("Square snacks are not tasty.")
         elif "cube" in last_message:
             yield self.error_event(
                 "Cube snacks are even less tasty.", allow_retry=False
             )
-        elif "scratch" in last_message:
-            # This is not legal according to the protocol; we do this to demonstrate
-            # the report_error endpoint.
-            yield ("purr", {"text": "purr"})  # type: ignore
         elif "count" in last_message:
             for i in range(1, 11):
                 yield self.replace_response_event(str(i))
-                await asyncio.sleep(1)
+                if "quickly" not in last_message:
+                    await asyncio.sleep(1)
+        # These messages make Altai do something that's not allowed by the protocol
+        elif "scratch" in last_message:
+            yield ("purr", {"text": "purr"})  # type: ignore
+        elif "toy" in last_message:
+            for _ in range(1010):
+                yield self.text_event("hit ")
+        elif "bed" in last_message:
+            yield self.text_event("z" * 10_010)
         else:
             yield self.text_event("zzz")
 
     async def on_feedback(self, feedback: ReportFeedbackRequest) -> None:
         """Called when we receive user feedback such as likes."""
         print(
             f"User {feedback['user_id']} gave feedback on {feedback['conversation_id']}"
```

### Comparing `aiohttp_poe-0.0.6/src/aiohttp_poe/samples/echo.py` & `aiohttp_poe-0.0.7/src/aiohttp_poe/samples/echo.py`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.6/README.md` & `aiohttp_poe-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_poe-0.0.6/pyproject.toml` & `aiohttp_poe-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aiohttp_poe"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Jelle Zijlstra", email="jelle@quora.com" },
 ]
 description = "A demonstration of the Poe protocol using aiohttp"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aiohttp_poe-0.0.6/PKG-INFO` & `aiohttp_poe-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp_poe
-Version: 0.0.6
+Version: 0.0.7
 Summary: A demonstration of the Poe protocol using aiohttp
 Project-URL: Homepage, https://github.com/quora/poe-protocol
 Author-email: Jelle Zijlstra <jelle@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

