# Comparing `tmp/pvrhinodemo-2.1.9.tar.gz` & `tmp/pvrhinodemo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvrhinodemo-2.1.9.tar", last modified: Mon Jul 25 18:35:54 2022, max compression
+gzip compressed data, was "pvrhinodemo-2.2.0.tar", last modified: Wed Apr 12 18:00:55 2023, max compression
```

## Comparing `pvrhinodemo-2.1.9.tar` & `pvrhinodemo-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:35:54.803246 pvrhinodemo-2.1.9/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      102 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/MANIFEST.in
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4087 2022-07-25 18:35:54.803246 pvrhinodemo-2.1.9/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     3367 2022-07-25 18:26:52.000000 pvrhinodemo-2.1.9/README.md
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:35:54.803246 pvrhinodemo-2.1.9/pvrhinodemo/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     5517 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo/rhino_demo_file.py
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     9856 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo/rhino_demo_mic.py
-drwxrwxr-x   0 kwangsoo  (1000) kwangsoo  (1000)        0 2022-07-25 18:35:54.803246 pvrhinodemo-2.1.9/pvrhinodemo.egg-info/
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     4087 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo.egg-info/PKG-INFO
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      303 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo.egg-info/SOURCES.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)        1 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo.egg-info/dependency_links.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)      119 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo.egg-info/entry_points.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       33 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo.egg-info/requires.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       12 2022-07-25 18:35:54.000000 pvrhinodemo-2.1.9/pvrhinodemo.egg-info/top_level.txt
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)       38 2022-07-25 18:35:54.803246 pvrhinodemo-2.1.9/setup.cfg
--rw-rw-r--   0 kwangsoo  (1000) kwangsoo  (1000)     1979 2022-07-25 18:34:22.000000 pvrhinodemo-2.1.9/setup.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      102 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/MANIFEST.in
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     3359 2023-04-06 17:38:28.000000 pvrhinodemo-2.2.0/README.md
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/pvrhinodemo/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     5697 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_file.py
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     6001 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_mic.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4042 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      303 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/SOURCES.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 18:00:54.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/dependency_links.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      118 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/entry_points.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       33 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/requires.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       12 2023-04-12 18:00:55.000000 pvrhinodemo-2.2.0/pvrhinodemo.egg-info/top_level.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 18:00:55.512664 pvrhinodemo-2.2.0/setup.cfg
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     1979 2023-04-06 17:38:28.000000 pvrhinodemo-2.2.0/setup.py
```

### Comparing `pvrhinodemo-2.1.9/PKG-INFO` & `pvrhinodemo-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.1.9
+Version: 2.2.0
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -74,15 +72,15 @@
 
 It allows testing Rhino on a corpus of audio files. The demo is mainly useful for quantitative performance
 benchmarking. It accepts 16kHz audio files. Rhino processes a single-channel audio stream if a stereo file is
 provided it only processes the first (left) channel. Note that only the relevant spoken command should be present in the
 file and no other speech. There also needs to be at least one second of silence at the end of the file.
 
 ```console
-rhino_demo_file --input_audio_path ${AUDIO_PATH} --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} 
+rhino_demo_file --wav_path ${AUDIO_PATH} --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} 
 ```
 
 ### Microphone Demo
 
 It opens an audio stream from a microphone and performs inference in spoken commands:
 
 ```console
@@ -111,9 +109,7 @@
 ```
 
 If a problem occurs, we suggest storing the recorded audio into a file for inspection. This can be achieved by:
 
 ```console
 rhino_demo_mic --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} --audio_device_index 0 --output_path ~/test.wav
 ```
-
-
```

### Comparing `pvrhinodemo-2.1.9/README.md` & `pvrhinodemo-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 It allows testing Rhino on a corpus of audio files. The demo is mainly useful for quantitative performance
 benchmarking. It accepts 16kHz audio files. Rhino processes a single-channel audio stream if a stereo file is
 provided it only processes the first (left) channel. Note that only the relevant spoken command should be present in the
 file and no other speech. There also needs to be at least one second of silence at the end of the file.
 
 ```console
-rhino_demo_file --input_audio_path ${AUDIO_PATH} --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} 
+rhino_demo_file --wav_path ${AUDIO_PATH} --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} 
 ```
 
 ### Microphone Demo
 
 It opens an audio stream from a microphone and performs inference in spoken commands:
 
 ```console
```

