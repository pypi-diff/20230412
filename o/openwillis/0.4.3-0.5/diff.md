# Comparing `tmp/openwillis-0.4.3.tar.gz` & `tmp/openwillis-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-0.4.3.tar", last modified: Sun Apr  9 12:20:21 2023, max compression
+gzip compressed data, was "openwillis-0.5.tar", last modified: Wed Apr 12 18:35:38 2023, max compression
```

## Comparing `openwillis-0.4.3.tar` & `openwillis-0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    13641 2023-04-09 12:18:45.000000 openwillis-0.4.3/LICENSE.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      205 2023-04-09 12:18:45.000000 openwillis-0.4.3/MANIFEST.in
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1115 2023-04-09 12:20:21.321899 openwillis-0.4.3/PKG-INFO
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      814 2023-04-09 12:18:45.000000 openwillis-0.4.3/README.md
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-09 12:18:45.000000 openwillis-0.4.3/RELEASE.md
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      469 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/features/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      373 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/api.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/features/audio/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      103 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/audio/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    15820 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/audio/acoustic.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis/features/audio/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      706 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/audio/config/acoustic.json
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/speech/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      346 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     2388 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/aws_transcribe.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/speech/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1593 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/config/speech.json
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     6061 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/speech_attribute.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     7234 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/speech_separation.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     9148 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/speech_transcribe.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    30695 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/speech/util.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/video/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.321899 openwillis-0.4.3/openwillis/features/video/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      185 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/config/facial.json
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    16067 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/face_landmark.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    10471 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/features/video/facial_emotion.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      145 2023-04-09 12:18:45.000000 openwillis-0.4.3/openwillis/usability.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-09 12:20:21.311899 openwillis-0.4.3/openwillis.egg-info/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1115 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/PKG-INFO
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      989 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/SOURCES.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/dependency_links.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/not-zip-safe
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      372 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/requires.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       11 2023-04-09 12:20:21.000000 openwillis-0.4.3/openwillis.egg-info/top_level.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      385 2023-04-09 12:18:45.000000 openwillis-0.4.3/requirements.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       79 2023-04-09 12:20:21.321899 openwillis-0.4.3/setup.cfg
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      936 2023-04-09 12:19:12.000000 openwillis-0.4.3/setup.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    13641 2023-04-12 18:35:17.000000 openwillis-0.5/LICENSE.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      205 2023-04-12 18:35:17.000000 openwillis-0.5/MANIFEST.in
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-12 18:35:38.447394 openwillis-0.5/PKG-INFO
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      814 2023-04-12 18:35:17.000000 openwillis-0.5/README.md
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-12 18:35:17.000000 openwillis-0.5/RELEASE.md
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      469 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/__init__.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      373 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/api.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/audio/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      103 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/audio/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    15855 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/audio/acoustic.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/audio/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      706 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/audio/config/acoustic.json
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/speech/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      346 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/__init__.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     2388 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/aws_transcribe.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/speech/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1593 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/config/speech.json
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     6061 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/speech_attribute.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     7234 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/speech_separation.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     9148 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/speech_transcribe.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    30695 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/speech/util.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/video/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/__init__.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis/features/video/config/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      185 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/config/facial.json
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    16067 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/face_landmark.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    10471 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/features/video/facial_emotion.py
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      145 2023-04-12 18:35:17.000000 openwillis-0.5/openwillis/usability.py
+drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-12 18:35:38.447394 openwillis-0.5/openwillis.egg-info/
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/PKG-INFO
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      989 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/not-zip-safe
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      372 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/requires.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       11 2023-04-12 18:35:38.000000 openwillis-0.5/openwillis.egg-info/top_level.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      385 2023-04-12 18:35:17.000000 openwillis-0.5/requirements.txt
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       79 2023-04-12 18:35:38.447394 openwillis-0.5/setup.cfg
+-rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      934 2023-04-12 18:35:17.000000 openwillis-0.5/setup.py
```

### Comparing `openwillis-0.4.3/LICENSE.txt` & `openwillis-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/PKG-INFO` & `openwillis-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 0.4.3
+Version: 0.5
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6.*
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-0.4.3/README.md` & `openwillis-0.5/README.md`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/audio/acoustic.py` & `openwillis-0.5/openwillis/features/audio/acoustic.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,14 +235,16 @@
 
     for i in range(4):
         formant_values = call(formant, "To Matrix", i+1).values[0,:]
         formant_dict['form' + str(i+1) + 'freq'] = list(formant_values)
 
     cols = [measures['form1freq'], measures['form2freq'], measures['form3freq'], measures['form4freq']]
     df_formant = pd.DataFrame(formant_dict)
+    
+    df_formant.columns = cols
     return df_formant
 
 def loudness(sound, measures):
     """
     ------------------------------------------------------------------------------------------------------
 
     Calculates the audio intensity of an audio file.
@@ -459,15 +461,15 @@
         df_shimmer = shimmer(sound, measures)
 
         df_hnr = harmonic_ratio(sound, measures)
         df_gne = glottal_ratio(sound, measures)
         df_formant = formfreq(sound, measures)
         df_silence = get_voice_silence(audio_path, 500, measures)
 
-        framewise = pd.concat([df_pitch, df_loudness, df_hnr, df_formant], axis=1)
+        framewise = pd.concat([df_pitch, df_formant, df_loudness, df_hnr], axis=1)
         sig_df = pd.concat([df_jitter, df_shimmer, df_gne], axis=1)
 
         df_summary = get_summary(sound, framewise, sig_df, df_silence, measures)
         return framewise, df_silence, df_summary
 
     except Exception as e:
         logger.error(f'Error in acoustic calculation- file: {audio_path} & Error: {e}')
```

### Comparing `openwillis-0.4.3/openwillis/features/audio/config/acoustic.json` & `openwillis-0.5/openwillis/features/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/speech/aws_transcribe.py` & `openwillis-0.5/openwillis/features/speech/aws_transcribe.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/speech/config/speech.json` & `openwillis-0.5/openwillis/features/speech/config/speech.json`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/speech/speech_attribute.py` & `openwillis-0.5/openwillis/features/speech/speech_attribute.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/speech/speech_separation.py` & `openwillis-0.5/openwillis/features/speech/speech_separation.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/speech/speech_transcribe.py` & `openwillis-0.5/openwillis/features/speech/speech_transcribe.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/speech/util.py` & `openwillis-0.5/openwillis/features/speech/util.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/video/face_landmark.py` & `openwillis-0.5/openwillis/features/video/face_landmark.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis/features/video/facial_emotion.py` & `openwillis-0.5/openwillis/features/video/facial_emotion.py`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/openwillis.egg-info/PKG-INFO` & `openwillis-0.5/openwillis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 0.4.3
+Version: 0.5
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6.*
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-0.4.3/openwillis.egg-info/SOURCES.txt` & `openwillis-0.5/openwillis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwillis-0.4.3/setup.py` & `openwillis-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='0.4.3',
+                 version='0.5',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
                  python_requires='>=3.6.*',
                  install_requires=install_requires,
```

