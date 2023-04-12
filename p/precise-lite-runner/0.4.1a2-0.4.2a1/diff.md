# Comparing `tmp/precise_lite_runner-0.4.1a2-py3-none-any.whl.zip` & `tmp/precise_lite_runner-0.4.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11791 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1572 b- defN 23-Apr-06 22:43 precise_lite_runner/__init__.py
--rw-r--r--  2.0 unx     1358 b- defN 23-Apr-06 22:43 precise_lite_runner/params.py
--rw-r--r--  2.0 unx     8727 b- defN 23-Apr-06 22:43 precise_lite_runner/runner.py
--rw-r--r--  2.0 unx     2741 b- defN 23-Apr-06 22:43 precise_lite_runner/util.py
--rw-r--r--  2.0 unx     1315 b- defN 23-Apr-06 22:43 precise_lite_runner/vectorization.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-06 22:43 precise_lite_runner/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-06 22:43 precise_lite_runner-0.4.1a2.dist-info/LICENSE
--rw-r--r--  2.0 unx      438 b- defN 23-Apr-06 22:43 precise_lite_runner-0.4.1a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 22:43 precise_lite_runner-0.4.1a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-06 22:43 precise_lite_runner-0.4.1a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      979 b- defN 23-Apr-06 22:43 precise_lite_runner-0.4.1a2.dist-info/RECORD
-11 files, 28768 bytes uncompressed, 10111 bytes compressed:  64.9%
+Zip file size: 11863 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1572 b- defN 23-Apr-12 07:19 precise_lite_runner/__init__.py
+-rw-r--r--  2.0 unx     1358 b- defN 23-Apr-12 07:19 precise_lite_runner/params.py
+-rw-r--r--  2.0 unx     8989 b- defN 23-Apr-12 07:19 precise_lite_runner/runner.py
+-rw-r--r--  2.0 unx     2741 b- defN 23-Apr-12 07:19 precise_lite_runner/util.py
+-rw-r--r--  2.0 unx     1315 b- defN 23-Apr-12 07:19 precise_lite_runner/vectorization.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-12 07:19 precise_lite_runner/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-12 07:19 precise_lite_runner-0.4.2a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      415 b- defN 23-Apr-12 07:19 precise_lite_runner-0.4.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 07:19 precise_lite_runner-0.4.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-12 07:19 precise_lite_runner-0.4.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Apr-12 07:19 precise_lite_runner-0.4.2a1.dist-info/RECORD
+11 files, 29007 bytes uncompressed, 10183 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: precise_lite_runner/vectorization.py
 Comment: 
 
 Filename: precise_lite_runner/version.py
 Comment: 
 
-Filename: precise_lite_runner-0.4.1a2.dist-info/LICENSE
+Filename: precise_lite_runner-0.4.2a1.dist-info/LICENSE
 Comment: 
 
-Filename: precise_lite_runner-0.4.1a2.dist-info/METADATA
+Filename: precise_lite_runner-0.4.2a1.dist-info/METADATA
 Comment: 
 
-Filename: precise_lite_runner-0.4.1a2.dist-info/WHEEL
+Filename: precise_lite_runner-0.4.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: precise_lite_runner-0.4.1a2.dist-info/top_level.txt
+Filename: precise_lite_runner-0.4.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: precise_lite_runner-0.4.1a2.dist-info/RECORD
+Filename: precise_lite_runner-0.4.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## precise_lite_runner/runner.py

