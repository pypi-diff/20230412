# Comparing `tmp/Zeraora-0.1.1.tar.gz` & `tmp/Zeraora-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.1.1.tar", last modified: Mon Apr  3 08:11:30 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.0.tar", last modified: Wed Apr 12 10:18:06 2023, max compression
```

## Comparing `Zeraora-0.1.1.tar` & `Zeraora-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:11:30.000000 Zeraora-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-03 08:11:30.000000 Zeraora-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-03 08:11:17.000000 Zeraora-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:11:30.000000 Zeraora-0.1.1/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-03 08:11:30.000000 Zeraora-0.1.1/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-03 08:11:30.000000 Zeraora-0.1.1/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 08:11:30.000000 Zeraora-0.1.1/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 08:11:30.000000 Zeraora-0.1.1/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 08:11:30.000000 Zeraora-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-03 08:11:17.000000 Zeraora-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:11:30.000000 Zeraora-0.1.1/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-03 08:11:17.000000 Zeraora-0.1.1/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-03 08:11:17.000000 Zeraora-0.1.1/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-03 08:11:17.000000 Zeraora-0.1.1/zeraora/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-03 08:11:17.000000 Zeraora-0.1.1/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-03 08:11:17.000000 Zeraora-0.1.1/zeraora/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-03 08:11:17.000000 Zeraora-0.1.1/zeraora/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-03 08:11:17.000000 Zeraora-0.1.1/zeraora/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:06.000000 Zeraora-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-12 10:18:06.000000 Zeraora-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-12 10:17:55.000000 Zeraora-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 10:18:06.000000 Zeraora-0.2.0/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:18:06.000000 Zeraora-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-12 10:17:55.000000 Zeraora-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:06.000000 Zeraora-0.2.0/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-12 10:17:55.000000 Zeraora-0.2.0/zeraora/typing.py
```

### Comparing `Zeraora-0.1.1/PKG-INFO` & `Zeraora-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,44 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.1.1
+Version: 0.2.0
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
         
-        <div align="center"><i>长期维护的个人开源工具库<br>An original utility Python package with LTS supports for my personal and company projects</i></div>
+        <div align="center"><i>长期维护的个人开源工具库<br>An utility Python package supports for my personal and company projects</i></div>
         
