# Comparing `tmp/torchkeras-3.8.1.tar.gz` & `tmp/torchkeras-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchkeras-3.8.1.tar", last modified: Wed Apr  5 15:41:53 2023, max compression
+gzip compressed data, was "dist/torchkeras-3.8.2.tar", last modified: Wed Apr 12 10:17:48 2023, max compression
```

## Comparing `torchkeras-3.8.1.tar` & `torchkeras-3.8.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-05 15:41:53.876184 torchkeras-3.8.1/
--rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.8.1/LICENSE
--rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.8.1/MANIFEST.in
--rw-r--r--   0 liangyun2   (502) staff       (20)     4846 2023-04-05 15:41:53.875837 torchkeras-3.8.1/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)     5744 2023-03-21 09:46:29.000000 torchkeras-3.8.1/README.md
--rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-04-05 15:41:53.876241 torchkeras-3.8.1/setup.cfg
--rw-r--r--   0 liangyun2   (502) staff       (20)     1326 2023-03-11 07:11:27.000000 torchkeras-3.8.1/setup.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-05 15:41:53.850344 torchkeras-3.8.1/torchkeras/
--rw-r--r--   0 liangyun2   (502) staff       (20)      237 2023-04-05 15:10:52.000000 torchkeras-3.8.1/torchkeras/__init__.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-05 15:41:53.871688 torchkeras-3.8.1/torchkeras/assets/
--rw-r--r--   0 liangyun2   (502) staff       (20)   773236 2023-02-09 16:00:16.000000 torchkeras-3.8.1/torchkeras/assets/Arial.ttf
--rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.8.1/torchkeras/assets/SimHei.ttf
--rw-r--r--   0 liangyun2   (502) staff       (20)   487438 2023-02-09 16:00:16.000000 torchkeras-3.8.1/torchkeras/assets/bus.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.8.1/torchkeras/assets/park.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.8.1/torchkeras/assets/zidane.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)     5250 2023-04-05 15:39:12.000000 torchkeras-3.8.1/torchkeras/data.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    16012 2023-03-10 13:34:22.000000 torchkeras-3.8.1/torchkeras/fastprogress.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     7636 2023-03-10 07:45:35.000000 torchkeras-3.8.1/torchkeras/kerascallbacks.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10430 2023-04-05 14:45:11.000000 torchkeras-3.8.1/torchkeras/kerasmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5922 2023-02-21 03:41:47.000000 torchkeras-3.8.1/torchkeras/lightcallbacks.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     4733 2023-02-09 16:00:16.000000 torchkeras-3.8.1/torchkeras/lightmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.8.1/torchkeras/metrics.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-05 15:41:53.875457 torchkeras-3.8.1/torchkeras/models/
--rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.8.1/torchkeras/models/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.8.1/torchkeras/models/resnet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    31294 2023-03-10 08:17:36.000000 torchkeras-3.8.1/torchkeras/models/ssd.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.8.1/torchkeras/models/unet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     8782 2023-03-21 09:49:41.000000 torchkeras-3.8.1/torchkeras/plots.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5101 2023-02-09 16:00:16.000000 torchkeras-3.8.1/torchkeras/summary.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3472 2023-03-05 07:02:53.000000 torchkeras-3.8.1/torchkeras/utils.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-05 15:41:53.852399 torchkeras-3.8.1/torchkeras.egg-info/
--rw-r--r--   0 liangyun2   (502) staff       (20)     4846 2023-04-05 15:41:53.000000 torchkeras-3.8.1/torchkeras.egg-info/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)      683 2023-04-05 15:41:53.000000 torchkeras-3.8.1/torchkeras.egg-info/SOURCES.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-04-05 15:41:53.000000 torchkeras-3.8.1/torchkeras.egg-info/dependency_links.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       27 2023-04-05 15:41:53.000000 torchkeras-3.8.1/torchkeras.egg-info/top_level.txt
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-12 10:17:48.375369 torchkeras-3.8.2/
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.8.2/LICENSE
+-rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.8.2/MANIFEST.in
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4846 2023-04-12 10:17:48.375027 torchkeras-3.8.2/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5744 2023-03-21 09:46:29.000000 torchkeras-3.8.2/README.md
+-rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-04-12 10:17:48.375447 torchkeras-3.8.2/setup.cfg
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1326 2023-03-11 07:11:27.000000 torchkeras-3.8.2/setup.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-12 10:17:48.344483 torchkeras-3.8.2/torchkeras/
+-rw-r--r--   0 liangyun2   (502) staff       (20)      237 2023-04-12 09:34:26.000000 torchkeras-3.8.2/torchkeras/__init__.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-12 10:17:48.370742 torchkeras-3.8.2/torchkeras/assets/
+-rw-r--r--   0 liangyun2   (502) staff       (20)   773236 2023-02-09 16:00:16.000000 torchkeras-3.8.2/torchkeras/assets/Arial.ttf
+-rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.8.2/torchkeras/assets/SimHei.ttf
+-rw-r--r--   0 liangyun2   (502) staff       (20)   487438 2023-02-09 16:00:16.000000 torchkeras-3.8.2/torchkeras/assets/bus.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.8.2/torchkeras/assets/park.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.8.2/torchkeras/assets/zidane.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5685 2023-04-12 09:31:57.000000 torchkeras-3.8.2/torchkeras/data.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    16012 2023-03-10 13:34:22.000000 torchkeras-3.8.2/torchkeras/fastprogress.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7636 2023-03-10 07:45:35.000000 torchkeras-3.8.2/torchkeras/kerascallbacks.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10430 2023-04-12 09:43:55.000000 torchkeras-3.8.2/torchkeras/kerasmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5922 2023-02-21 03:41:47.000000 torchkeras-3.8.2/torchkeras/lightcallbacks.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4733 2023-02-09 16:00:16.000000 torchkeras-3.8.2/torchkeras/lightmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.8.2/torchkeras/metrics.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-12 10:17:48.374539 torchkeras-3.8.2/torchkeras/models/
+-rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.8.2/torchkeras/models/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.8.2/torchkeras/models/resnet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    31294 2023-03-10 08:17:36.000000 torchkeras-3.8.2/torchkeras/models/ssd.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.8.2/torchkeras/models/unet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     8782 2023-03-21 09:49:41.000000 torchkeras-3.8.2/torchkeras/plots.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5101 2023-02-09 16:00:16.000000 torchkeras-3.8.2/torchkeras/summary.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3528 2023-04-12 09:43:29.000000 torchkeras-3.8.2/torchkeras/utils.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-04-12 10:17:48.346709 torchkeras-3.8.2/torchkeras.egg-info/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4846 2023-04-12 10:17:48.000000 torchkeras-3.8.2/torchkeras.egg-info/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)      683 2023-04-12 10:17:48.000000 torchkeras-3.8.2/torchkeras.egg-info/SOURCES.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-04-12 10:17:48.000000 torchkeras-3.8.2/torchkeras.egg-info/dependency_links.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       20 2023-04-12 10:17:48.000000 torchkeras-3.8.2/torchkeras.egg-info/top_level.txt
```

### Comparing `torchkeras-3.8.1/LICENSE` & `torchkeras-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/PKG-INFO` & `torchkeras-3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.8.1
+Version: 3.8.2
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.8.1 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.8.2 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
```

### Comparing `torchkeras-3.8.1/README.md` & `torchkeras-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/setup.py` & `torchkeras-3.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/assets/Arial.ttf` & `torchkeras-3.8.2/torchkeras/assets/Arial.ttf`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/assets/SimHei.ttf` & `torchkeras-3.8.2/torchkeras/assets/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/assets/bus.jpg` & `torchkeras-3.8.2/torchkeras/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/assets/park.jpg` & `torchkeras-3.8.2/torchkeras/assets/park.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/assets/zidane.jpg` & `torchkeras-3.8.2/torchkeras/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/data.py` & `torchkeras-3.8.2/torchkeras/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path 
 from PIL import Image 
 import numpy as np 
 import os
 import sys 
-import time 
+import time,datetime 
 from tqdm import tqdm 
 import re
 import requests
-from urllib import parse 
+from urllib.parse import quote,unquote
 
 path = Path(__file__)
 
 def resize_and_pad_image(image,width,height):
     img = image
     w, h = img.size 
     ratio = w / float(h)
@@ -63,24 +63,35 @@
 
 def download_image(url):
     import PIL,requests
     image = PIL.Image.open(requests.get(url, stream=True).raw)
     image = PIL.ImageOps.exif_transpose(image)
     return image
 
+def download_github_file(url,save_name=None):
+    import torch
+    raw_url = url.replace('://github.com/','://raw.githubusercontent.com/').replace('/blob/','/')
+    if save_name is None:
+        save_name = unquote(os.path.basename(raw_url))
+    torch.hub.download_url_to_file(raw_url,save_name)
+    print('saved file: '+save_name,file = sys.stderr)
+    return save_name
+
+
 def download_baidu_pictures(keyword,needed_pics_num=100,save_dir=None):
     spider = _BaiduPictures(keyword,needed_pics_num,save_dir)
     spider.run()
      
 class _BaiduPictures:
     def __init__(self,keyword,needed_pics_num=100,save_dir=None):
         from fake_useragent import UserAgent 
+        
         self.save_dir = save_dir if save_dir is not None else './{}'.format(keyword)
         self.name_ = keyword
-        self.name = parse.quote(self.name_) 
+        self.name = quote(self.name_) 
         self.needed_pics_num = needed_pics_num
         self.times = str(int(time.time()*1000)) 
         self.url = 'https://image.baidu.com/search/acjson?tn=resultjson_com&logid=8032920601831512061&ipn=rj&ct=201326592&is=&fp=result&fr=&word={}&cg=star&queryWord={}&cl=2&lm=-1&ie=utf-8&oe=utf-8&adpicid=&st=&z=&ic=&hd=&latest=&copyright=&s=&se=&tab=&width=&height=&face=&istype=&qc=&nc=1&expermode=&nojc=&isAsync=&pn={}&rn=30&gsm=1e&{}='
         self.headers = {'User-Agent':UserAgent().random}
 
     def get_one_html(self,url,pn):
         response = requests.get(url=url.format(self.name,self.name, pn, self.times), headers=self.headers).content.decode('utf-8')
@@ -98,30 +109,30 @@
         if not os.path.exists(self.save_dir):
             os.mkdir(self.save_dir)
         response = self.get_one_html(self.url,0)
         regex1 = re.compile('"displayNum":(.*?),')
         ori_num = self.parse_html(regex1,response)[0] 
         num = min(int(ori_num),self.needed_pics_num)
         print('{} {} pictures founded. start downloading {} pictures...'.format(
-            ori_num,self.name_,num)) 
+            ori_num,self.name_,num),file = sys.stderr) 
     
         if int(num)%30 == 0:
             pn = int(int(num)/30)
         else:
             pn = int(int(num)//30 + 2)
-        cnt,loop = 0,tqdm(total=num,file=sys.stdout)
+        cnt,loop = 0,tqdm(total=num)
         for i in range(pn): 
             try:
                 resp = self.get_one_html(self.url, i * 30)
                 regex2 = re.compile('"middleURL":"(.*?)"')
                 urls = [x for x in self.parse_html(regex2,resp) if x.startswith('http')]
                 for u in urls:  
                     try:
                         content = self.get_two_html(u) 
-                        img_name = '{}.jpg'.format('0'*max(6-len(str(cnt)),1)+str(cnt))
+                        img_name = '{}.jpg'.format(datetime.datetime.now().strftime('%Y%m%d_%H%M%S_%f'))
                         img_path = os.path.join(self.save_dir,img_name)
                         with open(img_path,'wb') as f:
                             f.write(content)
                         cnt+=1
                         loop.update(1)
                         if cnt>=num:
                             break
@@ -130,8 +141,8 @@
                 else:
                     continue
                 break
             except Exception as err:
                 print(err,file=sys.stderr)
             time.sleep(1.0) 
         loop.close()
-        print('saved {} pictures in dir {}'.format(cnt, self.save_dir))
+        print('saved {} pictures in dir {}'.format(cnt, self.save_dir),file = sys.stderr)
```

