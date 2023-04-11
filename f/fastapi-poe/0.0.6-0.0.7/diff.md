# Comparing `tmp/fastapi_poe-0.0.6.tar.gz` & `tmp/fastapi_poe-0.0.7.tar.gz`

## Comparing `fastapi_poe-0.0.6.tar` & `fastapi_poe-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/__main__.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/base.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/types.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/samples/catbot.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/samples/echo.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/.gitignore
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/__main__.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/base.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/types.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/samples/catbot.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/src/fastapi_poe/samples/echo.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 fastapi_poe-0.0.7/PKG-INFO
```

### Comparing `fastapi_poe-0.0.6/src/fastapi_poe/base.py` & `fastapi_poe-0.0.7/src/fastapi_poe/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.6/src/fastapi_poe/types.py` & `fastapi_poe-0.0.7/src/fastapi_poe/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.6/src/fastapi_poe/samples/catbot.py` & `fastapi_poe-0.0.7/src/fastapi_poe/samples/catbot.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,21 +71,27 @@
                 await asyncio.sleep(1)
         elif "square" in last_message:
             yield self.error_event("Square snacks are not tasty.")
         elif "cube" in last_message:
             yield self.error_event(
                 "Cube snacks are even less tasty.", allow_retry=False
             )
-        elif "scratch" in last_message:
-            # Note this is illegal according to the protocol
-            yield ServerSentEvent(event="purr", data=json.dumps({"text": "purr"}))
         elif "count" in last_message:
             for i in range(1, 11):
                 yield self.replace_response_event(str(i))
-                await asyncio.sleep(1)
+                if "quickly" not in last_message:
+                    await asyncio.sleep(1)
+        # These messages make Altai do something that's not allowed by the protocol
+        elif "scratch" in last_message:
+            yield ServerSentEvent(event="purr", data=json.dumps({"text": "purr"}))
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
             f"User {feedback.user_id} gave feedback on {feedback.conversation_id}"
```

### Comparing `fastapi_poe-0.0.6/src/fastapi_poe/samples/echo.py` & `fastapi_poe-0.0.7/src/fastapi_poe/samples/echo.py`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.6/README.md` & `fastapi_poe-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.6/pyproject.toml` & `fastapi_poe-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_poe"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Lida Li", email="lli@quora.com" },
 ]
 description = "A demonstration of the Poe protocol using FastAPI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fastapi_poe-0.0.6/PKG-INFO` & `fastapi_poe-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_poe
-Version: 0.0.6
+Version: 0.0.7
 Summary: A demonstration of the Poe protocol using FastAPI
 Project-URL: Homepage, https://github.com/quora/poe-protocol
 Author-email: Lida Li <lli@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