-        ## Description
-        
-        [![Python](https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow)](https://docs.python.org/zh-cn/3/whatsnew/index.html) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://en.wikipedia.org/wiki/MIT_License) ![PyPI](https://img.shields.io/pypi/v/zeraora) ![conda](https://img.shields.io/conda/v/conda-forge/zeraora)
-        
-        解决在不同项目、不同环境之间快速使用自己编写的工具类及快捷函数的痛点。
+        [![Python](https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow)](https://docs.python.org/zh-cn/3/whatsnew/index.html) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://en.wikipedia.org/wiki/MIT_License) [![PyPI](https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI)](https://pypi.org/project/Zeraora/) ![conda](https://img.shields.io/conda/v/conda-forge/zeraora)
         
         ## Usage
         
-        可以使用 pip 直接安装：
+        使用 pip 直接安装：
         
         ```shell
         pip install zeraora
         ```
         
-        未来将发布到 Anaconda Cloud，以便使用 conda 安装：
-        
-        ```shell
-        conda install zeraora
-        ```
-        
-        不能保证所有工具类和快捷函数自始至终都放在同一个子包，因此应该像这样直接导入：
+        不能保证所有工具类和快捷函数自始至终都放在同一个子包，因此应该直接从根目录导入：
         
         ```python
         from zeraora import BearTimer
         
         with BearTimer() as bear:
             summary = 0
             for i in range(1000000):
                 bear.step(f'loop to {i} now.')
                 summary += i
         ```
         
-        亦或者像这样导入：
+        亦或者：
         
         ```python
         import zeraora
         
         with BearTimer.BearTimer() as bear:
             summary = 0
             for i in range(1000000):
@@ -69,26 +59,27 @@
             [
                 print(make_pwd(16)) for _ in range(20)
             ]
         ```
         
         ## Compatibility
         
-        [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，跨越这个版本保证的兼容性的代码可能会存在不易察觉的错误，因此将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
+        > 目前仍处于早期开发阶段。
         
-        ## Change
+        [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
         
-        此处仅列出不兼容旧版的修改，其余变动见git历史。
+        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现难以解决的错误。
         
-        暂无。
+        ## Change
         
-        ## APIs
+        > 仅列出不兼容旧版的修改，其余变动见git历史。
         
-        > 一个成熟的IDE应该学会自己生成文档~
+        ### 0.2.0（2023-4-12）
         
+        - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前面两个类。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Zeraora-0.1.1/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.0/Zeraora.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,44 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.1.1
+Version: 0.2.0
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
 Description: <h1 align="center" style="padding-top: 32px">Zeraora</h1>
         
-        <div align="center"><i>长期维护的个人开源工具库<br>An original utility Python package with LTS supports for my personal and company projects</i></div>
+        <div align="center"><i>长期维护的个人开源工具库<br>An utility Python package supports for my personal and company projects</i></div>
         
-        ## Description
-        
-        [![Python](https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow)](https://docs.python.org/zh-cn/3/whatsnew/index.html) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://en.wikipedia.org/wiki/MIT_License) ![PyPI](https://img.shields.io/pypi/v/zeraora) ![conda](https://img.shields.io/conda/v/conda-forge/zeraora)
-        
-        解决在不同项目、不同环境之间快速使用自己编写的工具类及快捷函数的痛点。
+        [![Python](https://img.shields.io/badge/Python-3.7%20%2B-blue.svg?logo=python&logoColor=yellow)](https://docs.python.org/zh-cn/3/whatsnew/index.html) [![License](https://img.shields.io/badge/License-MIT-purple.svg)](https://en.wikipedia.org/wiki/MIT_License) [![PyPI](https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI)](https://pypi.org/project/Zeraora/) ![conda](https://img.shields.io/conda/v/conda-forge/zeraora)
         
         ## Usage
         
-        可以使用 pip 直接安装：
+        使用 pip 直接安装：
         
         ```shell
         pip install zeraora
         ```
         
-        未来将发布到 Anaconda Cloud，以便使用 conda 安装：
-        
-        ```shell
-        conda install zeraora
-        ```
-        
-        不能保证所有工具类和快捷函数自始至终都放在同一个子包，因此应该像这样直接导入：
+        不能保证所有工具类和快捷函数自始至终都放在同一个子包，因此应该直接从根目录导入：
         
         ```python
         from zeraora import BearTimer
         
         with BearTimer() as bear:
             summary = 0
             for i in range(1000000):
                 bear.step(f'loop to {i} now.')
                 summary += i
         ```
         
-        亦或者像这样导入：
+        亦或者：
         
         ```python
         import zeraora
         
         with BearTimer.BearTimer() as bear:
             summary = 0
             for i in range(1000000):
@@ -69,26 +59,27 @@
             [
                 print(make_pwd(16)) for _ in range(20)
             ]
         ```
         
         ## Compatibility
         
-        [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，跨越这个版本保证的兼容性的代码可能会存在不易察觉的错误，因此将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
+        > 目前仍处于早期开发阶段。
         
-        ## Change
+        [Python 3.7](https://docs.python.org/zh-cn/3/whatsnew/3.7.html#summary-release-highlights) 开始 `dict` 正式按照插入顺序存储，考虑到 `dict` 是 Python 的基石，为了避免出现难以察觉的错误，因而将该版本定为兼容下限。这也是我接触过的项目中的最低运行版本，故而不太希望维护对更低版本的兼容。
         
-        此处仅列出不兼容旧版的修改，其余变动见git历史。
+        项目会尽力保证向后兼容性，但还是建议在requirements中写明特定的版本号，避免因为版本更新或回退而出现难以解决的错误。
         
-        暂无。
+        ## Change
         
-        ## APIs
+        > 仅列出不兼容旧版的修改，其余变动见git历史。
         
-        > 一个成熟的IDE应该学会自己生成文档~
+        ### 0.2.0（2023-4-12）
         
+        - 将 `JSONObject` 与 `JsonObject` 合并为 `OnionObject` ，并删去前面两个类。
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Zeraora-0.1.1/setup.py` & `Zeraora-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.1.1/zeraora/charsets.py` & `Zeraora-0.2.0/zeraora/charsets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+常用字符集。包括按分类定义和按编码定义两大类。
+"""
+
 # print(''.join(map(chr, range(32, 127))))
 
 # 按分类定义的字符集
 DIGITS = '0123456789'
 UPPERS = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
 LOWERS = 'abcdefghijklmnopqrstuvwxyz'
 SYMBOL = r'''!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~'''
```

### Comparing `Zeraora-0.1.1/zeraora/generators.py` & `Zeraora-0.2.0/zeraora/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+生成器。主要包含随机生成和特定顺序生成的实现。
+"""
+
 import os
 from random import getrandbits
 from time import time
 
 from zeraora.charsets import BASE62, BASE64
```

### Comparing `Zeraora-0.1.1/zeraora/time.py` & `Zeraora-0.2.0/zeraora/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+时间相关的处理。包括日期时间类型转换和计时。
+"""
+
 import sys
 from datetime import timedelta, datetime
 from functools import wraps
 from io import TextIOWrapper
 
 
 def delta2hms(delta: timedelta) -> tuple:
@@ -32,30 +36,35 @@
 class BearTimer(object):
     """
     熊牌计时器。
 
     这个类可以让你对代码进行计时功能并输出提示。
 
     最简单的用法是使用 with 语句包裹需要计时的代码：
+
     >>> with BearTimer():
     >>>     for i in range(1000000):
     >>>         print(i)
 
     如果不方便使用 with 包裹，可以直接实例化一个类对象：
+
     >>> bear = BearTimer()
     >>> bear.start()
     >>> bear.stop()
 
     计时开始后，如果需要打印提示，请使用 .step() 方法，例如：
+
     >>> with BearTimer() as bear:
     >>>     summary = 0
     >>>     for i in range(1000000):
     >>>         bear.step(f'loop to {i} now.')
     >>>         summary += i
+
     又或者是
+
     >>> bear = BearTimer()
     >>> bear.start()
     >>> bear.step('operate somethings now.')
     >>> bear.stop()
     """
     file: TextIOWrapper = sys.stdout
```

