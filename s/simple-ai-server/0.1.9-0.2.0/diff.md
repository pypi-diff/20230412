# Comparing `tmp/simple_ai_server-0.1.9.tar.gz` & `tmp/simple_ai_server-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ai_server-0.1.9.tar", max compression
+gzip compressed data, was "simple_ai_server-0.2.0.tar", max compression
```

## Comparing `simple_ai_server-0.1.9.tar` & `simple_ai_server-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
--rw-r--r--   0        0        0      451 2023-03-23 17:59:04.553718 simple_ai_server-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      563 2023-03-20 16:51:40.215061 simple_ai_server-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-03-18 16:45:18.115514 simple_ai_server-0.1.9/simple_ai/__init__.py
--rw-r--r--   0        0        0     1109 2023-03-18 18:01:39.466310 simple_ai_server-0.1.9/simple_ai/__main__.py
--rw-r--r--   0        0        0     1462 2023-03-22 01:04:56.836893 simple_ai_server-0.1.9/simple_ai/api_models.py
--rw-r--r--   0        0        0     1697 2023-03-22 01:25:18.930300 simple_ai_server-0.1.9/simple_ai/clients/completion/client.py
--rw-r--r--   0        0        0     2047 2023-03-15 17:38:47.972578 simple_ai_server-0.1.9/simple_ai/clients/completion/llm_pb2.py
--rw-r--r--   0        0        0     1926 2023-03-15 17:38:47.973078 simple_ai_server-0.1.9/simple_ai/clients/completion/llm_pb2.pyi
--rw-r--r--   0        0        0     3773 2023-03-18 16:53:40.235586 simple_ai_server-0.1.9/simple_ai/clients/completion/llm_pb2_grpc.py
--rw-r--r--   0        0        0      810 2023-03-23 17:50:13.056561 simple_ai_server-0.1.9/simple_ai/clients/embedding/client.py
--rw-r--r--   0        0        0     1697 2023-03-22 01:29:14.275596 simple_ai_server-0.1.9/simple_ai/clients/embedding/llm_embed_pb2.py
--rw-r--r--   0        0        0     1104 2023-03-22 01:29:14.275596 simple_ai_server-0.1.9/simple_ai/clients/embedding/llm_embed_pb2.pyi
--rw-r--r--   0        0        0     2382 2023-03-22 01:33:22.061456 simple_ai_server-0.1.9/simple_ai/clients/embedding/llm_embed_pb2_grpc.py
--rw-r--r--   0        0        0     1999 2023-03-14 21:43:22.144207 simple_ai_server-0.1.9/simple_ai/dummy.py
--rw-r--r--   0        0        0     2805 2023-03-22 01:36:32.554405 simple_ai_server-0.1.9/simple_ai/models.py
--rw-r--r--   0        0        0      226 2023-03-17 17:21:47.275098 simple_ai_server-0.1.9/simple_ai/models.toml
--rw-r--r--   0        0        0      192 2023-03-20 11:45:04.823985 simple_ai_server-0.1.9/simple_ai/models.toml.template
--rw-r--r--   0        0        0      955 2023-03-15 17:13:39.396817 simple_ai_server-0.1.9/simple_ai/protos/llm.proto
--rw-r--r--   0        0        0      599 2023-03-22 02:19:19.527562 simple_ai_server-0.1.9/simple_ai/protos/llm_embed.proto
--rw-r--r--   0        0        0     1708 2023-03-16 18:28:09.804190 simple_ai_server-0.1.9/simple_ai/serve/cpp/CMakeLists.txt
--rw-r--r--   0        0        0     1568 2023-03-17 00:52:18.985443 simple_ai_server-0.1.9/simple_ai/serve/cpp/Dockerfile
--rw-r--r--   0        0        0     3440 2023-03-15 16:45:36.948848 simple_ai_server-0.1.9/simple_ai/serve/cpp/Makefile
--rw-r--r--   0        0        0     1850 2023-03-17 11:25:34.312682 simple_ai_server-0.1.9/simple_ai/serve/cpp/server.cpp
--rw-r--r--   0        0        0     2047 2023-03-15 17:38:47.972578 simple_ai_server-0.1.9/simple_ai/serve/python/completion/llm_pb2.py
--rw-r--r--   0        0        0     1926 2023-03-15 17:38:47.973078 simple_ai_server-0.1.9/simple_ai/serve/python/completion/llm_pb2.pyi
--rw-r--r--   0        0        0     3773 2023-03-20 15:05:11.813737 simple_ai_server-0.1.9/simple_ai/serve/python/completion/llm_pb2_grpc.py
--rw-r--r--   0        0        0      808 2023-03-20 16:11:47.401481 simple_ai_server-0.1.9/simple_ai/serve/python/completion/model.py
--rw-r--r--   0        0        0      675 2023-03-16 17:23:28.892975 simple_ai_server-0.1.9/simple_ai/serve/python/completion/README.md
--rw-r--r--   0        0        0     2545 2023-03-22 02:18:16.254113 simple_ai_server-0.1.9/simple_ai/serve/python/completion/server.py
--rw-r--r--   0        0        0     1697 2023-03-22 01:29:14.275596 simple_ai_server-0.1.9/simple_ai/serve/python/embedding/llm_embed_pb2.py
--rw-r--r--   0        0        0     1104 2023-03-22 01:29:14.275596 simple_ai_server-0.1.9/simple_ai/serve/python/embedding/llm_embed_pb2.pyi
--rw-r--r--   0        0        0     2382 2023-03-22 01:33:33.028685 simple_ai_server-0.1.9/simple_ai/serve/python/embedding/llm_embed_pb2_grpc.py
--rw-r--r--   0        0        0      251 2023-03-23 17:52:12.408395 simple_ai_server-0.1.9/simple_ai/serve/python/embedding/model.py
--rw-r--r--   0        0        0      687 2023-03-22 01:16:30.848145 simple_ai_server-0.1.9/simple_ai/serve/python/embedding/README.md
--rw-r--r--   0        0        0     1603 2023-03-23 17:52:38.917327 simple_ai_server-0.1.9/simple_ai/serve/python/embedding/server.py
--rw-r--r--   0        0        0     3601 2023-03-22 01:07:22.640860 simple_ai_server-0.1.9/simple_ai/server.py
--rw-r--r--   0        0        0     2641 2023-03-22 01:25:55.045713 simple_ai_server-0.1.9/simple_ai/utils.py
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 simple_ai_server-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-12 14:38:29.075976 simple_ai_server-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5572 2023-04-12 15:29:07.213015 simple_ai_server-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5386 2023-04-12 14:38:29.076977 simple_ai_server-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 16:45:18.115514 simple_ai_server-0.2.0/src/simple_ai/__init__.py
+-rw-r--r--   0        0        0     1072 2023-04-05 13:55:01.576228 simple_ai_server-0.2.0/src/simple_ai/__main__.py
+-rw-r--r--   0        0        0     3286 2023-03-31 16:24:31.515208 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     2027 2023-03-31 15:37:59.978527 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     3570 2023-03-31 16:24:31.521708 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/llm_chat_pb2_grpc.cpython-311.pyc
+-rw-r--r--   0        0        0     1219 2023-03-31 15:37:59.985026 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     3138 2023-04-12 14:38:29.078476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/client.py
+-rw-r--r--   0        0        0     2432 2023-04-12 14:38:29.078476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2.py
+-rw-r--r--   0        0        0     2402 2023-04-05 13:55:01.577727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2.pyi
+-rw-r--r--   0        0        0     4016 2023-04-12 14:38:29.078976 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2_grpc.py
+-rw-r--r--   0        0        0      435 2023-04-12 14:38:29.079476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/model.py
+-rw-r--r--   0        0        0     2883 2023-04-12 14:38:29.079975 simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/server.py
+-rw-r--r--   0        0        0     2387 2023-03-31 16:24:31.475207 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     1958 2023-03-31 16:24:31.498707 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     4830 2023-03-31 16:24:31.513707 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/__pycache__/llm_pb2_grpc.cpython-311.pyc
+-rw-r--r--   0        0        0     2969 2023-04-12 14:38:29.080975 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/client.py
+-rw-r--r--   0        0        0     2186 2023-04-05 13:55:01.579226 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.py
+-rw-r--r--   0        0        0     2246 2023-04-05 13:55:01.579727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.pyi
+-rw-r--r--   0        0        0     3956 2023-04-05 13:55:01.580227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2_grpc.py
+-rw-r--r--   0        0        0     1326 2023-04-12 14:38:29.081475 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/model.py
+-rw-r--r--   0        0        0     2564 2023-04-12 14:38:29.081975 simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/server.py
+-rw-r--r--   0        0        0     1788 2023-03-31 16:24:31.524207 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     1880 2023-03-31 16:24:31.525208 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     3594 2023-03-31 16:24:31.526707 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/__pycache__/llm_embed_pb2_grpc.cpython-311.pyc
+-rw-r--r--   0        0        0      813 2023-04-05 13:55:01.581227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/client.py
+-rw-r--r--   0        0        0     1808 2023-04-05 13:55:01.581727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.py
+-rw-r--r--   0        0        0     1175 2023-04-05 13:55:01.581727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.pyi
+-rw-r--r--   0        0        0     2483 2023-04-05 13:55:01.582227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2_grpc.py
+-rw-r--r--   0        0        0      266 2023-04-05 13:55:01.582727 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/model.py
+-rw-r--r--   0        0        0     1577 2023-04-05 13:55:01.583227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/server.py
+-rw-r--r--   0        0        0     1005 2023-04-12 14:38:29.082476 simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_chat.proto
+-rw-r--r--   0        0        0      955 2023-04-05 13:55:01.584227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_complete.proto
+-rw-r--r--   0        0        0      599 2023-04-05 13:55:01.584227 simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_embed.proto
+-rw-r--r--   0        0        0     1233 2023-04-12 14:38:29.082975 simple_ai_server-0.2.0/src/simple_ai/api_models.py
+-rw-r--r--   0        0        0     2345 2023-04-12 15:10:37.779433 simple_ai_server-0.2.0/src/simple_ai/dummy.py
+-rw-r--r--   0        0        0     5743 2023-04-12 14:38:29.083476 simple_ai_server-0.2.0/src/simple_ai/models.py
+-rw-r--r--   0        0        0      226 2023-03-17 17:21:47.275098 simple_ai_server-0.2.0/src/simple_ai/models.toml
+-rw-r--r--   0        0        0      214 2023-04-05 13:55:01.586227 simple_ai_server-0.2.0/src/simple_ai/models.toml.template
+-rw-r--r--   0        0        0     6049 2023-04-12 14:38:29.083975 simple_ai_server-0.2.0/src/simple_ai/server.py
+-rw-r--r--   0        0        0     3677 2023-04-12 15:10:37.779934 simple_ai_server-0.2.0/src/simple_ai/utils.py
+-rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 simple_ai_server-0.2.0/PKG-INFO
```

### Comparing `simple_ai_server-0.1.9/simple_ai/__main__.py` & `simple_ai_server-0.2.0/src/simple_ai/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import shutil
 import argparse
