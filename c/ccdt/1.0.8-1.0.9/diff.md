# Comparing `tmp/ccdt-1.0.8.tar.gz` & `tmp/ccdt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-1.0.8.tar", last modified: Sat Jan 22 08:14:56 2022, max compression
+gzip compressed data, was "ccdt-1.0.9.tar", last modified: Sun Jan 23 09:36:12 2022, max compression
```

## Comparing `ccdt-1.0.8.tar` & `ccdt-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.532729 ccdt-1.0.8/
--rw-rw-rw-   0        0        0    35149 2021-10-27 01:51:07.000000 ccdt-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     4360 2022-01-22 08:14:56.531730 ccdt-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3672 2022-01-06 09:36:06.000000 ccdt-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.434989 ccdt-1.0.8/ccdt/
--rw-rw-rw-   0        0        0      148 2022-01-07 08:59:32.000000 ccdt-1.0.8/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.467901 ccdt-1.0.8/ccdt/dataset/
--rw-rw-rw-   0        0        0       70 2021-11-05 07:47:13.000000 ccdt-1.0.8/ccdt/dataset/__init__.py
--rw-rw-rw-   0        0        0     8703 2022-01-13 09:22:17.000000 ccdt-1.0.8/ccdt/dataset/__main__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.482862 ccdt-1.0.8/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0       70 2021-11-08 03:06:12.000000 ccdt-1.0.8/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0    28275 2022-01-15 08:53:50.000000 ccdt-1.0.8/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.504804 ccdt-1.0.8/ccdt/dataset/coco/
--rw-rw-rw-   0        0        0       46 2021-11-15 03:38:50.000000 ccdt-1.0.8/ccdt/dataset/coco/__init__.py
--rw-rw-rw-   0        0        0    11371 2021-12-02 02:17:04.000000 ccdt-1.0.8/ccdt/dataset/coco/coco-bak.py
--rw-rw-rw-   0        0        0    11833 2021-12-29 07:43:31.000000 ccdt-1.0.8/ccdt/dataset/coco/coco.py
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.515773 ccdt-1.0.8/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      105 2021-08-30 07:00:12.000000 ccdt-1.0.8/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      390 2021-08-10 10:59:40.000000 ccdt-1.0.8/ccdt/dataset/utils/coder.py
--rw-rw-rw-   0        0        0     3598 2022-01-12 06:49:34.000000 ccdt-1.0.8/ccdt/dataset/utils/path.py
--rw-rw-rw-   0        0        0      530 2021-07-15 01:06:36.000000 ccdt-1.0.8/ccdt/version.py
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.528739 ccdt-1.0.8/ccdt/video_tool/
--rw-rw-rw-   0        0        0       47 2022-01-12 08:16:46.000000 ccdt-1.0.8/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     2614 2022-01-22 08:08:30.000000 ccdt-1.0.8/ccdt/video_tool/__main__.py
--rw-rw-rw-   0        0        0     2137 2022-01-22 08:08:30.000000 ccdt-1.0.8/ccdt/video_tool/split.py
-drwxrwxrwx   0        0        0        0 2022-01-22 08:14:56.456930 ccdt-1.0.8/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4360 2022-01-22 08:14:56.000000 ccdt-1.0.8/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2022-01-22 08:14:56.000000 ccdt-1.0.8/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-22 08:14:56.000000 ccdt-1.0.8/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2022-01-22 08:14:56.000000 ccdt-1.0.8/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2022-01-22 08:14:56.000000 ccdt-1.0.8/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-01-22 08:14:56.000000 ccdt-1.0.8/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-10-25 09:44:52.000000 ccdt-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-01-22 08:14:56.532729 ccdt-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2172 2022-01-22 08:14:06.000000 ccdt-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.633890 ccdt-1.0.9/
+-rw-rw-rw-   0        0        0    35149 2021-10-27 01:51:07.000000 ccdt-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4360 2022-01-23 09:36:12.631896 ccdt-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3672 2022-01-06 09:36:06.000000 ccdt-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.500191 ccdt-1.0.9/ccdt/
+-rw-rw-rw-   0        0        0      148 2022-01-07 08:59:32.000000 ccdt-1.0.9/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.520135 ccdt-1.0.9/ccdt/dataset/
+-rw-rw-rw-   0        0        0       70 2021-11-05 07:47:13.000000 ccdt-1.0.9/ccdt/dataset/__init__.py
+-rw-rw-rw-   0        0        0     8703 2022-01-13 09:22:17.000000 ccdt-1.0.9/ccdt/dataset/__main__.py
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.525123 ccdt-1.0.9/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0       70 2021-11-08 03:06:12.000000 ccdt-1.0.9/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0    28275 2022-01-15 08:53:50.000000 ccdt-1.0.9/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.569062 ccdt-1.0.9/ccdt/dataset/coco/
+-rw-rw-rw-   0        0        0       46 2021-11-15 03:38:50.000000 ccdt-1.0.9/ccdt/dataset/coco/__init__.py
+-rw-rw-rw-   0        0        0    11371 2021-12-02 02:17:04.000000 ccdt-1.0.9/ccdt/dataset/coco/coco-bak.py
+-rw-rw-rw-   0        0        0    11833 2021-12-29 07:43:31.000000 ccdt-1.0.9/ccdt/dataset/coco/coco.py
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.621921 ccdt-1.0.9/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      105 2021-08-30 07:00:12.000000 ccdt-1.0.9/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      390 2021-08-10 10:59:40.000000 ccdt-1.0.9/ccdt/dataset/utils/coder.py
+-rw-rw-rw-   0        0        0     3598 2022-01-12 06:49:34.000000 ccdt-1.0.9/ccdt/dataset/utils/path.py
+-rw-rw-rw-   0        0        0      530 2021-07-15 01:06:36.000000 ccdt-1.0.9/ccdt/version.py
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.629901 ccdt-1.0.9/ccdt/video_tool/
+-rw-rw-rw-   0        0        0       47 2022-01-12 08:16:46.000000 ccdt-1.0.9/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     3595 2022-01-23 09:35:55.000000 ccdt-1.0.9/ccdt/video_tool/__main__.py
+-rw-rw-rw-   0        0        0     2728 2022-01-23 08:40:39.000000 ccdt-1.0.9/ccdt/video_tool/split.py
+drwxrwxrwx   0        0        0        0 2022-01-23 09:36:12.515151 ccdt-1.0.9/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4360 2022-01-23 09:36:12.000000 ccdt-1.0.9/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2022-01-23 09:36:12.000000 ccdt-1.0.9/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-23 09:36:12.000000 ccdt-1.0.9/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2022-01-23 09:36:12.000000 ccdt-1.0.9/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2022-01-23 09:36:12.000000 ccdt-1.0.9/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-01-23 09:36:12.000000 ccdt-1.0.9/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-10-25 09:44:52.000000 ccdt-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-01-23 09:36:12.633890 ccdt-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2172 2022-01-23 09:35:55.000000 ccdt-1.0.9/setup.py
```

### Comparing `ccdt-1.0.8/LICENSE` & `ccdt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/PKG-INFO` & `ccdt-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Platform: UNKNOWN
```

### Comparing `ccdt-1.0.8/README.md` & `ccdt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/ccdt/dataset/__main__.py` & `ccdt-1.0.9/ccdt/dataset/__main__.py`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-1.0.9/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/ccdt/dataset/coco/coco-bak.py` & `ccdt-1.0.9/ccdt/dataset/coco/coco-bak.py`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/ccdt/dataset/coco/coco.py` & `ccdt-1.0.9/ccdt/dataset/coco/coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/ccdt/dataset/utils/path.py` & `ccdt-1.0.9/ccdt/dataset/utils/path.py`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/ccdt/version.py` & `ccdt-1.0.9/ccdt/version.py`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/ccdt/video_tool/__main__.py` & `ccdt-1.0.9/ccdt/video_tool/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,50 +2,62 @@
 import multiprocessing
 import os
 import ccdt.video_tool.split
 
 
 def get_args():
     parser = argparse.ArgumentParser('视频按帧切片（需要传入两个参数videos_dir，imgs_dir）')
