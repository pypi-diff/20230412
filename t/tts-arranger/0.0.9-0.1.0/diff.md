# Comparing `tmp/tts_arranger-0.0.9.tar.gz` & `tmp/tts_arranger-0.1.0.tar.gz`

## Comparing `tts_arranger-0.0.9.tar` & `tts_arranger-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    25944 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    14625 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/data/replace
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/data/replace_de
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/data/replace_en
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/LICENSE
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    26358 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    14625 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 tts_arranger-0.1.0/PKG-INFO
```

### Comparing `tts_arranger-0.0.9/src/tts_arranger/tts_processor.py` & `tts_arranger-0.1.0/src/tts_arranger/tts_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import contextlib
 import copy
 import csv
+import json
+import os
 import re
 import string
 from pathlib import Path
 from typing import Optional
 
 import numpy as np  # type: ignore
 import TTS  # type: ignore
@@ -64,25 +66,21 @@
         # if speakers:
         #     self.default_speakers = speakers
 
         self.replace = {}
 
         source_dir = Path(__file__).resolve().parent
 
-        # Load general replace list
-        with open(source_dir / 'data/replace', 'r') as file:
-            for row in csv.reader(file, delimiter='\t'):
-                self.replace[row[0]] = row[1]
-
-        # Load language specific replace list
-        lang = self.model.split('/')[1] if '/' in self.model else 'en'
-
-        with open(source_dir / f'data/replace_{lang}', 'r') as file:
-            for row in csv.reader(file, delimiter='\t'):
-                self.replace[row[0]] = row[1]
+        lang = self.model.split('/')[1]
+
+        for file_path in ['data/replace.json', f'data/replace_{lang}.json']:
+            with open(os.path.join(source_dir, file_path), 'r') as file:
+                data = file.read()
+                # Convert the data to a Python dictionary and update the replace dict
+                self.replace.update(json.loads(data))
 
     # def __del__(self):
     #     self.temp_dir.cleanup()
     #     self.synthesizer = None
     #     gc.collect()
 
     def initialize(self) -> None:
@@ -242,43 +240,55 @@
             # tts_items = self.break_start_end(tts_items, (r'\(', r'\)'), pause_post=150)
             tts_items = self._break_items(tts_items, ('*', '*'))
 
             final_items = []
 
             for tts_item in tts_items:
                 text = tts_item.text
+                if tts_item.text:
 
-                if not text and tts_item.length > 0:
-                    final_items.append(tts_item)
+                    if not text and tts_item.length > 0:
+                        final_items.append(tts_item)
 
-                # text = re.sub(r'([\.\?\!;:]) ', r'\1\n', text)
-                text = re.sub(r'[–—]', r'-', text)
-                text = re.sub(r'[„“”]', r'"', text)
-                text = re.sub(r'[‘’]', r"'", text)
-
-                # Remove all remaining punctuation after first occurrence
-                # text = re.sub(r'([\.\?\!;:])\s?[\.\?\!;:,\)\"\'.\]]+', r'\1', text)
-                text = text.rstrip(string.punctuation + ' ')
-
-                # Strip starting punctuation and normalize ending punctuation
-                text = text.strip().lstrip(string.punctuation).strip()
-
-                if self.model != 'tts_models/en/vctk/vits':
-                    # Add a full stop if necessary to avoid synthesizing problems with some models
-                    text = re.sub(r'([a-zA-Z0-9])$', r'\1.', text)
+                    # text = re.sub(r'([\.\?\!;:]) ', r'\1\n', text)
+                    text = re.sub(r'[–—]', r'-', text)
+                    text = re.sub(r'[„“”]', r'"', text)
+                    text = re.sub(r'[‘’]', r"'", text)
+
+                    # Remove all remaining punctuation after first occurrence
+                    punctuation_regex = '[' + re.escape(string.punctuation) + ']'
+                    regex = r'(' + punctuation_regex + r'(?:\s+)?)+$'
+
+                    match = re.search(regex, text)
+
+                    if match:
+                        matched_text = match.group(0)
+                        if len(matched_text) > 2:
+                            first_char = matched_text[0]
+                            text = re.sub(regex, first_char, text)
+
+                    # Strip starting punctuation and normalize ending punctuation
+                    text = text.strip().lstrip(string.punctuation).strip()
+
+                    if self.model != 'tts_models/en/vctk/vits':
+                        # Add a full stop if necessary to avoid synthesizing problems with some models
+                        text = re.sub(r'([a-zA-Z0-9])$', r'\1.', text)
 
                 if len(text) > 0:
                     if re.search(r'[a-zA-Z0-9]', text):
                         tts_item.text = text
                         final_items.append(tts_item)
 
                         if text[-1] in ['.', ':']:
                             final_items.append(TTS_Item(length=self.pause_sentence))
                         elif text[-1] in ['!', '?']:
                             final_items.append(TTS_Item(length=self.pause_question_exclamation))
