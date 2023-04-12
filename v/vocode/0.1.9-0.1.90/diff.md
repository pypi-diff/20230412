# Comparing `tmp/vocode-0.1.9.tar.gz` & `tmp/vocode-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocode-0.1.9.tar", max compression
+gzip compressed data, was "vocode-0.1.90.tar", max compression
```

## Comparing `vocode-0.1.9.tar` & `vocode-0.1.90.tar`

### file list

```diff
@@ -1,21 +1,99 @@
--rw-r--r--   0        0        0     1037 2023-03-02 21:15:36.594335 vocode-0.1.9/README.md
--rw-r--r--   0        0        0      416 2023-03-03 00:15:40.135268 vocode-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       94 2023-02-26 05:14:14.763240 vocode-0.1.9/vocode/__init__.py
--rw-r--r--   0        0        0     3198 2023-03-02 21:15:36.604376 vocode-0.1.9/vocode/conversation.py
--rw-r--r--   0        0        0     1644 2023-02-27 19:22:49.888374 vocode-0.1.9/vocode/helpers.py
--rw-r--r--   0        0        0      448 2023-02-19 07:33:59.411644 vocode-0.1.9/vocode/input_device/base_input_device.py
--rw-r--r--   0        0        0     1284 2023-02-27 19:30:50.394673 vocode-0.1.9/vocode/input_device/microphone_input.py
--rw-r--r--   0        0        0     2715 2023-03-03 00:06:16.198715 vocode-0.1.9/vocode/models/agent.py
--rw-r--r--   0        0        0      100 2023-02-17 08:34:02.846253 vocode-0.1.9/vocode/models/audio_encoding.py
--rw-r--r--   0        0        0     1468 2023-03-02 21:15:42.667485 vocode-0.1.9/vocode/models/model.py
--rw-r--r--   0        0        0      872 2023-02-22 21:57:26.044989 vocode-0.1.9/vocode/models/synthesizer.py
--rw-r--r--   0        0        0      372 2023-02-20 08:53:28.748885 vocode-0.1.9/vocode/models/telephony.py
--rw-r--r--   0        0        0     1181 2023-02-27 19:22:49.889614 vocode-0.1.9/vocode/models/transcriber.py
--rw-r--r--   0        0        0     1024 2023-02-19 08:38:54.611719 vocode-0.1.9/vocode/models/websocket.py
--rw-r--r--   0        0        0      376 2023-02-16 23:41:55.730892 vocode-0.1.9/vocode/output_device/base_output_device.py
--rw-r--r--   0        0        0      951 2023-02-27 19:22:49.890156 vocode-0.1.9/vocode/output_device/speaker_output.py
--rw-r--r--   0        0        0      316 2023-03-02 21:15:42.667630 vocode-0.1.9/vocode/user_implemented_agent/base_agent.py
--rw-r--r--   0        0        0      503 2023-03-02 21:15:42.667775 vocode-0.1.9/vocode/user_implemented_agent/restful_agent.py
--rw-r--r--   0        0        0     1109 2023-03-02 21:15:42.667914 vocode-0.1.9/vocode/user_implemented_agent/websocket_agent.py
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 vocode-0.1.9/setup.py
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 vocode-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-28 17:29:00.108721 vocode-0.1.90/LICENSE
+-rw-r--r--   0        0        0     8266 2023-04-12 08:05:58.013355 vocode-0.1.90/README.md
+-rw-r--r--   0        0        0     2059 2023-04-12 20:14:46.898125 vocode-0.1.90/pyproject.toml
+-rw-r--r--   0        0        0      308 2023-03-28 17:30:02.280446 vocode-0.1.90/vocode/__init__.py
+-rw-r--r--   0        0        0     2390 2023-03-28 07:12:57.812230 vocode-0.1.90/vocode/helpers.py
+-rw-r--r--   0        0        0     1536 2023-04-11 21:06:59.690563 vocode-0.1.90/vocode/streaming/agent/base_agent.py
+-rw-r--r--   0        0        0     2007 2023-03-29 06:28:34.480507 vocode-0.1.90/vocode/streaming/agent/bot_sentiment_analyser.py
+-rw-r--r--   0        0        0     6659 2023-04-11 17:15:11.306264 vocode-0.1.90/vocode/streaming/agent/chat_gpt_agent.py
+-rw-r--r--   0        0        0      591 2023-04-11 17:15:11.306521 vocode-0.1.90/vocode/streaming/agent/echo_agent.py
+-rw-r--r--   0        0        0     1467 2023-04-11 21:06:59.691054 vocode-0.1.90/vocode/streaming/agent/factory.py
+-rw-r--r--   0        0        0     1481 2023-03-28 17:30:02.281854 vocode-0.1.90/vocode/streaming/agent/information_retrieval_agent.py
+-rw-r--r--   0        0        0     5724 2023-04-11 17:15:11.307183 vocode-0.1.90/vocode/streaming/agent/llm_agent.py
+-rw-r--r--   0        0        0     2053 2023-04-11 17:15:11.308601 vocode-0.1.90/vocode/streaming/agent/restful_user_implemented_agent.py
+-rw-r--r--   0        0        0      684 2023-03-28 17:30:02.282322 vocode-0.1.90/vocode/streaming/agent/utils.py
+-rw-r--r--   0        0        0     3259 2023-04-04 06:04:39.618650 vocode-0.1.90/vocode/streaming/client_backend/conversation.py
+-rw-r--r--   0        0        0       96 2023-03-28 17:30:02.282460 vocode-0.1.90/vocode/streaming/constants.py
+-rw-r--r--   0        0        0     3724 2023-04-12 18:22:27.897471 vocode-0.1.90/vocode/streaming/hosted_streaming_conversation.py
+-rw-r--r--   0        0        0      476 2023-03-28 07:12:57.812101 vocode-0.1.90/vocode/streaming/input_device/base_input_device.py
+-rw-r--r--   0        0        0     1648 2023-03-28 07:12:57.809750 vocode-0.1.90/vocode/streaming/input_device/microphone_input.py
+-rw-r--r--   0        0        0      334 2023-03-28 07:12:57.811970 vocode-0.1.90/vocode/streaming/input_device/telephone_input.py
+-rw-r--r--   0        0        0     5314 2023-04-11 21:06:59.691420 vocode-0.1.90/vocode/streaming/models/agent.py
+-rw-r--r--   0        0        0      102 2023-03-28 17:30:02.283498 vocode-0.1.90/vocode/streaming/models/audio_encoding.py
+-rw-r--r--   0        0        0      856 2023-04-03 01:45:30.651534 vocode-0.1.90/vocode/streaming/models/events.py
+-rw-r--r--   0        0        0      299 2023-03-28 07:12:57.772953 vocode-0.1.90/vocode/streaming/models/message.py
+-rw-r--r--   0        0        0     1455 2023-03-28 17:30:02.283821 vocode-0.1.90/vocode/streaming/models/model.py
+-rw-r--r--   0        0        0     3468 2023-04-11 21:06:59.691711 vocode-0.1.90/vocode/streaming/models/synthesizer.py
+-rw-r--r--   0        0        0     1806 2023-03-28 17:30:02.284366 vocode-0.1.90/vocode/streaming/models/telephony.py
+-rw-r--r--   0        0        0     3254 2023-04-12 08:06:19.437996 vocode-0.1.90/vocode/streaming/models/transcriber.py
+-rw-r--r--   0        0        0     1765 2023-04-04 06:04:39.619062 vocode-0.1.90/vocode/streaming/models/websocket.py
+-rw-r--r--   0        0        0      396 2023-03-28 17:30:02.285240 vocode-0.1.90/vocode/streaming/output_device/base_output_device.py
+-rw-r--r--   0        0        0     1015 2023-03-28 07:12:57.807120 vocode-0.1.90/vocode/streaming/output_device/speaker_output.py
+-rw-r--r--   0        0        0      262 2023-03-28 07:12:57.809162 vocode-0.1.90/vocode/streaming/output_device/telephone_output.py
+-rw-r--r--   0        0        0     1148 2023-04-04 06:04:39.619476 vocode-0.1.90/vocode/streaming/output_device/twilio_output_device.py
+-rw-r--r--   0        0        0      800 2023-04-04 06:04:39.619698 vocode-0.1.90/vocode/streaming/output_device/websocket_output_device.py
+-rw-r--r--   0        0        0    21220 2023-04-12 07:56:17.824251 vocode-0.1.90/vocode/streaming/streaming_conversation.py
+-rw-r--r--   0        0        0    10570 2023-04-10 22:54:02.366120 vocode-0.1.90/vocode/streaming/synthesizer/azure_synthesizer.py
+-rw-r--r--   0        0        0     7673 2023-04-11 21:06:59.693069 vocode-0.1.90/vocode/streaming/synthesizer/base_synthesizer.py
+-rw-r--r--   0        0        0     2355 2023-04-12 08:05:58.014267 vocode-0.1.90/vocode/streaming/synthesizer/eleven_labs_synthesizer.py
+-rw-r--r--   0        0        0     1448 2023-04-11 21:06:59.693827 vocode-0.1.90/vocode/streaming/synthesizer/factory.py
+-rw-r--r--   0        0        0  6548060 2023-03-28 17:30:02.328281 vocode-0.1.90/vocode/streaming/synthesizer/filler_audio/typing-noise.wav
+-rw-r--r--   0        0        0     3396 2023-04-11 21:06:59.694063 vocode-0.1.90/vocode/streaming/synthesizer/google_synthesizer.py
+-rw-r--r--   0        0        0     2463 2023-04-11 21:06:59.694296 vocode-0.1.90/vocode/streaming/synthesizer/play_ht_synthesizer.py
+-rw-r--r--   0        0        0     1795 2023-04-12 06:50:30.491534 vocode-0.1.90/vocode/streaming/synthesizer/rime_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-03-28 17:30:02.329443 vocode-0.1.90/vocode/streaming/telephony/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-28 17:30:02.330427 vocode-0.1.90/vocode/streaming/telephony/config_manager/base_config_manager.py
+-rw-r--r--   0        0        0      609 2023-03-28 23:14:27.148000 vocode-0.1.90/vocode/streaming/telephony/config_manager/in_memory_config_manager.py
+-rw-r--r--   0        0        0     1248 2023-03-28 17:30:02.331245 vocode-0.1.90/vocode/streaming/telephony/config_manager/redis_config_manager.py
+-rw-r--r--   0        0        0      170 2023-03-28 17:30:02.331397 vocode-0.1.90/vocode/streaming/telephony/constants.py
+-rw-r--r--   0        0        0     6799 2023-04-11 21:06:59.694996 vocode-0.1.90/vocode/streaming/telephony/conversation/call.py
+-rw-r--r--   0        0        0     4136 2023-04-11 17:15:11.315392 vocode-0.1.90/vocode/streaming/telephony/conversation/outbound_call.py
+-rw-r--r--   0        0        0     2802 2023-03-28 17:30:02.332164 vocode-0.1.90/vocode/streaming/telephony/conversation/zoom_dial_in.py
+-rw-r--r--   0        0        0      106 2023-04-03 01:45:30.652609 vocode-0.1.90/vocode/streaming/telephony/hosted/exceptions.py
+-rw-r--r--   0        0        0     2264 2023-03-28 17:30:02.332438 vocode-0.1.90/vocode/streaming/telephony/hosted/inbound_call_server.py
+-rw-r--r--   0        0        0     1697 2023-03-28 17:30:02.332777 vocode-0.1.90/vocode/streaming/telephony/hosted/inbound_call_user_agent_server.py
+-rw-r--r--   0        0        0     3032 2023-04-03 01:45:30.652914 vocode-0.1.90/vocode/streaming/telephony/hosted/outbound_call.py
+-rw-r--r--   0        0        0     2458 2023-04-03 01:45:30.653149 vocode-0.1.90/vocode/streaming/telephony/hosted/zoom_dial_in.py
+-rw-r--r--   0        0        0     5845 2023-04-11 21:06:59.695325 vocode-0.1.90/vocode/streaming/telephony/server/base.py
+-rw-r--r--   0        0        0     2439 2023-04-11 21:06:59.695619 vocode-0.1.90/vocode/streaming/telephony/server/router/calls.py
+-rw-r--r--   0        0        0      865 2023-04-04 06:04:39.620616 vocode-0.1.90/vocode/streaming/telephony/server/router/twiml.py
+-rw-r--r--   0        0        0      150 2023-03-28 17:30:02.333925 vocode-0.1.90/vocode/streaming/telephony/templates/connect_call.xml
+-rw-r--r--   0        0        0      653 2023-03-28 17:30:02.333757 vocode-0.1.90/vocode/streaming/telephony/templates.py
+-rw-r--r--   0        0        0      434 2023-04-11 21:06:59.695870 vocode-0.1.90/vocode/streaming/telephony/twilio.py
+-rw-r--r--   0        0        0     2220 2023-03-21 03:19:41.096039 vocode-0.1.90/vocode/streaming/telephony/zoom_dial_in.py
+-rw-r--r--   0        0        0     3452 2023-04-12 08:03:51.421371 vocode-0.1.90/vocode/streaming/transcriber/assembly_ai_transcriber.py
+-rw-r--r--   0        0        0     1241 2023-04-11 21:06:59.696653 vocode-0.1.90/vocode/streaming/transcriber/base_transcriber.py
+-rw-r--r--   0        0        0     7975 2023-04-12 07:59:00.960353 vocode-0.1.90/vocode/streaming/transcriber/deepgram_transcriber.py
+-rw-r--r--   0        0        0     1249 2023-04-12 08:05:58.014409 vocode-0.1.90/vocode/streaming/transcriber/factory.py
+-rw-r--r--   0        0        0     4377 2023-04-12 08:00:45.683444 vocode-0.1.90/vocode/streaming/transcriber/google_transcriber.py
+-rw-r--r--   0        0        0     4800 2023-04-12 08:05:58.014523 vocode-0.1.90/vocode/streaming/transcriber/rev_ai_transcriber.py
+-rw-r--r--   0        0        0     3353 2023-04-11 23:13:05.536070 vocode-0.1.90/vocode/streaming/transcriber/whisper_cpp_transcriber.py
+-rw-r--r--   0        0        0      216 2023-03-28 07:12:57.762251 vocode-0.1.90/vocode/streaming/user_implemented_agent/base_agent.py
+-rw-r--r--   0        0        0      697 2023-03-28 07:12:57.762593 vocode-0.1.90/vocode/streaming/user_implemented_agent/restful_agent.py
+-rw-r--r--   0        0        0     2183 2023-03-28 07:12:57.762008 vocode-0.1.90/vocode/streaming/user_implemented_agent/websocket_agent.py
+-rw-r--r--   0        0        0     1768 2023-03-28 17:30:02.335417 vocode-0.1.90/vocode/streaming/utils/__init__.py
+-rw-r--r--   0        0        0      125 2023-04-04 06:04:39.620775 vocode-0.1.90/vocode/streaming/utils/base_router.py
+-rw-r--r--   0        0        0        0 2023-03-28 17:30:02.335448 vocode-0.1.90/vocode/streaming/utils/goodbye_embeddings/.gitkeep
+-rw-r--r--   0        0        0     2237 2023-03-29 06:27:49.549508 vocode-0.1.90/vocode/streaming/utils/goodbye_model.py
+-rw-r--r--   0        0        0     7782 2023-03-28 17:30:02.335881 vocode-0.1.90/vocode/streaming/utils/sse_client.py
+-rw-r--r--   0        0        0     1085 2023-03-28 17:30:02.336058 vocode-0.1.90/vocode/streaming/utils/transcript.py
+-rw-r--r--   0        0        0      233 2023-03-28 07:12:57.813897 vocode-0.1.90/vocode/turn_based/agent/base_agent.py
+-rw-r--r--   0        0        0     1758 2023-04-11 23:08:06.680994 vocode-0.1.90/vocode/turn_based/agent/chat_gpt_agent.py
+-rw-r--r--   0        0        0      155 2023-03-28 07:12:57.813754 vocode-0.1.90/vocode/turn_based/agent/echo_agent.py
+-rw-r--r--   0        0        0      201 2023-03-28 07:12:57.817990 vocode-0.1.90/vocode/turn_based/input_device/base_input_device.py
+-rw-r--r--   0        0        0     2040 2023-04-04 06:04:39.620961 vocode-0.1.90/vocode/turn_based/input_device/microphone_input.py
+-rw-r--r--   0        0        0      185 2023-03-28 07:12:57.817099 vocode-0.1.90/vocode/turn_based/output_device/base_output_device.py
+-rw-r--r--   0        0        0     1244 2023-04-04 06:04:39.621216 vocode-0.1.90/vocode/turn_based/output_device/speaker_output.py
+-rw-r--r--   0        0        0     2413 2023-04-04 06:04:39.621552 vocode-0.1.90/vocode/turn_based/synthesizer/azure_synthesizer.py
+-rw-r--r--   0        0        0      138 2023-03-28 07:12:57.815598 vocode-0.1.90/vocode/turn_based/synthesizer/base_synthesizer.py
+-rw-r--r--   0        0        0     1733 2023-04-04 06:04:39.621772 vocode-0.1.90/vocode/turn_based/synthesizer/eleven_labs_synthesizer.py
+-rw-r--r--   0        0        0      409 2023-04-11 17:15:11.317870 vocode-0.1.90/vocode/turn_based/synthesizer/gtts_synthesizer.py
+-rw-r--r--   0        0        0     1562 2023-04-11 21:06:59.697759 vocode-0.1.90/vocode/turn_based/synthesizer/play_ht_synthesizer.py
+-rw-r--r--   0        0        0      973 2023-04-11 17:15:11.318340 vocode-0.1.90/vocode/turn_based/synthesizer/rime_synthesizer.py
+-rw-r--r--   0        0        0      152 2023-03-28 07:12:57.812543 vocode-0.1.90/vocode/turn_based/transcriber/base_transcriber.py
+-rw-r--r--   0        0        0     1532 2023-04-11 23:13:05.536284 vocode-0.1.90/vocode/turn_based/transcriber/whisper_cpp_transcriber.py
+-rw-r--r--   0        0        0      770 2023-03-28 17:30:02.337446 vocode-0.1.90/vocode/turn_based/transcriber/whisper_transcriber.py
+-rw-r--r--   0        0        0     1638 2023-03-28 07:12:57.817247 vocode-0.1.90/vocode/turn_based/turn_based_conversation.py
+-rw-r--r--   0        0        0      872 2023-04-11 23:13:05.536499 vocode-0.1.90/vocode/utils/whisper_cpp/helpers.py
+-rw-r--r--   0        0        0     2124 2023-04-11 23:13:05.536728 vocode-0.1.90/vocode/utils/whisper_cpp/whisper_params.py
+-rw-r--r--   0        0        0    11497 1970-01-01 00:00:00.000000 vocode-0.1.90/PKG-INFO
```

### Comparing `vocode-0.1.9/vocode/conversation.py` & `vocode-0.1.90/vocode/streaming/hosted_streaming_conversation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,102 @@
 import websockets
