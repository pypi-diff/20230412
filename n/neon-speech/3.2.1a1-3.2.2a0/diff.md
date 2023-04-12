# Comparing `tmp/neon_speech-3.2.1a1-py3-none-any.whl.zip` & `tmp/neon_speech-3.2.2a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 23401 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Mar-23 16:36 neon_speech/__init__.py
--rw-r--r--  2.0 unx     2632 b- defN 23-Mar-23 16:36 neon_speech/__main__.py
--rw-r--r--  2.0 unx     5085 b- defN 23-Mar-23 16:36 neon_speech/cli.py
--rw-r--r--  2.0 unx     9916 b- defN 23-Mar-23 16:36 neon_speech/listener.py
--rw-r--r--  2.0 unx     4810 b- defN 23-Mar-23 16:36 neon_speech/mic.py
--rw-r--r--  2.0 unx    21458 b- defN 23-Mar-23 16:36 neon_speech/service.py
--rw-r--r--  2.0 unx     4396 b- defN 23-Mar-23 16:36 neon_speech/stt.py
--rw-r--r--  2.0 unx     4294 b- defN 23-Mar-23 16:36 neon_speech/utils.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Mar-23 16:36 neon_speech-3.2.1a1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2551 b- defN 23-Mar-23 16:36 neon_speech-3.2.1a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-23 16:36 neon_speech-3.2.1a1.dist-info/WHEEL
--rw-r--r--  2.0 unx      111 b- defN 23-Mar-23 16:36 neon_speech-3.2.1a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Mar-23 16:36 neon_speech-3.2.1a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1143 b- defN 23-Mar-23 16:36 neon_speech-3.2.1a1.dist-info/RECORD
-14 files, 59965 bytes uncompressed, 21509 bytes compressed:  64.1%
+Zip file size: 23520 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Apr-12 01:13 neon_speech/__init__.py
+-rw-r--r--  2.0 unx     2632 b- defN 23-Apr-12 01:13 neon_speech/__main__.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-Apr-12 01:13 neon_speech/cli.py
+-rw-r--r--  2.0 unx     9996 b- defN 23-Apr-12 01:13 neon_speech/listener.py
+-rw-r--r--  2.0 unx     4810 b- defN 23-Apr-12 01:13 neon_speech/mic.py
+-rw-r--r--  2.0 unx    21797 b- defN 23-Apr-12 01:13 neon_speech/service.py
+-rw-r--r--  2.0 unx     4396 b- defN 23-Apr-12 01:13 neon_speech/stt.py
+-rw-r--r--  2.0 unx     4294 b- defN 23-Apr-12 01:13 neon_speech/utils.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2551 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      111 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1143 b- defN 23-Apr-12 01:13 neon_speech-3.2.2a0.dist-info/RECORD
+14 files, 60384 bytes uncompressed, 21628 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: neon_speech/stt.py
 Comment: 
 
 Filename: neon_speech/utils.py
 Comment: 
 
-Filename: neon_speech-3.2.1a1.dist-info/LICENSE.md
+Filename: neon_speech-3.2.2a0.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_speech-3.2.1a1.dist-info/METADATA
+Filename: neon_speech-3.2.2a0.dist-info/METADATA
 Comment: 
 
-Filename: neon_speech-3.2.1a1.dist-info/WHEEL
+Filename: neon_speech-3.2.2a0.dist-info/WHEEL
 Comment: 
 
-Filename: neon_speech-3.2.1a1.dist-info/entry_points.txt
+Filename: neon_speech-3.2.2a0.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_speech-3.2.1a1.dist-info/top_level.txt
+Filename: neon_speech-3.2.2a0.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_speech-3.2.1a1.dist-info/RECORD
+Filename: neon_speech-3.2.2a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_speech/listener.py

```diff
@@ -82,14 +82,15 @@
             try:
                 transcriptions = self.loop.stt.execute(audio, language=lang)
                 LOG.debug(f'transcriptions={transcriptions}')
                 if not transcriptions or (isinstance(transcriptions, list)
                                           and not any(transcriptions)):
                     raise RuntimeError("Primary STT returned nothing")
             except Exception as e:
+                self.loop.init_fallback_stt()
                 if self.loop.fallback_stt:
                     LOG.warning(f"Using fallback STT, main plugin failed: {e}")
                     transcriptions = \
                         self.loop.fallback_stt.execute(audio, language=lang)
                 else:
                     LOG.debug("No fallback_stt to try")
                     raise e
@@ -164,24 +165,26 @@
                     LOG.exception(e)
         self.create_hotword_engines()
         self.state = RecognizerLoopState()
         self.responsive_recognizer = NeonResponsiveRecognizer(self)
         self.config_loaded.set()
         # TODO: Update recognizer to support passed config
 
-    def start_async(self):
-        """Start consumer and producer threads."""
-        self.state.running = True
-        if not self.stt:
-            self.stt = STTFactory.create(self.config_core)
+    def init_fallback_stt(self):
         if not self.fallback_stt:
             clazz = self.get_fallback_stt()
             if clazz:
                 LOG.debug(f"Initializing fallback STT engine")
                 self.fallback_stt = clazz()
+
+    def start_async(self):
+        """Start consumer and producer threads."""
+        self.state.running = True
+        if not self.stt:
+            self.stt = STTFactory.create(self.config_core)
         self.queue = Queue()
         self.audio_consumer = NeonAudioConsumer(self)
         self.audio_consumer.name = "audio_consumer"
         self.audio_consumer.start()
         self.audio_producer = AudioProducer(self)
         self.audio_producer.name = "audio_producer"
         try:
```

