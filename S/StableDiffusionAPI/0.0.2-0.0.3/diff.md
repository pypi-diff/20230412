# Comparing `tmp/StableDiffusionAPI-0.0.2.tar.gz` & `tmp/StableDiffusionAPI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StableDiffusionAPI-0.0.2.tar", last modified: Mon Apr 10 23:32:38 2023, max compression
+gzip compressed data, was "StableDiffusionAPI-0.0.3.tar", last modified: Wed Apr 12 07:54:07 2023, max compression
```

## Comparing `StableDiffusionAPI-0.0.2.tar` & `StableDiffusionAPI-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 23:32:38.135461 StableDiffusionAPI-0.0.2/
--rw-rw-rw-   0        0        0     2185 2023-04-10 10:15:54.000000 StableDiffusionAPI-0.0.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-10 23:23:24.000000 StableDiffusionAPI-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      824 2023-04-10 23:32:38.134462 StableDiffusionAPI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-10 23:26:40.000000 StableDiffusionAPI-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 23:32:38.130928 StableDiffusionAPI-0.0.2/StableDiffusionAPI/
--rw-rw-rw-   0        0        0     3522 2023-04-10 23:27:11.000000 StableDiffusionAPI-0.0.2/StableDiffusionAPI/StableDiffusionAPI.py
--rw-rw-rw-   0        0        0       49 2023-04-10 23:28:58.000000 StableDiffusionAPI-0.0.2/StableDiffusionAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 23:32:38.134462 StableDiffusionAPI-0.0.2/StableDiffusionAPI.egg-info/
--rw-rw-rw-   0        0        0      824 2023-04-10 23:32:38.000000 StableDiffusionAPI-0.0.2/StableDiffusionAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-10 23:32:38.000000 StableDiffusionAPI-0.0.2/StableDiffusionAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 23:32:38.000000 StableDiffusionAPI-0.0.2/StableDiffusionAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-10 23:32:38.000000 StableDiffusionAPI-0.0.2/StableDiffusionAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      730 2023-04-10 23:31:05.000000 StableDiffusionAPI-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 23:32:38.135461 StableDiffusionAPI-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 07:54:07.025546 StableDiffusionAPI-0.0.3/
+-rw-rw-rw-   0        0        0     2185 2023-04-10 10:15:54.000000 StableDiffusionAPI-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-10 23:23:24.000000 StableDiffusionAPI-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      923 2023-04-12 07:54:07.025546 StableDiffusionAPI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-04-12 07:52:41.000000 StableDiffusionAPI-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 07:54:07.019158 StableDiffusionAPI-0.0.3/StableDiffusionAPI/
+-rw-rw-rw-   0        0        0      125 2023-04-12 07:46:30.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/SetKey.py
+-rw-rw-rw-   0        0        0     4013 2023-04-12 07:45:58.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/Text2Img.py
+-rw-rw-rw-   0        0        0      144 2023-04-12 07:53:33.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-12 07:45:34.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/__main__.py
+-rw-rw-rw-   0        0        0      115 2023-04-12 07:46:13.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI/key.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:54:07.024545 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-12 07:54:07.000000 StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      790 2023-04-12 07:51:03.000000 StableDiffusionAPI-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 07:54:07.025546 StableDiffusionAPI-0.0.3/setup.cfg
```

### Comparing `StableDiffusionAPI-0.0.2/LICENSE` & `StableDiffusionAPI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `StableDiffusionAPI-0.0.2/PKG-INFO` & `StableDiffusionAPI-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: StableDiffusionAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to interface with the StableDiffusionAPI.com API
 Author-email: Jonathan Caraveo <jon@ziawe.com>
 Project-URL: Homepage, https://StableDiffusionAPI.com
 Project-URL: GitHub, https://github.com/caraveo/SDAPI/
 Project-URL: Bug Tracker, https://github.com/Caraveo/SDAPI/issues
+Project-URL: Guide, https://www.sparkandwave.com/stablediffusionapi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SDAPI
+# StableDiffuionAPI
 ```
-import sys
-import os
-import StableDiffusionAPI as sdapi
+import StableDiffusionAPI
 
