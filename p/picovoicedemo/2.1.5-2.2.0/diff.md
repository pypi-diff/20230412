# Comparing `tmp/picovoicedemo-2.1.5.tar.gz` & `tmp/picovoicedemo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picovoicedemo-2.1.5.tar", last modified: Mon Jul 25 18:16:22 2022, max compression
+gzip compressed data, was "picovoicedemo-2.2.0.tar", last modified: Wed Apr 12 18:12:50 2023, max compression
```

## Comparing `picovoicedemo-2.1.5.tar` & `picovoicedemo-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:16:22.315075 picovoicedemo-2.1.5/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      119 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/MANIFEST.in
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4951 2022-07-25 18:16:22.315075 picovoicedemo-2.1.5/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4244 2022-07-25 17:24:32.000000 picovoicedemo-2.1.5/README.md
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:16:22.315075 picovoicedemo-2.1.5/picovoicedemo/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11344 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo/LICENSE
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6353 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo/picovoice_demo_file.py
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     9316 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo/picovoice_demo_mic.py
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:16:22.315075 picovoicedemo-2.1.5/picovoicedemo.egg-info/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4951 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo.egg-info/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      349 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo.egg-info/SOURCES.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo.egg-info/dependency_links.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      139 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo.egg-info/entry_points.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       35 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo.egg-info/requires.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       14 2022-07-25 18:16:22.000000 picovoicedemo-2.1.5/picovoicedemo.egg-info/top_level.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2022-07-25 18:16:22.315075 picovoicedemo-2.1.5/setup.cfg
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2537 2022-07-25 18:15:36.000000 picovoicedemo-2.1.5/setup.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      119 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/MANIFEST.in
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4236 2023-04-10 19:55:03.000000 picovoicedemo-2.2.0/README.md
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:12:50.022604 picovoicedemo-2.2.0/picovoicedemo/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/picovoicedemo/LICENSE
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6576 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/picovoicedemo/picovoice_demo_file.py
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6876 2023-04-12 18:12:48.000000 picovoicedemo-2.2.0/picovoicedemo/picovoice_demo_mic.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/picovoicedemo.egg-info/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4906 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      349 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      138 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/entry_points.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       35 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/requires.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       14 2023-04-12 18:12:49.000000 picovoicedemo-2.2.0/picovoicedemo.egg-info/top_level.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 18:12:50.026604 picovoicedemo-2.2.0/setup.cfg
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2537 2023-04-12 18:08:55.000000 picovoicedemo-2.2.0/setup.py
```

### Comparing `picovoicedemo-2.1.5/PKG-INFO` & `picovoicedemo-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.1.5
+Version: 2.2.0
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -62,15 +60,15 @@
 provided it only processes the first (left) channel. The following processes a file looking for instances of the wake 
 phrase defined in the file located at `${PATH_TO_PORCUPINE_KEYWORD_FILE}` and then infers the follow-on spoken command
 using the context defined by the file located at `${PATH_TO_RHINO_CONTEXT_FILE)}`:
 
 ```console
 picovoice_demo_file \
 --access_key ${ACCESS_KEY} \
---input_audio_path ${PATH_TO_INPUT_AUDIO_FILE} \
+--wav_path ${PATH_TO_INPUT_AUDIO_FILE} \
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)}
 ```
 
 ### Mic Demo
 
 It opens an audio stream from a microphone and detects utterances of a give wake word(s). The following processes
@@ -119,9 +117,7 @@
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)} \
 --audio_device_index 0 \
 --output_path ~/test.wav
 ```
 
 If after listening to stored file there is no apparent problem detected please open an issue.
-
-
```

### Comparing `picovoicedemo-2.1.5/README.md` & `picovoicedemo-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 provided it only processes the first (left) channel. The following processes a file looking for instances of the wake 
 phrase defined in the file located at `${PATH_TO_PORCUPINE_KEYWORD_FILE}` and then infers the follow-on spoken command
 using the context defined by the file located at `${PATH_TO_RHINO_CONTEXT_FILE)}`:
 
 ```console
 picovoice_demo_file \
 --access_key ${ACCESS_KEY} \
---input_audio_path ${PATH_TO_INPUT_AUDIO_FILE} \
+--wav_path ${PATH_TO_INPUT_AUDIO_FILE} \
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)}
 ```
 
 ### Mic Demo
 
 It opens an audio stream from a microphone and detects utterances of a give wake word(s). The following processes
```

### Comparing `picovoicedemo-2.1.5/picovoicedemo/LICENSE` & `picovoicedemo-2.2.0/picovoicedemo/LICENSE`

 * *Files identical despite different names*

### Comparing `picovoicedemo-2.1.5/picovoicedemo/picovoice_demo_file.py` & `picovoicedemo-2.2.0/picovoicedemo/picovoice_demo_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,62 +15,81 @@
 
 from picovoice import *
 
 
 def read_file(file_name, sample_rate):
     wav_file = wave.open(file_name, mode="rb")
     channels = wav_file.getnchannels()
+    sample_width = wav_file.getsampwidth()
     num_frames = wav_file.getnframes()
 
     if wav_file.getframerate() != sample_rate:
         raise ValueError("Audio file should have a sample rate of %d. got %d" % (sample_rate, wav_file.getframerate()))
