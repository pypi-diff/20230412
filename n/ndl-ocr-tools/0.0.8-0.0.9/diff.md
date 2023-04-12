# Comparing `tmp/ndl_ocr_tools-0.0.8.tar.gz` & `tmp/ndl_ocr_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ndl_ocr_tools-0.0.8.tar", last modified: Thu Jan 26 11:22:33 2023, max compression
+gzip compressed data, was "dist/ndl_ocr_tools-0.0.9.tar", last modified: Sat Feb 11 22:23:45 2023, max compression
```

## Comparing `ndl_ocr_tools-0.0.8.tar` & `ndl_ocr_tools-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 ndl_ocr_tools-0.0.8/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2022-09-05 16:31:43.000000 ndl_ocr_tools-0.0.8/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1043 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      311 2023-01-25 06:37:21.000000 ndl_ocr_tools-0.0.8/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)        0 2023-01-26 11:04:15.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1790 2023-01-26 11:04:15.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     6476 2023-01-26 11:04:15.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools/api.py
--rw-r--r--   0 nakamura   (501) staff       (20)      402 2023-01-25 06:39:07.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1043 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      405 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       48 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-01-25 06:40:57.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       21 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       14 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      895 2023-01-26 11:22:30.000000 ndl_ocr_tools-0.0.8/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-01-26 11:22:33.000000 ndl_ocr_tools-0.0.8/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 ndl_ocr_tools-0.0.8/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 ndl_ocr_tools-0.0.9/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2022-09-05 16:31:43.000000 ndl_ocr_tools-0.0.9/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1043 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      311 2023-01-26 12:19:49.000000 ndl_ocr_tools-0.0.9/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)        0 2023-02-11 22:23:16.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1285 2023-02-11 22:23:16.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     6735 2023-02-11 22:23:16.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools/api.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1043 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      383 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       48 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       28 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       14 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      902 2023-02-11 22:23:21.000000 ndl_ocr_tools-0.0.9/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-02-11 22:23:45.000000 ndl_ocr_tools-0.0.9/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 ndl_ocr_tools-0.0.9/setup.py
```

### Comparing `ndl_ocr_tools-0.0.8/LICENSE` & `ndl_ocr_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ndl_ocr_tools-0.0.8/PKG-INFO` & `ndl_ocr_tools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndl_ocr_tools
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/nakamura196/ndl_ocr_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ndl_ocr_tools-0.0.8/ndl_ocr_tools/_modidx.py` & `ndl_ocr_tools-0.0.9/ndl_ocr_tools/_modidx.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,12 +8,8 @@
   'syms': { 'ndl_ocr_tools.api': { 'ndl_ocr_tools.api.Client': ('api.html#client', 'ndl_ocr_tools/api.py'),
                                    'ndl_ocr_tools.api.Client.__init__': ('api.html#client.__init__', 'ndl_ocr_tools/api.py'),
                                    'ndl_ocr_tools.api.Client.convertBB': ('api.html#client.convertbb', 'ndl_ocr_tools/api.py'),
                                    'ndl_ocr_tools.api.Client.createIIIFManifest3': ( 'api.html#client.createiiifmanifest3',
                                                                                      'ndl_ocr_tools/api.py'),
                                    'ndl_ocr_tools.api.Client.downloadImagesFromManifest': ( 'api.html#client.downloadimagesfrommanifest',
                                                                                             'ndl_ocr_tools/api.py'),
-                                   'ndl_ocr_tools.api.Client.getAnnotations': ('api.html#client.getannotations', 'ndl_ocr_tools/api.py')},
-            'ndl_ocr_tools.core': { 'ndl_ocr_tools.core.ApiClient': ('api.html#apiclient', 'ndl_ocr_tools/core.py'),
-                                    'ndl_ocr_tools.core.ApiClient.__init__': ('api.html#apiclient.__init__', 'ndl_ocr_tools/core.py'),
-                                    'ndl_ocr_tools.core.ApiClient.get': ('api.html#apiclient.get', 'ndl_ocr_tools/core.py'),
-                                    'ndl_ocr_tools.core.ApiClient.post': ('api.html#apiclient.post', 'ndl_ocr_tools/core.py')}}}
+                                   'ndl_ocr_tools.api.Client.getAnnotations': ('api.html#client.getannotations', 'ndl_ocr_tools/api.py')}}}
```

### Comparing `ndl_ocr_tools-0.0.8/ndl_ocr_tools/api.py` & `ndl_ocr_tools-0.0.9/ndl_ocr_tools/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # %% ../nbs/api.ipynb 4
 class Client:
     "API client"
     def __init__(self):
         pass
 
     @staticmethod
