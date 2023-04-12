# Comparing `tmp/alipan-1.3.6.tar.gz` & `tmp/alipan-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alipan-1.3.6.tar", last modified: Fri Dec 16 12:39:46 2022, max compression
+gzip compressed data, was "alipan-1.3.8.tar", last modified: Wed Apr 12 10:43:30 2023, max compression
```

## Comparing `alipan-1.3.6.tar` & `alipan-1.3.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-12-16 12:39:46.874484 alipan-1.3.6/
--rw-rw-rw-   0        0        0     1089 2022-05-09 03:01:35.000000 alipan-1.3.6/LICENSE
--rw-rw-rw-   0        0        0      298 2022-12-16 12:39:46.873485 alipan-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     1368 2022-12-16 12:38:58.000000 alipan-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-16 12:39:46.857513 alipan-1.3.6/alipan/
--rw-rw-rw-   0        0        0        0 2022-05-09 03:01:35.000000 alipan-1.3.6/alipan/__init__.py
--rw-rw-rw-   0        0        0     1386 2022-05-15 15:51:22.000000 alipan-1.3.6/alipan/__main__.py
--rw-rw-rw-   0        0        0     5791 2022-05-14 16:43:19.000000 alipan-1.3.6/alipan/aligo_utils.py
--rw-rw-rw-   0        0        0     1557 2022-12-16 12:38:13.000000 alipan-1.3.6/alipan/help.py
-drwxrwxrwx   0        0        0        0 2022-12-16 12:39:46.871485 alipan-1.3.6/alipan.egg-info/
--rw-rw-rw-   0        0        0      298 2022-12-16 12:39:46.000000 alipan-1.3.6/alipan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2022-12-16 12:39:46.000000 alipan-1.3.6/alipan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-16 12:39:46.000000 alipan-1.3.6/alipan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-12-16 12:39:46.000000 alipan-1.3.6/alipan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2022-12-16 12:39:46.000000 alipan-1.3.6/alipan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-16 12:39:46.000000 alipan-1.3.6/alipan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-16 12:39:46.874484 alipan-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      688 2022-12-14 09:52:35.000000 alipan-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:43:30.148081 alipan-1.3.8/
+-rw-rw-rw-   0        0        0      284 2023-04-12 10:43:30.147106 alipan-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1368 2023-04-12 08:33:32.000000 alipan-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 10:43:30.131106 alipan-1.3.8/alipan/
+-rw-rw-rw-   0        0        0        0 2023-04-12 08:33:32.000000 alipan-1.3.8/alipan/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-04-12 08:33:32.000000 alipan-1.3.8/alipan/__main__.py
+-rw-rw-rw-   0        0        0     6236 2023-04-12 10:33:42.000000 alipan-1.3.8/alipan/aligo_utils.py
+-rw-rw-rw-   0        0        0     1557 2023-04-12 10:34:23.000000 alipan-1.3.8/alipan/help.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:43:30.145105 alipan-1.3.8/alipan.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-04-12 10:43:30.000000 alipan-1.3.8/alipan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-12 10:43:30.000000 alipan-1.3.8/alipan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:43:30.000000 alipan-1.3.8/alipan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-12 10:43:30.000000 alipan-1.3.8/alipan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 10:43:30.000000 alipan-1.3.8/alipan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-12 10:43:30.000000 alipan-1.3.8/alipan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:43:30.148081 alipan-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-04-12 10:41:20.000000 alipan-1.3.8/setup.py
```

### Comparing `alipan-1.3.6/README.md` & `alipan-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `alipan-1.3.6/alipan/__main__.py` & `alipan-1.3.8/alipan/__main__.py`

 * *Files identical despite different names*

### Comparing `alipan-1.3.6/alipan/aligo_utils.py` & `alipan-1.3.8/alipan/aligo_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,50 +18,51 @@
     aligo_tmp_file = Path.home().joinpath('.aligo').joinpath('aligo_tmp.json')
     aligo_config_file = Path.home().joinpath('.aligo').joinpath('aligo.json')
     os.remove(aligo_tmp_file)
     os.remove(aligo_config_file)
     print('logout success!')
 
 
-def download(pan_file_path, local_folder):
+def download(pan_file_path, local_folder='./'):
     pan_file_path = pan_file_path.strip()
     pan_file_path = pan_file_path if pan_file_path.startswith('/') else get_work_dir() + pan_file_path
     ali = Aligo(level=logging.INFO)
-    remote_file = ali.get_file_by_path(pan_file_path)
-    if remote_file.type == 'file':
-        download_result = ali.download_file(file=remote_file, local_folder=local_folder)
-    else:
+    remote_file = ali.get_folder_by_path(pan_file_path)
+    if remote_file is not None and remote_file.type != 'file':
         download_result = ali.download_folder(remote_file.file_id, local_folder=local_folder)
+    else:
+        remote_file = ali.get_file_by_path(pan_file_path)
+        download_result = ali.download_file(file=remote_file, local_folder=local_folder)
     print(download_result)
 
 
-def upload(target_file, pan_path):
+def upload(target_file, pan_path=None):
     pan_path = pan_path if pan_path is not None else get_work_dir()
     pan_path = pan_path.strip()
     pan_path = pan_path if pan_path.startswith('/') else get_work_dir() + pan_path
     ali = Aligo(level=logging.INFO)