+import shutil
 from pathlib import Path
 
 import uvicorn
 
-def serve_app(host='127.0.0.1', port=8080, **kwargs):
+
+def serve_app(host="127.0.0.1", port=8080, **kwargs):
     from . import server
-    uvicorn.run(
-        app=server.app,
-        host=host,
-        port=port
-    )
 
-def init_app(path='./', **kwargs):
+    uvicorn.run(app=server.app, host=host, port=port)
+
+
+def init_app(path="./", **kwargs):
     shutil.copy(
-        src=Path(Path(__file__).parent.absolute(), 'models.toml.template'),
-        dst=Path(path, 'models.toml')
+        src=Path(Path(__file__).parent.absolute(), "models.toml.template"),
+        dst=Path(path, "models.toml"),
     )
 
+
 def main():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers()
-    
+
     # Init config args
-    init_parser = subparsers.add_parser('init')
-    init_parser.add_argument('--path', default='./')
+    init_parser = subparsers.add_parser("init")
+    init_parser.add_argument("--path", default="./")
     init_parser.set_defaults(func=init_app)
 
     # Serving args
-    serving_parser = subparsers.add_parser('serve')
-    serving_parser.add_argument('--host', default='127.0.0.1')
-    serving_parser.add_argument('--port', default=8080)
+    serving_parser = subparsers.add_parser("serve")
+    serving_parser.add_argument("--host", default="127.0.0.1")
+    serving_parser.add_argument("--port", default=8080)
     serving_parser.set_defaults(func=serve_app)
