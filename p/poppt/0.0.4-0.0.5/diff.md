# Comparing `tmp/poppt-0.0.4.tar.gz` & `tmp/poppt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poppt-0.0.4.tar", last modified: Sat Mar 25 09:59:38 2023, max compression
+gzip compressed data, was "poppt-0.0.5.tar", last modified: Wed Apr 12 12:44:17 2023, max compression
```

## Comparing `poppt-0.0.4.tar` & `poppt-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.213754 poppt-0.0.4/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5255 2023-03-25 09:59:38.214761 poppt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4730 2022-10-28 04:35:32.000000 poppt-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.123225 poppt-0.0.4/poppt/
--rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.4/poppt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.177757 poppt-0.0.4/poppt/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.4/poppt/api/__init__.py
--rw-rw-rw-   0        0        0      775 2023-03-05 10:03:19.000000 poppt-0.0.4/poppt/api/ppt.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.184751 poppt-0.0.4/poppt/core/
--rw-rw-rw-   0        0        0     2791 2023-03-25 09:58:58.000000 poppt-0.0.4/poppt/core/PPTType.py
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.4/poppt/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.186755 poppt-0.0.4/poppt/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.4/poppt/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.194757 poppt-0.0.4/poppt/lib/ppt/
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.4/poppt/lib/ppt/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-03-25 09:58:19.000000 poppt-0.0.4/poppt/lib/ppt/ppt2pdf_service.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.165232 poppt-0.0.4/poppt.egg-info/
--rw-rw-rw-   0        0        0     5255 2023-03-25 09:59:37.000000 poppt-0.0.4/poppt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-03-25 09:59:37.000000 poppt-0.0.4/poppt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 09:59:37.000000 poppt-0.0.4/poppt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.4/poppt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2023-03-25 09:59:37.000000 poppt-0.0.4/poppt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-25 09:59:37.000000 poppt-0.0.4/poppt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2023-03-25 09:59:38.217758 poppt-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:59:38.211754 poppt-0.0.4/tests/
--rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0      498 2023-03-05 09:50:26.000000 poppt-0.0.4/tests/test_ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.497109 poppt-0.0.5/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poppt-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5248 2023-04-12 12:44:17.497109 poppt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4723 2023-04-02 05:09:26.000000 poppt-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.444696 poppt-0.0.5/poppt/
+-rw-rw-rw-   0        0        0       29 2022-09-17 08:54:05.000000 poppt-0.0.5/poppt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.480552 poppt-0.0.5/poppt/api/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.5/poppt/api/__init__.py
+-rw-rw-rw-   0        0        0      806 2023-04-12 12:34:20.000000 poppt-0.0.5/poppt/api/ppt.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.485578 poppt-0.0.5/poppt/core/
+-rw-rw-rw-   0        0        0     2576 2023-04-12 12:39:47.000000 poppt-0.0.5/poppt/core/PPTType.py
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.5/poppt/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.487105 poppt-0.0.5/poppt/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 poppt-0.0.5/poppt/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.490597 poppt-0.0.5/poppt/lib/ppt/
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 poppt-0.0.5/poppt/lib/ppt/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-04-12 12:42:46.000000 poppt-0.0.5/poppt/lib/ppt/ppt2pdf_service.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.476570 poppt-0.0.5/poppt.egg-info/
+-rw-rw-rw-   0        0        0     5248 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-05 09:51:54.000000 poppt-0.0.5/poppt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-12 12:44:17.000000 poppt-0.0.5/poppt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      713 2023-04-12 12:44:17.499105 poppt-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poppt-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:44:17.496095 poppt-0.0.5/tests/
+-rw-rw-rw-   0        0        0      181 2022-09-17 08:54:05.000000 poppt-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      529 2023-04-12 12:35:31.000000 poppt-0.0.5/tests/test_ppt.py
```

### Comparing `poppt-0.0.4/LICENSE` & `poppt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poppt-0.0.4/PKG-INFO` & `poppt-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.4
+Version: 0.0.5
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
@@ -26,24 +26,24 @@
 
 -------------------------------------------------------------------------------
 
 
 ## 📚简介
 
 
