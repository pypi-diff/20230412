# Comparing `tmp/audalign-1.2.2.tar.gz` & `tmp/audalign-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audalign-1.2.2.tar", last modified: Mon Feb  6 05:12:09 2023, max compression
+gzip compressed data, was "audalign-1.2.3.tar", last modified: Wed Apr 12 19:13:56 2023, max compression
```

## Comparing `audalign-1.2.2.tar` & `audalign-1.2.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.587234 audalign-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-02-06 05:11:49.000000 audalign-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-02-06 05:12:09.587234 audalign-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-02-06 05:11:49.000000 audalign-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign/
--rw-r--r--   0 runner    (1001) docker     (123)    31803 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign/align/
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/align/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/config/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/config/correlation_spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/config/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/config/visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/datalign.py
--rw-r--r--   0 runner    (1001) docker     (123)    27519 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/filehandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign/recognizers/
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign/recognizers/correcognize/
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/correcognize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/correcognize/correcognize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign/recognizers/correcognizeSpectrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/correcognizeSpectrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22722 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign/recognizers/fingerprint/
--rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/fingerprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/fingerprint/fingerprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/fingerprint/recognize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.587234 audalign-1.2.2/audalign/recognizers/visrecognize/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/visrecognize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-02-06 05:11:49.000000 audalign-1.2.2/audalign/recognizers/visrecognize/visrecognize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.583233 audalign-1.2.2/audalign.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-02-06 05:12:09.000000 audalign-1.2.2/audalign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-02-06 05:12:09.000000 audalign-1.2.2/audalign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 05:12:09.000000 audalign-1.2.2/audalign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-06 05:12:09.000000 audalign-1.2.2/audalign.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-06 05:12:09.000000 audalign-1.2.2/audalign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 05:12:09.587234 audalign-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-06 05:11:49.000000 audalign-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 05:12:09.587234 audalign-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 05:11:49.000000 audalign-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-02-06 05:11:49.000000 audalign-1.2.2/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-02-06 05:11:49.000000 audalign-1.2.2/tests/test_audalign.py
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-02-06 05:11:49.000000 audalign-1.2.2/tests/test_recognize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-12 19:13:45.000000 audalign-1.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-12 19:13:56.637598 audalign-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-12 19:13:45.000000 audalign-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/
+-rw-r--r--   0 runner    (1001) docker     (123)    34505 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/align/
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/align/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/config/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/config/correlation_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/config/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/config/visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/datalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27519 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/filehandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/recognizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/recognizers/correcognize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/correcognize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/correcognize/correcognize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/recognizers/correcognizeSpectrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/correcognizeSpectrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22722 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/recognizers/fingerprint/
+-rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/fingerprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/fingerprint/fingerprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/fingerprint/recognize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign/recognizers/visrecognize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/visrecognize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-04-12 19:13:45.000000 audalign-1.2.3/audalign/recognizers/visrecognize/visrecognize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/audalign.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-12 19:13:56.000000 audalign-1.2.3/audalign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 19:13:56.000000 audalign-1.2.3/audalign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:13:56.000000 audalign-1.2.3/audalign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-12 19:13:56.000000 audalign-1.2.3/audalign.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 19:13:56.000000 audalign-1.2.3/audalign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:13:56.637598 audalign-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 19:13:45.000000 audalign-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:56.637598 audalign-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:13:45.000000 audalign-1.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-04-12 19:13:45.000000 audalign-1.2.3/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-12 19:13:45.000000 audalign-1.2.3/tests/test_audalign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-04-12 19:13:45.000000 audalign-1.2.3/tests/test_recognize.py
```

### Comparing `audalign-1.2.2/LICENSE.md` & `audalign-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/PKG-INFO` & `audalign-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audalign
-Version: 1.2.2
+Version: 1.2.3
 Summary: Audio Alignment and Recognition in Python
 Home-page: http://github.com/benfmiller/audalign
 Author: Ben Miller
 Author-email: benfmiller132@gmail.com
 Maintainer: Ben Miller
 Maintainer-email: benfmiller132@gmail.com
 License: MIT