+from websockets.exceptions import ConnectionClosedOK
+from websockets.client import WebSocketClientProtocol
 import asyncio
-from dotenv import load_dotenv
-import os
 import logging
 import threading
 import queue
+import vocode
+from vocode.streaming.input_device.base_input_device import (
+    BaseInputDevice,
+)
+from vocode.streaming.output_device.base_output_device import BaseOutputDevice
+from vocode.streaming.models.transcriber import TranscriberConfig
+from vocode.streaming.models.agent import AgentConfig
+from vocode.streaming.models.synthesizer import SynthesizerConfig
+from vocode.streaming.models.websocket import (
+    ReadyMessage,
+    AudioMessage,
+    StartMessage,
+    StopMessage,
+)
 
-load_dotenv()
-
-from .input_device.base_input_device import BaseInputDevice
-from .output_device.base_output_device import BaseOutputDevice
-from .models.transcriber import TranscriberConfig
-from .models.agent import AgentConfig
-from .models.synthesizer import SynthesizerConfig
-from .models.websocket import ReadyMessage, AudioMessage, StartMessage, StopMessage
-from . import api_key
-
-VOCODE_WEBSOCKET_URL = f'wss://api.vocode.dev/conversation'
-
-class Conversation:
 
+class HostedStreamingConversation:
     def __init__(
         self,
-        input_device: BaseInputDevice, 
-        output_device: BaseOutputDevice, 
-        transcriber_config: TranscriberConfig, 
+        input_device: BaseInputDevice,
+        output_device: BaseOutputDevice,
+        transcriber_config: TranscriberConfig,
         agent_config: AgentConfig,
-        synthesizer_config: SynthesizerConfig
+        synthesizer_config: SynthesizerConfig,
+        id: str = None,
     ):