-    remote_folder = ali.get_file_by_path(pan_path)
+    remote_folder = ali.get_folder_by_path(pan_path)
     if os.path.isfile(target_file):
         upload_result = ali.upload_file(target_file, remote_folder.file_id)
     else:
         upload_result = ali.upload_folder(target_file, remote_folder.file_id)
     print(upload_result)
 
 
-def ls(pan_path):
+def ls(pan_path=None):
     pan_path = get_work_dir() if pan_path is None else pan_path
     pan_path = pan_path.strip()
     pan_path = pan_path if pan_path.endswith('/') else pan_path + '/'
     pan_path = pan_path if pan_path.startswith('/') else get_work_dir() + pan_path
     if not exist(pan_path):
         print('%s not exist' % pan_path[:-1])
         return
     ali = Aligo(level=logging.ERROR)
-    remote_folder = ali.get_file_by_path(pan_path)
-    if remote_folder.type == 'file':
+    remote_folder = ali.get_folder_by_path(pan_path)
+    if remote_folder is None or remote_folder.type == 'file':
         print('%s is not a folder' % pan_path[:-1])
         return
     files = ali.get_file_list(remote_folder.file_id)
     # 遍历文件列表
     for f in files:
         updated_date = f.updated_at.replace('T', ' ')[:19]
         file_size = str(round(f.size / 1024.0 / 1024.0, 3)) + 'M' if f.type == 'file' else '-'
@@ -70,35 +71,42 @@
 
 
 def mv(old_pan_file_name, new_pan_file_name):
     old_pan_file_name = old_pan_file_name.strip()
     old_pan_file_name = old_pan_file_name if old_pan_file_name.startswith('/') else get_work_dir() + old_pan_file_name
     ali = Aligo(level=logging.ERROR)
     old_remote_pan_file = ali.get_file_by_path(old_pan_file_name)
-    return ali.rename_file(old_remote_pan_file.file_id, new_pan_file_name)
+    if old_remote_pan_file is None:
+        print('%s not exist' % old_pan_file_name)
+        return
+    mv_result = ali.rename_file(old_remote_pan_file.file_id, new_pan_file_name)
+    return mv_result
 
 
 def rm(pan_file_name):
     pan_file_name = pan_file_name.strip()
     pan_file_name = pan_file_name if pan_file_name.startswith('/') else get_work_dir() + pan_file_name
     ali = Aligo(level=logging.ERROR)
     remote_pan_file = ali.get_file_by_path(pan_file_name)
+    if remote_pan_file is None:
+        print('%s not exist' % remote_pan_file)
+        return
     return ali.move_file_to_trash(remote_pan_file.file_id)
 
 
 def cd(pan_path):
     pan_path = '/' if pan_path is None else pan_path.strip()
     pan_path = pan_path if pan_path.startswith('/') else get_work_dir() + pan_path
     pan_path = pan_path if pan_path.endswith('/') else pan_path + '/'
     if not exist(pan_path):
         print('%s not exist' % pan_path[:-1])
         return
     ali = Aligo(level=logging.ERROR)
-    remote_pan_file = ali.get_file_by_path(pan_path)
-    if remote_pan_file.type == 'file':
+    remote_pan_file = ali.get_folder_by_path(pan_path)
+    if remote_pan_file is None or remote_pan_file.type == 'file':
         print('%s is not a folder' % pan_path[:-1])
         return
     if remote_pan_file is not None and remote_pan_file.type == 'folder':
         write_aligo_env(pan_path)
         print(pan_path[:-1] if pan_path != '/' else '/')
 
 
@@ -113,30 +121,32 @@
     for i, path_check in enumerate(pan_pathes):
         if i == len(pan_pathes) - 1:
             break
         if i == 0:
             target_path = target_path + path_check
         else:
             target_path = target_path + '/' + path_check
-        remote_target_path = ali.get_file_by_path(target_path)
+        remote_target_path = ali.get_folder_by_path(target_path)
         files = ali.get_file_list(remote_target_path.file_id)
         is_exist = False
         for f in files:
             if f.name == pan_pathes[i + 1]:
                 is_exist = True
                 break
         if not is_exist:
             return False
     return True
 
 
 def pwd():
     pwd_path = read_aligo_env()
     pwd_path = '/' if pwd_path is None else pwd_path
-    print(pwd_path[:-1] if pwd_path != '/' else '/')
+    pwd_result = pwd_path[:-1] if pwd_path != '/' else '/'
+    print(pwd_result)
+    return pwd_result
 
 
 def read_aligo_env():
     aligo_tmp_file = Path.home().joinpath('.aligo').joinpath('aligo_tmp.json')
     try:
         with open(aligo_tmp_file, 'r') as file_object:
             return file_object.read()
```

### Comparing `alipan-1.3.6/alipan/help.py` & `alipan-1.3.8/alipan/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 # Author: qicongsheng
 def get_version():
-    return '1.3.6'
+    return '1.3.8'
 
 
 def print_version():
     print('''alipan %s
 Commandline tools for aliyundrive[阿里云盘].''' % get_version())
```

### Comparing `alipan-1.3.6/setup.py` & `alipan-1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     url='https://github.com/qicongsheng/alipan',
     author='qicongsheng',
     author_email='qicongsheng@outlook.com',
     packages=find_packages(),
     include_package_data=True,
     platforms='any',
     install_requires=[
-        'aligo==3.5.1'
+        'aligo==5.5.26'
     ],
     entry_points={
         'console_scripts': [
             'alipan = alipan.__main__:main'
         ]
     }
 )
```

