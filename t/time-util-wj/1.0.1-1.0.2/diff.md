# Comparing `tmp/time_util_wj-1.0.1.tar.gz` & `tmp/time_util_wj-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_util_wj-1.0.1.tar", last modified: Thu Mar 30 08:33:25 2023, max compression
+gzip compressed data, was "time_util_wj-1.0.2.tar", last modified: Wed Apr 12 08:13:41 2023, max compression
```

## Comparing `time_util_wj-1.0.1.tar` & `time_util_wj-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,10 @@
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-03-30 08:33:25.632254 time_util_wj-1.0.1/
--rw-r--r--   0 wangjie    (501) staff       (20)     1068 2023-03-30 08:21:31.000000 time_util_wj-1.0.1/LICENSE
--rw-r--r--   0 wangjie    (501) staff       (20)      459 2023-03-30 08:33:25.632127 time_util_wj-1.0.1/PKG-INFO
--rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-03-30 08:33:25.632293 time_util_wj-1.0.1/setup.cfg
--rw-r--r--   0 wangjie    (501) staff       (20)     1022 2023-03-30 08:30:17.000000 time_util_wj-1.0.1/setup.py
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-03-30 08:33:25.628973 time_util_wj-1.0.1/time_util_wj/
--rw-r--r--   0 wangjie    (501) staff       (20)      137 2023-03-30 08:21:27.000000 time_util_wj-1.0.1/time_util_wj/__init__.py
--rw-r--r--   0 wangjie    (501) staff       (20)     5354 2023-03-30 08:21:27.000000 time_util_wj-1.0.1/time_util_wj/time_utils.py
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-03-30 08:33:25.631946 time_util_wj-1.0.1/time_util_wj.egg-info/
--rw-r--r--   0 wangjie    (501) staff       (20)      459 2023-03-30 08:33:25.000000 time_util_wj-1.0.1/time_util_wj.egg-info/PKG-INFO
--rw-r--r--   0 wangjie    (501) staff       (20)      212 2023-03-30 08:33:25.000000 time_util_wj-1.0.1/time_util_wj.egg-info/SOURCES.txt
--rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-03-30 08:33:25.000000 time_util_wj-1.0.1/time_util_wj.egg-info/dependency_links.txt
--rw-r--r--   0 wangjie    (501) staff       (20)       13 2023-03-30 08:33:25.000000 time_util_wj-1.0.1/time_util_wj.egg-info/top_level.txt
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:13:41.428718 time_util_wj-1.0.2/
+-rw-r--r--   0 wangjie    (501) staff       (20)     1300 2023-04-12 08:13:41.428608 time_util_wj-1.0.2/PKG-INFO
+-rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-04-12 08:13:41.428751 time_util_wj-1.0.2/setup.cfg
+-rw-r--r--   0 wangjie    (501) staff       (20)      976 2023-04-12 08:13:36.000000 time_util_wj-1.0.2/setup.py
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:13:41.428462 time_util_wj-1.0.2/time_util_wj.egg-info/
+-rw-r--r--   0 wangjie    (501) staff       (20)     1300 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/PKG-INFO
+-rw-r--r--   0 wangjie    (501) staff       (20)      166 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)       11 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/top_level.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)     5374 2023-04-12 08:03:30.000000 time_util_wj-1.0.2/time_utils.py
```

### Comparing `time_util_wj-1.0.1/setup.py` & `time_util_wj-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # !/usr/bin/python
 # -*- coding:utf-8 -*-
-# @Time : 2023/3/30 16:26
-# @Author : wangjie
-# @File : setup.py
-# @project : Automation
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="time_util_wj",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.0.1",  # 程序版本
+    version="1.0.2",  # 程序版本
+    py_modules=['time_utils'],
     author="WangJie",  # 项目作者
     author_email="1641540482@qq.com",  # 作者邮件
     description="提供了各种时间转换的方法",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
-    url="https://github.com/wangjie-jason",  # 项目地址
+    url="https://github.com/wangjie-jason/time_utils",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3",  # 使用Python3
         "License :: OSI Approved :: Apache Software License",  # 开源协议
         "Operating System :: OS Independent",
     ],
-)
+)
```

### Comparing `time_util_wj-1.0.1/time_util_wj/time_utils.py` & `time_util_wj-1.0.2/time_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,16 @@
         :param date_time2: 传入datatime类型
         :return: 布尔值
         """
         date_time1 = date_time1.replace()
         date_time2 = date_time2.replace()
         return date_time1 > date_time2
 
+def foo():
+    pass
 
 if __name__ == '__main__':
     print(TimeUtil.get_current_time_str())
     print(TimeUtil.get_current_time_unix())
     print(TimeUtil.get_seven_days_ago_time_unix())
     print(TimeUtil.str_time_to_unix("2022-07-07 20:28:50"))
     print(TimeUtil.unix_time_to_str(1657197749260))
```

