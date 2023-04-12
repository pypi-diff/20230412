# Comparing `tmp/whisper-ctranslate2-0.1.6.tar.gz` & `tmp/whisper-ctranslate2-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.1.6.tar", last modified: Mon Apr 10 13:55:18 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.1.7.tar", last modified: Wed Apr 12 17:51:16 2023, max compression
```

## Comparing `whisper-ctranslate2-0.1.6.tar` & `whisper-ctranslate2-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.6/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3331 2023-04-09 16:29:17.000000 whisper-ctranslate2-0.1.6/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-10 13:39:26.000000 whisper-ctranslate2-0.1.6/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-10 13:24:17.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5136 2023-04-10 13:24:17.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-10 13:39:26.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    11529 2023-04-10 13:39:26.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-10 13:55:18.262423 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3982 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      522 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       80 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-10 13:55:18.000000 whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.7/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3558 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-12 16:34:42.000000 whisper-ctranslate2-0.1.7/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4310 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-10 14:05:51.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5319 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-10 14:05:51.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12169 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      554 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       98 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.1.6/LICENSE` & `whisper-ctranslate2-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.6/PKG-INFO` & `whisper-ctranslate2-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -93,14 +93,20 @@
 
     --print-colors PRINT_COLORS
 
 Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
+    --live_transcribe
+
+Adding the `----live_transcribe True` will activate the live transcription mode from your microphone.
+
+https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
+
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
 
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
```

### Comparing `whisper-ctranslate2-0.1.6/README.md` & `whisper-ctranslate2-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 
     --print-colors PRINT_COLORS
 
 Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
+    --live_transcribe
+
+Adding the `----live_transcribe True` will activate the live transcription mode from your microphone.
+
+https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
+
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
 
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
```

### Comparing `whisper-ctranslate2-0.1.6/setup.py` & `whisper-ctranslate2-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/models.py` & `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/models.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/transcribe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from .writers import format_timestamp
 from typing import NamedTuple, Optional, List, Union
 import tqdm
 import sys
 from faster_whisper import WhisperModel
 from .languages import LANGUAGES
+from typing import BinaryIO
+import numpy as np
+
 
 system_encoding = sys.getdefaultencoding()
 
 if system_encoding != "utf-8":
 
     def make_safe(string):
         return string.encode(system_encoding, errors="replace").decode(system_encoding)
@@ -66,23 +69,24 @@
             end_mark = "\033[0m"
             text_words += f"{k_colors[col]}{word.word}{end_mark}"
 
         return text_words
 
     def inference(
         self,
-        audio: str,
+        audio: Union[str, BinaryIO, np.ndarray],
         model_path: str,
         task: str,
         language: str,
         threads: int,
         device: str,
         device_index: Union[int, List[int]],
         compute_type: str,
         verbose: bool,
+        live: bool,
         options: TranscriptionOptions,
     ):
         model = WhisperModel(
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
@@ -110,38 +114,40 @@
             vad_filter=options.vad_filter,
             vad_parameters={
                 "min_silence_duration_ms": options.vad_min_silence_duration_ms
             },
         )
 
         language_name = LANGUAGES[info.language].title()
-        print(
-            "Detected language '%s' with probability %f"
-            % (language_name, info.language_probability)
-        )
+        if not live:
+            print(
+                "Detected language '%s' with probability %f"
+                % (language_name, info.language_probability)
+            )
 
         list_segments = []
         last_pos = 0
         accumated_inc = 0
         all_text = ""
         with tqdm.tqdm(
-            total=info.duration, unit="seconds", disable=verbose is not False
+            total=info.duration, unit="seconds", disable=verbose or live is not False
         ) as pbar:
             for segment in segments:
                 start, end, text = segment.start, segment.end, segment.text
                 all_text += segment.text
 
                 if verbose or options.print_colors:
                     if options.print_colors and segment.words:
                         text = self._get_colored_text(segment.words)
                     else:
                         text = segment.text
 
-                    line = f"[{format_timestamp(start)} --> {format_timestamp(end)}] {text}"
-                    print(make_safe(line))
+                    if not live:
+                        line = f"[{format_timestamp(start)} --> {format_timestamp(end)}] {text}"
+                        print(make_safe(line))
 
                 segment_dict = segment._asdict()
                 if segment.words:
                     segment_dict["words"] = [word._asdict() for word in segment.words]
 
                 list_segments.append(segment_dict)
                 duration = segment.end - last_pos
