# Comparing `tmp/tts-gen-1.2.3.tar.gz` & `tmp/tts-gen-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tts-gen-1.2.3.tar", last modified: Wed Nov 30 11:31:51 2022, max compression
+gzip compressed data, was "dist/tts-gen-1.2.4.tar", last modified: Wed Apr 12 11:16:10 2023, max compression
```

## Comparing `tts-gen-1.2.3.tar` & `tts-gen-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2022-11-30 11:31:51.244420 tts-gen-1.2.3/
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      499 2022-11-30 11:31:51.244420 tts-gen-1.2.3/PKG-INFO
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       38 2022-11-30 11:31:51.244420 tts-gen-1.2.3/setup.cfg
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1617 2022-08-10 02:41:51.000000 tts-gen-1.2.3/setup.py
-drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2022-11-30 11:31:51.244420 tts-gen-1.2.3/tts_gen.egg-info/
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      499 2022-11-30 11:31:51.000000 tts-gen-1.2.3/tts_gen.egg-info/PKG-INFO
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      263 2022-11-30 11:31:51.000000 tts-gen-1.2.3/tts_gen.egg-info/SOURCES.txt
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)        1 2022-11-30 11:31:51.000000 tts-gen-1.2.3/tts_gen.egg-info/dependency_links.txt
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2022-11-30 11:31:51.000000 tts-gen-1.2.3/tts_gen.egg-info/requires.txt
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2022-11-30 11:31:51.000000 tts-gen-1.2.3/tts_gen.egg-info/top_level.txt
-drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2022-11-30 11:31:51.244420 tts-gen-1.2.3/tts_generator/
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      254 2022-11-30 11:17:24.000000 tts-gen-1.2.3/tts_generator/__init__.py
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1995 2022-11-30 10:36:27.000000 tts-gen-1.2.3/tts_generator/__main__.py
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     8314 2022-11-30 10:25:51.000000 tts-gen-1.2.3/tts_generator/gen_voice.py
--rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1995 2022-11-30 11:17:17.000000 tts-gen-1.2.3/tts_generator/tts-gen
+drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-04-12 11:16:10.000000 tts-gen-1.2.4/
+drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-04-12 11:16:10.000000 tts-gen-1.2.4/tts_gen.egg-info/
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      263 2023-04-12 11:16:10.000000 tts-gen-1.2.4/tts_gen.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)        1 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      555 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/PKG-INFO
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/requires.txt
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       14 2023-04-12 11:16:09.000000 tts-gen-1.2.4/tts_gen.egg-info/top_level.txt
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1617 2022-08-10 02:41:51.000000 tts-gen-1.2.4/setup.py
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      555 2023-04-12 11:16:10.000000 tts-gen-1.2.4/PKG-INFO
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)       38 2023-04-12 11:16:10.000000 tts-gen-1.2.4/setup.cfg
+drwxrwxr-x   0 zhengdi   (1007) zhengdi   (1007)        0 2023-04-12 11:16:10.000000 tts-gen-1.2.4/tts_generator/
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1995 2022-11-30 11:17:17.000000 tts-gen-1.2.4/tts_generator/tts-gen
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     1995 2022-11-30 10:36:27.000000 tts-gen-1.2.4/tts_generator/__main__.py
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)     8510 2023-04-12 11:15:15.000000 tts-gen-1.2.4/tts_generator/gen_voice.py
+-rw-rw-r--   0 zhengdi   (1007) zhengdi   (1007)      254 2023-04-12 09:00:21.000000 tts-gen-1.2.4/tts_generator/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tts-gen-1.2.3/setup.py` & `tts-gen-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tts-gen-1.2.3/tts_generator/__main__.py` & `tts-gen-1.2.4/tts_generator/tts-gen`

 * *Files identical despite different names*

### Comparing `tts-gen-1.2.3/tts_generator/gen_voice.py` & `tts-gen-1.2.4/tts_generator/gen_voice.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from tts_generator import __server_url__, __server_bridge_url__
 
 headers = {
         'User-Agent'         : 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.61 Safari/537.36',
         'Accept-Language'    : 'zh-CN,zh;q=0.9',
         }
 
+def gen_wav_dir_str(s):
+    return s.replace(" ", "_")
+
 def gen_gx_voice(texts, output_dir, server_url=None, voice_num=None, wav_type='all', tts_server_name='gx'):
     if not server_url:
         server_url = __server_url__
     server_synthesize_url = server_url + '/api/synthesize_multi'
     server_info_url = server_url + '/api/info'
 
     if not os.path.exists(output_dir):
@@ -34,27 +37,28 @@
         if not voice_num:
             voice_num = max_voice_num
         total_voice_num = min(max_voice_num, voice_num)
 
         for text in texts:
             print('generate %s wavs ...' % text)
 
-            text_dir = os.path.join(output_dir, text)
+            wav_dir_str = gen_wav_dir_str(text)
+            text_dir = os.path.join(output_dir, wav_dir_str)
             if not os.path.exists(text_dir):
                 os.mkdir(text_dir)
 
             if wav_type in ('train', 'test'):
                 text_dir = os.path.join(text_dir, wav_type)
                 if not os.path.exists(text_dir):
                     os.mkdir(text_dir)
-                list_f_name = '%s_%s.list' % (text, wav_type)
-                wav_dir = '%s/%s' % (text, wav_type)
+                list_f_name = '%s_%s.list' % (wav_dir_str, wav_type)
+                wav_dir = '%s/%s' % (wav_dir_str, wav_type)
             else:
-                list_f_name = '%s.list' % text
-                wav_dir = '%s' % text
+                list_f_name = '%s.list' % wav_dir_str
+                wav_dir = '%s' % wav_dir_str
 
             list_f_path = os.path.join(output_dir, list_f_name)
             list_f = open(list_f_path, "w")
             blk_voice_num = 10 # 分块传输
             for voice_index in tqdm(range(0, total_voice_num, blk_voice_num)):
                 data = {
                     'text': text,
@@ -75,20 +79,21 @@
 def other_voice_post_task(lock, index, total_texts_num, total_voice_num, wav_type, tts_server_name,
                           server_synthesize_url, output_dir, text, language, with_style):
     try:
         wav_name = text
         if len(wav_name) > 100:
             wav_name = wav_name[:100]
 
-        text_dir = os.path.join(output_dir, wav_name)
+        wav_dir_str = gen_wav_dir_str(wav_name)
+        text_dir = os.path.join(output_dir, wav_dir_str)
         if not os.path.exists(text_dir):
             os.mkdir(text_dir)
 
-        list_f_name = '%s.list' % wav_name
-        wav_dir = '%s' % wav_name
+        list_f_name = '%s.list' % wav_dir_str
+        wav_dir = '%s' % wav_dir_str
         list_f_path = os.path.join(output_dir, list_f_name)
         list_f = open(list_f_path, "w")
 
         with lock:
             bar = tqdm(
                 desc='[%d/%d] %s' % (index, total_texts_num, text),
                 total=total_voice_num,
```

### Comparing `tts-gen-1.2.3/tts_generator/tts-gen` & `tts-gen-1.2.4/tts_generator/__main__.py`

 * *Files identical despite different names*