-wftools是python自动化办公的小工具的代码合集。
+poppt是python自动化办公的小工具的代码合集。
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple wftools -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ poppt -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
@@ -93,15 +93,15 @@
 6. 等待维护者合并
 
 
 ### 🐞提供bug反馈或建议
 
 提交问题反馈时，请务必填写和python-office代码本身有关的问题，不进行有关python学习，甚至是个人练习的知识答疑和讨论。
 
-- [Github issue](https://github.com/CoderWanFeng/wftools/issues)
+- [Github issue](https://github.com/CoderWanFeng/poppt/issues)
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
```

### Comparing `poppt-0.0.4/README.md` & `poppt-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 -------------------------------------------------------------------------------
 
 
 ## 📚简介
 
 
-wftools是python自动化办公的小工具的代码合集。
+poppt是python自动化办公的小工具的代码合集。
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple wftools -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ poppt -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
@@ -77,15 +77,15 @@
 6. 等待维护者合并
 
 
 ### 🐞提供bug反馈或建议
 
 提交问题反馈时，请务必填写和python-office代码本身有关的问题，不进行有关python学习，甚至是个人练习的知识答疑和讨论。
 
-- [Github issue](https://github.com/CoderWanFeng/wftools/issues)
+- [Github issue](https://github.com/CoderWanFeng/poppt/issues)
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
```

### Comparing `poppt-0.0.4/poppt/api/ppt.py` & `poppt-0.0.5/poppt/api/ppt.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from poppt.core.PPTType import MainPPT
 
 mainPPT = MainPPT()
 
 
 # todo：输入文件路径
 # @except_dec()
-def ppt2pdf(path: str):
-    mainPPT.ppt2pdf(path)
+def ppt2pdf(path: str, output_path='./'):
+    mainPPT.ppt2pdf(path, output_path)
 
 
 # def ppt2img(intput_path, output_path=r'./', img_type='img'):
 #     mainPPT.ppt2img(intput_path, output_path, img_type)
 def ppt2img(input_path, output_path, img_type):
     """
     :param intput_path:
```

### Comparing `poppt-0.0.4/poppt/core/PPTType.py` & `poppt-0.0.5/poppt/core/PPTType.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 import os
 import time
+from pathlib import *
 
+import win32com.client
+from pofile import get_files
 from poprogress import simple_progress
 
 from poppt.lib.ppt.ppt2pdf_service import ppt2pdf_single
-import win32com.client
-from pathlib import *
 
 
 class MainPPT():
 
-    def ppt2pdf(self, path):
+    def ppt2pdf(self, path, output_path):
         """
         @Author & Date  : CoderWanFeng 2022/5/9 23:34
         @Desc  : path:存放ppt的路径
         """
         # 如果是相对路径，转为绝对路径
-        if not os.path.isabs(path):
-            path = os.path.abspath(path)
-        # 列出指定目录的内容
-        filenames = os.listdir(path)
+        filenames = get_files(path)
         # for循环依次访问指定目录的所有文件名
         for filename in simple_progress(filenames):
             # 判断文件的类型，对所有的ppt文件进行处理(ppt文件以ppt或者pptx结尾的)
             if filename.endswith('ppt') or filename.endswith('pptx'):
                 # print(filename)           # PPT素材1.pptx -> PPT素材1.pdf
-                # 将filename以.进行分割，返回2个信息，文件的名称和文件的后缀名
-                base, ext = filename.split('.')  # base=PPT素材1 ext=pdf
-                new_pdf_name = base + '.pdf'  # PPT素材1.pdf
+                new_pdf_name = Path(filename).stem + '.pdf'  # PPT素材1.pdf
                 # ppt文件的完整位置: C:/Users/Administrator/Desktop/PPT办公自动化/ppt/PPT素材1.pptx
-                filename = path + '/' + filename
+                # filename = path + '/' + filename
                 # pdf文件的完整位置: C:/Users/Administrator/Desktop/PPT办公自动化/ppt/PPT素材1.pdf
-                output_pdf_filename = path + '/' + new_pdf_name
+                output_pdf_filename = Path(output_path).absolute() / new_pdf_name
                 # 将ppt转成pdf文件
-                ppt2pdf_single(filename, output_pdf_filename)
-                time.sleep(3)
+                ppt2pdf_single(filename, str(output_pdf_filename))
+                # time.sleep(3)
 
     def ppt2img(self, input_path, output_path, img_type):
         '''将PPT另存为图片格式
           arguments:
               pptFullName: 要转换的ppt文件，
               pptName：转换后的存放JPG文件的目录
               imgType: 图片类型
```

### Comparing `poppt-0.0.4/poppt/lib/ppt/ppt2pdf_service.py` & `poppt-0.0.5/poppt/lib/ppt/ppt2pdf_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,29 @@
 1. 如何设置编辑器字体的大小?
 File(文件)-> Settings(设置) -> Editor(编辑器) -> Font(字体), 修改字体的大小
 2. 注释: 代码的解释说明
 """
 
 # 1). 导入需要的模块(打开应用程序的模块)
 import win32com.client
-import os
 
 
 def ppt2pdf_single(filename, output_filename):
     """
     PPT文件导出为pdf格式
     :param filename: PPT文件的名称
     :param output_filename: 导出的pdf文件的名称
     :return:
     """
     # 2). 打开PPT程序
     ppt_app = win32com.client.Dispatch('PowerPoint.Application')
-    ppt_app.Visible = False  # 程序操作应用程序的过程是否可视化
+    ppt_app.Visible = True  # 程序操作应用程序的过程是否可视化
 
     # 3). 通过PPT的应用程序打开指定的PPT文件
     # filename = "C:/Users/Administrator/Desktop/PPT办公自动化/ppt/PPT素材1.pptx"
     # output_filename = "C:/Users/Administrator/Desktop/PPT办公自动化/ppt/PPT素材1.pdf"
-    ppt = ppt_app.Presentations.Open(filename)
+    ppt = ppt_app.Presentations.Open(filename, WithWindow=False)
 
     # 4). 打开的PPT另存为pdf文件。17数字是ppt转图片，32数字是ppt转pdf。
     ppt.SaveAs(output_filename, 32)
     # 退出PPT程序
-    # ppt_app.Quit()
-
-
+    ppt_app.Quit()
```

### Comparing `poppt-0.0.4/poppt.egg-info/PKG-INFO` & `poppt-0.0.5/poppt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poppt
-Version: 0.0.4
+Version: 0.0.5
 Summary: pip install poppt
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poppt/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poppt/blob/master/README.md
@@ -26,24 +26,24 @@
 
 -------------------------------------------------------------------------------
 
 
 ## 📚简介
 
 
-wftools是python自动化办公的小工具的代码合集。
+poppt是python自动化办公的小工具的代码合集。
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
 ```
-pip install -i https://pypi.tuna.tsinghua.edu.cn/simple wftools -U
+pip install -i https://mirrors.aliyun.com/pypi/simple/ poppt -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
@@ -93,15 +93,15 @@
 6. 等待维护者合并
 
 
 ### 🐞提供bug反馈或建议
 
 提交问题反馈时，请务必填写和python-office代码本身有关的问题，不进行有关python学习，甚至是个人练习的知识答疑和讨论。
 
-- [Github issue](https://github.com/CoderWanFeng/wftools/issues)
+- [Github issue](https://github.com/CoderWanFeng/poppt/issues)
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
```

### Comparing `poppt-0.0.4/setup.cfg` & `poppt-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f70 7074 0d0a 7665 7273 696f   = poppt..versio
-00000020: 6e20 3d20 302e 302e 340d 0a64 6573 6372  n = 0.0.4..descr
+00000020: 6e20 3d20 302e 302e 350d 0a64 6573 6372  n = 0.0.5..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f70 7074 0d0a 6c6f 6e67  tall poppt..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

