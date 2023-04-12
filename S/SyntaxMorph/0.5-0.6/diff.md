# Comparing `tmp/SyntaxMorph-0.5.tar.gz` & `tmp/SyntaxMorph-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SyntaxMorph-0.5.tar", last modified: Wed Apr 12 19:04:01 2023, max compression
+gzip compressed data, was "SyntaxMorph-0.6.tar", last modified: Wed Apr 12 19:09:00 2023, max compression
```

## Comparing `SyntaxMorph-0.5.tar` & `SyntaxMorph-0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:04:01.480654 SyntaxMorph-0.5/
--rw-r--r--   0 root         (0) root         (0)     1235 2023-04-12 19:04:01.476654 SyntaxMorph-0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:04:01.472654 SyntaxMorph-0.5/SyntaxMorph.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     1235 2023-04-12 19:04:01.000000 SyntaxMorph-0.5/SyntaxMorph.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      314 2023-04-12 19:04:01.000000 SyntaxMorph-0.5/SyntaxMorph.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-12 19:04:01.000000 SyntaxMorph-0.5/SyntaxMorph.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:00:57.000000 SyntaxMorph-0.5/SyntaxMorph.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)        7 2023-04-12 19:04:01.000000 SyntaxMorph-0.5/SyntaxMorph.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        6 2023-04-12 19:04:01.000000 SyntaxMorph-0.5/SyntaxMorph.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:04:01.476654 SyntaxMorph-0.5/morph/
--rw-rw-r--   0 root         (0) root         (0)     2249 2023-04-12 18:29:35.000000 SyntaxMorph-0.5/morph/columDetect.py
--rw-rw-r--   0 root         (0) root         (0)     1995 2023-04-12 18:13:50.000000 SyntaxMorph-0.5/morph/formatCode.py
--rw-rw-r--   0 root         (0) root         (0)     3650 2023-04-12 18:59:08.000000 SyntaxMorph-0.5/morph/languageDetect.py
--rw-rw-r--   0 root         (0) root         (0)      808 2023-04-12 18:39:46.000000 SyntaxMorph-0.5/morph/main.py
--rw-rw-r--   0 root         (0) root         (0)     5999 2023-04-12 18:29:42.000000 SyntaxMorph-0.5/morph/translate.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 19:04:01.480654 SyntaxMorph-0.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1419 2023-04-12 19:03:30.000000 SyntaxMorph-0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:09:00.056418 SyntaxMorph-0.6/
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-04-12 19:09:00.056418 SyntaxMorph-0.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4900 2023-04-12 18:50:37.000000 SyntaxMorph-0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:09:00.056418 SyntaxMorph-0.6/SyntaxMorph.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     1235 2023-04-12 19:09:00.000000 SyntaxMorph-0.6/SyntaxMorph.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      325 2023-04-12 19:09:00.000000 SyntaxMorph-0.6/SyntaxMorph.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-12 19:09:00.000000 SyntaxMorph-0.6/SyntaxMorph.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:00:57.000000 SyntaxMorph-0.6/SyntaxMorph.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)        7 2023-04-12 19:09:00.000000 SyntaxMorph-0.6/SyntaxMorph.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-04-12 19:09:00.000000 SyntaxMorph-0.6/SyntaxMorph.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:09:00.056418 SyntaxMorph-0.6/morph/
+-rw-rw-r--   0 root         (0) root         (0)     2220 2023-04-12 19:08:41.000000 SyntaxMorph-0.6/morph/columDetect.py
+-rw-rw-r--   0 root         (0) root         (0)     1995 2023-04-12 18:13:50.000000 SyntaxMorph-0.6/morph/formatCode.py
+-rw-rw-r--   0 root         (0) root         (0)     3608 2023-04-12 19:08:39.000000 SyntaxMorph-0.6/morph/languageDetect.py
+-rw-rw-r--   0 root         (0) root         (0)      808 2023-04-12 18:39:46.000000 SyntaxMorph-0.6/morph/main.py
+-rw-rw-r--   0 root         (0) root         (0)     5969 2023-04-12 19:08:50.000000 SyntaxMorph-0.6/morph/translate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 19:09:00.056418 SyntaxMorph-0.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1419 2023-04-12 19:08:56.000000 SyntaxMorph-0.6/setup.py
```

### Comparing `SyntaxMorph-0.5/PKG-INFO` & `SyntaxMorph-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SyntaxMorph
-Version: 0.5
+Version: 0.6
 Summary: SyntaxMorph is a Python module that enables code conversion between different programming languages
 Home-page: https://github.com/Enderjua/SyntaxMorph
 Author: Marijua
 Author-email: enderjua@gmail.com
 License: UNKNOWN
 Description: 
         SyntaxMorph is a Python module that enables code conversion between different programming languages using the OpenAI API. It uses advanced deep learning algorithms to ensure that the functionality and structural integrity of the code are preserved during the conversion process. Users simply need to provide the source code and the target programming language to SyntaxMorph, and it automatically analyzes and converts the code to the target language.
