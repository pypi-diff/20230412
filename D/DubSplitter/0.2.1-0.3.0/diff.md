# Comparing `tmp/DubSplitter-0.2.1.tar.gz` & `tmp/DubSplitter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DubSplitter-0.2.1.tar", last modified: Sat Apr  8 10:08:39 2023, max compression
+gzip compressed data, was "DubSplitter-0.3.0.tar", last modified: Wed Apr 12 01:29:10 2023, max compression
```

## Comparing `DubSplitter-0.2.1.tar` & `DubSplitter-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 10:08:39.143252 DubSplitter-0.2.1/
-drwxrwxrwx   0        0        0        0 2023-04-08 10:08:39.137066 DubSplitter-0.2.1/DubSplitter.egg-info/
--rw-rw-rw-   0        0        0     3402 2023-04-08 10:08:38.000000 DubSplitter-0.2.1/DubSplitter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-04-08 10:08:38.000000 DubSplitter-0.2.1/DubSplitter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 10:08:38.000000 DubSplitter-0.2.1/DubSplitter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-08 10:08:38.000000 DubSplitter-0.2.1/DubSplitter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 00:03:48.000000 DubSplitter-0.2.1/DubSplitter.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-04-08 10:08:38.000000 DubSplitter-0.2.1/DubSplitter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-08 10:08:38.000000 DubSplitter-0.2.1/DubSplitter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3402 2023-04-08 10:08:39.143252 DubSplitter-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-08 10:08:39.138672 DubSplitter-0.2.1/dubSplitter/
--rw-rw-rw-   0        0        0        0 2023-04-07 01:02:52.000000 DubSplitter-0.2.1/dubSplitter/__init__.py
--rw-rw-rw-   0        0        0     1592 2023-04-08 09:43:34.000000 DubSplitter-0.2.1/dubSplitter/constants.py
--rw-rw-rw-   0        0        0     3162 2023-04-08 10:07:21.000000 DubSplitter-0.2.1/dubSplitter/dubSplitter.py
-drwxrwxrwx   0        0        0        0 2023-04-08 10:08:39.141986 DubSplitter-0.2.1/dubSplitter/functions/
--rw-rw-rw-   0        0        0        0 2023-04-07 01:03:14.000000 DubSplitter-0.2.1/dubSplitter/functions/__init__.py
--rw-rw-rw-   0        0        0      130 2023-04-08 09:55:32.000000 DubSplitter-0.2.1/dubSplitter/functions/exitWithInfo.py
--rw-rw-rw-   0        0        0      628 2023-04-07 01:33:33.000000 DubSplitter-0.2.1/dubSplitter/functions/path.py
--rw-rw-rw-   0        0        0     1556 2023-04-08 10:07:55.000000 DubSplitter-0.2.1/dubSplitter/functions/slicer.py
--rw-rw-rw-   0        0        0      399 2023-04-07 00:58:45.000000 DubSplitter-0.2.1/dubSplitter/functions/stringEx.py
--rw-rw-rw-   0        0        0     2887 2023-04-08 10:00:57.000000 DubSplitter-0.2.1/dubSplitter/functions/voiceRecognition.py
--rw-rw-rw-   0        0        0       42 2023-04-08 10:08:39.143252 DubSplitter-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-04-07 13:18:37.000000 DubSplitter-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.323684 DubSplitter-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.316105 DubSplitter-0.3.0/DubSplitter.egg-info/
+-rw-rw-rw-   0        0        0     6158 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-07 00:03:48.000000 DubSplitter-0.3.0/DubSplitter.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 01:29:10.000000 DubSplitter-0.3.0/DubSplitter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6158 2023-04-12 01:29:10.323684 DubSplitter-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.318110 DubSplitter-0.3.0/dubSplitter/
+-rw-rw-rw-   0        0        0        0 2023-04-07 01:02:52.000000 DubSplitter-0.3.0/dubSplitter/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-04-12 01:10:41.000000 DubSplitter-0.3.0/dubSplitter/constants.py
+-rw-rw-rw-   0        0        0     5084 2023-04-12 01:25:22.000000 DubSplitter-0.3.0/dubSplitter/dubSplitter.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:29:10.322276 DubSplitter-0.3.0/dubSplitter/functions/
+-rw-rw-rw-   0        0        0        0 2023-04-07 01:03:14.000000 DubSplitter-0.3.0/dubSplitter/functions/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-04-08 09:55:32.000000 DubSplitter-0.3.0/dubSplitter/functions/exitWithInfo.py
+-rw-rw-rw-   0        0        0      630 2023-04-12 00:43:28.000000 DubSplitter-0.3.0/dubSplitter/functions/path.py
+-rw-rw-rw-   0        0        0     3772 2023-04-12 01:25:45.000000 DubSplitter-0.3.0/dubSplitter/functions/slicer.py
+-rw-rw-rw-   0        0        0      445 2023-04-11 15:43:19.000000 DubSplitter-0.3.0/dubSplitter/functions/stringEx.py
+-rw-rw-rw-   0        0        0     3478 2023-04-12 01:22:36.000000 DubSplitter-0.3.0/dubSplitter/functions/voiceRecognition.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 01:29:10.323684 DubSplitter-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1345 2023-04-12 01:28:25.000000 DubSplitter-0.3.0/setup.py
```

### Comparing `DubSplitter-0.2.1/DubSplitter.egg-info/SOURCES.txt` & `DubSplitter-0.3.0/DubSplitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DubSplitter-0.2.1/dubSplitter/constants.py` & `DubSplitter-0.3.0/dubSplitter/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,18 +38,23 @@
 
     tempFile = tempPath + 'temp.wav'
 
     # print("default output path {}".format(defaultOutPath))
     # print("temp path {}".format(tempPath))
 
 