-    def downloadImagesFromManifest(manifest_url, output_dir, pos_start=1, pos_end=-1, sleep_time=0, continue_with_error=True):
+    def downloadImagesFromManifest(manifest_url, output_dir, pos_start=1, pos_end=-1, sleep_time=0, continue_with_error=True, resized_height=1024):
         # sleep_time = 0
 
         start = pos_start - 1
         end = pos_end
 
         df = requests.get(manifest_url).json()
         canvases = df["sequences"][0]["canvases"]
@@ -43,15 +43,18 @@
             os.makedirs(os.path.dirname(path), exist_ok=True)
             url = canvases[i]["images"][0]["resource"]["@id"]
 
             
             url_ = url
 
             if "/full/full/" in url_:
-                url_ = url_.replace("/full/full/", "/full/,1000/")
+                if type(resized_height) == int: 
+                    url_ = url_.replace("/full/full/", f"/full/,{resized_height}/")
+                else:
+                    url_ = url_.replace("/full/full/", f"/full/{resized_height}/")
             
             url = url_
             
             '''
             '''
 
             time.sleep(sleep_time)
@@ -123,15 +126,15 @@
                     "value": text
                 }
             })
 
         return items
 
     @staticmethod
-    def createIIIFManifest3(output_path, urls, img_dir, json_path):
+    def createIIIFManifest3(output_path, urls, img_dir, json_path, check_iiif=True, resized_height=1024):
         json_files = glob.glob(json_path + "/*.json")
         json_files.sort()
 
         img_files = glob.glob(img_dir + "/*.jpg")
         img_files.sort()
 
         canvases = []
@@ -140,30 +143,30 @@
 
             original = urls[i]
 
             isIIIF = False
 
             r = 1
 
-            if "/full/" in original and "/0/default" in original:
+            if check_iiif and "/full/" in original and "/0/default" in original:
                 isIIIF = True
 
                 info = requests.get(original.split("/full/")[0] + "/info.json").json()
-                o_width = info["width"]
+                # o_width = info["width"]
                 o_height = info["height"]
 
-                r = o_height / 1000
+                r = o_height / resized_height
 
             img = Image.open(img_files[i])
             width, height = img.size
 
             width = int(width * r)
             height = int(height * r)
 
-            filename = os.path.basename(img_files[i]).split(".")[0]
+            # filename = os.path.basename(img_files[i]).split(".")[0]
 
             body = {
                 "format": "image/jpeg",
                 "height": height,
                 "id": "{}".format(original),
                 "type": "Image",
                 "width": width
```

### Comparing `ndl_ocr_tools-0.0.8/ndl_ocr_tools.egg-info/PKG-INFO` & `ndl_ocr_tools-0.0.9/ndl_ocr_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndl-ocr-tools
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/nakamura196/ndl_ocr_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `ndl_ocr_tools-0.0.8/settings.ini` & `ndl_ocr_tools-0.0.9/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ndl_ocr_tools
 lib_name = %(repo)s
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ndl_ocr_tools
 nbs_path = nbs
@@ -33,10 +33,10 @@
 description = 
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = nakamura196
 
 ### Optional ###
-requirements = requests tqdm
+requirements = requests tqdm Pillow
 # dev_requirements = 
 # console_scripts =
```

### Comparing `ndl_ocr_tools-0.0.8/setup.py` & `ndl_ocr_tools-0.0.9/setup.py`

 * *Files identical despite different names*

