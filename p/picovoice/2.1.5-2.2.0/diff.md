# Comparing `tmp/picovoice-2.1.5.tar.gz` & `tmp/picovoice-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picovoice-2.1.5.tar", last modified: Thu Jun 30 15:54:29 2022, max compression
+gzip compressed data, was "picovoice-2.2.0.tar", last modified: Wed Apr 12 18:05:03 2023, max compression
```

## Comparing `picovoice-2.1.5.tar` & `picovoice-2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2022-06-30 15:54:29.252807 picovoice-2.1.5/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       87 2022-06-30 15:54:28.000000 picovoice-2.1.5/MANIFEST.in
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4412 2022-06-30 15:54:29.252807 picovoice-2.1.5/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     3684 2022-06-13 15:28:43.000000 picovoice-2.1.5/README.md
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2022-06-30 15:54:29.252807 picovoice-2.1.5/picovoice/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2022-06-30 15:54:28.000000 picovoice-2.1.5/picovoice/LICENSE
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     1116 2022-06-30 15:54:28.000000 picovoice-2.1.5/picovoice/__init__.py
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    12278 2022-06-30 15:54:28.000000 picovoice-2.1.5/picovoice/picovoice.py
-drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2022-06-30 15:54:29.252807 picovoice-2.1.5/picovoice.egg-info/
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4412 2022-06-30 15:54:28.000000 picovoice-2.1.5/picovoice.egg-info/PKG-INFO
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      257 2022-06-30 15:54:29.000000 picovoice-2.1.5/picovoice.egg-info/SOURCES.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2022-06-30 15:54:28.000000 picovoice-2.1.5/picovoice.egg-info/dependency_links.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       34 2022-06-30 15:54:29.000000 picovoice-2.1.5/picovoice.egg-info/requires.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       10 2022-06-30 15:54:29.000000 picovoice-2.1.5/picovoice.egg-info/top_level.txt
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2022-06-30 15:54:29.252807 picovoice-2.1.5/setup.cfg
--rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2281 2022-06-30 15:54:15.000000 picovoice-2.1.5/setup.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:05:03.575489 picovoice-2.2.0/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       88 2023-04-12 18:05:02.000000 picovoice-2.2.0/MANIFEST.in
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4412 2023-04-12 18:05:03.575489 picovoice-2.2.0/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     3684 2022-06-13 15:28:43.000000 picovoice-2.2.0/README.md
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:05:03.571489 picovoice-2.2.0/picovoice/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    11344 2023-04-12 18:05:02.000000 picovoice-2.2.0/picovoice/LICENSE
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      534 2023-04-12 18:05:02.000000 picovoice-2.2.0/picovoice/__init__.py
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)    12966 2023-04-12 18:05:02.000000 picovoice-2.2.0/picovoice/_picovoice.py
+drwxrwxr-x   0 picovoice  (1000) picovoice  (1000)        0 2023-04-12 18:05:03.575489 picovoice-2.2.0/picovoice.egg-info/
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     4412 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/PKG-INFO
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)      258 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/SOURCES.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)        1 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/dependency_links.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       34 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/requires.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       10 2023-04-12 18:05:03.000000 picovoice-2.2.0/picovoice.egg-info/top_level.txt
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)       38 2023-04-12 18:05:03.575489 picovoice-2.2.0/setup.cfg
+-rw-rw-r--   0 picovoice  (1000) picovoice  (1000)     2284 2023-04-10 19:55:03.000000 picovoice-2.2.0/setup.py
```

### Comparing `picovoice-2.1.5/PKG-INFO` & `picovoice-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picovoice
-Version: 2.1.5
+Version: 2.2.0
 Summary: Picovoice is an end-to-end platform for building voice products on your terms.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `picovoice-2.1.5/README.md` & `picovoice-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `picovoice-2.1.5/picovoice/LICENSE` & `picovoice-2.2.0/picovoice/LICENSE`

 * *Files identical despite different names*

### Comparing `picovoice-2.1.5/picovoice/picovoice.py` & `picovoice-2.2.0/picovoice/_picovoice.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 #
-
 import os
+from typing import Callable, Optional, Sequence
 
 import pvporcupine
 import pvrhino
 
 
 class PicovoiceError(Exception):
     pass
