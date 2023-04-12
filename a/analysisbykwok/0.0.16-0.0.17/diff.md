# Comparing `tmp/analysisbykwok-0.0.16.tar.gz` & `tmp/analysisbykwok-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.16.tar", last modified: Mon Apr 10 07:23:31 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.17.tar", last modified: Wed Apr 12 03:56:47 2023, max compression
```

## Comparing `analysisbykwok-0.0.16.tar` & `analysisbykwok-0.0.17.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/
--rw-rw-rw-   0        0        0       62 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/analysisbykwok/
--rw-rw-rw-   0        0        0    14263 2023-04-10 07:23:06.000000 analysisbykwok-0.0.16/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-10 07:22:53.000000 analysisbykwok-0.0.16/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 07:23:31.000000 analysisbykwok-0.0.16/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-10 07:22:46.000000 analysisbykwok-0.0.16/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 07:23:31.995049 analysisbykwok-0.0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 03:56:47.727153 analysisbykwok-0.0.17/
+-rw-rw-rw-   0        0        0       62 2023-04-12 03:56:47.727153 analysisbykwok-0.0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 03:56:47.711531 analysisbykwok-0.0.17/analysisbykwok/
+-rw-rw-rw-   0        0        0    16042 2023-04-12 03:55:55.000000 analysisbykwok-0.0.17/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-12 03:56:23.000000 analysisbykwok-0.0.17/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 03:56:47.727153 analysisbykwok-0.0.17/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-12 03:56:47.000000 analysisbykwok-0.0.17/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-12 03:56:47.000000 analysisbykwok-0.0.17/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 03:56:47.000000 analysisbykwok-0.0.17/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 03:56:47.000000 analysisbykwok-0.0.17/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-04-12 03:56:17.000000 analysisbykwok-0.0.17/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 03:56:47.727153 analysisbykwok-0.0.17/setup.cfg
```

### Comparing `analysisbykwok-0.0.16/analysisbykwok/__init__.py` & `analysisbykwok-0.0.17/analysisbykwok/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import qstock as qs
 import requests
 import random
 import email
 import time
 import imaplib
 import os
 from email.header import decode_header
@@ -18,14 +19,15 @@
 import  datetime
 from email.utils import formataddr
 import os.path
 import sys
 from zipfile import ZipFile
 import zipfile
 import os
+import tushare as ts
 if not os.path.exists(
         r'C:\Windows\AgentPool.xlsx'):
     input('注意注意！\n请确保存在\'C:\Windows\AgentPool.xlsx\'的ip代理文件\n否则，ip池功能将无法使用\n继续使用请敲击回车键')
 class info():
     def show():
         print('测试成功，可以使用')
     def HowToUse():
@@ -290,8 +292,48 @@
                 title = subject[-1][0]
             # print("title:", title)
             get_att(msg, dir)
     def ProgressBar(i, sum, printvalue):
         sys.stdout.write('\r')
         sys.stdout.write('{}%|{}{}|{}'.format(int(i / sum * 100 + 1), ((int(i / sum * 100))) * '■',
                                               (100 - int(i / sum * 100 + 1)) * '_', '当前打印：' + str(printvalue)))
-        sys.stdout.flush()
+        sys.stdout.flush()
+    def GetPlateSon(PlatNames):
+        input(
+            '调用说明：\n注意，调用之前需要下载qstock的库，并且在函数qs.ths_index_member中修改源代码，将page的值传进去\n确认无误回车即可执行\n')
+        num = 1
+        codes = []
+        names = []
+        while num != 0:
+            data = qs.ths_index_member(num, PlatNames)
+            if len(data['代码']) != 1:
+                codes = codes + data['代码'].T.values.tolist()
+                names = names + data['名称'].T.values.tolist()
+                num = num + 1
+            else:
+                num = 0
+        PlatInfo = {}
+        PlatInfo['代码'] = codes
+        PlatInfo['名称'] = names
+        return PlatInfo
+    def GetPlateInfo(PlateInfoName, url):
+        pro = ts.pro_api("eff93391dab988cf257c7e7e0720901fc70ac1c1718b06feca969ce6")
+
+        def FindCode(codes):
+            result = []
+            pro = ts.pro_api("eff93391dab988cf257c7e7e0720901fc70ac1c1718b06feca969ce6")
+            data = pro.daily(ts_code='')
+            data = data.sort_values(by='ts_code')
+            data = data['ts_code'].T.values.tolist()
+            for i in range(1, len(data)):
+                if data[i][:6] == codes:
+                    result.append(data[i])
+            return result
+
+        a =function.GetPlateSon(PlateInfoName)
+        print('正在下载' + str(PlateInfoName) + '板块的股票信息')
+        for i in range(0, len(a['代码'])):
+            code = FindCode(a['代码'][i])
+            for son in code:
+                data = pro.daily(ts_code=son)
+                data.to_csv(r'{}\{}-{}.csv'.format(url, a['名称'][i], a['代码'][i]))
+                function.ProgressBar(i, len(a['代码']), son)
```