```

### Comparing `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from .models import Models
 from .languages import LANGUAGES, TO_LANGUAGE_CODE, from_language_to_iso_code
 import numpy as np
 import warnings
 from typing import Union, List
 from .writers import get_writer
 from .version import __version__
+from .live import Live
+import sys
 
 
 def optional_int(string):
     return None if string == "None" else int(string)
 
 
 def str2bool(string):
@@ -27,15 +29,15 @@
 
 
 def read_command_line():
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
     parser.add_argument(
-        "audio", nargs="+", type=str, help="audio file(s) to transcribe"
+        "audio", nargs="*", type=str, help="audio file(s) to transcribe"
     )
     parser.add_argument(
         "--model",
         default="small",
         choices=Models().get_list(),
         help="name of the Whisper model to use",
     )
@@ -241,14 +243,18 @@
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
         help="Show program's version number and exit",
     )
 
+    parser.add_argument(
+        "--live_transcribe", type=str2bool, default=False, help="Live transcribe mode"
+    )
+
     return parser.parse_args().__dict__
 
 
 def main():
     args = read_command_line()
     output_dir: str = args.pop("output_dir")
     output_format: str = args.pop("output_format")
@@ -260,14 +266,16 @@
     device: str = args.pop("device")
     compute_type: str = args.pop("compute_type")
     verbose: bool = args.pop("verbose")
     model_directory: str = args.pop("model_directory")
     cache_directory: str = args.pop("model_dir")
     device_index: Union[int, List[int]] = args.pop("device_index")
     suppress_tokens: str = args.pop("suppress_tokens")
+    live_transcribe: bool = args.pop("live_transcribe")
+    audio: str = args.pop("audio")
 
     temperature = args.pop("temperature")
     if (increment := args.pop("temperature_increment_on_fallback")) is not None:
         temperature = tuple(np.arange(temperature, 1.0 + 1e-6, increment))
     else:
         temperature = [temperature]
 
@@ -322,25 +330,45 @@
         model_filename = os.path.join(model_directory, "model.bin")
         if not os.path.exists(model_filename):
             raise RuntimeError(f"Model file '{model_filename}' does not exists")
         model_dir = model_directory
     else:
         model_dir = Models(cache_directory).get_model_dir(model)
 
-    for audio_path in args.pop("audio"):
+    if live_transcribe:
+        Live(
+            model_dir,
+            task,
+            language,
+            threads,
+            device,
+            device_index,
+            compute_type,
+            verbose,
+            options,
+        ).inference()
+
+        return
+
+    if len(audio) == 0:
+        sys.stderr.write("You need to specify one or more audio files\n")
+        return
+
+    for audio_path in audio:
         result = Transcribe().inference(
             audio_path,
             model_dir,
             task,
             language,
             threads,
             device,
             device_index,
             compute_type,
             verbose,
+            False,
             options,
         )
         writer = get_writer(output_format, output_dir)
         writer(result, audio_path)
 
 
 if __name__ == "__main__":
```

### Comparing `whisper-ctranslate2-0.1.6/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -93,14 +93,20 @@
 
     --print-colors PRINT_COLORS
 
 Adding the `--print_colors True` argument will print the transcribed text using an experimental color coding strategy based on [whisper.cpp](https://github.com/ggerganov/whisper.cpp) to highlight words with high or low confidence:
 
 <img alt="image" src="https://user-images.githubusercontent.com/309265/228054378-48ac6af4-ce4b-44da-b4ec-70ce9f2f2a6c.png">
 
+    --live_transcribe
+
+Adding the `----live_transcribe True` will activate the live transcription mode from your microphone.
+
+https://user-images.githubusercontent.com/309265/231533784-e58c4b92-e9fb-4256-b4cd-12f1864131d9.mov
+
 # Need help?
 
 Check our [frequently asked questions](FAQ.md) for common questions.
 
 # Contact
 
 Jordi Mas <jmas@softcatala.org>
```

### Comparing `whisper-ctranslate2-0.1.6/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/whisper_ctranslate2/languages.py
+src/whisper_ctranslate2/live.py
 src/whisper_ctranslate2/models.py
 src/whisper_ctranslate2/transcribe.py
 src/whisper_ctranslate2/version.py
 src/whisper_ctranslate2/whisper_ctranslate2.py
 src/whisper_ctranslate2/writers.py
 whisper_ctranslate2.egg-info/PKG-INFO
 whisper_ctranslate2.egg-info/SOURCES.txt
```