+                else:
+                    if tts_item.length > 0:
+                        final_items.append(tts_item)
 
             # if len(final_items) > 0:
             #     tts_items[-1].properties.pause_pre += pause_pre
             #     tts_items[-1].properties.pause_post += pause_post
         else:
             final_items = [tts_item]
```

### Comparing `tts_arranger-0.0.9/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.1.0/src/tts_arranger/tts_processor_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.1.0/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/src/tts_arranger/tts_writer.py` & `tts_arranger-0.1.0/src/tts_arranger/tts_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.1.0/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.1.0/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.1.0/src/tts_arranger/items/tts_project.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/src/tts_arranger/utils/audio.py` & `tts_arranger-0.1.0/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/src/tts_arranger/utils/log.py` & `tts_arranger-0.1.0/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/tests/tts_arranger_test.py` & `tts_arranger-0.1.0/tests/tts_arranger_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         t = TTS_Processor()
 
         tts_item = TTS_Item('This. Is: A t:est!', 'p330')
 
         tts_items = t._prepare_item(tts_item)
 
         self.assertEqual(tts_items[0].text, 'This. Is')
-        self.assertEqual(tts_items[1].length, 150)
+        self.assertEqual(tts_items[1].length, 100)
         self.assertEqual(tts_items[2].text, 'A t:est!')
         self.assertEqual(tts_items[3].length, 1000)
 
     # def test_break2(self):
     #     t = TTS_Arranger()
 
     #     tts_item = TTS_Item('This “Is” a test, right?', 'test', 10, 10, True)
```

### Comparing `tts_arranger-0.0.9/LICENSE` & `tts_arranger-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.9/README.md` & `tts_arranger-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # TTS Arranger
 
 A set of classes that simplify arranging text fragments with multiple speakers and processing it using coqui.ai TTS.
 
 # Examples
 
 ```python
-#!/usr/bin/python3
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
@@ -30,12 +29,15 @@
 items2.append(TTS_Item('Another test',  speaker_idx=0))
 items2.append(TTS_Item('This is getting boring!',  speaker_idx=1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
-project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
+project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
-writer.synthesize_and_write(project.author + ' - ' + project.title)
+# Add a cover image
+project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
+
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', output_format='mp3')
+writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```

### Comparing `tts_arranger-0.0.9/pyproject.toml` & `tts_arranger-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.0.9"
+version = "0.1.0"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.0.9/PKG-INFO` & `tts_arranger-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,14 @@
 # TTS Arranger
 
 A set of classes that simplify arranging text fragments with multiple speakers and processing it using coqui.ai TTS.
 
 # Examples
 
 ```python
-#!/usr/bin/python3
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
@@ -44,12 +43,15 @@
 items2.append(TTS_Item('Another test',  speaker_idx=0))
 items2.append(TTS_Item('This is getting boring!',  speaker_idx=1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
-project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
+project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
-writer.synthesize_and_write(project.author + ' - ' + project.title)
+# Add a cover image
+project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
+
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', output_format='mp3')
+writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
 ```
```