+defaultWhisperPrompt = '简体中文'
 defaultWhisperLanguage = 'Chinese'
 
 defaultWhisperModel = 'base'
 whisperModel = Enum('WhisperModel',
                     (
                         'tiny',
                         'base',
                         'small',
                         'medium',
                         'large',
                     ))
+
+defaultOutputFormat = 'ogg'
+defaultFileNameFormat = '{2:0>4d}_{3:0>8d}.{1}'
+defaultFileNameVRFormat = '{2:0>4d}_{3:0>8d}_{5}.{1}'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DubSplitter-0.2.1/dubSplitter/functions/path.py` & `DubSplitter-0.3.0/dubSplitter/functions/path.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     bExist = os.path.exists(path)
 
     if not bExist:
         os.makedirs(path)
 
 
 def invalid_file_character_escape(file):
-    invalidChar = ['\\', '/', '*', '?', '<', '>', '|']
+    invalidChars = ['\\', '/', '*', '?', '<', '>', '|']
     fileStr: str = file
 
-    for char in invalidChar:
+    for char in invalidChars:
         fileStr = fileStr.replace(char, '_')
 
     return fileStr
 
 
 def user_path():
     return os.path.expanduser('~')
```

### Comparing `DubSplitter-0.2.1/dubSplitter/functions/voiceRecognition.py` & `DubSplitter-0.3.0/dubSplitter/functions/voiceRecognition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,98 @@
 """
 voice recognition
 """
+from colorama import Fore, Style
 
 '''
 whisper import
 '''
 
 import whisper
 from whisper import Whisper
 
-from ..constants import whisperModel, defaultWhisperModel, defaultWhisperLanguage
+from ..constants import whisperModel, defaultWhisperModel, defaultWhisperLanguage, defaultWhisperPrompt
 
 '''
 speech_recognition import
 '''
 
 '''
 import speech_recognition as sr
 from pydub import AudioSegment
 
 from functions.path import mkdir
 from constants import tempPath, tempFile
 '''
 
 model: Whisper | None = None
+modelPrompt: str = defaultWhisperPrompt
 modelLanguage: str = defaultWhisperLanguage
 
 '''
 use whisper
 
 https://github.com/openai/whisper
 '''
 
 
+# prompt
+# https://platform.openai.com/docs/guides/speech-to-text/prompting
+# https://github.com/openai/whisper/discussions/355
+# https://github.com/openai/whisper/discussions/277
+def update_model_prompt(prompt):
+    global modelPrompt
+    modelPrompt = prompt
+
+    print(Fore.WHITE + Style.DIM + '  recognize prompt {}'.format(prompt))
+
+
 def update_model_language(lang):
     global modelLanguage
     modelLanguage = lang
 
-    print('recognize in language {}'.format(lang))
+    print(Fore.WHITE + Style.DIM + '  recognize in language {}'.format(lang))
 
 
 def get_whisper_model(model_name):
     for name, member in whisperModel.__members__.items():
         if model_name.lower() == name:
             return model_name.lower()
 
-    print('given model name not found, use \'base\' instead')
+    print(Fore.RED + '  given model name not found, use \'base\' instead')
 
     return defaultWhisperModel
 
 
 def update_whisper_model(model_name):
     global model
 
     # Model path (Windows)
     # C:\Users\[UserName]\.cache\whisper
     # Download links:
     # https://github.com/openai/whisper/discussions/63#discussioncomment-3798552
     actual_model_name = get_whisper_model(model_name)
 
-    print('loading voice recognition model {}'.format(actual_model_name))
+    print(Fore.WHITE + Style.DIM + '  loading voice recognition model {}'.format(actual_model_name))
     model = whisper.load_model(actual_model_name)
-    print('load complete')
+    print(Fore.WHITE + Style.DIM + '  load complete')
 
 
 def recognition_with_whisper(file):
     # model = whisper.load_model("base")
     # result = model.transcribe(file)
 
     if model is None:
         return 'InvalidModel'
 
     # Update options here
-    # result = model.transcribe(file, fp16=False, language='Chinese')
-    result = model.transcribe(file, fp16=False, language=modelLanguage)
+    result = model.transcribe(file,
+                              fp16=False,
+                              language=modelLanguage,
+                              initial_prompt=modelPrompt)
     # print(result["text"])
 
     return result["text"]
 
 
 '''
 use speech_recognition (google)
```

### Comparing `DubSplitter-0.2.1/setup.py` & `DubSplitter-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 from dubSplitter.dubSplitter import VERSION
 
-with open('ReadMe.md') as f:
+with open('ReadMe.md', encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='DubSplitter',
     version=VERSION,
     author='defisym',
     author_email='defisym@outlook.com',
@@ -20,14 +20,15 @@
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'sympy',
         'pydub',
         'openai-whisper',
+        'colorama',
     ],
     entry_points={
         'console_scripts': [
             'DubSplitter = dubSplitter.dubSplitter:main'
         ]
     },
     classifiers=[
```