### Comparing `torchkeras-3.8.1/torchkeras/fastprogress.py` & `torchkeras-3.8.2/torchkeras/fastprogress.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/kerascallbacks.py` & `torchkeras-3.8.2/torchkeras/kerascallbacks.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/kerasmodel.py` & `torchkeras-3.8.2/torchkeras/kerasmodel.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/lightcallbacks.py` & `torchkeras-3.8.2/torchkeras/lightcallbacks.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/lightmodel.py` & `torchkeras-3.8.2/torchkeras/lightmodel.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/metrics.py` & `torchkeras-3.8.2/torchkeras/metrics.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/models/resnet.py` & `torchkeras-3.8.2/torchkeras/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/models/ssd.py` & `torchkeras-3.8.2/torchkeras/models/ssd.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/models/unet.py` & `torchkeras-3.8.2/torchkeras/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/plots.py` & `torchkeras-3.8.2/torchkeras/plots.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/summary.py` & `torchkeras-3.8.2/torchkeras/summary.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.1/torchkeras/utils.py` & `torchkeras-3.8.2/torchkeras/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from copy import deepcopy
 import random
 import numpy as np 
 import pandas as pd 
 from PIL import Image, ImageFont, ImageDraw
 import pathlib
 from argparse import Namespace
+import os 
 
 def seed_everything(seed=42):
     print(f"Global seed set to {seed}")
     random.seed(seed)
+    os.environ['PYTHONHASHSEED'] = str(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
     return seed
 
 def text_to_image(text):
     path = pathlib.Path(__file__)
```

### Comparing `torchkeras-3.8.1/torchkeras.egg-info/PKG-INFO` & `torchkeras-3.8.2/torchkeras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.8.1
+Version: 3.8.2
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.8.1 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.8.2 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
```

### Comparing `torchkeras-3.8.1/torchkeras.egg-info/SOURCES.txt` & `torchkeras-3.8.2/torchkeras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