@@ -104,27 +104,27 @@
     `.frame_length`. The incoming audio needs to have a sample rate equal to `.sample_rate` and be 16-bit
     linearly-encoded. Picovoice operates on single-channel audio. It uses Porcupine wake word engine for wake word
     detection and Rhino Speech-to-Intent engine for intent inference.
     """
 
     def __init__(
             self,
-            access_key,
-            keyword_path,
-            wake_word_callback,
-            context_path,
-            inference_callback,
-            porcupine_library_path=None,
-            porcupine_model_path=None,
-            porcupine_sensitivity=0.5,
-            rhino_library_path=None,
-            rhino_model_path=None,
-            rhino_sensitivity=0.5,
-            endpoint_duration_sec=1.,
-            require_endpoint=True):
+            access_key: str,
+            keyword_path: str,
+            wake_word_callback: Callable[[], None],
+            context_path: str,
+            inference_callback: Callable[[pvrhino.Inference], None],
+            porcupine_library_path: Optional[str] = None,
+            porcupine_model_path: Optional[str] = None,
+            porcupine_sensitivity: float = 0.5,
+            rhino_library_path: Optional[str] = None,
+            rhino_model_path: Optional[str] = None,
+            rhino_sensitivity: float = 0.5,
+            endpoint_duration_sec: float = 1.,
+            require_endpoint: bool = True):
         """
         Constructor.
 
         :param access_key: AccessKey obtained from Picovoice Console (https://console.picovoice.ai/).
         :param keyword_path: Absolute path to Porcupine's keyword model file.
         :param wake_word_callback: User-defined callback invoked upon detection of the wake phrase. The callback accepts
         no input arguments.
@@ -227,15 +227,15 @@
 
     def delete(self):
         """Releases resources acquired."""
 
         self._porcupine.delete()
         self._rhino.delete()
 
-    def process(self, pcm):
+    def process(self, pcm: Sequence[int]) -> None:
         """
         Processes a frame of the incoming audio stream. Upon detection of wake word and completion of follow-on command
         inference invokes user-defined callbacks.
 
         :param pcm: A frame of audio samples. The number of samples per frame can be attained by calling
         `.frame_length`. The incoming audio needs to have a sample rate equal to `.sample_rate` and be 16-bit
         linearly-encoded. Picovoice operates on single-channel audio.
@@ -258,32 +258,49 @@
                     self._is_wake_word_detected = False
                     inference = self._rhino.get_inference()
                     self._inference_callback(inference)
             except pvrhino.RhinoError as e:
                 raise _PPN_RHN_ERROR_TO_PICOVOICE_ERROR[type(e)] from e
 
     @property
-    def sample_rate(self):
+    def sample_rate(self) -> int:
         """Audio sample rate accepted by Picovoice."""
 
         return self._sample_rate
 
     @property
-    def frame_length(self):
+    def frame_length(self) -> int:
         """Number of audio samples per frame."""
 
         return self._frame_length
 
     @property
-    def version(self):
+    def version(self) -> str:
         """Version"""
 
-        return '2.1.0'
+        return '2.2.0'
 
     @property
-    def context_info(self):
+    def context_info(self) -> str:
         """Context information."""
 
         return self._rhino.context_info
 
     def __str__(self):
         return 'Picovoice %s {Porcupine %s, Rhino %s}' % (self.version, self._porcupine.version, self._rhino.version)
+
+
+__all__ = [
+    'Picovoice',
+    'PicovoiceError',
+    'PicovoiceMemoryError',
+    'PicovoiceIOError',
+    'PicovoiceInvalidArgumentError',
+    'PicovoiceStopIterationError',
+    'PicovoiceKeyError',
+    'PicovoiceInvalidStateError',
+    'PicovoiceRuntimeError',
+    'PicovoiceActivationError',
+    'PicovoiceActivationLimitError',
+    'PicovoiceActivationThrottledError',
+    'PicovoiceActivationRefusedError'
+]
```

### Comparing `picovoice-2.1.5/picovoice.egg-info/PKG-INFO` & `picovoice-2.2.0/picovoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picovoice
-Version: 2.1.5
+Version: 2.2.0
 Summary: Picovoice is an end-to-end platform for building voice products on your terms.
 Home-page: https://github.com/Picovoice/picovoice
 Author: Picovoice Inc.
 Author-email: hello@picovoice.ai
 Keywords: wake word,voice control,speech recognition,voice recognition,natural language understanding
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `picovoice-2.1.5/setup.py` & `picovoice-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,35 +17,35 @@
 os.system('git clean -dfx')
 
 package_folder = os.path.join(os.path.dirname(__file__), 'picovoice')
 os.mkdir(package_folder)
 
 shutil.copy(os.path.join(os.path.dirname(__file__), '../../LICENSE'), package_folder)
 shutil.copy(os.path.join(os.path.dirname(__file__), '__init__.py'), os.path.join(package_folder, '__init__.py'))
-shutil.copy(os.path.join(os.path.dirname(__file__), 'picovoice.py'), os.path.join(package_folder, 'picovoice.py'))
+shutil.copy(os.path.join(os.path.dirname(__file__), '_picovoice.py'), os.path.join(package_folder, '_picovoice.py'))
 
 with open(os.path.join(os.path.dirname(__file__), 'MANIFEST.in'), 'w') as f:
     f.write('include picovoice/LICENSE\n')
     f.write('include picovoice/__init__.py\n')
-    f.write('include picovoice/picovoice.py\n')
+    f.write('include picovoice/_picovoice.py\n')
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="picovoice",
-    version="2.1.5",
+    version="2.2.0",
     author="Picovoice Inc.",
     author_email="hello@picovoice.ai",
     description="Picovoice is an end-to-end platform for building voice products on your terms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/picovoice",
     packages=["picovoice"],
-    install_requires=["pvporcupine==2.1.4", "pvrhino==2.1.7"],
+    install_requires=["pvporcupine==2.2.0", "pvrhino==2.2.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