+        self.id = id
         self.input_device = input_device
         self.output_device = output_device
         self.transcriber_config = transcriber_config
         self.agent_config = agent_config
         self.synthesizer_config = synthesizer_config
         self.logger = logging.getLogger(__name__)
         self.receiver_ready = False
         self.active = True
         self.output_loop = asyncio.new_event_loop()
         self.output_audio_queue = queue.Queue()
+        self.vocode_websocket_url = f"wss://{vocode.base_url}/conversation"
 
     async def wait_for_ready(self):
         while not self.receiver_ready:
             await asyncio.sleep(0.1)
         return True
-    
+
     def deactivate(self):
         self.active = False
 
     def play_audio(self):
         async def run():
             while self.active:
                 try:
                     audio = self.output_audio_queue.get(timeout=5)
                     await self.output_device.send_async(audio)
                 except queue.Empty:
                     continue
+
         loop = asyncio.new_event_loop()
         loop.run_until_complete(run())
-    
+
     async def start(self):
-        async with websockets.connect(f"{VOCODE_WEBSOCKET_URL}?key={api_key}") as ws:
-            async def sender(ws):
+        async with websockets.connect(
+            f"{self.vocode_websocket_url}?key={vocode.api_key}"
+        ) as ws:
+
+            async def sender(ws: WebSocketClientProtocol):
                 start_message = StartMessage(
-                    transcriber_config=self.transcriber_config, 
-                    agent_config=self.agent_config, 
-                    synthesizer_config=self.synthesizer_config
+                    transcriber_config=self.transcriber_config,
+                    agent_config=self.agent_config,
+                    synthesizer_config=self.synthesizer_config,
+                    conversation_id=self.id,
                 )
                 await ws.send(start_message.json())
                 await self.wait_for_ready()
                 self.logger.info("Listening...press Ctrl+C to stop")
                 while self.active:
                     data = self.input_device.get_audio()
                     if data:
-                        await ws.send(AudioMessage.from_bytes(data).json())
+                        try:
+                            await ws.send(AudioMessage.from_bytes(data).json())
+                        except ConnectionClosedOK:
+                            self.deactivate()
+                            return
                         await asyncio.sleep(0)
                 await ws.send(StopMessage().json())
 
-            async def receiver(ws):
+            async def receiver(ws: WebSocketClientProtocol):
                 ReadyMessage.parse_raw(await ws.recv())
                 self.receiver_ready = True
                 async for msg in ws:
                     audio_message = AudioMessage.parse_raw(msg)
                     self.output_audio_queue.put_nowait(audio_message.get_bytes())
 
-
             output_thread = threading.Thread(target=self.play_audio)
             output_thread.start()
             return await asyncio.gather(sender(ws), receiver(ws))
-
```

### Comparing `vocode-0.1.9/vocode/input_device/microphone_input.py` & `vocode-0.1.90/vocode/streaming/input_device/microphone_input.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,51 @@
-import pyaudio
+import sounddevice as sd
+import numpy as np
 from typing import Optional
 import queue
+import wave
 
-from .base_input_device import BaseInputDevice
-from ..models.audio_encoding import AudioEncoding
+from vocode.streaming.input_device.base_input_device import BaseInputDevice
+from vocode.streaming.models.audio_encoding import AudioEncoding
 