-    parser.add_argument('--input_dir',
+    parser.add_argument('--input',
                         default=r'C:/Users/54071/Desktop/55/data/rename_video_test',
                         help='需要切片的视频路径(支持中文和英文)')
     parser.add_argument('--output_dir',
                         default=r'C:/Users/54071/Desktop/55/data/rename_video_test/output_video',
                         help='图片保存路径')
     parser.add_argument('--file_types',
                         default=['.mp4', '.MP4', '.mov', '.avi', '.MOV', '.264', '.dav', '.wmv', '.AVI', '.avi',
                                  '.webm', '.mkv', '.mkv', '.WMV', '.FLV', '.flv', '.MPG', '.mpg'],
                         help='视频文件格式')
-    parser.add_argument('--image_format', default='jpg', help='图片格式')
-    parser.add_argument('--interval', default=50, help='几帧切一次')
+    parser.add_argument('--filename_format', default='{:0>8d}.jpg', help='默认文件前缀8位按帧号递增、文件后缀.jpg。可自定义文件名前缀与后缀，png、JPEG、jpg')
+    parser.add_argument('--images_save', default='00.images', help='默认图片归档存储文件夹为00.images。可自定义')
+    parser.add_argument('--interval', default=50, help='默认按50帧提取视频，可自定义几帧切一次')
     parser.add_argument('--function', type=str, help="输入操作功能参数:split只能输入单个")
     args = parser.parse_args()
     return args
 
 
 def main():
     args = get_args()
     if args.function == 'split':
-        videos_path = ccdt.Split.get_videos_path(args.input_dir, args.file_types)
+        # 如果输入是一个文件路径,就直接加入列表进行处理，如果输入是一个目录，就递归后把文件路径加入列表
+        if os.path.isfile(args.input):
+            videos_path = list()
+            videos_path.append(args.input)
+        else:
+            videos_path = ccdt.Split.get_videos_path(args.input, args.file_types)
         # 创建进程池
-        po = multiprocessing.Pool(20)
+        po = multiprocessing.Pool(2)
         # 创建一个队列
         q = multiprocessing.Manager().Queue()
-        for video_path in videos_path[3]:
-            new_path = video_path.replace(args.input_dir, args.output_dir)
+        for video_path in videos_path:
+            if os.path.isfile(args.input):
+                structure_input_path = os.path.dirname(args.input)
+                new_path = video_path.replace(structure_input_path, args.output_dir)
+            else:
+                new_path = video_path.replace(args.input, args.output_dir)
             dir_name = os.path.dirname(new_path)
             file_name = os.path.basename(new_path)
             file_prefix = os.path.splitext(file_name)[-2]
             output_dir = os.path.join(dir_name, file_prefix)
+            final_output_dir = os.path.join(output_dir, args.images_save)
             # 向进程池中添加,截取视频中的每一帧图片的任务
-            po.apply_async(ccdt.Split.video_loader, args=(q, video_path, args.interval, output_dir))
+            # po.apply_async(ccdt.Split.__call__(), args=(q, video_path, args.interval, output_dir))
+            po.apply_async(ccdt.Split.video_loader, args=(q, video_path, args.interval, final_output_dir, args.filename_format))
         po.close()
         # po.join()  # 加上这个打印进度就会一次性打印完毕，不会分段打印
-        all_file_num = len(videos_path[3])
+        all_file_num = len(videos_path)
         copy_ok_num = 0
         while True:
             file_name = q.get()
             print("\r已经完成提取视频帧：%s" % file_name)
             copy_ok_num += 1
             print("\r提取视频帧的进度为：%.2f %%" % (copy_ok_num * 100 / all_file_num), end="")
             if copy_ok_num >= all_file_num:
```

### Comparing `ccdt-1.0.8/ccdt/video_tool/split.py` & `ccdt-1.0.9/ccdt/video_tool/split.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,65 @@
 import os
 import cv2
 
 
 class Split(object):
     @classmethod
     def get_videos_path(cls, root_dir, file_formats):
-        dir_name_list = list()  # 文件夹名称
-        files_name = list()  # 文件名称
-        path_name = list()  # 文件夹路径
+        # dir_name_list = list()  # 文件夹名称
+        # files_name = list()  # 文件名称
+        # path_name = list()  # 文件夹路径
         file_path_name = list()  # 文件路径
         for root, dirs, files in os.walk(root_dir, topdown=True):
             dirs.sort()
             files.sort()
-            for dir_name in dirs:
-                if dir_name != '00.images' and dir_name != '01.labelme':
-                    dir_name_list.append(dir_name)
+            # for dir_name in dirs:
+            # if dir_name != '00.images' and dir_name != '01.labelme':
+            # dir_name_list.append(dir_name)
             # 遍历文件名称列表
             for file in files:
                 # 获取文件后缀
                 file_suffix = os.path.splitext(file)[-1]
                 # 如果读取的文件后缀，在指定的后缀列表中，则返回真继续往下执行
                 if file_suffix in file_formats:
                     # 如果文件在文件列表中，则返回真继续往下执行
-                    files_name.append(file)
-                    # path_name.append(root.replace("//", "/"))
-                    # file_path_name.append(os.path.join(root, file).replace("//", "/"))
-                    path_name.append(root)
+                    # files_name.append(file)
+                    # path_name.append(root)
                     file_path_name.append(os.path.join(root, file))
-        return dir_name_list, files_name, path_name, file_path_name
+        return file_path_name
+
+    # def __call__(self, q, video_path, interval, output_dir):
+    #     os.makedirs(output_dir, exist_ok=True)
+    #     video = cv2.VideoCapture(video_path)
+    #     cur_frame = 0
+    #     num = 1
+    #     while True:
+    #         ret, frame = video.read()
+    #         if not ret:
+    #             break
+    #         if cur_frame % int(interval) == 0:
+    #             image_name = '{:0>8d}.jpg'.format(cur_frame)
+    #             img_dir = os.path.join(output_dir, image_name)
+    #             cv2.imencode('.jpg', frame)[1].tofile(img_dir)
+    #             num += 1
+    #         cur_frame += 1
+    #     # 如果提取视频帧完成，那么就向队列中写入一个消息，表示已经完成
+    #     q.put(video_path)
 
     @classmethod
-    def video_loader(cls, q, video_path, interval, output_dir):
+    def video_loader(cls, q, video_path, interval, output_dir, filename_format):
         os.makedirs(output_dir, exist_ok=True)
         video = cv2.VideoCapture(video_path)
         cur_frame = 0
         num = 1
         while True:
             ret, frame = video.read()
             if not ret:
                 break
             if cur_frame % int(interval) == 0:
-                image_name = '{:0>8d}.jpg'.format(cur_frame)
+                image_name = filename_format.format(cur_frame)
                 img_dir = os.path.join(output_dir, image_name)
                 cv2.imencode('.jpg', frame)[1].tofile(img_dir)
                 num += 1
             cur_frame += 1
         # 如果提取视频帧完成，那么就向队列中写入一个消息，表示已经完成
         q.put(video_path)
```

### Comparing `ccdt-1.0.8/ccdt.egg-info/PKG-INFO` & `ccdt-1.0.9/ccdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Platform: UNKNOWN
```

### Comparing `ccdt-1.0.8/ccdt.egg-info/SOURCES.txt` & `ccdt-1.0.9/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-1.0.8/setup.py` & `ccdt-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

