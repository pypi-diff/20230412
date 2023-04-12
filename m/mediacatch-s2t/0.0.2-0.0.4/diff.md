# Comparing `tmp/mediacatch-s2t-0.0.2.tar.gz` & `tmp/mediacatch-s2t-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediacatch-s2t-0.0.2.tar", last modified: Thu Dec  1 14:53:01 2022, max compression
+gzip compressed data, was "mediacatch-s2t-0.0.4.tar", last modified: Wed Apr 12 14:49:16 2023, max compression
```

## Comparing `mediacatch-s2t-0.0.2.tar` & `mediacatch-s2t-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 suman     (1000) suman     (1000)        0 2022-12-01 14:53:01.133129 mediacatch-s2t-0.0.2/
--rw-rw-r--   0 suman     (1000) suman     (1000)    10172 2022-11-30 18:33:13.000000 mediacatch-s2t-0.0.2/LICENSE
--rw-rw-r--   0 suman     (1000) suman     (1000)       27 2022-11-28 11:03:53.000000 mediacatch-s2t-0.0.2/MANIFEST.in
--rw-rw-r--   0 suman     (1000) suman     (1000)    12910 2022-12-01 14:53:01.133129 mediacatch-s2t-0.0.2/PKG-INFO
--rw-rw-r--   0 suman     (1000) suman     (1000)      795 2022-12-01 08:52:40.000000 mediacatch-s2t-0.0.2/README.md
--rw-rw-r--   0 suman     (1000) suman     (1000)      898 2022-12-01 14:52:00.000000 mediacatch-s2t-0.0.2/pyproject.toml
--rw-rw-r--   0 suman     (1000) suman     (1000)       38 2022-12-01 14:53:01.133129 mediacatch-s2t-0.0.2/setup.cfg
-drwxrwxr-x   0 suman     (1000) suman     (1000)        0 2022-12-01 14:53:01.133129 mediacatch-s2t-0.0.2/src/
-drwxrwxr-x   0 suman     (1000) suman     (1000)        0 2022-12-01 14:53:01.133129 mediacatch-s2t-0.0.2/src/mediacatch_s2t/
--rw-rw-r--   0 suman     (1000) suman     (1000)      508 2022-12-01 14:51:26.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t/__init__.py
--rw-rw-r--   0 suman     (1000) suman     (1000)     1181 2022-11-30 18:33:13.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t/__main__.py
--rw-rw-r--   0 suman     (1000) suman     (1000)     4667 2022-11-30 18:33:13.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t/uploader.py
-drwxrwxr-x   0 suman     (1000) suman     (1000)        0 2022-12-01 14:53:01.133129 mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/
--rw-rw-r--   0 suman     (1000) suman     (1000)    12910 2022-12-01 14:53:01.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/PKG-INFO
--rw-rw-r--   0 suman     (1000) suman     (1000)      391 2022-12-01 14:53:01.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/SOURCES.txt
--rw-rw-r--   0 suman     (1000) suman     (1000)        1 2022-12-01 14:53:01.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/dependency_links.txt
--rw-rw-r--   0 suman     (1000) suman     (1000)       54 2022-12-01 14:53:01.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/entry_points.txt
--rw-rw-r--   0 suman     (1000) suman     (1000)       80 2022-12-01 14:53:01.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/requires.txt
--rw-rw-r--   0 suman     (1000) suman     (1000)       15 2022-12-01 14:53:01.000000 mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/top_level.txt
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    10172 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/LICENSE
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       27 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/MANIFEST.in
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/PKG-INFO
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      795 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/README.md
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      898 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/pyproject.toml
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       38 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/setup.cfg
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/src/
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/src/mediacatch_s2t/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      546 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t/__init__.py
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     1181 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t/__main__.py
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     5622 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t/uploader.py
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/PKG-INFO
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      414 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/SOURCES.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)        1 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/dependency_links.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       54 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/entry_points.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       80 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/requires.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       15 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/top_level.txt
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/tests/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     2447 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/tests/test_uploader.py
```

### Comparing `mediacatch-s2t-0.0.2/LICENSE` & `mediacatch-s2t-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.2/PKG-INFO` & `mediacatch-s2t-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.2
+Version: 0.0.4
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mediacatch-s2t-0.0.2/README.md` & `mediacatch-s2t-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.2/pyproject.toml` & `mediacatch-s2t-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mediacatch-s2t"
-version = "0.0.2"
+version = "0.0.4"
 description = "Upload a media file and get the transcription link."
 readme = "README.md"
 authors = [{ name = "MediaCatch", email = "support@mediacatch.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mediacatch-s2t-0.0.2/src/mediacatch_s2t/__main__.py` & `mediacatch-s2t-0.0.4/src/mediacatch_s2t/__main__.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.2/src/mediacatch_s2t/uploader.py` & `mediacatch-s2t-0.0.4/src/mediacatch_s2t/uploader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import json
 import os
 import pathlib
 
-import pymediainfo
 import requests
+import subprocess
+import json
+from typing import NamedTuple
+
 
 from mediacatch_s2t import (
-    PRESIGNED_URL, TRANSCRIPT_URL, UPDATE_STATUS_URL, PROCESSING_TIME_RATIO
+    URL, PRESIGNED_ENDPOINT, TRANSCRIPT_ENDPOINT, UPDATE_STATUS_ENDPOINT, PROCESSING_TIME_RATIO
 )
 
+class FFProbeResult(NamedTuple):
+    return_code: int
+    json: str
+    error: str
 
 class UploaderException(Exception):
     pass
 
 
 class Uploader:
     def __init__(self, file, api_key):
@@ -38,43 +45,59 @@
                 raise Exception(msg)
             return response
         except Exception as e:
             raise UploaderException(str(e))
 
     @property
     def _transcript_link(self):
-        return f"{TRANSCRIPT_URL}?id={self.file_id}&api_key={self.api_key}"
+        return f"{URL}{TRANSCRIPT_ENDPOINT}?id={self.file_id}&api_key={self.api_key}"
+
+    @staticmethod
+    def _ffprobe(file_path) -> FFProbeResult:
+        command_array = ["ffprobe",
+                        "-v", "quiet",
+                        "-print_format", "json",
+                        "-show_format",
+                        "-show_streams",
+                        file_path]
+        result = subprocess.run(command_array, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
+        return FFProbeResult(return_code=result.returncode,
+                            json=json.loads(result.stdout),
+                            error=result.stderr)
 
     def get_duration(self):
         """Get audio track duration of a file.
 
         :return
-        tuple: (bool, duration_in_miliseconds)
+        tuple: (duration_in_miliseconds, stream_json | error_msg)
         """
         try:
-            mi = pymediainfo.MediaInfo.parse(self.file)
-            if not mi.audio_tracks:
-                return True, 0
-            return True, mi.audio_tracks[0].duration
-        except OSError:
-            return False, 0
-        except Exception:
-            return False, 0
+            probe = self._ffprobe(self.file)
+            if probe.return_code:
+                return 0, probe.error
+            else:
+                for stream in probe.json['streams']:
+                    if stream['codec_type'] == 'audio':
+                        return int(float(stream['duration']) * 1000), stream
+                else:
+                    return 0, "The file doesn't have an audio track"
+        except OSError as e:
+            return 0, 'FFmpeg not installed (sudo apt install ffmpeg)'
 
     def estimated_result_time(self, audio_length=0):
         """Estimated processing time in seconds"""
 
         if not isinstance(audio_length, int):
             return 0
         processing_time = PROCESSING_TIME_RATIO * audio_length
         return round(processing_time / 1000)
 
     def _get_upload_url(self, mime_file):
         response = self._make_post_request(
-            url=PRESIGNED_URL,
+            url=f'{URL}{PRESIGNED_ENDPOINT}',
             json=mime_file,
             headers={
                 "Content-type": 'application/json',
                 "X-API-KEY": self.api_key
             }
         )
         response_data = json.loads(response.text)
@@ -94,15 +117,15 @@
                 data=data,
                 files={'file': f}
             )
             return response
 
     def _get_transcript_link(self):
         self._make_post_request(
-            url=UPDATE_STATUS_URL,
+            url=f'{URL}{UPDATE_STATUS_ENDPOINT}',
             json={"id": self.file_id},
             headers={
                 "Content-type": 'application/json',
                 "X-API-KEY": self.api_key
             }
         )
         return self._transcript_link
@@ -115,18 +138,18 @@
             "message": ""
         }
         if not self._is_file_exist():
             result["status"] = "error"
             result["message"] = "The file doesn't exist"
             return result
 
-        is_having_duration, file_duration = self.get_duration()
-        if is_having_duration and not file_duration:
+        file_duration, msg = self.get_duration()
+        if not file_duration:
             result["status"] = "error"
-            result["message"] = "The file doesn't have an audio track"
+            result["message"] = msg
             return result
 
         mime_file = {
             "duration": file_duration,
             "filename": pathlib.Path(self.file).name,
             "file_ext": pathlib.Path(self.file).suffix,
             "filesize": os.path.getsize(self.file),
```

### Comparing `mediacatch-s2t-0.0.2/src/mediacatch_s2t.egg-info/PKG-INFO` & `mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.2
+Version: 0.0.4
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