-class MicrophoneInput(BaseInputDevice):
 
+class MicrophoneInput(BaseInputDevice):
     DEFAULT_SAMPLING_RATE = 44100
     DEFAULT_CHUNK_SIZE = 2048
 
-    def __init__(self, pa: pyaudio.PyAudio, device_info: dict, sampling_rate: int = None, chunk_size: int = DEFAULT_CHUNK_SIZE):
+    def __init__(
+        self,
+        device_info: dict,
+        sampling_rate: int = None,
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
+        microphone_gain: int = 1,
+    ):
         self.device_info = device_info
-        sampling_rate = sampling_rate or (self.device_info.get('defaultSampleRate', self.DEFAULT_SAMPLING_RATE))
+        sampling_rate = sampling_rate or (
+            self.device_info.get("default_samplerate", self.DEFAULT_SAMPLING_RATE)
+        )
         super().__init__(int(sampling_rate), AudioEncoding.LINEAR16, chunk_size)
-        self.pa = pa
-        self.stream = pa.open(
-            format=pyaudio.paInt16,
+        self.stream = sd.InputStream(
+            dtype=np.int16,
             channels=1,
-            rate=self.sampling_rate,
-            input=True,
-            frames_per_buffer=self.chunk_size,
-            input_device_index=int(self.device_info['index']),
-            stream_callback=self._stream_callback
+            samplerate=self.sampling_rate,
+            blocksize=self.chunk_size,
+            device=int(self.device_info["index"]),
+            callback=self._stream_callback,
         )
+        self.stream.start()
         self.queue = queue.Queue()
+        self.microphone_gain = microphone_gain
 
-    def _stream_callback(self, in_data, *_args):
-        self.queue.put_nowait(in_data)
-        return (None, pyaudio.paContinue)
+    def _stream_callback(self, in_data: np.ndarray[np.int16], *_args):
+        if self.microphone_gain > 1:
+            in_data = in_data * (2 ^ self.microphone_gain)
+        else:
+            in_data = in_data // (2 ^ self.microphone_gain)
+        audio_bytes = in_data.tobytes()
+        self.queue.put_nowait(audio_bytes)
 
     def get_audio(self) -> Optional[bytes]:
         try:
             return self.queue.get_nowait()
         except queue.Empty:
-            return None
+            return None
```

### Comparing `vocode-0.1.9/vocode/models/model.py` & `vocode-0.1.90/vocode/streaming/models/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 import pydantic
 
-class BaseModel(pydantic.BaseModel):
 
+class BaseModel(pydantic.BaseModel):
     def __init__(self, **data):
         for key, value in data.items():
             if isinstance(value, dict):
-                if 'type' in value:
+                if "type" in value:
                     data[key] = TypedModel.parse_obj(value)
         super().__init__(**data)
 
+
 # Adapted from https://github.com/pydantic/pydantic/discussions/3091
 class TypedModel(BaseModel):
-
     _subtypes_ = []
 
     def __init_subclass__(cls, type=None):
         cls._subtypes_.append([type, cls])
 
     @classmethod
     def get_cls(_cls, type):
         for t, cls in _cls._subtypes_:
             if t == type:
                 return cls
-        raise ValueError(f'Unknown type {type}')
-    
+        raise ValueError(f"Unknown type {type}")
+
     @classmethod
     def get_type(_cls, cls_name):
         for t, cls in _cls._subtypes_:
             if cls.__name__ == cls_name:
                 return t
-        raise ValueError(f'Unknown class {cls_name}')
-    
+        raise ValueError(f"Unknown class {cls_name}")
+
     @classmethod
     def parse_obj(cls, obj):
-        data_type = obj.get('type')
+        data_type = obj.get("type")
         if data_type is None:
-            raise ValueError(f'type is required for {cls.__name__}')
-    
+            raise ValueError(f"type is required for {cls.__name__}")
+
         sub = cls.get_cls(data_type)
         if sub is None:
-            raise ValueError(f'Unknown type {data_type}')
+            raise ValueError(f"Unknown type {data_type}")
         return sub(**obj)
 
     def _iter(self, **kwargs):
-        yield 'type', self.get_type(self.__class__.__name__)
+        yield "type", self.get_type(self.__class__.__name__)
         yield from super()._iter(**kwargs)
 
     @property
     def type(self):
         return self.get_type(self.__class__.__name__)
-
```

### Comparing `vocode-0.1.9/vocode/output_device/speaker_output.py` & `vocode-0.1.90/vocode/streaming/output_device/speaker_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-import pyaudio
+import sounddevice as sd
+import numpy as np
 
 from .base_output_device import BaseOutputDevice
-from ..models.audio_encoding import AudioEncoding
+from vocode.streaming.models.audio_encoding import AudioEncoding
 
-class SpeakerOutput(BaseOutputDevice):
 
+class SpeakerOutput(BaseOutputDevice):
     DEFAULT_SAMPLING_RATE = 44100
 
-    def __init__(self, pa: pyaudio.PyAudio, device_info: dict, sampling_rate: int = None, audio_encoding: AudioEncoding = AudioEncoding.LINEAR16):
+    def __init__(
+        self,
+        device_info: dict,
+        sampling_rate: int = None,
+        audio_encoding: AudioEncoding = AudioEncoding.LINEAR16,
+    ):
         self.device_info = device_info
-        sampling_rate = sampling_rate or int(self.device_info.get('defaultSampleRate', self.DEFAULT_SAMPLING_RATE))
+        sampling_rate = sampling_rate or int(
+            self.device_info.get("default_samplerate", self.DEFAULT_SAMPLING_RATE)
+        )
         super().__init__(sampling_rate, audio_encoding)
-        self.pa = pa
-        self.stream = self.pa.open(
-            output=True,
+        self.stream = sd.OutputStream(
             channels=1,
-            rate=self.sampling_rate,
-            format=pyaudio.paInt16,
-            output_device_index=int(self.device_info['index'])
+            samplerate=self.sampling_rate,
+            dtype=np.int16,
+            device=int(self.device_info["index"]),
         )
+        self.stream.start()
 
     async def send_async(self, chunk):
-        self.stream.write(chunk)
+        self.stream.write(np.frombuffer(chunk, dtype=np.int16))
 
     def terminate(self):
         self.stream.close()
-        self.pa.close()
```