-    
+
     # Parse, call the appropriate function
     args = parser.parse_args()
     args.func(**args.__dict__)
 
-    
+
 if __name__ == "__main__":
     main()
```

### Comparing `simple_ai_server-0.1.9/simple_ai/clients/completion/llm_pb2.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/chat/llm_chat_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,45 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: llm.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tllm.proto\x12\rlanguagemodel\"\x84\x02\n\x07Message\x12\x0e\n\x06prompt\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\x12\n\nmax_tokens\x18\x03 \x01(\x05\x12\x13\n\x0btemperature\x18\x04 \x01(\x02\x12\r\n\x05top_p\x18\x05 \x01(\x02\x12\t\n\x01n\x18\x06 \x01(\x05\x12\x0e\n\x06stream\x18\x07 \x01(\x08\x12\x10\n\x08logprobs\x18\x08 \x01(\x05\x12\x0c\n\x04\x65\x63ho\x18\t \x01(\x08\x12\x0c\n\x04stop\x18\n \x01(\t\x12\x18\n\x10presence_penalty\x18\x0b \x01(\x02\x12\x19\n\x11\x66requence_penalty\x18\x0c \x01(\x02\x12\x0f\n\x07\x62\x65st_of\x18\r \x01(\x05\x12\x12\n\nlogit_bias\x18\x0e \x01(\t\"\x1c\n\x0b\x43ompletions\x12\r\n\x05reply\x18\x01 \x01(\t2\x9b\x01\n\rLanguageModel\x12@\n\x08\x43omplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions\"\x00\x12H\n\x0eStreamComplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions\"\x00\x30\x01\x42+\n\x13io.grpc.examples.lmB\rLanguageModelP\x01\xa2\x02\x02LMb\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'llm_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\023io.grpc.examples.lmB\rLanguageModelP\001\242\002\002LM'
-  _MESSAGE._serialized_start=29
-  _MESSAGE._serialized_end=289
-  _COMPLETIONS._serialized_start=291
-  _COMPLETIONS._serialized_end=319
-  _LANGUAGEMODEL._serialized_start=322
-  _LANGUAGEMODEL._serialized_end=477
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: llm_chat.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x0ellm_chat.proto\x12\x11languagemodelchat"\xe3\x01\n\x0c\x43hatLogInput\x12)\n\x08messages\x18\x01'
+    b" \x03(\x0b\x32\x17.languagemodelchat.Chat\x12\x12\n\nmax_tokens\x18\x02"
+    b" \x01(\x05\x12\x13\n\x0btemperature\x18\x03 \x01(\x02\x12\r\n\x05top_p\x18\x04"
+    b" \x01(\x02\x12\t\n\x01n\x18\x05 \x01(\x05\x12\x0e\n\x06stream\x18\x06"
+    b" \x01(\x08\x12\x0c\n\x04stop\x18\x07 \x01(\t\x12\x18\n\x10presence_penalty\x18\x08"
+    b" \x01(\x02\x12\x19\n\x11\x66requence_penalty\x18\t \x01(\x02\x12\x12\n\nlogit_bias\x18\n"
+    b' \x01(\t":\n\rChatLogOutput\x12)\n\x08messages\x18\x01'
+    b' \x03(\x0b\x32\x17.languagemodelchat.Chat"D\n\x04\x43hat\x12\x11\n\x04role\x18\x01'
+    b" \x01(\tH\x00\x88\x01\x01\x12\x14\n\x07\x63ontent\x18\x02"
+    b" \x01(\tH\x01\x88\x01\x01\x42\x07\n\x05_roleB\n\n\x08_content2\xad\x01\n\rLanguageModel\x12K\n\x04\x43hat\x12\x1f.languagemodelchat.ChatLogInput\x1a"
+    b' .languagemodelchat.ChatLogOutput"\x00\x12O\n\x06Stream\x12\x1f.languagemodelchat.ChatLogInput\x1a'
+    b' .languagemodelchat.ChatLogOutput"\x00\x30\x01\x42\x33\n\x15io.grpc.examples.chatB\x11LanguageModelChatP\x01\xa2\x02\x04\x63hatb\x06proto3'
+)
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "llm_chat_pb2", globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = (
+        b"\n\025io.grpc.examples.chatB\021LanguageModelChatP\001\242\002\004chat"
+    )
+    _CHATLOGINPUT._serialized_start = 38
+    _CHATLOGINPUT._serialized_end = 265
+    _CHATLOGOUTPUT._serialized_start = 267
+    _CHATLOGOUTPUT._serialized_end = 325
+    _CHAT._serialized_start = 327
+    _CHAT._serialized_end = 395
+    _LANGUAGEMODEL._serialized_start = 398
+    _LANGUAGEMODEL._serialized_end = 571
+# @@protoc_insertion_point(module_scope)
```

### Comparing `simple_ai_server-0.1.9/simple_ai/clients/completion/llm_pb2.pyi` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,74 @@
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional
-
-DESCRIPTOR: _descriptor.FileDescriptor
-
-class Completions(_message.Message):
-    __slots__ = ["reply"]
-    REPLY_FIELD_NUMBER: _ClassVar[int]
-    reply: str
-    def __init__(self, reply: _Optional[str] = ...) -> None: ...
-
-class Message(_message.Message):
-    __slots__ = ["best_of", "echo", "frequence_penalty", "logit_bias", "logprobs", "max_tokens", "n", "presence_penalty", "prompt", "stop", "stream", "suffix", "temperature", "top_p"]
-    BEST_OF_FIELD_NUMBER: _ClassVar[int]
-    ECHO_FIELD_NUMBER: _ClassVar[int]
-    FREQUENCE_PENALTY_FIELD_NUMBER: _ClassVar[int]
-    LOGIT_BIAS_FIELD_NUMBER: _ClassVar[int]
-    LOGPROBS_FIELD_NUMBER: _ClassVar[int]
-    MAX_TOKENS_FIELD_NUMBER: _ClassVar[int]
-    N_FIELD_NUMBER: _ClassVar[int]
-    PRESENCE_PENALTY_FIELD_NUMBER: _ClassVar[int]
-    PROMPT_FIELD_NUMBER: _ClassVar[int]
-    STOP_FIELD_NUMBER: _ClassVar[int]
-    STREAM_FIELD_NUMBER: _ClassVar[int]
-    SUFFIX_FIELD_NUMBER: _ClassVar[int]
-    TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
-    TOP_P_FIELD_NUMBER: _ClassVar[int]
-    best_of: int
-    echo: bool
-    frequence_penalty: float
-    logit_bias: str
-    logprobs: int
-    max_tokens: int
-    n: int
-    presence_penalty: float
-    prompt: str
-    stop: str
-    stream: bool
-    suffix: str
-    temperature: float
-    top_p: float
-    def __init__(self, prompt: _Optional[str] = ..., suffix: _Optional[str] = ..., max_tokens: _Optional[int] = ..., temperature: _Optional[float] = ..., top_p: _Optional[float] = ..., n: _Optional[int] = ..., stream: bool = ..., logprobs: _Optional[int] = ..., echo: bool = ..., stop: _Optional[str] = ..., presence_penalty: _Optional[float] = ..., frequence_penalty: _Optional[float] = ..., best_of: _Optional[int] = ..., logit_bias: _Optional[str] = ...) -> None: ...
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import ClassVar as _ClassVar, Optional as _Optional
+
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class Completions(_message.Message):
+    __slots__ = ["reply"]
+    REPLY_FIELD_NUMBER: _ClassVar[int]
+    reply: str
+    def __init__(self, reply: _Optional[str] = ...) -> None: ...
+
+class Message(_message.Message):
+    __slots__ = [
+        "best_of",
+        "echo",
+        "frequence_penalty",
+        "logit_bias",
+        "logprobs",
+        "max_tokens",
+        "n",
+        "presence_penalty",
+        "prompt",
+        "stop",
+        "stream",
+        "suffix",
+        "temperature",
+        "top_p",
+    ]
+    BEST_OF_FIELD_NUMBER: _ClassVar[int]
+    ECHO_FIELD_NUMBER: _ClassVar[int]
+    FREQUENCE_PENALTY_FIELD_NUMBER: _ClassVar[int]
+    LOGIT_BIAS_FIELD_NUMBER: _ClassVar[int]
+    LOGPROBS_FIELD_NUMBER: _ClassVar[int]
+    MAX_TOKENS_FIELD_NUMBER: _ClassVar[int]
+    N_FIELD_NUMBER: _ClassVar[int]
+    PRESENCE_PENALTY_FIELD_NUMBER: _ClassVar[int]
+    PROMPT_FIELD_NUMBER: _ClassVar[int]
+    STOP_FIELD_NUMBER: _ClassVar[int]
+    STREAM_FIELD_NUMBER: _ClassVar[int]
+    SUFFIX_FIELD_NUMBER: _ClassVar[int]
+    TEMPERATURE_FIELD_NUMBER: _ClassVar[int]
+    TOP_P_FIELD_NUMBER: _ClassVar[int]
+    best_of: int
+    echo: bool
+    frequence_penalty: float
+    logit_bias: str
+    logprobs: int
+    max_tokens: int
+    n: int
+    presence_penalty: float
+    prompt: str
+    stop: str
+    stream: bool
+    suffix: str
+    temperature: float
+    top_p: float
+    def __init__(
+        self,
+        prompt: _Optional[str] = ...,
+        suffix: _Optional[str] = ...,
+        max_tokens: _Optional[int] = ...,
+        temperature: _Optional[float] = ...,
+        top_p: _Optional[float] = ...,
+        n: _Optional[int] = ...,
+        stream: bool = ...,
+        logprobs: _Optional[int] = ...,
+        echo: bool = ...,
+        stop: _Optional[str] = ...,
+        presence_penalty: _Optional[float] = ...,
+        frequence_penalty: _Optional[float] = ...,
+        best_of: _Optional[int] = ...,
+        logit_bias: _Optional[str] = ...,
+    ) -> None: ...
```