### Comparing `pvrhinodemo-2.1.9/pvrhinodemo/rhino_demo_file.py` & `pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_file.py`

 * *Files 14% similar despite different names*

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
@@ -15,62 +15,71 @@
 
 import pvrhino
 
 
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
 
-    parser.add_argument('--input_audio_path', help='Absolute path to input audio file.',
-                        required=True)
+    parser.add_argument(
+        '--access_key',
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
+        required=True)
 
-    parser.add_argument('--access_key',
-                        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
-                        required=True)
+    parser.add_argument(
+        '--wav_path',
+        help='Absolute path to input audio file.',
+        required=True)
 
-    parser.add_argument('--context_path', help="Absolute path to context file.", required=True)
+    parser.add_argument(
+        '--context_path',
+        help="Absolute path to context file.",
+        required=True)
 
-    parser.add_argument('--library_path', help='Absolute path to dynamic library.', default=pvrhino.LIBRARY_PATH)
+    parser.add_argument(
+        '--library_path',
+        help='Absolute path to dynamic library. Default: using the library provided by `pvrhino`')
 
     parser.add_argument(
         '--model_path',
-        help='Absolute path to the file containing model parameters.',
-        default=pvrhino.MODEL_PATH)
+        help='Absolute path to the file containing model parameters. Default: using the library provided by `pvrhino`')
 
     parser.add_argument(
         '--sensitivity',
-        help="Inference sensitivity. It should be a number within [0, 1]. A higher sensitivity value results in " +
+        help="Inference sensitivity. It should be a number within [0, 1]. A higher sensitivity value results in "
              "fewer misses at the cost of (potentially) increasing the erroneous inference rate.",
         type=float,
         default=0.5)
 
     parser.add_argument(
         '--endpoint_duration_sec',
         help="Endpoint duration in seconds. An endpoint is a chunk of silence at the end of an utterance that marks "
              "the end of spoken command. It should be a positive number within [0.5, 5]. A lower endpoint duration "
              "reduces delay and improves responsiveness. A higher endpoint duration assures Rhino doesn't return "
-             "inference pre-emptively in case the user pauses before finishing the request.",
+             "inference preemptively in case the user pauses before finishing the request.",
         type=float,
         default=1.)
 
     parser.add_argument(
         '--require_endpoint',
         help="If set to `True`, Rhino requires an endpoint (a chunk of silence) after the spoken command. If set to "
              "`False`, Rhino tries to detect silence, but if it cannot, it still will provide inference regardless. "
@@ -111,15 +120,15 @@
     except pvrhino.RhinoActivationThrottledError as e:
         print("AccessKey '%s' has been throttled" % args.access_key)
         raise e
     except pvrhino.RhinoError as e:
         print("Failed to initialize Rhino")
         raise e
 
-    audio = read_file(args.input_audio_path, rhino.sample_rate)
+    audio = read_file(args.wav_path, rhino.sample_rate)
 
     num_frames = len(audio) // rhino.frame_length
     for i in range(num_frames):
         frame = audio[i * rhino.frame_length:(i + 1) * rhino.frame_length]
         is_finalized = rhino.process(frame)
         if is_finalized:
             inference = rhino.get_inference()
```

### Comparing `pvrhinodemo-2.1.9/pvrhinodemo/rhino_demo_mic.py` & `pvrhinodemo-2.2.0/pvrhinodemo/rhino_demo_mic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,206 +1,60 @@
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
 import struct
 import wave
-from threading import Thread
 
 import pvrhino
 from pvrecorder import PvRecorder
 
 
-class RhinoDemo(Thread):
-    """
-    Microphone Demo for Rhino Speech-to-Intent engine. It creates an input audio stream from a microphone, monitors
-    it, and extracts the intent from the speech command. It optionally saves the recorded audio into a file for further
-    debugging.
-    """
-
-    def __init__(
-            self,
-            access_key,
-            library_path,
-            model_path,
-            context_path,
-            endpoint_duration_sec,
-            require_endpoint,
-            audio_device_index=None,
-            output_path=None):
-        """
-        Constructor.
-
-        :param access_key: AccessKey obtained from Picovoice Console (https://console.picovoice.ai/).
-        :param library_path: Absolute path to Rhino's dynamic library.
-        :param model_path: Absolute path to file containing model parameters.
-        :param context_path: Absolute path to file containing context model (file with `.rhn` extension). A context
-        represents the set of expressions (spoken commands), intents, and intent arguments (slots) within a domain of
-        interest.
-        :param endpoint_duration_sec: Endpoint duration in seconds. An endpoint is a chunk of silence at the end of an
-        utterance that marks the end of spoken command. It should be a positive number within [0.5, 5]. A lower endpoint
-        duration reduces delay and improves responsiveness. A higher endpoint duration assures Rhino doesn't return
-        inference pre-emptively in case the user pauses before finishing the request.
-        require_endpoint: If set to `True`, Rhino requires an endpoint (a chunk of silence) after the spoken command.
-        If set to `False`, Rhino tries to detect silence, but if it cannot, it still will provide inference regardless.
-        Set to `False` only if operating in an environment with overlapping speech (e.g. people talking in the
-        background).
-        :param audio_device_index: Optional argument. If provided, audio is recorded from this input device. Otherwise,
-        the default audio input device is used.
-        :param output_path: If provided recorded audio will be stored in this location at the end of the run.
-        """
-
-        super(RhinoDemo, self).__init__()
-
-        self._access_key = access_key
-        self._library_path = library_path
-        self._model_path = model_path
-        self._context_path = context_path
-        self._endpoint_duration_sec = endpoint_duration_sec
-        self._require_endpoint = require_endpoint
-        self._audio_device_index = audio_device_index
-
-        self._output_path = output_path
-
-    def run(self):
-        """
-         Creates an input audio stream, instantiates an instance of Rhino object, and infers the intent from spoken
-         commands.
-         """
-
-        rhino = None
-        recorder = None
-        wav_file = None
-
-        try:
-            rhino = pvrhino.create(
-                access_key=self._access_key,
-                library_path=self._library_path,
-                model_path=self._model_path,
-                context_path=self._context_path,
-                endpoint_duration_sec=self._endpoint_duration_sec,
-                require_endpoint=self._require_endpoint)
-
-            recorder = PvRecorder(device_index=self._audio_device_index, frame_length=rhino.frame_length)
-            recorder.start()
-
-            if self._output_path is not None:
-                wav_file = wave.open(self._output_path, "w")
-                wav_file.setparams((1, 2, 16000, 512, "NONE", "NONE"))
-
-            print(rhino.context_info)
-            print()
-
-            print("Using device: %s" % recorder.selected_device)
-            print("Listening...")
-            print()
-
-            while True:
-                pcm = recorder.read()
-
-                if wav_file is not None:
-                    wav_file.writeframes(struct.pack("h" * len(pcm), *pcm))
-
-                is_finalized = rhino.process(pcm)
-                if is_finalized:
-                    inference = rhino.get_inference()
-                    if inference.is_understood:
-                        print('{')
-                        print("  intent : '%s'" % inference.intent)
-                        print('  slots : {')
-                        for slot, value in inference.slots.items():
-                            print("    %s : '%s'" % (slot, value))
-                        print('  }')
-                        print('}\n')
-                    else:
-                        print("Didn't understand the command.\n")
-        except pvrhino.RhinoInvalidArgumentError as e:
-            args = (
-                self._access_key,
-                self._library_path,
-                self._model_path,
-                self._context_path,
-                self._require_endpoint
-            )
-            print("One or more arguments provided to Rhino is invalid: ", args)
-            print("If all other arguments seem valid, ensure that '%s' is a valid AccessKey" % self._access_key)
-            raise e
-        except pvrhino.RhinoActivationError as e:
-            print("AccessKey activation error")
-            raise e
-        except pvrhino.RhinoActivationLimitError as e:
-            print("AccessKey '%s' has reached it's temporary device limit" % self._access_key)
-            raise e
-        except pvrhino.RhinoActivationRefusedError as e:
-            print("AccessKey '%s' refused" % self._access_key)
-            raise e
-        except pvrhino.RhinoActivationThrottledError as e:
-            print("AccessKey '%s' has been throttled" % self._access_key)
-            raise e
-        except pvrhino.RhinoError as e:
-            print("Failed to initialize Rhino")
-            raise e
-        except KeyboardInterrupt:
-            print('Stopping ...')
-
-        finally:
-            if recorder is not None:
-                recorder.delete()
-
-            if rhino is not None:
-                rhino.delete()
-
-            if wav_file is not None:
-                wav_file.close()
-
-    @classmethod
-    def show_audio_devices(cls):
-        devices = PvRecorder.get_audio_devices()
-
-        for i in range(len(devices)):
-            print("index: %d, device name: %s" % (i, devices[i]))
-
-
 def main():
     parser = argparse.ArgumentParser()
 
-    parser.add_argument('--access_key',
-                        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
-                        required=True)
+    parser.add_argument(
+        '--access_key',
+        help='AccessKey obtained from Picovoice Console (https://console.picovoice.ai/)',
+        required=True)
 
-    parser.add_argument('--context_path', help="Absolute path to context file.", required=True)
+    parser.add_argument(
+        '--context_path',
+        help="Absolute path to context file.",
+        required=True)
 
-    parser.add_argument('--library_path', help="Absolute path to dynamic library.", default=pvrhino.LIBRARY_PATH)
+    parser.add_argument(
+        '--library_path',
+        help='Absolute path to dynamic library. Default: using the library provided by `pvrhino`')
 
     parser.add_argument(
         '--model_path',
-        help="Absolute path to the file containing model parameters.",
-        default=pvrhino.MODEL_PATH)
+        help='Absolute path to the file containing model parameters. Default: using the library provided by `pvrhino`')
 
     parser.add_argument(
         '--sensitivity',
-        help="Inference sensitivity. It should be a number within [0, 1]. A higher sensitivity value results in " +
+        help="Inference sensitivity. It should be a number within [0, 1]. A higher sensitivity value results in "
              "fewer misses at the cost of (potentially) increasing the erroneous inference rate.",
         type=float,
         default=0.5)
 
     parser.add_argument(
         '--endpoint_duration_sec',
         help="Endpoint duration in seconds. An endpoint is a chunk of silence at the end of an utterance that marks "
              "the end of spoken command. It should be a positive number within [0.5, 5]. A lower endpoint duration "
              "reduces delay and improves responsiveness. A higher endpoint duration assures Rhino doesn't return "
-             "inference pre-emptively in case the user pauses before finishing the request.",
+             "inference preemptively in case the user pauses before finishing the request.",
         type=float,
         default=1.)
 
     parser.add_argument(
         '--require_endpoint',
         help="If set to `True`, Rhino requires an endpoint (a chunk of silence) after the spoken command. If set to "
              "`False`, Rhino tries to detect silence, but if it cannot, it still will provide inference regardless. "
@@ -219,25 +73,89 @@
 
     if args.require_endpoint.lower() == 'false':
         require_endpoint = False
     else:
         require_endpoint = True
 
     if args.show_audio_devices:
-        RhinoDemo.show_audio_devices()
-    else:
-        if not args.context_path:
-            raise ValueError('Missing path to context file')
+        for i, device in enumerate(PvRecorder.get_audio_devices()):
+            print('Device %d: %s' % (i, device))
+        return
 
-        RhinoDemo(
+    try:
+        rhino = pvrhino.create(
             access_key=args.access_key,
             library_path=args.library_path,
             model_path=args.model_path,
             context_path=args.context_path,
+            sensitivity=args.sensitivity,
             endpoint_duration_sec=args.endpoint_duration_sec,
-            require_endpoint=require_endpoint,
-            audio_device_index=args.audio_device_index,
-            output_path=args.output_path).run()
+            require_endpoint=require_endpoint)
+    except pvrhino.RhinoInvalidArgumentError as e:
+        print("One or more arguments provided to Rhino is invalid: ", args)
+        print("If all other arguments seem valid, ensure that '%s' is a valid AccessKey" % args.access_key)
+        raise e
+    except pvrhino.RhinoActivationError as e:
+        print("AccessKey activation error")
+        raise e
+    except pvrhino.RhinoActivationLimitError as e:
+        print("AccessKey '%s' has reached it's temporary device limit" % args.access_key)
+        raise e
+    except pvrhino.RhinoActivationRefusedError as e:
+        print("AccessKey '%s' refused" % args.access_key)
+        raise e
+    except pvrhino.RhinoActivationThrottledError as e:
+        print("AccessKey '%s' has been throttled" % args.access_key)
+        raise e
+    except pvrhino.RhinoError as e:
+        print("Failed to initialize Rhino")
+        raise e
+
+    print('Rhino version: %s' % rhino.version)
+    print('Context info: %s' % rhino.context_info)
+
+    recorder = PvRecorder(
+        device_index=args.audio_device_index,
+        frame_length=rhino.frame_length)
+    recorder.start()
+
+    print('Using device: %s' % recorder.device)
+    print('Listening ... Press Ctrl+C to exit.\n')
+
+    wav_file = None
+    if args.output_path is not None:
+        wav_file = wave.open(args.output_path, 'wb')
+        wav_file.setnchannels(1)
+        wav_file.setsampwidth(2)
+        wav_file.setframerate(recorder.sample_rate)
+
+    try:
+        while True:
+            pcm = recorder.read()
+
+            if wav_file is not None:
+                wav_file.writeframes(struct.pack("h" * len(pcm), *pcm))
+
+            is_finalized = rhino.process(pcm)
+            if is_finalized:
+                inference = rhino.get_inference()
+                if inference.is_understood:
+                    print('{')
+                    print("  intent : '%s'" % inference.intent)
+                    print('  slots : {')
+                    for slot, value in inference.slots.items():
+                        print("    %s : '%s'" % (slot, value))
+                    print('  }')
+                    print('}\n')
+                else:
+                    print("Didn't understand the command.\n")
+    except KeyboardInterrupt:
+        print('Stopping ...')
+    finally:
+        recorder.delete()
+        rhino.delete()
+        if wav_file is not None:
+            wav_file.close()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pvrhinodemo-2.1.9/pvrhinodemo.egg-info/PKG-INFO` & `pvrhinodemo-2.2.0/pvrhinodemo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pvrhinodemo
-Version: 2.1.9
+Version: 2.2.0
 Summary: Rhino Speech-to-Intent engine demos.
 Home-page: https://github.com/Picovoice/rhino
 Author: Picovoice
 Author-email: hello@picovoice.ai
-License: UNKNOWN
 Keywords: Speech-to-Intent,voice commands,voice control,speech recognition,natural language understanding
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.5
@@ -74,15 +72,15 @@
 
 It allows testing Rhino on a corpus of audio files. The demo is mainly useful for quantitative performance
 benchmarking. It accepts 16kHz audio files. Rhino processes a single-channel audio stream if a stereo file is
 provided it only processes the first (left) channel. Note that only the relevant spoken command should be present in the
 file and no other speech. There also needs to be at least one second of silence at the end of the file.
 
 ```console
-rhino_demo_file --input_audio_path ${AUDIO_PATH} --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} 
+rhino_demo_file --wav_path ${AUDIO_PATH} --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} 
 ```
 
 ### Microphone Demo
 
 It opens an audio stream from a microphone and performs inference in spoken commands:
 
 ```console
@@ -111,9 +109,7 @@
 ```
 
 If a problem occurs, we suggest storing the recorded audio into a file for inspection. This can be achieved by:
 
 ```console
 rhino_demo_mic --access_key ${ACCESS_KEY} --context_path ${CONTEXT_PATH} --audio_device_index 0 --output_path ~/test.wav
 ```
-
-
```

### Comparing `pvrhinodemo-2.1.9/setup.py` & `pvrhinodemo-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     f.write('include pvrhinodemo/rhino_demo_mic.py')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvrhinodemo",
-    version="2.1.9",
+    version="2.2.0",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Rhino Speech-to-Intent engine demos.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/rhino",
     packages=["pvrhinodemo"],
-    install_requires=["pvrhino==2.1.7", "pvrecorder==1.1.1"],
+    install_requires=["pvrhino==2.2.0", "pvrecorder==1.1.1"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