```

### Comparing `SyntaxMorph-0.5/SyntaxMorph.egg-info/PKG-INFO` & `SyntaxMorph-0.6/SyntaxMorph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SyntaxMorph
-Version: 0.5
+Version: 0.6
 Summary: SyntaxMorph is a Python module that enables code conversion between different programming languages
 Home-page: https://github.com/Enderjua/SyntaxMorph
 Author: Marijua
 Author-email: enderjua@gmail.com
 License: UNKNOWN
 Description: 
         SyntaxMorph is a Python module that enables code conversion between different programming languages using the OpenAI API. It uses advanced deep learning algorithms to ensure that the functionality and structural integrity of the code are preserved during the conversion process. Users simply need to provide the source code and the target programming language to SyntaxMorph, and it automatically analyzes and converts the code to the target language.
```

### Comparing `SyntaxMorph-0.5/morph/columDetect.py` & `SyntaxMorph-0.6/morph/columDetect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import openai
 
-openai.api_key = "OPENAI-KEY"
+
 code = """
 (ns example
   (:gen-class))
 
 (defn factors [n]
   " Find the proper factors of a number "
   (into (sorted-set)
```

### Comparing `SyntaxMorph-0.5/morph/formatCode.py` & `SyntaxMorph-0.6/morph/formatCode.py`

 * *Files identical despite different names*

### Comparing `SyntaxMorph-0.5/morph/languageDetect.py` & `SyntaxMorph-0.6/morph/languageDetect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import openai
 
-key = "OPENAI-KEY"
-
-openai.api_key = key
-
 
 code = """
 (ns example
   (:gen-class))
 
 (defn factors [n]
   " Find the proper factors of a number "
```

### Comparing `SyntaxMorph-0.5/morph/main.py` & `SyntaxMorph-0.6/morph/main.py`

 * *Files identical despite different names*

### Comparing `SyntaxMorph-0.5/morph/translate.py` & `SyntaxMorph-0.6/morph/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import openai
 
-openai.api_key = "OPENAI-KEY"
 
 class ChatSoftware:
     
     @staticmethod
     def translateFunction(languageOne, languageTwo, code, on):
         if on == True:
             prompt = f"#### Translate this function from {languageOne} into {languageTwo}\n {languageOne} \n {code} \n### {languageTwo}"
```

### Comparing `SyntaxMorph-0.5/setup.py` & `SyntaxMorph-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 SyntaxMorph is a Python module that enables code conversion between different programming languages using the OpenAI API. It uses advanced deep learning algorithms to ensure that the functionality and structural integrity of the code are preserved during the conversion process. Users simply need to provide the source code and the target programming language to SyntaxMorph, and it automatically analyzes and converts the code to the target language.
 
 SyntaxMorph offers developers a significant advantage in terms of speeding up the code conversion process between different programming languages. With this module, developers can complete their projects more efficiently and effectively."""
 
 
 setup(
     name="SyntaxMorph",
-    version="0.5",
+    version="0.6",
     author="Marijua",
     author_email="enderjua@gmail.com",
     description="SyntaxMorph is a Python module that enables code conversion between different programming languages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Enderjua/SyntaxMorph",
     packages = ['morph'],
```

