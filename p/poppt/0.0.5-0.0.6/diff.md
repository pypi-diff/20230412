# Comparing `tmp/poppt-0.0.5.tar.gz` & `tmp/poppt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poppt-0.0.5.tar", last modified: Wed Apr 12 12:44:17 2023, max compression
+gzip compressed data, was "poppt-0.0.6.tar", last modified: Wed Apr 12 13:11:10 2023, max compression
```

## Comparing `poppt-0.0.5.tar` & `poppt-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.497109 poppt-0.0.5/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5248 2023-04-12 12:44:17.497109 poppt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.444696 poppt-0.0.5/poppt/
--rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.5/poppt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.480552 poppt-0.0.5/poppt/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.5/poppt/api/__init__.py
--rw-rw-rw-   0        0        0      806 2023-04-12 12:34:20.000000 poppt-0.0.5/poppt/api/ppt.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.485578 poppt-0.0.5/poppt/core/
--rw-rw-rw-   0        0        0     2576 2023-04-12 12:39:47.000000 poppt-0.0.5/poppt/core/PPTType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.5/poppt/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.487105 poppt-0.0.5/poppt/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.5/poppt/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.490597 poppt-0.0.5/poppt/lib/ppt/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.5/poppt/lib/ppt/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.0.5/poppt/lib/ppt/ppt2pdf_service.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.476570 poppt-0.0.5/poppt.egg-info/
--rw-rw-rw-   0        0        0     5248 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.5/poppt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2023-04-12 12:44:17.499105 poppt-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.496095 poppt-0.0.5/tests/
--rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0      529 2023-04-12 12:35:31.000000 poppt-0.0.5/tests/test_ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.277933 poppt-0.0.6/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5248 2023-04-12 13:11:10.278931 poppt-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.230660 poppt-0.0.6/poppt/
+-rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.6/poppt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.260656 poppt-0.0.6/poppt/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.6/poppt/api/__init__.py
+-rw-rw-rw-   0        0        0      806 2023-04-12 12:34:20.000000 poppt-0.0.6/poppt/api/ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.266666 poppt-0.0.6/poppt/core/
+-rw-rw-rw-   0        0        0     2120 2023-04-12 13:10:10.000000 poppt-0.0.6/poppt/core/PPTType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.6/poppt/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.268663 poppt-0.0.6/poppt/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.6/poppt/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.271658 poppt-0.0.6/poppt/lib/ppt/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.6/poppt/lib/ppt/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.0.6/poppt/lib/ppt/ppt2pdf_service.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.257657 poppt-0.0.6/poppt.egg-info/
+-rw-rw-rw-   0        0        0     5248 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.6/poppt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 13:11:10.000000 poppt-0.0.6/poppt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      713 2023-04-12 13:11:10.280943 poppt-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:11:10.275929 poppt-0.0.6/tests/
+-rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      530 2023-04-12 13:02:45.000000 poppt-0.0.6/tests/test_ppt.py
```

### Comparing `poppt-0.0.5/LICENSE` & `poppt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poppt-0.0.5/PKG-INFO` & `poppt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.5
+Version: 0.0.6
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.0.5/README.md` & `poppt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `poppt-0.0.5/poppt/api/ppt.py` & `poppt-0.0.6/poppt/api/ppt.py`

 * *Files identical despite different names*

### Comparing `poppt-0.0.5/poppt/core/PPTType.py` & `poppt-0.0.6/poppt/core/PPTType.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 import os
 import time
 from pathlib import *
 
 import win32com.client
-from pofile import get_files
+from pofile import get_files, mkdir
 from poprogress import simple_progress
 
 from poppt.lib.ppt.ppt2pdf_service import ppt2pdf_single
 
 
 class MainPPT():
 
     def ppt2pdf(self, path, output_path):
         """
         @Author & Date  : CoderWanFeng 2022/5/9 23:34
         @Desc  : path:存放ppt的路径
         """
-        # 如果是相对路径，转为绝对路径
         filenames = get_files(path)
-        # for循环依次访问指定目录的所有文件名
+        exsit, abs_output_path = mkdir(output_path)
         for filename in simple_progress(filenames):
             # 判断文件的类型，对所有的ppt文件进行处理(ppt文件以ppt或者pptx结尾的)
             if filename.endswith('ppt') or filename.endswith('pptx'):
-                # print(filename)           # PPT素材1.pptx -> PPT素材1.pdf
                 new_pdf_name = Path(filename).stem + '.pdf'  # PPT素材1.pdf
-                # ppt文件的完整位置: C:/Users/Administrator/Desktop/PPT办公自动化/ppt/PPT素材1.pptx
-                # filename = path + '/' + filename
-                # pdf文件的完整位置: C:/Users/Administrator/Desktop/PPT办公自动化/ppt/PPT素材1.pdf
-                output_pdf_filename = Path(output_path).absolute() / new_pdf_name
-                # 将ppt转成pdf文件
+                output_pdf_filename = Path(abs_output_path).absolute() / new_pdf_name
                 ppt2pdf_single(filename, str(output_pdf_filename))
                 # time.sleep(3)
 
     def ppt2img(self, input_path, output_path, img_type):
         '''将PPT另存为图片格式
           arguments:
               pptFullName: 要转换的ppt文件，
```

### Comparing `poppt-0.0.5/poppt/lib/ppt/ppt2pdf_service.py` & `poppt-0.0.6/poppt/lib/ppt/ppt2pdf_service.py`

 * *Files identical despite different names*

### Comparing `poppt-0.0.5/poppt.egg-info/PKG-INFO` & `poppt-0.0.6/poppt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.5
+Version: 0.0.6
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
```

### Comparing `poppt-0.0.5/setup.cfg` & `poppt-0.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f70 7074 0d0a 7665 7273 696f   = poppt..versio
-00000020: 6e20 3d20 302e 302e 350d 0a64 6573 6372  n = 0.0.5..descr
+00000020: 6e20 3d20 302e 302e 360d 0a64 6573 6372  n = 0.0.6..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f70 7074 0d0a 6c6f 6e67  tall poppt..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `poppt-0.0.5/tests/test_ppt.py` & `poppt-0.0.6/tests/test_ppt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 from poppt.api.ppt import *
 
 
 class TestPPT(unittest.TestCase):
     def test_ppt2pdf(self):
-        ppt2pdf(path=r'./ppt/', output_path=r'./ppt/test_pdf')
+        ppt2pdf(path=r'./ppt/', output_path=r'./ppt/test_pdf2')
 
     # def test_ppt2img(self):
     #     ppt2img(intput_path=r'D:\test\py310\ppt_test')
     def test_single_ppt2imgg(self):
         ppt2img(intput_path=r'D:\test\py310\ppt_test\代码之外，程序员能力提升必备的8个软件（刘兆锋）.pptx',
                 output_path=r'D:\test\py310\ppt_test',
                 img_type='jpg')
```