### Comparing `simple_ai_server-0.1.9/simple_ai/clients/completion/llm_pb2_grpc.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,124 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from . import llm_pb2 as llm__pb2
-
-
-class LanguageModelStub(object):
-    """Interface exported by the server.
-    """
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.Complete = channel.unary_unary(
-                '/languagemodel.LanguageModel/Complete',
-                request_serializer=llm__pb2.Message.SerializeToString,
-                response_deserializer=llm__pb2.Completions.FromString,
-                )
-        self.StreamComplete = channel.unary_stream(
-                '/languagemodel.LanguageModel/StreamComplete',
-                request_serializer=llm__pb2.Message.SerializeToString,
-                response_deserializer=llm__pb2.Completions.FromString,
-                )
-
-
-class LanguageModelServicer(object):
-    """Interface exported by the server.
-    """
-
-    def Complete(self, request, context):
-        """Simple RPC.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def StreamComplete(self, request, context):
-        """Server-to-client streaming RPC.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_LanguageModelServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'Complete': grpc.unary_unary_rpc_method_handler(
-                    servicer.Complete,
-                    request_deserializer=llm__pb2.Message.FromString,
-                    response_serializer=llm__pb2.Completions.SerializeToString,
-            ),
-            'StreamComplete': grpc.unary_stream_rpc_method_handler(
-                    servicer.StreamComplete,
-                    request_deserializer=llm__pb2.Message.FromString,
-                    response_serializer=llm__pb2.Completions.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'languagemodel.LanguageModel', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class LanguageModel(object):
-    """Interface exported by the server.
-    """
-
-    @staticmethod
-    def Complete(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/languagemodel.LanguageModel/Complete',
-            llm__pb2.Message.SerializeToString,
-            llm__pb2.Completions.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def StreamComplete(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/languagemodel.LanguageModel/StreamComplete',
-            llm__pb2.Message.SerializeToString,
-            llm__pb2.Completions.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from . import llm_pb2 as llm__pb2
+
+
+class LanguageModelStub(object):
+    """Interface exported by the server."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.Complete = channel.unary_unary(
+            "/languagemodel.LanguageModel/Complete",
+            request_serializer=llm__pb2.Message.SerializeToString,
+            response_deserializer=llm__pb2.Completions.FromString,
+        )
+        self.StreamComplete = channel.unary_stream(
+            "/languagemodel.LanguageModel/StreamComplete",
+            request_serializer=llm__pb2.Message.SerializeToString,
+            response_deserializer=llm__pb2.Completions.FromString,
+        )
+
+
+class LanguageModelServicer(object):
+    """Interface exported by the server."""
+
+    def Complete(self, request, context):
+        """Simple RPC."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+    def StreamComplete(self, request, context):
+        """Server-to-client streaming RPC."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+
+def add_LanguageModelServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+        "Complete": grpc.unary_unary_rpc_method_handler(
+            servicer.Complete,
+            request_deserializer=llm__pb2.Message.FromString,
+            response_serializer=llm__pb2.Completions.SerializeToString,
+        ),
+        "StreamComplete": grpc.unary_stream_rpc_method_handler(
+            servicer.StreamComplete,
+            request_deserializer=llm__pb2.Message.FromString,
+            response_serializer=llm__pb2.Completions.SerializeToString,
+        ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+        "languagemodel.LanguageModel", rpc_method_handlers
+    )
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+# This class is part of an EXPERIMENTAL API.
+class LanguageModel(object):
+    """Interface exported by the server."""
+
+    @staticmethod
+    def Complete(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/languagemodel.LanguageModel/Complete",
+            llm__pb2.Message.SerializeToString,
+            llm__pb2.Completions.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def StreamComplete(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            "/languagemodel.LanguageModel/StreamComplete",
+            llm__pb2.Message.SerializeToString,
+            llm__pb2.Completions.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
```

### Comparing `simple_ai_server-0.1.9/simple_ai/clients/embedding/client.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 from typing import List
 
 import grpc
 from google.protobuf.json_format import MessageToDict
 from . import llm_embed_pb2
 from . import llm_embed_pb2_grpc
 
+
 def get_embeddings(stub, sentences):
     response = stub.Embed(sentences)
     results = []
     for message in response.embedding:
-        results.append(MessageToDict(message).get('feature'))
+        results.append(MessageToDict(message).get("feature"))
     return results
 
 
 def run(
-    url: str='localhost:50051',
-    inputs: List[str]='',
+    url: str = "localhost:50051",
+    inputs: List[str] = "",
 ):
     with grpc.insecure_channel(url) as channel:
-        stub    = llm_embed_pb2_grpc.LanguageModelStub(channel)
+        stub = llm_embed_pb2_grpc.LanguageModelStub(channel)
         sentences = llm_embed_pb2.Sentences(
             inputs=inputs,
         )
         return get_embeddings(stub, sentences)
```

### Comparing `simple_ai_server-0.1.9/simple_ai/clients/embedding/llm_embed_pb2.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: llm_embed.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fllm_embed.proto\x12\x17languagemodelembeddings\"\x1b\n\tSentences\x12\x0e\n\x06inputs\x18\x01 \x03(\t\"\x1c\n\tEmbedding\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x03(\x02\"I\n\x10ListOfEmbeddings\x12\x35\n\tembedding\x18\x01 \x03(\x0b\x32\".languagemodelembeddings.Embedding2i\n\rLanguageModel\x12X\n\x05\x45mbed\x12\".languagemodelembeddings.Sentences\x1a).languagemodelembeddings.ListOfEmbeddings\"\x00\x42:\n\x16io.grpc.examples.embedB\x16LanguageModelEmbeddingP\x01\xa2\x02\x05\x65mbedb\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'llm_embed_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\026io.grpc.examples.embedB\026LanguageModelEmbeddingP\001\242\002\005embed'
-  _SENTENCES._serialized_start=44
-  _SENTENCES._serialized_end=71
-  _EMBEDDING._serialized_start=73
-  _EMBEDDING._serialized_end=101
-  _LISTOFEMBEDDINGS._serialized_start=103
-  _LISTOFEMBEDDINGS._serialized_end=176
-  _LANGUAGEMODEL._serialized_start=178
-  _LANGUAGEMODEL._serialized_end=283
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: llm_embed.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\x0fllm_embed.proto\x12\x17languagemodelembeddings"\x1b\n\tSentences\x12\x0e\n\x06inputs\x18\x01'
+    b' \x03(\t"\x1c\n\tEmbedding\x12\x0f\n\x07\x66\x65\x61ture\x18\x01'
+    b' \x03(\x02"I\n\x10ListOfEmbeddings\x12\x35\n\tembedding\x18\x01'
+    b' \x03(\x0b\x32".languagemodelembeddings.Embedding2i\n\rLanguageModel\x12X\n\x05\x45mbed\x12".languagemodelembeddings.Sentences\x1a).languagemodelembeddings.ListOfEmbeddings"\x00\x42:\n\x16io.grpc.examples.embedB\x16LanguageModelEmbeddingP\x01\xa2\x02\x05\x65mbedb\x06proto3'
+)
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "llm_embed_pb2", globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = (
+        b"\n\026io.grpc.examples.embedB\026LanguageModelEmbeddingP\001\242\002\005embed"
+    )
+    _SENTENCES._serialized_start = 44
+    _SENTENCES._serialized_end = 71
+    _EMBEDDING._serialized_start = 73
+    _EMBEDDING._serialized_end = 101
+    _LISTOFEMBEDDINGS._serialized_start = 103
+    _LISTOFEMBEDDINGS._serialized_end = 176
+    _LANGUAGEMODEL._serialized_start = 178
+    _LANGUAGEMODEL._serialized_end = 283
+# @@protoc_insertion_point(module_scope)
```

### Comparing `simple_ai_server-0.1.9/simple_ai/clients/embedding/llm_embed_pb2.pyi` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-from google.protobuf.internal import containers as _containers
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
-
-DESCRIPTOR: _descriptor.FileDescriptor
-
-class Embedding(_message.Message):
-    __slots__ = ["feature"]
-    FEATURE_FIELD_NUMBER: _ClassVar[int]
-    feature: _containers.RepeatedScalarFieldContainer[float]
-    def __init__(self, feature: _Optional[_Iterable[float]] = ...) -> None: ...
-
-class ListOfEmbeddings(_message.Message):
-    __slots__ = ["embedding"]
-    EMBEDDING_FIELD_NUMBER: _ClassVar[int]
-    embedding: _containers.RepeatedCompositeFieldContainer[Embedding]
-    def __init__(self, embedding: _Optional[_Iterable[_Union[Embedding, _Mapping]]] = ...) -> None: ...
-
-class Sentences(_message.Message):
-    __slots__ = ["inputs"]
-    INPUTS_FIELD_NUMBER: _ClassVar[int]
-    inputs: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, inputs: _Optional[_Iterable[str]] = ...) -> None: ...
+from google.protobuf.internal import containers as _containers
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import (
+    ClassVar as _ClassVar,
+    Iterable as _Iterable,
+    Mapping as _Mapping,
+    Optional as _Optional,
+    Union as _Union,
+)
+
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class Embedding(_message.Message):
+    __slots__ = ["feature"]
+    FEATURE_FIELD_NUMBER: _ClassVar[int]
+    feature: _containers.RepeatedScalarFieldContainer[float]
+    def __init__(self, feature: _Optional[_Iterable[float]] = ...) -> None: ...
+
+class ListOfEmbeddings(_message.Message):
+    __slots__ = ["embedding"]
+    EMBEDDING_FIELD_NUMBER: _ClassVar[int]
+    embedding: _containers.RepeatedCompositeFieldContainer[Embedding]
+    def __init__(
+        self, embedding: _Optional[_Iterable[_Union[Embedding, _Mapping]]] = ...
+    ) -> None: ...
+
+class Sentences(_message.Message):
+    __slots__ = ["inputs"]
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
+    inputs: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, inputs: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `simple_ai_server-0.1.9/simple_ai/clients/embedding/llm_embed_pb2_grpc.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/llm_embed_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,79 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-from . import llm_embed_pb2 as llm__embed__pb2
-
-
-class LanguageModelStub(object):
-    """Interface exported by the server.
-    """
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.Embed = channel.unary_unary(
-                '/languagemodelembeddings.LanguageModel/Embed',
-                request_serializer=llm__embed__pb2.Sentences.SerializeToString,
-                response_deserializer=llm__embed__pb2.ListOfEmbeddings.FromString,
-                )
-
-
-class LanguageModelServicer(object):
-    """Interface exported by the server.
-    """
-
-    def Embed(self, request, context):
-        """Simple RPC
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_LanguageModelServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'Embed': grpc.unary_unary_rpc_method_handler(
-                    servicer.Embed,
-                    request_deserializer=llm__embed__pb2.Sentences.FromString,
-                    response_serializer=llm__embed__pb2.ListOfEmbeddings.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'languagemodelembeddings.LanguageModel', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class LanguageModel(object):
-    """Interface exported by the server.
-    """
-
-    @staticmethod
-    def Embed(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/languagemodelembeddings.LanguageModel/Embed',
-            llm__embed__pb2.Sentences.SerializeToString,
-            llm__embed__pb2.ListOfEmbeddings.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+from . import llm_embed_pb2 as llm__embed__pb2
+
+
+class LanguageModelStub(object):
+    """Interface exported by the server."""
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.Embed = channel.unary_unary(
+            "/languagemodelembeddings.LanguageModel/Embed",
+            request_serializer=llm__embed__pb2.Sentences.SerializeToString,
+            response_deserializer=llm__embed__pb2.ListOfEmbeddings.FromString,
+        )
+
+
+class LanguageModelServicer(object):
+    """Interface exported by the server."""
+
+    def Embed(self, request, context):
+        """Simple RPC"""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+
+def add_LanguageModelServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+        "Embed": grpc.unary_unary_rpc_method_handler(
+            servicer.Embed,
+            request_deserializer=llm__embed__pb2.Sentences.FromString,
+            response_serializer=llm__embed__pb2.ListOfEmbeddings.SerializeToString,
+        ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+        "languagemodelembeddings.LanguageModel", rpc_method_handlers
+    )
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+# This class is part of an EXPERIMENTAL API.
+class LanguageModel(object):
+    """Interface exported by the server."""
+
+    @staticmethod
+    def Embed(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/languagemodelembeddings.LanguageModel/Embed",
+            llm__embed__pb2.Sentences.SerializeToString,
+            llm__embed__pb2.ListOfEmbeddings.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
```

### Comparing `simple_ai_server-0.1.9/simple_ai/protos/llm.proto` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_complete.proto`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.1.9/simple_ai/protos/llm_embed.proto` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/protos/llm_embed.proto`

 * *Files identical despite different names*

### Comparing `simple_ai_server-0.1.9/simple_ai/serve/python/completion/llm_pb2.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/llm_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: llm.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tllm.proto\x12\rlanguagemodel\"\x84\x02\n\x07Message\x12\x0e\n\x06prompt\x18\x01 \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\x12\n\nmax_tokens\x18\x03 \x01(\x05\x12\x13\n\x0btemperature\x18\x04 \x01(\x02\x12\r\n\x05top_p\x18\x05 \x01(\x02\x12\t\n\x01n\x18\x06 \x01(\x05\x12\x0e\n\x06stream\x18\x07 \x01(\x08\x12\x10\n\x08logprobs\x18\x08 \x01(\x05\x12\x0c\n\x04\x65\x63ho\x18\t \x01(\x08\x12\x0c\n\x04stop\x18\n \x01(\t\x12\x18\n\x10presence_penalty\x18\x0b \x01(\x02\x12\x19\n\x11\x66requence_penalty\x18\x0c \x01(\x02\x12\x0f\n\x07\x62\x65st_of\x18\r \x01(\x05\x12\x12\n\nlogit_bias\x18\x0e \x01(\t\"\x1c\n\x0b\x43ompletions\x12\r\n\x05reply\x18\x01 \x01(\t2\x9b\x01\n\rLanguageModel\x12@\n\x08\x43omplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions\"\x00\x12H\n\x0eStreamComplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions\"\x00\x30\x01\x42+\n\x13io.grpc.examples.lmB\rLanguageModelP\x01\xa2\x02\x02LMb\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'llm_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\023io.grpc.examples.lmB\rLanguageModelP\001\242\002\002LM'
-  _MESSAGE._serialized_start=29
-  _MESSAGE._serialized_end=289
-  _COMPLETIONS._serialized_start=291
-  _COMPLETIONS._serialized_end=319
-  _LANGUAGEMODEL._serialized_start=322
-  _LANGUAGEMODEL._serialized_end=477
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: llm.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
+    b'\n\tllm.proto\x12\rlanguagemodel"\x84\x02\n\x07Message\x12\x0e\n\x06prompt\x18\x01'
+    b" \x01(\t\x12\x0e\n\x06suffix\x18\x02 \x01(\t\x12\x12\n\nmax_tokens\x18\x03"
+    b" \x01(\x05\x12\x13\n\x0btemperature\x18\x04 \x01(\x02\x12\r\n\x05top_p\x18\x05"
+    b" \x01(\x02\x12\t\n\x01n\x18\x06 \x01(\x05\x12\x0e\n\x06stream\x18\x07"
+    b" \x01(\x08\x12\x10\n\x08logprobs\x18\x08 \x01(\x05\x12\x0c\n\x04\x65\x63ho\x18\t"
+    b" \x01(\x08\x12\x0c\n\x04stop\x18\n \x01(\t\x12\x18\n\x10presence_penalty\x18\x0b"
+    b" \x01(\x02\x12\x19\n\x11\x66requence_penalty\x18\x0c"
+    b" \x01(\x02\x12\x0f\n\x07\x62\x65st_of\x18\r \x01(\x05\x12\x12\n\nlogit_bias\x18\x0e"
+    b' \x01(\t"\x1c\n\x0b\x43ompletions\x12\r\n\x05reply\x18\x01'
+    b' \x01(\t2\x9b\x01\n\rLanguageModel\x12@\n\x08\x43omplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions"\x00\x12H\n\x0eStreamComplete\x12\x16.languagemodel.Message\x1a\x1a.languagemodel.Completions"\x00\x30\x01\x42+\n\x13io.grpc.examples.lmB\rLanguageModelP\x01\xa2\x02\x02LMb\x06proto3'
+)
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "llm_pb2", globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = b"\n\023io.grpc.examples.lmB\rLanguageModelP\001\242\002\002LM"
+    _MESSAGE._serialized_start = 29
+    _MESSAGE._serialized_end = 289
+    _COMPLETIONS._serialized_start = 291
+    _COMPLETIONS._serialized_end = 319
+    _LANGUAGEMODEL._serialized_start = 322
+    _LANGUAGEMODEL._serialized_end = 477
+# @@protoc_insertion_point(module_scope)
```

### Comparing `simple_ai_server-0.1.9/simple_ai/serve/python/completion/server.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/completion/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,78 +8,69 @@
 from . import llm_pb2_grpc
 
 from .model import LanguageModel
 
 
 class LanguageModelServicer(llm_pb2_grpc.LanguageModelServicer):
     """Provides methods that implement functionality of route guide server."""
-    
+
     def __init__(self, model=LanguageModel()) -> None:
         super().__init__()
         self.model = model
-    
+
     def Complete(self, request, context):
         predicted = self.model.complete(
             prompt=request.prompt,
             suffix=request.suffix,
-
             max_tokens=request.max_tokens,
             temperature=request.temperature,
-
             top_p=request.top_p,
             n=request.n,
             stream=request.stream,
-
             logprobs=request.logprobs,
             echo=request.echo,
             stop=request.stop,
             presence_penalty=request.presence_penalty,
             frequence_penalty=request.frequence_penalty,
-
             best_of=request.best_of,
-            logit_bias=request.logit_bias
+            logit_bias=request.logit_bias,
         )
         return llm_pb2.Completions(reply=predicted)
 
     def StreamComplete(self, request, context):
-        predicted = self.model.complete(
+        predicted_stream = self.model.stream_complete(
             prompt=request.prompt,
             suffix=request.suffix,
-
             max_tokens=request.max_tokens,
             temperature=request.temperature,
-
             top_p=request.top_p,
             n=request.n,
             stream=request.stream,
-
             logprobs=request.logprobs,
             echo=request.echo,
             stop=request.stop,
             presence_penalty=request.presence_penalty,
             frequence_penalty=request.frequence_penalty,
-
             best_of=request.best_of,
-            logit_bias=request.logit_bias
+            logit_bias=request.logit_bias,
         )
-        return llm_pb2.Completions(reply=predicted)
+        yield from map(lambda predicted: llm_pb2.Completions(reply=predicted), predicted_stream)
 
 
-def serve(address='[::]:50051', model_servicer=LanguageModelServicer(), max_workers=10):
+def serve(address="[::]:50051", model_servicer=LanguageModelServicer(), max_workers=10):
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=max_workers))
-    llm_pb2_grpc.add_LanguageModelServicer_to_server(
-        model_servicer, server)
+    llm_pb2_grpc.add_LanguageModelServicer_to_server(model_servicer, server)
     server.add_insecure_port(address=address)
     server.start()
     server.wait_for_termination()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import argparse
-    
+
     logging.basicConfig()
-    
+
     parser = argparse.ArgumentParser()
-    parser.add_argument('address', type=str, default='[::]:50051')
+    parser.add_argument("address", type=str, default="[::]:50051")
     args = parser.parse_args()
 
     serve(address=args.address)
```

### Comparing `simple_ai_server-0.1.9/simple_ai/serve/python/embedding/server.py` & `simple_ai_server-0.2.0/src/simple_ai/api/grpc/embedding/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,44 +8,43 @@
 from . import llm_embed_pb2_grpc
 
 from .model import LanguageModel
 
 
 class LanguageModelServicer(llm_embed_pb2_grpc.LanguageModelServicer):
     """Provides methods that implement functionality of route guide server."""
-    
+
     def __init__(self, model=LanguageModel()) -> None:
         super().__init__()
         self.model = model
-    
+
     def Embed(self, request, context):
         embeddings = self.model.embed(
             inputs=request.inputs,
         )
         grpc_embeddings = llm_embed_pb2.ListOfEmbeddings()
         for embedding in embeddings:
             grpc_embedding = llm_embed_pb2.Embedding()
             for feature in embedding:
                 grpc_embedding.feature.append(feature)
             grpc_embeddings.embedding.append(grpc_embedding)
         return grpc_embeddings
 
 
-def serve(address='[::]:50051', model_servicer=LanguageModelServicer(), max_workers=10):
+def serve(address="[::]:50051", model_servicer=LanguageModelServicer(), max_workers=10):
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=max_workers))
-    llm_embed_pb2_grpc.add_LanguageModelServicer_to_server(
-        model_servicer, server)
+    llm_embed_pb2_grpc.add_LanguageModelServicer_to_server(model_servicer, server)
     server.add_insecure_port(address=address)
     server.start()
     server.wait_for_termination()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import argparse
-    
+
     logging.basicConfig()
-    
+
     parser = argparse.ArgumentParser()
-    parser.add_argument('address', type=str, default='[::]:50051')
+    parser.add_argument("address", type=str, default="[::]:50051")
     args = parser.parse_args()
 
     serve(address=args.address)
```