-strapi = sdapi.StableDiffusionAPI("Moo", 512, 512, 1, "moo.png")
+StableDiffusionAPI.Key("StableDiffusionAPI_KEY")
+StableDiffusionAPI.Text2Img("Tractor", 512, 512, "Tractor.png")
 ```
 # Requires API Key
 [StableDiffusionAPI.com](https://stablediffusionapi.com/)
```

### Comparing `StableDiffusionAPI-0.0.2/StableDiffusionAPI/StableDiffusionAPI.py` & `StableDiffusionAPI-0.0.3/StableDiffusionAPI/Text2Img.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,70 @@
 import sys
 import os
 import random
 import json
 import time
 from urllib.parse import urlparse
+from urllib.parse import quote
 import urllib.parse
 import http.client
+from StableDiffusionAPI import key as key
 
-def SetKey(key):
-    if key == "":
-        print("Please set a key")
-    else:
-        print("Key set")
-
-def sdapi(query2, width, height, samples, name):
-    query = urllib.parse.quote(query2)
+def Text2Img(query2, width, height, name):
+    query = quote(query2)
     img = name
     conn = http.client.HTTPSConnection("stablediffusionapi.com")
     payload = ''
 
-    if width < 512:
-        width = urllib.parse.quote(512)
-    else:
-        width = urllib.parse.quote(width)
-
-    if width > 1024:
-        width = urllib.parse.quote(1024)
+    if width <= 512:
+        width = 512
+    elif width >= 1024:
+        width = 1024
     else:
-        width = urllib.parse.quote(width)
-
-    if height < 512:
-        height = urllib.parse.quote(512)
-    else:
-        height = urllib.parse.quote(height)
-
-    if height > 1024:
-        wiheightdth = urllib.parse.quote(1024)
+        check_width = width.to_bytes(10, byteorder='big')
+    check_width = width.to_bytes(10, byteorder='big')
+    
+    if height <= 512:
+        height = 512
+    elif height >= 1024:
+        height = 1024
     else:
-        height = urllib.parse.quote(height)
+        check_height = height.to_bytes(10, byteorder='big')
+    check_height = height.to_bytes(10, byteorder='big')
 
+    try:
+        quote(check_height)
+        quote(check_width)
+        print("Height and Width are valid")
+    except:
+        print("Height and Width are invalid")
+        exit()
+
+    try:
+        key
+        print("Key Set")
+        print(key)
+    except:
+        print("No Key Error: No value detected, Set a key with SetKey()")
+        exit()
+
+
+    #convert bytes to int
+    string_height_int = str(height)
+    string_width_int = str(width)
+
+    print(string_height_int)
+    print(string_width_int)
+    
     headers = {
-    'key': key
+    'key': key.value
     }
-    uriPrompt = str("/api/v3/text2img?prompt=" + query + "&width=" + width + "&height="+ height +"&samples=1")
+    uriPrompt = str("/api/v3/text2img?prompt=" + query + "&width=" + string_width_int + "&height="+ string_height_int +"&samples=1")
+    
+    print(uriPrompt)
     conn.request("POST", uriPrompt, payload, headers)
     res = conn.getresponse()
     data = res.read()
     print(data)
 
     jrespone = json.loads(data)
```

### Comparing `StableDiffusionAPI-0.0.2/StableDiffusionAPI.egg-info/PKG-INFO` & `StableDiffusionAPI-0.0.3/StableDiffusionAPI.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: StableDiffusionAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to interface with the StableDiffusionAPI.com API
 Author-email: Jonathan Caraveo <jon@ziawe.com>
 Project-URL: Homepage, https://StableDiffusionAPI.com
 Project-URL: GitHub, https://github.com/caraveo/SDAPI/
 Project-URL: Bug Tracker, https://github.com/Caraveo/SDAPI/issues
+Project-URL: Guide, https://www.sparkandwave.com/stablediffusionapi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SDAPI
+# StableDiffuionAPI
 ```
-import sys
-import os
-import StableDiffusionAPI as sdapi
+import StableDiffusionAPI
 
-strapi = sdapi.StableDiffusionAPI("Moo", 512, 512, 1, "moo.png")
+StableDiffusionAPI.Key("StableDiffusionAPI_KEY")
+StableDiffusionAPI.Text2Img("Tractor", 512, 512, "Tractor.png")
 ```
 # Requires API Key
 [StableDiffusionAPI.com](https://stablediffusionapi.com/)
```