```diff
@@ -1,14 +1,17 @@
 import atexit
 import time
 from threading import Thread, Event
 
 import numpy as np
-import pyaudio
-from pyaudio import PyAudio, paInt16
+try:
+    import pyaudio
+    from pyaudio import PyAudio, paInt16
+except ImportError:
+    pyaudio = None
 
 try:
     import tensorflow.lite as tflite
 except:
     import tflite_runtime.interpreter as tflite
 
 from precise_lite_runner.params import params
@@ -202,25 +205,28 @@
         atexit.register(self.stop)
 
     def _wrap_stream_read(self, stream):
         """
         pyaudio.Stream.read takes samples as n, not bytes
         so read(n) should be read(n // sample_depth)
         """
-
-        if getattr(stream.read, '__func__', None) is pyaudio.Stream.read:
-            stream.read = lambda x: pyaudio.Stream.read(stream, x // 2, False)
+        if pyaudio is not None:
+            if getattr(stream.read, '__func__', None) is pyaudio.Stream.read:
+                stream.read = lambda x: pyaudio.Stream.read(stream, x // 2, False)
 
     def start(self):
         """Start listening from stream"""
         if self.stream is None:
-            self.pa = PyAudio()
-            self.stream = self.pa.open(
-                16000, 1, paInt16, True, frames_per_buffer=self.chunk_size
-            )
+            if pyaudio is not None:
+                self.pa = PyAudio()
+                self.stream = self.pa.open(
+                    16000, 1, paInt16, True, frames_per_buffer=self.chunk_size
+                )
+            else:
+                raise ValueError("self.stream is None, pass a stream or install pyaudio to use mic")
 
         self._wrap_stream_read(self.stream)
 
         self.running = True
         self.thread = Thread(target=self._handle_predictions, daemon=True)
         self.thread.daemon = True
         self.thread.start()
```

## precise_lite_runner/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 4
-VERSION_BUILD = 1
-VERSION_ALPHA = 2
+VERSION_BUILD = 2
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `precise_lite_runner-0.4.1a2.dist-info/LICENSE` & `precise_lite_runner-0.4.2a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `precise_lite_runner-0.4.1a2.dist-info/RECORD` & `precise_lite_runner-0.4.2a1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 precise_lite_runner/__init__.py,sha256=1oFNsmnAH_Hary-SVr-TaXJ0dDmJi4XBQ2H93jH70Ok,1572
 precise_lite_runner/params.py,sha256=_CpLEAKX6ez56Kg1if6wK4ZfmWJTJqoFEDLJcNNv8YA,1358
-precise_lite_runner/runner.py,sha256=H8oyiIrlRaUNSN4Ay8flq3A3ZSMdzPrZIY9atRBzsd8,8727
+precise_lite_runner/runner.py,sha256=BrCKSlzW5A0Xr5aN_xO6JwoEXqDj_3K_VCDqH3kYP68,8989
 precise_lite_runner/util.py,sha256=6Kx1vWpAcGUNtQkOmBfrQ5ydGqZpKh1ZvwNj0GzwzK8,2741
 precise_lite_runner/vectorization.py,sha256=XGlNtWcUWYrqAPCUPVhRV_X4A832NQ8RxupmJeCx-yQ,1315
-precise_lite_runner/version.py,sha256=lmWycRh0if4UuIwI5QrCvityIr3sZ_pPq2rqSw4vEGo,177
-precise_lite_runner-0.4.1a2.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-precise_lite_runner-0.4.1a2.dist-info/METADATA,sha256=D2qQi0JKmapJYX3GY5og39IQw-xN2pZYVMKca3nL8v0,438
-precise_lite_runner-0.4.1a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-precise_lite_runner-0.4.1a2.dist-info/top_level.txt,sha256=HDhE401n7_kJUwCVNPCzoLYFPwo7ltaXKO2k1lfTUiM,20
-precise_lite_runner-0.4.1a2.dist-info/RECORD,,
+precise_lite_runner/version.py,sha256=crgIAIq5_SiYRkn1hX0zd6fYXS3Rk0XSdXJS1Puk5Xc,177
+precise_lite_runner-0.4.2a1.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+precise_lite_runner-0.4.2a1.dist-info/METADATA,sha256=7a556R3kSgVOVzT3T6fxOPem4b_PgOAm7bXkwbZtINE,415
+precise_lite_runner-0.4.2a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+precise_lite_runner-0.4.2a1.dist-info/top_level.txt,sha256=HDhE401n7_kJUwCVNPCzoLYFPwo7ltaXKO2k1lfTUiM,20
+precise_lite_runner-0.4.2a1.dist-info/RECORD,,
```