+    if sample_width != 2:
+        raise ValueError("Audio file should be 16-bit. got %d" % sample_width)
+    if channels == 2:
+        print("Picovoice processes single-channel audio but stereo file is provided. Processing left channel only.")
 
     samples = wav_file.readframes(num_frames)
     wav_file.close()
 
     frames = struct.unpack('h' * num_frames * channels, samples)
 
-    if channels == 2:
-        print("Picovoice processes single-channel audio but stereo file is provided. Processing left channel only.")
-
     return frames[::channels]
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         '--access_key',
         help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
         required=True)
 
-    parser.add_argument('--input_audio_path', help='Absolute path to input audio file.', required=True)
+    parser.add_argument(
+        '--wav_path',
+        help='Absolute path to input audio file.',
+        required=True)
 
-    parser.add_argument('--keyword_path', help="Absolute path to a Porcupine keyword file.", required=True)
+    parser.add_argument(
+        '--keyword_path',
+        help="Absolute path to a Porcupine keyword file.",
+        required=True)
 
-    parser.add_argument('--context_path', help="Absolute path to a Rhino context file.", required=True)
+    parser.add_argument(
+        '--context_path',
+        help="Absolute path to a Rhino context file.",
+        required=True)
 
-    parser.add_argument('--porcupine_library_path', help="Absolute path to Porcupine's dynamic library.", default=None)
+    parser.add_argument(
+        '--porcupine_library_path',
+        help="Absolute path to Porcupine's dynamic library.")
 
-    parser.add_argument('--porcupine_model_path', help="Absolute path to Porcupine's model file.", default=None)
+    parser.add_argument(
+        '--porcupine_model_path',
+        help="Absolute path to Porcupine's model file.")
 
     parser.add_argument(
         '--porcupine_sensitivity',
-        help="Sensitivity for detecting wake word. Each value should be a number within [0, 1]. A higher sensitivity " +
+        help="Sensitivity for detecting wake word. Each value should be a number within [0, 1]. A higher sensitivity "
              "results in fewer misses at the cost of increasing the false alarm rate.",
         type=float,
         default=0.5)
 
-    parser.add_argument('--rhino_library_path', help="Absolute path to Rhino's dynamic library.", default=None)
+    parser.add_argument(
+        '--rhino_library_path',
+        help="Absolute path to Rhino's dynamic library.")
 
-    parser.add_argument('--rhino_model_path', help="Absolute path to Rhino's model file.", default=None)
+    parser.add_argument(
+        '--rhino_model_path',
+        help="Absolute path to Rhino's model file.")
 
     parser.add_argument(
         '--rhino_sensitivity',
-        help="Inference sensitivity. It should be a number within [0, 1]. A higher sensitivity value results in fewer" +
+        help="Inference sensitivity. It should be a number within [0, 1]. A higher sensitivity value results in fewer "
              "misses at the cost of (potentially) increasing the erroneous inference rate.",
         type=float,
         default=0.5)
 
     parser.add_argument(
         '--endpoint_duration_sec',
         help="Endpoint duration in seconds. An endpoint is a chunk of silence at the end of an utterance that marks "
```

### Comparing `picovoicedemo-2.1.5/picovoicedemo.egg-info/PKG-INFO` & `picovoicedemo-2.2.0/picovoicedemo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: picovoicedemo
-Version: 2.1.5
+Version: 2.2.0
 Summary: Picovoice demos.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -62,15 +60,15 @@
 provided it only processes the first (left) channel. The following processes a file looking for instances of the wake 
 phrase defined in the file located at `${PATH_TO_PORCUPINE_KEYWORD_FILE}` and then infers the follow-on spoken command
 using the context defined by the file located at `${PATH_TO_RHINO_CONTEXT_FILE)}`:
 
 ```console
 picovoice_demo_file \
 --access_key ${ACCESS_KEY} \
---input_audio_path ${PATH_TO_INPUT_AUDIO_FILE} \
+--wav_path ${PATH_TO_INPUT_AUDIO_FILE} \
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)}
 ```
 
 ### Mic Demo
 
 It opens an audio stream from a microphone and detects utterances of a give wake word(s). The following processes
@@ -119,9 +117,7 @@
 --keyword_path ${PATH_TO_PORCUPINE_KEYWORD_FILE} \
 --context_path ${PATH_TO_RHINO_CONTEXT_FILE)} \
 --audio_device_index 0 \
 --output_path ~/test.wav
 ```
 
 If after listening to stored file there is no apparent problem detected please open an issue.
-
-
```

### Comparing `picovoicedemo-2.1.5/setup.py` & `picovoicedemo-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     f.write('include picovoicedemo/picovoice_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="picovoicedemo",
-    version="2.1.5",
+    version="2.2.0",
     author="Picovoice Inc.",
     author_email="hello@picovoice.ai",
     description="Picovoice demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/picovoice",
     packages=["picovoicedemo"],
-    install_requires=["picovoice==2.1.4", "pvrecorder==1.1.1"],
+    install_requires=["picovoice==2.2.0", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

