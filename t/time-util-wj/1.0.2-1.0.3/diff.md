# Comparing `tmp/time_util_wj-1.0.2.tar.gz` & `tmp/time_util_wj-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_util_wj-1.0.2.tar", last modified: Wed Apr 12 08:13:41 2023, max compression
+gzip compressed data, was "time_util_wj-1.0.3.tar", last modified: Wed Apr 12 08:26:43 2023, max compression
```

## Comparing `time_util_wj-1.0.2.tar` & `time_util_wj-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:13:41.428718 time_util_wj-1.0.2/
--rw-r--r--   0 wangjie    (501) staff       (20)     1300 2023-04-12 08:13:41.428608 time_util_wj-1.0.2/PKG-INFO
--rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-04-12 08:13:41.428751 time_util_wj-1.0.2/setup.cfg
--rw-r--r--   0 wangjie    (501) staff       (20)      976 2023-04-12 08:13:36.000000 time_util_wj-1.0.2/setup.py
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:13:41.428462 time_util_wj-1.0.2/time_util_wj.egg-info/
--rw-r--r--   0 wangjie    (501) staff       (20)     1300 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/PKG-INFO
--rw-r--r--   0 wangjie    (501) staff       (20)      166 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/SOURCES.txt
--rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/dependency_links.txt
--rw-r--r--   0 wangjie    (501) staff       (20)       11 2023-04-12 08:13:41.000000 time_util_wj-1.0.2/time_util_wj.egg-info/top_level.txt
--rw-r--r--   0 wangjie    (501) staff       (20)     5374 2023-04-12 08:03:30.000000 time_util_wj-1.0.2/time_utils.py
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:26:43.689494 time_util_wj-1.0.3/
+-rw-r--r--   0 wangjie    (501) staff       (20)     1314 2023-04-12 08:26:43.689400 time_util_wj-1.0.3/PKG-INFO
+-rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-04-12 08:26:43.689526 time_util_wj-1.0.3/setup.cfg
+-rw-r--r--   0 wangjie    (501) staff       (20)      976 2023-04-12 08:26:35.000000 time_util_wj-1.0.3/setup.py
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 08:26:43.689275 time_util_wj-1.0.3/time_util_wj.egg-info/
+-rw-r--r--   0 wangjie    (501) staff       (20)     1314 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/PKG-INFO
+-rw-r--r--   0 wangjie    (501) staff       (20)      166 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)       11 2023-04-12 08:26:43.000000 time_util_wj-1.0.3/time_util_wj.egg-info/top_level.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)     5374 2023-04-12 08:03:30.000000 time_util_wj-1.0.3/time_utils.py
```

### Comparing `time_util_wj-1.0.2/PKG-INFO` & `time_util_wj-1.0.3/time_util_wj.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: time_util_wj
-Version: 1.0.2
+Name: time-util-wj
+Version: 1.0.3
 Summary: 提供了各种时间转换的方法
 Home-page: https://github.com/wangjie-jason/time_utils
 Author: WangJie
 Author-email: 1641540482@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 ```python
 pip install time_utils
 ```
 
 # 使用
 
 ```python
-import time_utils
+from time_utils import TimeUtil
 
 print(TimeUtil.get_current_time_str())  ###获取当前字符串格式化时间
 print(TimeUtil.get_current_time_unix())  ###获取当前时间戳
 print(TimeUtil.get_seven_days_ago_time_unix())
 print(TimeUtil.str_time_to_unix("2022-07-07 20:28:50"))
 print(TimeUtil.unix_time_to_str(1657197749260))
 print(TimeUtil.get_recently_day(-7, 'unix'))
```

### Comparing `time_util_wj-1.0.2/setup.py` & `time_util_wj-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="time_util_wj",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.0.2",  # 程序版本
+    version="1.0.3",  # 程序版本
     py_modules=['time_utils'],
     author="WangJie",  # 项目作者
     author_email="1641540482@qq.com",  # 作者邮件
     description="提供了各种时间转换的方法",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/wangjie-jason/time_utils",  # 项目地址
```

### Comparing `time_util_wj-1.0.2/time_util_wj.egg-info/PKG-INFO` & `time_util_wj-1.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: time-util-wj
-Version: 1.0.2
+Name: time_util_wj
+Version: 1.0.3
 Summary: 提供了各种时间转换的方法
 Home-page: https://github.com/wangjie-jason/time_utils
 Author: WangJie
 Author-email: 1641540482@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 ```python
 pip install time_utils
 ```
 
 # 使用
 
 ```python
-import time_utils
+from time_utils import TimeUtil
 
 print(TimeUtil.get_current_time_str())  ###获取当前字符串格式化时间
 print(TimeUtil.get_current_time_unix())  ###获取当前时间戳
 print(TimeUtil.get_seven_days_ago_time_unix())
 print(TimeUtil.str_time_to_unix("2022-07-07 20:28:50"))
 print(TimeUtil.unix_time_to_str(1657197749260))
 print(TimeUtil.get_recently_day(-7, 'unix'))
```

### Comparing `time_util_wj-1.0.2/time_utils.py` & `time_util_wj-1.0.3/time_utils.py`

 * *Files identical despite different names*

