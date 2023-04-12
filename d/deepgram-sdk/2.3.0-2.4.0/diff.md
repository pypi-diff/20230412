# Comparing `tmp/deepgram-sdk-2.3.0.tar.gz` & `tmp/deepgram-sdk-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram-sdk-2.3.0.tar", last modified: Mon Jan 30 16:55:26 2023, max compression
+gzip compressed data, was "deepgram-sdk-2.4.0.tar", last modified: Wed Apr 12 15:19:21 2023, max compression
```

## Comparing `deepgram-sdk-2.3.0.tar` & `deepgram-sdk-2.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 16:55:26.001306 deepgram-sdk-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-01-30 16:55:26.001306 deepgram-sdk-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 16:55:26.001306 deepgram-sdk-2.3.0/deepgram/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/deepgram/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 16:55:26.001306 deepgram-sdk-2.3.0/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-01-30 16:55:25.000000 deepgram-sdk-2.3.0/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-30 16:55:25.000000 deepgram-sdk-2.3.0/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 16:55:25.000000 deepgram-sdk-2.3.0/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-30 16:55:25.000000 deepgram-sdk-2.3.0/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-30 16:55:25.000000 deepgram-sdk-2.3.0/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 16:55:26.001306 deepgram-sdk-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-01-30 16:55:06.000000 deepgram-sdk-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:19:21.524349 deepgram-sdk-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-12 15:19:21.520349 deepgram-sdk-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:19:21.520349 deepgram-sdk-2.4.0/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/deepgram/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:19:21.520349 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 15:19:21.000000 deepgram-sdk-2.4.0/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:19:21.524349 deepgram-sdk-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-12 15:19:03.000000 deepgram-sdk-2.4.0/setup.py
```

### Comparing `deepgram-sdk-2.3.0/LICENSE` & `deepgram-sdk-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/PKG-INFO` & `deepgram-sdk-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 2.3.0
+Version: 2.4.0
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Luca Todd
 Author-email: luca.todd@deepgram.com
 License: MIT
 Keywords: deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-2.3.0/README.md` & `deepgram-sdk-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/__init__.py` & `deepgram-sdk-2.4.0/deepgram/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/_types.py` & `deepgram-sdk-2.4.0/deepgram/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 })
 Keyword = Union[str, BoostedKeyword]
 
 
 class TranscriptionOptions(TypedDict, total=False):
     # References for the different meanings and values of these properties
     # can be found in the Deepgram docs:
-    # https://developers.deepgram.com/api-reference/speech-recognition-api#operation/transcribeAudio
-    # https://developers.deepgram.com/api-reference/speech-recognition-api#operation/transcribeStreamingAudio
+    # https://developers.deepgram.com/documentation/features/
     model: str
     version: str
     language: str
     punctuate: bool
     profanity_filter: bool
     redact: List[str]
     diarize: Literal['false', 'true']
@@ -75,36 +74,38 @@
     dates: bool
     date_format: str
     times: bool
     dictation: bool
     measurements: bool
     smart_format: bool
     replace: str
+    tag: List[str]
 
 
 class PrerecordedOptions(TranscriptionOptions, total=False):
     # References for the different meanings and values of these properties
     # can be found in the Deepgram docs:
-    # https://developers.deepgram.com/api-reference/speech-recognition-api#operation/transcribeAudio
+    # https://developers.deepgram.com/documentation/features/
     utterances: bool
     utt_split: float
     detect_entities: bool
     summarize: bool
     paragraphs: bool
     detect_language: bool
     detect_topics: bool
     translate: List[str]
     analyze_sentiment: bool
+    sentiment: bool
     sentiment_threshold: float
 
 
 class LiveOptions(TranscriptionOptions, total=False):
     # References for the different meanings and values of these properties
     # can be found in the Deepgram docs:
-    # https://developers.deepgram.com/api-reference/speech-recognition-api#operation/transcribeStreamingAudio
+    # https://developers.deepgram.com/documentation/features/
     interim_results: bool
     endpointing: bool
     vad_turnoff: int
     encoding: str
     channels: int
     sample_rate: int
```

### Comparing `deepgram-sdk-2.3.0/deepgram/_utils.py` & `deepgram-sdk-2.4.0/deepgram/_utils.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/billing.py` & `deepgram-sdk-2.4.0/deepgram/billing.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/invitations.py` & `deepgram-sdk-2.4.0/deepgram/invitations.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/keys.py` & `deepgram-sdk-2.4.0/deepgram/keys.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 from ._types import Options, Key, KeyResponse
 from ._utils import _request
-
+import datetime
 
 class Keys:
     _root = "/projects"
 
     def __init__(self, options: Options) -> None:
         self.options = options
 
@@ -18,20 +18,20 @@
     async def get(self, project_id: str, key: str) -> Key:
         """Retrieves a specific key associated with the provided projectId."""
         return await _request(
             f'{self._root}/{project_id}/keys/{key}', self.options
         )
 
     async def create(
-        self, project_id: str, comment: str, scopes: List[str]
+        self, project_id: str, comment: str, scopes: List[str], tags: List[str], expiration_date: datetime, time_to_live_in_seconds: int
     ) -> Key:
         """Creates an API key with the provided scopes."""
         return await _request(
             f'{self._root}/{project_id}/keys', self.options,
-            method='POST', payload={'comment': comment, 'scopes': scopes},
+            method='POST', payload={'comment': comment, 'scopes': scopes, 'tags': tags, 'expiration_date': expiration_date, 'time_to_live_in_seconds': time_to_live_in_seconds},
             headers={'Content-Type': 'application/json'}
         )
 
     async def delete(self, project_id: str, key: str) -> None:
         """Deletes an API key."""
         await _request(
             f'{self._root}/{project_id}/keys/{key}', self.options,
```

### Comparing `deepgram-sdk-2.3.0/deepgram/members.py` & `deepgram-sdk-2.4.0/deepgram/members.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/projects.py` & `deepgram-sdk-2.4.0/deepgram/projects.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/scopes.py` & `deepgram-sdk-2.4.0/deepgram/scopes.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/transcription.py` & `deepgram-sdk-2.4.0/deepgram/transcription.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram/usage.py` & `deepgram-sdk-2.4.0/deepgram/usage.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-2.3.0/deepgram_sdk.egg-info/PKG-INFO` & `deepgram-sdk-2.4.0/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 2.3.0
+Version: 2.4.0
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Luca Todd
 Author-email: luca.todd@deepgram.com
 License: MIT
 Keywords: deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-2.3.0/setup.py` & `deepgram-sdk-2.4.0/setup.py`

 * *Files identical despite different names*