```

### Comparing `audalign-1.2.2/README.md` & `audalign-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/__init__.py` & `audalign-1.2.3/audalign/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 This file serves as the host file for all audalign functions.
 
 recognitions and alignments use recognizer objects which can be configured with
-their respective configuration objects. 
+their respective configuration objects.
 
 There are a number of functions that can be used to enhance the alignments such
 as "uniform leveling" and "remove noise" functions. Writing shifts can also be nifty.
 
 One useful workflow could be to uniform level some files, do a remove noise on them, then
 align and fine align them. Then, to have the shifts applied to the original files, use
 "write_shifts_from_results".
 """
 
 import os
 from functools import wraps
 from pprint import PrettyPrinter
+from typing import Optional
 
 from pydub.utils import mediainfo
 
 import audalign.align as aligner
 import audalign.datalign as datalign
 import audalign.filehandler as filehandler
 from audalign.config import BaseConfig
@@ -51,25 +52,45 @@
                 results["rankings"]["match_info"] = rank_alignment(results, recognizer)
 
         return results
 
     return wrapper_decorator
 
 
+def filter_close_seconds(func):
+    @wraps(func)
+    def wrapper_decorator(*args, **kwargs):
+        results = func(*args, **kwargs)
+        if results is None:
+            return results
+        assert results.get("rankings") is not None #This should run after rankings are added
+        close_seconds_filter = BaseConfig.close_seconds_filter
+        if kwargs.get("recognizer") is not None:
+            close_seconds_filter = kwargs.get("recognizer").config.close_seconds_filter
+        if close_seconds_filter is None:
+            return results
+        if "names_and_paths" in results:
+            return __filter_close_seconds_alignment(results, close_seconds_filter)
+        else:
+            return __filter_close_seconds(results, close_seconds_filter)
+    return wrapper_decorator
+
+@filter_close_seconds
 @add_rankings
 def recognize(
     target_file: str,
     against_path: str = None,
     recognizer: BaseRecognizer = None,
 ) -> dict:
     if recognizer is None:
         recognizer = FingerprintRecognizer()
     return recognizer.recognize(target_file, against_path)
 
 
+@filter_close_seconds
 @add_rankings
 def align(
     directory_path: str,
     destination_path: str = None,
     write_extension: str = None,
     write_multi_channel: bool = False,
     recognizer: BaseRecognizer = None,
@@ -97,14 +118,15 @@
         file_dir=directory_path,
         destination_path=destination_path,
         write_extension=write_extension,
         write_multi_channel=write_multi_channel,
     )
 
 
+@filter_close_seconds
 @add_rankings
 def align_files(
     filename_a,
     filename_b,
     *filenames,
     destination_path: str = None,
     write_extension: str = None,
@@ -139,14 +161,15 @@
         file_dir=None,
         destination_path=destination_path,
         write_extension=write_extension,
         write_multi_channel=write_multi_channel,
     )
 
 
+@filter_close_seconds
 @add_rankings
 def target_align(
     target_file: str,
     directory_path: str,
     destination_path: str = None,
     write_extension: str = None,
     write_multi_channel: bool = False,
@@ -179,14 +202,15 @@
         destination_path=destination_path,
         target_aligning=True,
         write_extension=write_extension,
         write_multi_channel=write_multi_channel,
     )
 
 
+@filter_close_seconds
 @add_rankings
 def fine_align(
     results,
     destination_path: str = None,
     write_extension: str = None,
     write_multi_channel: bool = False,
     match_index: int = 0,
@@ -235,15 +259,15 @@
             sample_rate=recognizer.config.sample_rate,
             normalize=recognizer.config.normalize,
         )
 
     max_lags_not_set = False
     if recognizer.config.max_lags is None:
         recognizer.config.max_lags = 2
-        max_lags_set = True
+        max_lags_not_set = True
     new_results = aligner._align(
         recognizer=recognizer,
         filename_list=None,
         file_dir=None,
         fine_aud_file_dict=paths_audio,
     )
     if max_lags_not_set is True:
@@ -511,14 +535,52 @@
                 print(f"{match} : {results[match]}")
         print()
         print(f"max conf is {max(max_conf_list)} : min conf is {min(min_conf_list)}")
     else:
         print("No Matches Found")
     print()
 
+def __filter_close_seconds(results: dict, close_seconds_filter: float):
+    results_iterable_keys = []
+    # all list items in against_filename dictionary values
+    len_offset_seconds = len(list(results["match_info"].values())[0]["offset_seconds"])
+    for key, value in list(results["match_info"].values())[0].items():
+        if isinstance(value, list) and len(value) == len_offset_seconds:
+            results_iterable_keys.append(key)
+    for against_dict in results["match_info"].values():
+        iter_index_pop = []
+        unfiltered_offset_seconds = []
+        if len(against_dict["offset_seconds"]) > 0:
+            unfiltered_offset_seconds.append(against_dict["offset_seconds"][0])
+        for i, val in enumerate(against_dict["offset_seconds"][1:]):
+            # values are already sorted by confidence
+            match = False
+            for unfiltered_val in unfiltered_offset_seconds:
+                if abs(abs(val) - abs(unfiltered_val)) <= close_seconds_filter:
+                    iter_index_pop.append(i+1)
+                    match = True
+                    break
+            if not match:
+                unfiltered_offset_seconds.append(val)
+        for key in results_iterable_keys:
+            temp_list = against_dict[key]
+            for i in iter_index_pop[::-1]:
+                temp_list.pop(i)
+            against_dict[key] = temp_list
+    return results
+
+def __filter_close_seconds_alignment(results: dict, close_seconds_filter: float):
+    match_keys = ["match_info"]
+    if results.get("fine_match_info") is not None:
+        match_keys += ["fine_match_info"]
+    for match_key in match_keys:
+        for value in results.get(match_key).values():
+            __filter_close_seconds(value, close_seconds_filter)
+    return results
+
 
 def recalc_shifts(
     results: dict,
     key: str = None,
     match_index: int = 0,
     fine_match_index: int = 0,
     strength_stat: str = None,
```

### Comparing `audalign-1.2.2/audalign/align/__init__.py` & `audalign-1.2.3/audalign/align/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/config/__init__.py` & `audalign-1.2.3/audalign/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
     # Filters based on confidence.
     filter_matches: typing.Optional[int] = None
 
     # Limits number of matches returned. Defaults to 30.
     match_len_filter: typing.Optional[int] = None
 
+    # if set, filters out each result if is within x seconds of a result with a stronger confidence
+    close_seconds_filter: typing.Optional[float] = None
+
     # Filters matches to only count within locality. In seconds
     # Not all recognizers have to implement locality
     locality: typing.Optional[float] = None
 
     # Decodes audio file to this sample rate
     sample_rate = 44100
```

### Comparing `audalign-1.2.2/audalign/config/correlation.py` & `audalign-1.2.3/audalign/config/correlation.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/config/correlation_spectrogram.py` & `audalign-1.2.3/audalign/config/correlation_spectrogram.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/config/fingerprint.py` & `audalign-1.2.3/audalign/config/fingerprint.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/config/visual.py` & `audalign-1.2.3/audalign/config/visual.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/datalign.py` & `audalign-1.2.3/audalign/datalign.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/filehandler.py` & `audalign-1.2.3/audalign/filehandler.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/__init__.py` & `audalign-1.2.3/audalign/recognizers/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/correcognize/__init__.py` & `audalign-1.2.3/audalign/recognizers/correcognize/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/correcognize/correcognize.py` & `audalign-1.2.3/audalign/recognizers/correcognize/correcognize.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/correcognizeSpectrogram/__init__.py` & `audalign-1.2.3/audalign/recognizers/correcognizeSpectrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py` & `audalign-1.2.3/audalign/recognizers/correcognizeSpectrogram/correcognize_spectrogram.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/fingerprint/__init__.py` & `audalign-1.2.3/audalign/recognizers/fingerprint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,18 +297,19 @@
                 self.pool.join()
 
         else:
 
             result = []
 
             for filename in filenames_to_fingerprint:
-                file_name = os.path.basename(filename)
-                if file_name in self.file_names:
-                    print(f"{file_name} already fingerprinted, continuing...")
-                    continue
+                if isinstance(filename, str): # fine alignments are tuples with offsets
+                    file_name = os.path.basename(filename)
+                    if file_name in self.file_names:
+                        print(f"{file_name} already fingerprinted, continuing...")
+                        continue
                 file_name, hashes = _fingerprint_worker_directory(filename)
                 if file_name == None:
                     continue
                 result.append([file_name, hashes])
         return result
 
     def fingerprint_file(
```

### Comparing `audalign-1.2.2/audalign/recognizers/fingerprint/fingerprinter.py` & `audalign-1.2.3/audalign/recognizers/fingerprint/fingerprinter.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/fingerprint/recognize.py` & `audalign-1.2.3/audalign/recognizers/fingerprint/recognize.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/visrecognize/__init__.py` & `audalign-1.2.3/audalign/recognizers/visrecognize/__init__.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign/recognizers/visrecognize/visrecognize.py` & `audalign-1.2.3/audalign/recognizers/visrecognize/visrecognize.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
     _calculate_comp_values = partial(
         calculate_comp_values,
         img_width=img_width,
         calc_mse=calc_mse,
     )
 
     # calculate all mse and ssim values
-    if use_multiprocessing == True and sys.platform != "linux":
+    if use_multiprocessing == True and sys.platform not in ["linux", "darwin"]:
 
         try:
             nprocesses = num_processes or multiprocessing.cpu_count()
         except NotImplementedError:
             nprocesses = 1
         else:
             nprocesses = 1 if nprocesses <= 0 else nprocesses
```

### Comparing `audalign-1.2.2/audalign.egg-info/PKG-INFO` & `audalign-1.2.3/audalign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audalign
-Version: 1.2.2
+Version: 1.2.3
 Summary: Audio Alignment and Recognition in Python
 Home-page: http://github.com/benfmiller/audalign
 Author: Ben Miller
 Author-email: benfmiller132@gmail.com
 Maintainer: Ben Miller
 Maintainer-email: benfmiller132@gmail.com
 License: MIT
```

### Comparing `audalign-1.2.2/audalign.egg-info/SOURCES.txt` & `audalign-1.2.3/audalign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/audalign.egg-info/requires.txt` & `audalign-1.2.3/audalign.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/setup.py` & `audalign-1.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         nocomments = list(filter((lambda x: not x.startswith("#")), stripped))
         # remove empty lines
         reqs = list(filter((lambda x: x), nocomments))
         return reqs
 
 
 PACKAGE_NAME = "audalign"
-PACKAGE_VERSION = "1.2.2"
+PACKAGE_VERSION = "1.2.3"
 SUMMARY = "Audio Alignment and Recognition in Python"
 
 REQUIREMENTS = parse_requirements("requirements.txt")
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

### Comparing `audalign-1.2.2/tests/test_align.py` & `audalign-1.2.3/tests/test_align.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 from audalign import recognizers
 
 test_file_eig = "test_audio/test_shifts/Eigen-20sec.mp3"
 test_file_eig2 = "test_audio/test_shifts/Eigen-song-base.mp3"
 test_folder_eig = "test_audio/test_shifts/"
 
 
+def ensure_close_seconds_filter(result, close_seconds_filter, initial_filter="match_info"):
+    for target_file in list(result.get(initial_filter).values()):
+        for against_file in list(target_file["match_info"].values()):
+            offset_list = sorted(against_file["offset_seconds"])
+            start = offset_list[0]
+            for i in offset_list[1:]:
+                assert i - start > close_seconds_filter # results within close_seconds_filter
+                start = i
+
 class TestAlign:
     fingerprint_recognizer = ad.FingerprintRecognizer(
         load_fingerprints_file="tests/test_fingerprints.json"
     )
 
     @pytest.mark.smoke
     def test_align_fingerprint(self, tmpdir):
@@ -174,14 +183,39 @@
             "test_audio/test_shifts/Eigen-song-base.mp3",
             destination_path=tmpdir,
             write_extension=".wav",
             recognizer=recognizer,
         )
         assert result is not None
 
+    @pytest.mark.xfail
+    def test_align_close_seconds_filter_fail(self, tmpdir):
+        close_seconds_filter = 10
+        recognizer = ad.FingerprintRecognizer()
+        recognizer.config.multiprocessing = False
+        result = ad.align(
+            "test_audio/test_shifts",
+            tmpdir,
+            recognizer=recognizer,
+        )
+        assert result
+        ensure_close_seconds_filter(result, close_seconds_filter)
+
+    def test_align_close_seconds_filter(self, tmpdir):
+        close_seconds_filter = 10
+        recognizer = ad.FingerprintRecognizer()
+        recognizer.config.close_seconds_filter = close_seconds_filter
+        recognizer.config.multiprocessing = False
+        result = ad.align(
+            "test_audio/test_shifts",
+            tmpdir,
+            recognizer=recognizer,
+        )
+        assert result
+        ensure_close_seconds_filter(result, close_seconds_filter)
 
 class TestTargetAlign:
     def test_target_align_vis(self, tmpdir):
         recognizer = ad.VisualRecognizer()
         recognizer.config.volume_threshold = 214
         recognizer.config.img_width = 0.5
         result = ad.target_align(
@@ -278,14 +312,15 @@
             self.align_fing_results,
             recognizer=recognizer,
         )
         assert result is not None
         recognizer.config.multiprocessing = False
         result = ad.fine_align(
             self.align_fing_results,
+            recognizer=recognizer,
         )
         assert result is not None
 
     def test_fine_align_locality(self):
         recognizer = ad.CorrelationRecognizer()
         recognizer.config.locality = 10
         result = ad.fine_align(self.align_fing_results, recognizer=recognizer)
@@ -332,14 +367,42 @@
             self.align_fing_results,
             destination_path=tmpdir,
             recognizer=recognizer,
         )
         assert result is not None
         ad.pretty_print_alignment(result, match_keys="fine_match_info")
 
+    def test_fine_align_close_seconds_filter(self):
+        close_seconds_filter = 10
+        recognizer = ad.FingerprintRecognizer(
+            load_fingerprints_file="tests/test_fingerprints.json"
+        )
+        recognizer.config.close_seconds_filter = close_seconds_filter
+        recognizer.config.multiprocessing = False
+        result = ad.fine_align(
+            self.align_fing_results,
+            recognizer=recognizer,
+        )
+        assert result is not None
+        ensure_close_seconds_filter(result, close_seconds_filter, "fine_match_info")
+
+    @pytest.mark.xfail
+    def test_fine_align_close_seconds_filter_fail(self):
+        close_seconds_filter = 10
+        recognizer = ad.FingerprintRecognizer(
+            load_fingerprints_file="tests/test_fingerprints.json"
+        )
+        recognizer.config.multiprocessing = False
+        result = ad.fine_align(
+            self.align_fing_results,
+            recognizer=recognizer,
+        )
+        assert result is not None
+        ensure_close_seconds_filter(result, close_seconds_filter, "fine_match_info")
+
     def test_fine_align_options(self, tmpdir):
         recognizer = ad.CorrelationRecognizer()
         recognizer.config.sample_rate = 8000
         recognizer.config.max_lags = 5
         recognizer.config.filter_matches = 0.1
         result = ad.fine_align(
             self.align_fing_results,
```

### Comparing `audalign-1.2.2/tests/test_audalign.py` & `audalign-1.2.3/tests/test_audalign.py`

 * *Files identical despite different names*

### Comparing `audalign-1.2.2/tests/test_recognize.py` & `audalign-1.2.3/tests/test_recognize.py`

 * *Files identical despite different names*