## neon_speech/service.py

```diff
@@ -114,16 +114,20 @@
                                       on_started=started_hook)
         self.status = ProcessStatus('speech', self.bus, callbacks)
         self.status.set_started()
         self.status.bind(self.bus)
         self.loop = NeonRecognizerLoop(self.bus, watchdog)
         self.connect_loop_events()
         self.connect_bus_events()
-        self.api_stt = STTFactory.create(config=self.config,
-                                         results_event=None)
+        if self.config.get('listener', {}).get('enable_stt_api', True):
+            self.api_stt = STTFactory.create(config=self.config,
+                                             results_event=None)
+        else:
+            LOG.info("Skipping api_stt init")
+            self.api_stt = None
 
     def shutdown(self):
         LOG.info("Shutting Down")
         self.status.set_stopping()
         self.loop.stop()
 
     def connect_bus_events(self):
@@ -434,14 +438,17 @@
         """
         from neon_utils.file_utils import get_audio_file_stream
         lang = lang or 'en-us'  # TODO: read default from config
         segment = AudioSegment.from_file(wav_file)
         audio_data = AudioData(segment.raw_data, segment.frame_rate,
                                segment.sample_width)
         audio_stream = get_audio_file_stream(wav_file)
+        if not self.api_stt:
+            raise RuntimeError("api_stt not initialized."
+                               " is `listener['enable_stt_api'] set to False?")
         if hasattr(self.api_stt, 'stream_start'):
             if self.lock.acquire(True, 30):
                 LOG.info(f"Starting STT processing (lang={lang}): {wav_file}")
                 self.api_stt.stream_start(lang)
                 while True:
                     try:
                         data = audio_stream.read(1024)
```

## Comparing `neon_speech-3.2.1a1.dist-info/LICENSE.md` & `neon_speech-3.2.2a0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_speech-3.2.1a1.dist-info/METADATA` & `neon_speech-3.2.2a0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 3.2.1a1
+Version: 3.2.2a0
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `neon_speech-3.2.1a1.dist-info/RECORD` & `neon_speech-3.2.2a0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 neon_speech/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
 neon_speech/__main__.py,sha256=GYsKldh4iN7sY2kLnHtSYj1D56GQgdHuMXlUIf-d5ks,2632
 neon_speech/cli.py,sha256=2BiU-fTcmOyT3CJ6gmoCtUsP7bAUcDOt8-MkPEfMJX0,5085
-neon_speech/listener.py,sha256=p4Nve9zmD-xo7EdEZq9Qy3JBbifCL2geZH8xOB1-t3s,9916
+neon_speech/listener.py,sha256=Cct3GOVTrjEBUBq2pvrcDH7iixBo_6jvJCV02BeCwNE,9996
 neon_speech/mic.py,sha256=gcarKLkWfrzToACsiwRWDX5qeBizyJ0vquuqdg5EMeU,4810
-neon_speech/service.py,sha256=3i50utyWV7M_FmPlQJZhALd3Acqs2nf1C55-u7zVjIg,21458
+neon_speech/service.py,sha256=SXldmfNWkFVUaZnV_EG-3rxgeKQRXPxvjByclEzkjEs,21797
 neon_speech/stt.py,sha256=rCl2v2m1D1-t-92Me1qyA57gfw7i9jSzs7j0bQXTGOc,4396
 neon_speech/utils.py,sha256=5RNtze-kwo-_WvYNk8GoqG8vVdkbPs6hBdpF7Pn7Iqc,4294
-neon_speech-3.2.1a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_speech-3.2.1a1.dist-info/METADATA,sha256=QkiwSqi5otb_thnJH30wkDs_rP-sF7e0fCJLJGgBUyA,2551
-neon_speech-3.2.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_speech-3.2.1a1.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
-neon_speech-3.2.1a1.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
-neon_speech-3.2.1a1.dist-info/RECORD,,
+neon_speech-3.2.2a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_speech-3.2.2a0.dist-info/METADATA,sha256=1LiMMFGLJ9tXofZpZH-5_16S6i44Vd1N71oiX3bEgU4,2551
+neon_speech-3.2.2a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_speech-3.2.2a0.dist-info/entry_points.txt,sha256=Y5nCn6RrdZVozA3UnFkIX_43MJ5TF-bmlqsz3LA_9rM,111
+neon_speech-3.2.2a0.dist-info/top_level.txt,sha256=fXNizEfCNvNDWenv5znkv_2KPpvzwwsRM7S3sG7bllw,12
+neon_speech-3.2.2a0.dist-info/RECORD,,
```

