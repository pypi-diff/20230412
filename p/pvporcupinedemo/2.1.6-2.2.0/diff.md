# Comparing `tmp/pvporcupinedemo-2.1.6.tar.gz` & `tmp/pvporcupinedemo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvporcupinedemo-2.1.6.tar", last modified: Mon Jul 25 18:25:46 2022, max compression
+gzip compressed data, was "pvporcupinedemo-2.2.0.tar", last modified: Wed Apr 12 17:54:05 2023, max compression
```

## Comparing `pvporcupinedemo-2.1.6.tar` & `pvporcupinedemo-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:25:46.874700 pvporcupinedemo-2.1.6/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      125 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/MANIFEST.in
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6537 2022-07-25 18:25:46.874700 pvporcupinedemo-2.1.6/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5822 2022-07-06 18:53:49.000000 pvporcupinedemo-2.1.6/README.md
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:25:46.874700 pvporcupinedemo-2.1.6/pvporcupinedemo/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)    11344 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo/LICENSE
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5252 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo/porcupine_demo_file.py
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     8797 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo/porcupine_demo_mic.py
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:25:46.874700 pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     6537 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      367 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/SOURCES.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/dependency_links.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      143 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/entry_points.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       37 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/requires.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       16 2022-07-25 18:25:46.000000 pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/top_level.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2022-07-25 18:25:46.874700 pvporcupinedemo-2.1.6/setup.cfg
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     2053 2022-07-25 18:24:31.000000 pvporcupinedemo-2.1.6/setup.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      125 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/MANIFEST.in
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6460 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5782 2023-04-06 17:23:16.000000 pvporcupinedemo-2.2.0/README.md
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/pvporcupinedemo/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/pvporcupinedemo/LICENSE
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5453 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_file.py
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5572 2023-04-12 17:54:03.000000 pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_mic.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6460 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      367 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      142 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/entry_points.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       37 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/requires.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       16 2023-04-12 17:54:04.000000 pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/top_level.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 17:54:05.004299 pvporcupinedemo-2.2.0/setup.cfg
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2053 2023-04-06 17:23:16.000000 pvporcupinedemo-2.2.0/setup.py
```

### Comparing `pvporcupinedemo-2.1.6/PKG-INFO` & `pvporcupinedemo-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvporcupinedemo
-Version: 2.1.6
+Version: 2.2.0
 Summary: Porcupine wake word engine demos
 Home-page: https://github.com/Picovoice/porcupine
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word engine,hotword detection,keyword spotting,wake word detection,voice commands
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -124,56 +122,54 @@
 
 It allows testing Porcupine on a corpus of audio files. The demo is mainly useful for quantitative performance
 benchmarking. It accepts 16kHz audio files. Porcupine processes a single-channel audio stream if a stereo file is
 provided it only processes the first (left) channel. The following processes a file looking for instances of the phrase
 "Picovoice"
 
 ```console
-porcupine_demo_file --access_key ${ACCESS_KEY} --input_audio_path ${AUDIO_PATH} --keywords picovoice
+porcupine_demo_file --access_key ${ACCESS_KEY} --wav_path ${AUDIO_PATH} --keywords picovoice
 ```
 
 `keywords` is a shorthand for using default keyword files shipped with the package. The list of default keyword files
 can be seen in the usage string
 
 ```console
 porcupine_demo_file --help
 ```
 
 To detect multiple phrases concurrently provide them as separate arguments
 
 ```console
-porcupine_demo_file --access_key ${ACCESS_KEY} --input_audio_path ${AUDIO_PATH} --keywords grasshopper porcupine
+porcupine_demo_file --access_key ${ACCESS_KEY} --wav_path ${AUDIO_PATH} --keywords grasshopper porcupine
 ```
 
 To detect non-default keywords (e.g. models created using [Picovoice Console](https://console.picovoice.ai/))
 use `keyword_paths` argument
 
 ```console
 porcupine_demo_file --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --keyword_paths ${KEYWORD_PATH_ONE} ${KEYWORD_PATH_TWO}
 ```
 
 To detect non-English keywords provide the respective model path:
 
 ```console
 porcupine_demo_mic --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --model_path ${NON_ENGLISH_MODEL_PATH} \
 --keyword_paths ${NON_ENGLISH_KEYWORD_PATH} 
 ```
 
 The model files for all supported languages are available 
 [here](https://github.com/Picovoice/porcupine/tree/master/lib/common) on Porcupine's GitHub repository.
 
 The sensitivity of the engine can be tuned per keyword using the `sensitivities` input argument
 
 ```console
 porcupine_demo_file --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --keywords grasshopper porcupine --sensitivities 0.3 0.6
 ```
 
 Sensitivity is the parameter that enables trading miss rate for the false alarm rate. It is a floating point number within
 `[0, 1]`. A higher sensitivity reduces the miss rate at the cost of increased false alarm rate.
-
-
```

### Comparing `pvporcupinedemo-2.1.6/README.md` & `pvporcupinedemo-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,54 +105,54 @@
 
 It allows testing Porcupine on a corpus of audio files. The demo is mainly useful for quantitative performance
 benchmarking. It accepts 16kHz audio files. Porcupine processes a single-channel audio stream if a stereo file is
 provided it only processes the first (left) channel. The following processes a file looking for instances of the phrase
 "Picovoice"
 
 ```console
-porcupine_demo_file --access_key ${ACCESS_KEY} --input_audio_path ${AUDIO_PATH} --keywords picovoice
+porcupine_demo_file --access_key ${ACCESS_KEY} --wav_path ${AUDIO_PATH} --keywords picovoice
 ```
 
 `keywords` is a shorthand for using default keyword files shipped with the package. The list of default keyword files
 can be seen in the usage string
 
 ```console
 porcupine_demo_file --help
 ```
 
 To detect multiple phrases concurrently provide them as separate arguments
 
 ```console
-porcupine_demo_file --access_key ${ACCESS_KEY} --input_audio_path ${AUDIO_PATH} --keywords grasshopper porcupine
+porcupine_demo_file --access_key ${ACCESS_KEY} --wav_path ${AUDIO_PATH} --keywords grasshopper porcupine
 ```
 
 To detect non-default keywords (e.g. models created using [Picovoice Console](https://console.picovoice.ai/))
 use `keyword_paths` argument
 
 ```console
 porcupine_demo_file --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --keyword_paths ${KEYWORD_PATH_ONE} ${KEYWORD_PATH_TWO}
 ```
 
 To detect non-English keywords provide the respective model path:
 
 ```console
 porcupine_demo_mic --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --model_path ${NON_ENGLISH_MODEL_PATH} \
 --keyword_paths ${NON_ENGLISH_KEYWORD_PATH} 
 ```
 
 The model files for all supported languages are available 
 [here](https://github.com/Picovoice/porcupine/tree/master/lib/common) on Porcupine's GitHub repository.
 
 The sensitivity of the engine can be tuned per keyword using the `sensitivities` input argument
 
 ```console
 porcupine_demo_file --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --keywords grasshopper porcupine --sensitivities 0.3 0.6
 ```
 
 Sensitivity is the parameter that enables trading miss rate for the false alarm rate. It is a floating point number within
 `[0, 1]`. A higher sensitivity reduces the miss rate at the cost of increased false alarm rate.
```

### Comparing `pvporcupinedemo-2.1.6/pvporcupinedemo/LICENSE` & `pvporcupinedemo-2.2.0/pvporcupinedemo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvporcupinedemo-2.1.6/pvporcupinedemo/porcupine_demo_file.py` & `pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2018-2021 Picovoice Inc.
+# Copyright 2018-2023 Picovoice Inc.
 #
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
@@ -16,63 +16,69 @@
 
 import pvporcupine
 
 
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
 
-    parser.add_argument('--access_key',
-                        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
-                        required=True)
+    parser.add_argument(
+        '--access_key',
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
+        required=True)
 
-    parser.add_argument('--input_audio_path', help='Absolute path to input audio file.', required=True)
+    parser.add_argument('--wav_path', help='Absolute path to input .wav file', required=True)
 
     parser.add_argument(
         '--keywords',
         nargs='+',
-        help='List of default keywords for detection. Available keywords: %s' % ', '.join(sorted(pvporcupine.KEYWORDS)),
+        help='List of default keywords for detection. '
+             'Available keywords: %s' % ', '.join('%s' % w for w in sorted(pvporcupine.KEYWORDS)),
         choices=sorted(list(pvporcupine.KEYWORDS)),
         metavar='')
 
     parser.add_argument(
         '--keyword_paths',
         nargs='+',
         help="Absolute paths to keyword model files. If not set it will be populated from `--keywords` argument")
 
-    parser.add_argument('--library_path', help='Absolute path to dynamic library.', default=pvporcupine.LIBRARY_PATH)
+    parser.add_argument(
+        '--library_path',
+        help='Absolute path to dynamic library. Default: using the library provided by `pvporcupine`')
 
     parser.add_argument(
         '--model_path',
-        help='Absolute path to the file containing model parameters.',
-        default=pvporcupine.MODEL_PATH)
+        help='Absolute path to the file containing model parameters. '
+             'Default: using the library provided by `pvporcupine`')
 
     parser.add_argument(
         '--sensitivities',
         nargs='+',
-        help="Sensitivities for detecting keywords. Each value should be a number within [0, 1]. A higher " +
-             "sensitivity results in fewer misses at the cost of increasing the false alarm rate. If not set 0.5 " +
+        help="Sensitivities for detecting keywords. Each value should be a number within [0, 1]. A higher "
+             "sensitivity results in fewer misses at the cost of increasing the false alarm rate. If not set 0.5 "
              "will be used.",
         type=float,
         default=None)
 
     args = parser.parse_args()
 
     if args.keyword_paths is None:
@@ -112,15 +118,15 @@
     except pvporcupine.PorcupineActivationThrottledError as e:
         print("AccessKey '%s' has been throttled" % args.access_key)
         raise e
     except pvporcupine.PorcupineError as e:
         print("Failed to initialize Porcupine")
         raise e
 
-    audio = read_file(args.input_audio_path, porcupine.sample_rate)
+    audio = read_file(args.wav_path, porcupine.sample_rate)
 
     keywords = list()
     for x in keyword_paths:
         keyword_phrase_part = os.path.basename(x).replace('.ppn', '').split('_')
         if len(keyword_phrase_part) > 6:
             keywords.append(' '.join(keyword_phrase_part[0:-6]))
         else:
```

### Comparing `pvporcupinedemo-2.1.6/pvporcupinedemo/porcupine_demo_mic.py` & `pvporcupinedemo-2.2.0/pvporcupinedemo/porcupine_demo_mic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,231 +1,159 @@
 #
-# Copyright 2018-2021 Picovoice Inc.
+# Copyright 2018-2023 Picovoice Inc.
 #
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 #
 
 import argparse
 import os
 import struct
 import wave
 from datetime import datetime
-from threading import Thread
 
 import pvporcupine
 from pvrecorder import PvRecorder
 
 
-class PorcupineDemo(Thread):
-    """
-    Microphone Demo for Porcupine wake word engine. It creates an input audio stream from a microphone, monitors it, and
-    upon detecting the specified wake word(s) prints the detection time and wake word on console. It optionally saves
-    the recorded audio into a file for further debugging.
-    """
-
-    def __init__(
-            self,
-            access_key,
-            library_path,
-            model_path,
-            keyword_paths,
-            sensitivities,
-            input_device_index=None,
-            output_path=None):
-
-        """
-        Constructor.
-
-        :param library_path: Absolute path to Porcupine's dynamic library.
-        :param model_path: Absolute path to the file containing model parameters.
-        :param keyword_paths: Absolute paths to keyword model files.
-        :param sensitivities: Sensitivities for detecting keywords. Each value should be a number within [0, 1]. A
-        higher sensitivity results in fewer misses at the cost of increasing the false alarm rate. If not set 0.5 will
-        be used.
-        :param input_device_index: Optional argument. If provided, audio is recorded from this input device. Otherwise,
-        the default audio input device is used.
-        :param output_path: If provided recorded audio will be stored in this location at the end of the run.
-        """
-
-        super(PorcupineDemo, self).__init__()
-
-        self._access_key = access_key
-        self._library_path = library_path
-        self._model_path = model_path
-        self._keyword_paths = keyword_paths
-        self._sensitivities = sensitivities
-        self._input_device_index = input_device_index
-
-        self._output_path = output_path
-
-    def run(self):
-        """
-         Creates an input audio stream, instantiates an instance of Porcupine object, and monitors the audio stream for
-         occurrences of the wake word(s). It prints the time of detection for each occurrence and the wake word.
-         """
-
-        keywords = list()
-        for x in self._keyword_paths:
-            keyword_phrase_part = os.path.basename(x).replace('.ppn', '').split('_')
-            if len(keyword_phrase_part) > 6:
-                keywords.append(' '.join(keyword_phrase_part[0:-6]))
-            else:
-                keywords.append(keyword_phrase_part[0])
-
-        porcupine = None
-        recorder = None
-        wav_file = None
-        try:
-            porcupine = pvporcupine.create(
-                access_key=self._access_key,
-                library_path=self._library_path,
-                model_path=self._model_path,
-                keyword_paths=self._keyword_paths,
-                sensitivities=self._sensitivities)
-
-            recorder = PvRecorder(device_index=self._input_device_index, frame_length=porcupine.frame_length)
-            recorder.start()
-
-            if self._output_path is not None:
-                wav_file = wave.open(self._output_path, "w")
-                wav_file.setparams((1, 2, 16000, 512, "NONE", "NONE"))
-
-            print('Using device: %s', recorder.selected_device)
-
-            print('Listening {')
-            for keyword, sensitivity in zip(keywords, self._sensitivities):
-                print('  %s (%.2f)' % (keyword, sensitivity))
-            print('}')
-
-            while True:
-                pcm = recorder.read()
-
-                if wav_file is not None:
-                    wav_file.writeframes(struct.pack("h" * len(pcm), *pcm))
-
-                result = porcupine.process(pcm)
-                if result >= 0:
-                    print('[%s] Detected %s' % (str(datetime.now()), keywords[result]))
-        except pvporcupine.PorcupineInvalidArgumentError as e:
-            args = (
-                self._access_key,
-                self._library_path,
-                self._model_path,
-                self._keyword_paths,
-                self._sensitivities,
-            )
-            print("One or more arguments provided to Porcupine is invalid: ", args)
-            print("If all other arguments seem valid, ensure that '%s' is a valid AccessKey" % self._access_key)
-            raise e
-        except pvporcupine.PorcupineActivationError as e:
-            print("AccessKey activation error")
-            raise e
-        except pvporcupine.PorcupineActivationLimitError as e:
-            print("AccessKey '%s' has reached it's temporary device limit" % self._access_key)
-            raise e
-        except pvporcupine.PorcupineActivationRefusedError as e:
-            print("AccessKey '%s' refused" % self._access_key)
-            raise e
-        except pvporcupine.PorcupineActivationThrottledError as e:
-            print("AccessKey '%s' has been throttled" % self._access_key)
-            raise e
-        except pvporcupine.PorcupineError as e:
-            print("Failed to initialize Porcupine")
-            raise e
-        except KeyboardInterrupt:
-            print('Stopping ...')
-        finally:
-            if porcupine is not None:
-                porcupine.delete()
-
-            if recorder is not None:
-                recorder.delete()
-
-            if wav_file is not None:
-                wav_file.close()
-
-    @classmethod
-    def show_audio_devices(cls):
-        devices = PvRecorder.get_audio_devices()
-
-        for i in range(len(devices)):
-            print('index: %d, device name: %s' % (i, devices[i]))
-
-
 def main():
     parser = argparse.ArgumentParser()
 
-    parser.add_argument('--access_key',
-                        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)')
+    parser.add_argument(
+        '--access_key',
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
+        required=True)
 
     parser.add_argument(
         '--keywords',
         nargs='+',
-        help='List of default keywords for detection. Available keywords: %s' % ', '.join(sorted(pvporcupine.KEYWORDS)),
+        help='List of default keywords for detection. Available keywords: %s' % ', '.join(
+            '%s' % w for w in sorted(pvporcupine.KEYWORDS)),
         choices=sorted(pvporcupine.KEYWORDS),
         metavar='')
 
     parser.add_argument(
         '--keyword_paths',
         nargs='+',
         help="Absolute paths to keyword model files. If not set it will be populated from `--keywords` argument")
 
-    parser.add_argument('--library_path', help='Absolute path to dynamic library.', default=pvporcupine.LIBRARY_PATH)
+    parser.add_argument(
+        '--library_path',
+        help='Absolute path to dynamic library. Default: using the library provided by `pvporcupine`')
 
     parser.add_argument(
         '--model_path',
-        help='Absolute path to the file containing model parameters.',
-        default=pvporcupine.MODEL_PATH)
+        help='Absolute path to the file containing model parameters. '
+             'Default: using the library provided by `pvporcupine`')
 
     parser.add_argument(
         '--sensitivities',
         nargs='+',
-        help="Sensitivities for detecting keywords. Each value should be a number within [0, 1]. A higher " +
-             "sensitivity results in fewer misses at the cost of increasing the false alarm rate. If not set 0.5 " +
+        help="Sensitivities for detecting keywords. Each value should be a number within [0, 1]. A higher "
+             "sensitivity results in fewer misses at the cost of increasing the false alarm rate. If not set 0.5 "
              "will be used.",
         type=float,
         default=None)
 
     parser.add_argument('--audio_device_index', help='Index of input audio device.', type=int, default=-1)
 
     parser.add_argument('--output_path', help='Absolute path to recorded audio for debugging.', default=None)
 
     parser.add_argument('--show_audio_devices', action='store_true')
 
     args = parser.parse_args()
 
     if args.show_audio_devices:
-        PorcupineDemo.show_audio_devices()
-    else:
-        if args.access_key is None:
-            raise ValueError("AccessKey (--access_key) is required")
-        if args.keyword_paths is None:
-            if args.keywords is None:
-                raise ValueError("Either `--keywords` or `--keyword_paths` must be set.")
+        for i, device in enumerate(PvRecorder.get_audio_devices()):
+            print('Device %d: %s' % (i, device))
+        return
+
+    if args.keyword_paths is None:
+        if args.keywords is None:
+            raise ValueError("Either `--keywords` or `--keyword_paths` must be set.")
 
-            keyword_paths = [pvporcupine.KEYWORD_PATHS[x] for x in args.keywords]
-        else:
-            keyword_paths = args.keyword_paths
+        keyword_paths = [pvporcupine.KEYWORD_PATHS[x] for x in args.keywords]
+    else:
+        keyword_paths = args.keyword_paths
 
-        if args.sensitivities is None:
-            args.sensitivities = [0.5] * len(keyword_paths)
+    if args.sensitivities is None:
+        args.sensitivities = [0.5] * len(keyword_paths)
 
-        if len(keyword_paths) != len(args.sensitivities):
-            raise ValueError('Number of keywords does not match the number of sensitivities.')
+    if len(keyword_paths) != len(args.sensitivities):
+        raise ValueError('Number of keywords does not match the number of sensitivities.')
 
-        PorcupineDemo(
+    try:
+        porcupine = pvporcupine.create(
             access_key=args.access_key,
             library_path=args.library_path,
             model_path=args.model_path,
             keyword_paths=keyword_paths,
-            sensitivities=args.sensitivities,
-            output_path=args.output_path,
-            input_device_index=args.audio_device_index).run()
+            sensitivities=args.sensitivities)
+    except pvporcupine.PorcupineInvalidArgumentError as e:
+        print("One or more arguments provided to Porcupine is invalid: ", args)
+        print("If all other arguments seem valid, ensure that '%s' is a valid AccessKey" % args.access_key)
+        raise e
+    except pvporcupine.PorcupineActivationError as e:
+        print("AccessKey activation error")
+        raise e
+    except pvporcupine.PorcupineActivationLimitError as e:
+        print("AccessKey '%s' has reached it's temporary device limit" % args.access_key)
+        raise e
+    except pvporcupine.PorcupineActivationRefusedError as e:
+        print("AccessKey '%s' refused" % args.access_key)
+        raise e
+    except pvporcupine.PorcupineActivationThrottledError as e:
+        print("AccessKey '%s' has been throttled" % args.access_key)
+        raise e
+    except pvporcupine.PorcupineError as e:
+        print("Failed to initialize Porcupine")
+        raise e
+
+    keywords = list()
+    for x in keyword_paths:
+        keyword_phrase_part = os.path.basename(x).replace('.ppn', '').split('_')
+        if len(keyword_phrase_part) > 6:
+            keywords.append(' '.join(keyword_phrase_part[0:-6]))
+        else:
+            keywords.append(keyword_phrase_part[0])
+
+    print('Porcupine version: %s' % porcupine.version)
+
+    recorder = PvRecorder(
+        device_index=args.audio_device_index,
+        frame_length=porcupine.frame_length)
+    recorder.start()
+
+    wav_file = None
+    if args.output_path is not None:
+        wav_file = wave.open(args.output_path, "w")
+        wav_file.setnchannels(1)
+        wav_file.setsampwidth(2)
+        wav_file.setframerate(16000)
+
+    print('Listening ... (press Ctrl+C to exit)')
+
+    try:
+        while True:
+            pcm = recorder.read()
+            result = porcupine.process(pcm)
+
+            if wav_file is not None:
+                wav_file.writeframes(struct.pack("h" * len(pcm), *pcm))
+
+            if result >= 0:
+                print('[%s] Detected %s' % (str(datetime.now()), keywords[result]))
+    except KeyboardInterrupt:
+        print('Stopping ...')
+    finally:
+        recorder.delete()
+        porcupine.delete()
+        if wav_file is not None:
+            wav_file.close()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pvporcupinedemo-2.1.6/pvporcupinedemo.egg-info/PKG-INFO` & `pvporcupinedemo-2.2.0/pvporcupinedemo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvporcupinedemo
-Version: 2.1.6
+Version: 2.2.0
 Summary: Porcupine wake word engine demos
 Home-page: https://github.com/Picovoice/porcupine
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: wake word engine,hotword detection,keyword spotting,wake word detection,voice commands
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -124,56 +122,54 @@
 
 It allows testing Porcupine on a corpus of audio files. The demo is mainly useful for quantitative performance
 benchmarking. It accepts 16kHz audio files. Porcupine processes a single-channel audio stream if a stereo file is
 provided it only processes the first (left) channel. The following processes a file looking for instances of the phrase
 "Picovoice"
 
 ```console
-porcupine_demo_file --access_key ${ACCESS_KEY} --input_audio_path ${AUDIO_PATH} --keywords picovoice
+porcupine_demo_file --access_key ${ACCESS_KEY} --wav_path ${AUDIO_PATH} --keywords picovoice
 ```
 
 `keywords` is a shorthand for using default keyword files shipped with the package. The list of default keyword files
 can be seen in the usage string
 
 ```console
 porcupine_demo_file --help
 ```
 
 To detect multiple phrases concurrently provide them as separate arguments
 
 ```console
-porcupine_demo_file --access_key ${ACCESS_KEY} --input_audio_path ${AUDIO_PATH} --keywords grasshopper porcupine
+porcupine_demo_file --access_key ${ACCESS_KEY} --wav_path ${AUDIO_PATH} --keywords grasshopper porcupine
 ```
 
 To detect non-default keywords (e.g. models created using [Picovoice Console](https://console.picovoice.ai/))
 use `keyword_paths` argument
 
 ```console
 porcupine_demo_file --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --keyword_paths ${KEYWORD_PATH_ONE} ${KEYWORD_PATH_TWO}
 ```
 
 To detect non-English keywords provide the respective model path:
 
 ```console
 porcupine_demo_mic --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --model_path ${NON_ENGLISH_MODEL_PATH} \
 --keyword_paths ${NON_ENGLISH_KEYWORD_PATH} 
 ```
 
 The model files for all supported languages are available 
 [here](https://github.com/Picovoice/porcupine/tree/master/lib/common) on Porcupine's GitHub repository.
 
 The sensitivity of the engine can be tuned per keyword using the `sensitivities` input argument
 
 ```console
 porcupine_demo_file --access_key ${ACCESS_KEY} \
---input_audio_path ${AUDIO_PATH} \
+--wav_path ${AUDIO_PATH} \
 --keywords grasshopper porcupine --sensitivities 0.3 0.6
 ```
 
 Sensitivity is the parameter that enables trading miss rate for the false alarm rate. It is a floating point number within
 `[0, 1]`. A higher sensitivity reduces the miss rate at the cost of increased false alarm rate.
-
-
```

### Comparing `pvporcupinedemo-2.1.6/setup.py` & `pvporcupinedemo-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvporcupinedemo/porcupine_demo_mic.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvporcupinedemo",
-    version="2.1.6",
+    version="2.2.0",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Porcupine wake word engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/porcupine",
     packages=["pvporcupinedemo"],
-    install_requires=["pvporcupine==2.1.4", "pvrecorder==1.1.1"],
+    install_requires=["pvporcupine==2.2.0", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

