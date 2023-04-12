# Comparing `tmp/py3curl-1.1.0.tar.gz` & `tmp/py3curl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3curl-1.1.0.tar", last modified: Wed Apr 12 06:43:52 2023, max compression
+gzip compressed data, was "py3curl-1.1.1.tar", last modified: Wed Apr 12 06:49:50 2023, max compression
```

## Comparing `py3curl-1.1.0.tar` & `py3curl-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 06:43:52.667640 py3curl-1.1.0/
--rw-r--r--   0 wangjie    (501) staff       (20)      862 2023-04-12 06:43:52.667520 py3curl-1.1.0/PKG-INFO
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 06:43:52.666786 py3curl-1.1.0/py3curl/
--rw-r--r--   0 wangjie    (501) staff       (20)      137 2023-04-12 06:08:04.000000 py3curl-1.1.0/py3curl/__init__.py
--rw-r--r--   0 wangjie    (501) staff       (20)      999 2023-04-12 05:04:17.000000 py3curl-1.1.0/py3curl/py3curl.py
-drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 06:43:52.667361 py3curl-1.1.0/py3curl.egg-info/
--rw-r--r--   0 wangjie    (501) staff       (20)      862 2023-04-12 06:43:52.000000 py3curl-1.1.0/py3curl.egg-info/PKG-INFO
--rw-r--r--   0 wangjie    (501) staff       (20)      171 2023-04-12 06:43:52.000000 py3curl-1.1.0/py3curl.egg-info/SOURCES.txt
--rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-12 06:43:52.000000 py3curl-1.1.0/py3curl.egg-info/dependency_links.txt
--rw-r--r--   0 wangjie    (501) staff       (20)        8 2023-04-12 06:43:52.000000 py3curl-1.1.0/py3curl.egg-info/top_level.txt
--rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-04-12 06:43:52.667677 py3curl-1.1.0/setup.cfg
--rw-r--r--   0 wangjie    (501) staff       (20)      944 2023-04-12 06:43:51.000000 py3curl-1.1.0/setup.py
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 06:49:50.534438 py3curl-1.1.1/
+-rw-r--r--   0 wangjie    (501) staff       (20)      862 2023-04-12 06:49:50.534303 py3curl-1.1.1/PKG-INFO
+drwxr-xr-x   0 wangjie    (501) staff       (20)        0 2023-04-12 06:49:50.534141 py3curl-1.1.1/py3curl.egg-info/
+-rw-r--r--   0 wangjie    (501) staff       (20)      862 2023-04-12 06:49:50.000000 py3curl-1.1.1/py3curl.egg-info/PKG-INFO
+-rw-r--r--   0 wangjie    (501) staff       (20)      132 2023-04-12 06:49:50.000000 py3curl-1.1.1/py3curl.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-12 06:49:50.000000 py3curl-1.1.1/py3curl.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)        1 2023-04-12 06:49:50.000000 py3curl-1.1.1/py3curl.egg-info/top_level.txt
+-rw-r--r--   0 wangjie    (501) staff       (20)       38 2023-04-12 06:49:50.534486 py3curl-1.1.1/setup.cfg
+-rw-r--r--   0 wangjie    (501) staff       (20)      944 2023-04-12 06:49:42.000000 py3curl-1.1.1/setup.py
```

### Comparing `py3curl-1.1.0/PKG-INFO` & `py3curl-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3curl
-Version: 1.1.0
+Version: 1.1.1
 Summary: 将请求对象转换为curl命令字符串
 Home-page: https://github.com/wangjie-jason/py3curl
 Author: WangJie
 Author-email: 1641540482@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3curl-1.1.0/py3curl.egg-info/PKG-INFO` & `py3curl-1.1.1/py3curl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3curl
-Version: 1.1.0
+Version: 1.1.1
 Summary: 将请求对象转换为curl命令字符串
 Home-page: https://github.com/wangjie-jason/py3curl
 Author: WangJie
 Author-email: 1641540482@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py3curl-1.1.0/setup.py` & `py3curl-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py3curl",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.1.0",  # 程序版本
+    version="1.1.1",  # 程序版本
     author="WangJie",  # 项目作者
     author_email="1641540482@qq.com",  # 作者邮件
     description="将请求对象转换为curl命令字符串",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/wangjie-jason/py3curl",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

