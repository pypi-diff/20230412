# Comparing `tmp/qdata-0.2.3.tar.gz` & `tmp/qdata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qdata-0.2.3.tar", last modified: Tue Sep  6 10:13:55 2022, max compression
+gzip compressed data, was "dist/qdata-0.2.4.tar", last modified: Wed Apr 12 05:53:50 2023, max compression
```

## Comparing `qdata-0.2.3.tar` & `qdata-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       17 2021-03-25 14:20:13.000000 qdata-0.2.3/MANIFEST.in
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     2643 2022-09-06 10:13:55.000000 qdata-0.2.3/PKG-INFO
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     1590 2022-09-06 10:13:39.000000 qdata-0.2.3/README.md
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/examples/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)        0 2021-03-25 15:27:28.000000 qdata-0.2.3/examples/__init__.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     3365 2022-09-06 10:13:18.000000 qdata-0.2.3/examples/baidu_index_best_practice.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     2017 2022-09-06 10:13:18.000000 qdata-0.2.3/examples/test_baidu_index.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)      117 2021-03-26 10:13:55.000000 qdata-0.2.3/examples/test_baidu_login.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)      319 2021-03-25 15:27:28.000000 qdata-0.2.3/examples/test_baidu_search.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     4367 2021-04-13 01:28:42.000000 qdata-0.2.3/examples/test_tianyancha.py
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       31 2021-03-25 15:27:28.000000 qdata-0.2.3/qdata/__init__.py
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata/baidu_index/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)      239 2021-04-06 15:08:21.000000 qdata-0.2.3/qdata/baidu_index/__init__.py
--rwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)     2124 2021-03-25 15:27:28.000000 qdata-0.2.3/qdata/baidu_index/baidu_index.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     6319 2022-09-06 10:13:18.000000 qdata-0.2.3/qdata/baidu_index/common.py
--rwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)     7025 2021-03-25 15:27:28.000000 qdata-0.2.3/qdata/baidu_index/config.py
--rwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)     2588 2021-03-25 15:27:28.000000 qdata-0.2.3/qdata/baidu_index/extended_baidu_index.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     2106 2021-04-07 01:01:33.000000 qdata-0.2.3/qdata/baidu_index/live_baidu_index.py
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata/baidu_login/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       45 2021-03-26 09:41:48.000000 qdata-0.2.3/qdata/baidu_login/__init__.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     1229 2021-03-26 10:07:17.000000 qdata-0.2.3/qdata/baidu_login/common.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     4245 2021-04-13 13:13:52.000000 qdata-0.2.3/qdata/baidu_login/config.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     4170 2021-04-13 12:17:51.000000 qdata-0.2.3/qdata/baidu_login/qr_login.py
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata/baidu_search/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       53 2021-03-25 15:27:28.000000 qdata-0.2.3/qdata/baidu_search/__init__.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     2245 2021-03-25 15:27:28.000000 qdata-0.2.3/qdata/baidu_search/baidu_search.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     1419 2022-09-06 10:13:18.000000 qdata-0.2.3/qdata/errors.py
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata/tianyancha/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       53 2021-04-12 12:19:20.000000 qdata-0.2.3/qdata/tianyancha/__init__.py
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata/tianyancha/base_datas/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       54 2021-05-18 14:20:51.000000 qdata-0.2.3/qdata/tianyancha/base_datas/__init__.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)   142614 2021-05-18 14:20:33.000000 qdata-0.2.3/qdata/tianyancha/base_datas/area.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)    30520 2021-05-18 14:20:27.000000 qdata-0.2.3/qdata/tianyancha/base_datas/category.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     4166 2021-04-13 01:27:33.000000 qdata-0.2.3/qdata/tianyancha/company_count.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     1745 2021-05-18 14:22:27.000000 qdata-0.2.3/qdata/tianyancha/company_filter_options.py
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)        0 2021-03-25 15:27:28.000000 qdata-0.2.3/qdata/utils.py
-drwxr-xr-x   0 huanhuanyuzhu   (501) staff       (20)        0 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata.egg-info/
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     2643 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata.egg-info/PKG-INFO
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     1001 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata.egg-info/SOURCES.txt
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)        1 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata.egg-info/dependency_links.txt
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       56 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata.egg-info/requires.txt
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       15 2022-09-06 10:13:55.000000 qdata-0.2.3/qdata.egg-info/top_level.txt
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)       38 2022-09-06 10:13:55.000000 qdata-0.2.3/setup.cfg
--rw-r--r--   0 huanhuanyuzhu   (501) staff       (20)     1256 2022-09-06 10:13:33.000000 qdata-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 05:53:36.000000 qdata-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-12 05:53:50.000000 qdata-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-12 05:53:36.000000 qdata-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:36.000000 qdata-0.2.4/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-12 05:53:36.000000 qdata-0.2.4/examples/baidu_index_best_practice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-12 05:53:36.000000 qdata-0.2.4/examples/test_baidu_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 05:53:36.000000 qdata-0.2.4/examples/test_baidu_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 05:53:36.000000 qdata-0.2.4/examples/test_baidu_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 05:53:36.000000 qdata-0.2.4/examples/test_tianyancha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata/baidu_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_index/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2124 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_index/baidu_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_index/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7025 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_index/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2588 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_index/extended_baidu_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_index/live_baidu_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata/baidu_login/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_login/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_login/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_login/qr_login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata/baidu_search/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/baidu_search/baidu_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata/tianyancha/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/tianyancha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata/tianyancha/base_datas/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/tianyancha/base_datas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142614 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/tianyancha/base_datas/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30520 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/tianyancha/base_datas/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/tianyancha/company_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/tianyancha/company_filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:36.000000 qdata-0.2.4/qdata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 05:53:50.000000 qdata-0.2.4/qdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:53:50.000000 qdata-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-12 05:53:36.000000 qdata-0.2.4/setup.py
```

### Comparing `qdata-0.2.3/PKG-INFO` & `qdata-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python SDK for getting data quickly
 Home-page: https://github.com/longxiaofei/spider-BaiduIndex
 Author: longxiaofei
 Author-email: libra.19951002@gmail.com
 License: UNKNOWN
 Description: # Qdata - Python SDK for index and search
         
@@ -58,14 +58,20 @@
         * 2021/04/13 添加天眼查高级搜索公司数数据
         * 2021/05/18 修正打包问题
         * 2022/05/12 百度指数添加Cipher-Text(不确定部分逻辑)
         * 2022/05/16 一些小的改动
         * 2022/05/30 修正百度指数加密逻辑
         * 2022/09/06 添加检查关键词方法、添加最佳实践脚本
         
+        
+        ### Stargazers over time
+        
+        [![Stargazers over time](https://starchart.cc/longxiaofei/spider-BaiduIndex.svg)](https://starchart.cc/longxiaofei/spider-BaiduIndex)
+        
+        
 Keywords: data sdk
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qdata Version: 0.2.3 Summary: Python SDK for
+Metadata-Version: 2.1 Name: qdata Version: 0.2.4 Summary: Python SDK for
 getting data quickly Home-page: https://github.com/longxiaofei/spider-
 BaiduIndex Author: longxiaofei Author-email: libra.19951002@gmail.com License:
 UNKNOWN Description: # Qdata - Python SDK for index and search ###
 ä¸ºä»ä¹ç»é¡¹ç®æ¹äºå *
 æ³åä¸ä¸ªæä¾æ´å¤æ°æ®çSDKå,ä½ä¸ä¸å®ææ¶é´ããã *
 èçä»£ç åå¯ä»¥å¨old_baiduindexéæ¾å° *
 ä¼æ ¹æ®æèªå·±ä¸ªäººçæ°æ®éæ±ï¼å¾éé¢æ·»å ä¸åçæ°æ®æºï¼å¦ææ°å¥½å¸®å©å°ä½ ï¼å¾å¼å¿
@@ -18,13 +18,15 @@
 * å¹¸å¥½å·¥ä½ä¸åç¬è«ï¼å¿å¤ªç´¯äºã #### å¤©ç¼æ¥ `./examples/
 test_tianyancha.py` * èå©åæ±æ¥çæ¥ç¨ ### Changelog * 2021/03/25
 ä¸çº¿ * 2021/03/26 æ´æ°ç¾åº¦ç»å½åè½ * 2021/04/07 ç¾åº¦ææ°æ°å¢:
 å®æ¶ç¾åº¦ææ° * 2021/04/13 æ·»å å¤©ç¼æ¥é«çº§æç´¢å¬å¸æ°æ°æ® *
 2021/05/18 ä¿®æ­£æåé®é¢ * 2022/05/12 ç¾åº¦ææ°æ·»å Cipher-Text
 (ä¸ç¡®å®é¨åé»è¾) * 2022/05/16 ä¸äºå°çæ¹å¨ * 2022/05/30
 ä¿®æ­£ç¾åº¦ææ°å å¯é»è¾ * 2022/09/06
-æ·»å æ£æ¥å³é®è¯æ¹æ³ãæ·»å æä½³å®è·µèæ¬ Keywords: data sdk
-Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
+æ·»å æ£æ¥å³é®è¯æ¹æ³ãæ·»å æä½³å®è·µèæ¬ ### Stargazers over time
+[![Stargazers over time](https://starchart.cc/longxiaofei/spider-
+BaiduIndex.svg)](https://starchart.cc/longxiaofei/spider-BaiduIndex) Keywords:
+data sdk Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python Description-Content-Type: text/markdown
```

### Comparing `qdata-0.2.3/README.md` & `qdata-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -49,7 +49,13 @@
 * 2021/04/07 百度指数新增:实时百度指数
 * 2021/04/13 添加天眼查高级搜索公司数数据
 * 2021/05/18 修正打包问题
 * 2022/05/12 百度指数添加Cipher-Text(不确定部分逻辑)
 * 2022/05/16 一些小的改动
 * 2022/05/30 修正百度指数加密逻辑
 * 2022/09/06 添加检查关键词方法、添加最佳实践脚本
+
+
+### Stargazers over time
+
+[![Stargazers over time](https://starchart.cc/longxiaofei/spider-BaiduIndex.svg)](https://starchart.cc/longxiaofei/spider-BaiduIndex)
+
```

#### html2text {}

```diff
@@ -14,8 +14,10 @@
 * å¹¸å¥½å·¥ä½ä¸åç¬è«ï¼å¿å¤ªç´¯äºã #### å¤©ç¼æ¥ `./examples/
 test_tianyancha.py` * èå©åæ±æ¥çæ¥ç¨ ### Changelog * 2021/03/25
 ä¸çº¿ * 2021/03/26 æ´æ°ç¾åº¦ç»å½åè½ * 2021/04/07 ç¾åº¦ææ°æ°å¢:
 å®æ¶ç¾åº¦ææ° * 2021/04/13 æ·»å å¤©ç¼æ¥é«çº§æç´¢å¬å¸æ°æ°æ® *
 2021/05/18 ä¿®æ­£æåé®é¢ * 2022/05/12 ç¾åº¦ææ°æ·»å Cipher-Text
 (ä¸ç¡®å®é¨åé»è¾) * 2022/05/16 ä¸äºå°çæ¹å¨ * 2022/05/30
 ä¿®æ­£ç¾åº¦ææ°å å¯é»è¾ * 2022/09/06
-æ·»å æ£æ¥å³é®è¯æ¹æ³ãæ·»å æä½³å®è·µèæ¬
+æ·»å æ£æ¥å³é®è¯æ¹æ³ãæ·»å æä½³å®è·µèæ¬ ### Stargazers over time
+[![Stargazers over time](https://starchart.cc/longxiaofei/spider-
+BaiduIndex.svg)](https://starchart.cc/longxiaofei/spider-BaiduIndex)
```

### Comparing `qdata-0.2.3/examples/baidu_index_best_practice.py` & `qdata-0.2.4/examples/baidu_index_best_practice.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/examples/test_baidu_index.py` & `qdata-0.2.4/examples/test_baidu_index.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/examples/test_tianyancha.py` & `qdata-0.2.4/examples/test_tianyancha.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/baidu_index/baidu_index.py` & `qdata-0.2.4/qdata/baidu_index/baidu_index.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/baidu_index/common.py` & `qdata-0.2.4/qdata/baidu_index/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 
 from Crypto.Cipher import AES
 from qdata.errors import ErrorCode, QdataError
 
 import requests
 
 
+# pylint: disable=line-too-long
 headers = {
     'Host': 'index.baidu.com',
     'Connection': 'keep-alive',
     'X-Requested-With': 'XMLHttpRequest',
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36',
 }
+# pylint: enable=line-too-long
 
 
 def get_time_range_list(startdate: str, enddate: str) -> List[Tuple[str, str]]:
     """
         切分时间段
     """
     date_range_list = []
@@ -73,22 +75,22 @@
 
 def http_get(url: str, cookies: str, cipher_text: str = "") -> str:
     """
         发送get请求, 程序中所有的get都是调这个方法
         如果想使用多cookies抓取, 和请求重试功能
         在这自己添加
     """
-    _headers = headers.copy()
-    _headers['Cookie'] = cookies
+    cur_headers = headers.copy()
+    cur_headers['Cookie'] = cookies
     if cipher_text:
-        _headers["Cipher-Text"] = cipher_text
+        cur_headers["Cipher-Text"] = cipher_text
     try:
-        response = requests.get(url, headers=_headers, timeout=30)
-    except requests.Timeout:
-        raise QdataError(ErrorCode.NETWORK_ERROR)
+        response = requests.get(url, headers=cur_headers, timeout=30)
+    except requests.Timeout as exc:
+        raise QdataError(ErrorCode.NETWORK_ERROR) from exc
     if response.status_code != 200:
         raise QdataError(ErrorCode.NETWORK_ERROR)
     return response.text
 
 
 def get_key(uniqid: str, cookies: str) -> str:
     url = 'http://index.baidu.com/Interface/api/ptbk?uniqid=%s' % uniqid
```

### Comparing `qdata-0.2.3/qdata/baidu_index/config.py` & `qdata-0.2.4/qdata/baidu_index/config.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/baidu_index/extended_baidu_index.py` & `qdata-0.2.4/qdata/baidu_index/extended_baidu_index.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/baidu_index/live_baidu_index.py` & `qdata-0.2.4/qdata/baidu_index/live_baidu_index.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/baidu_login/common.py` & `qdata-0.2.4/qdata/baidu_login/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import uuid
 import hashlib
 
 from Crypto.Cipher import AES
 
 
 def _padding_pkcs7(m: str) -> str:
-    return m+chr(16-len(m)%16)*(16-len(m)%16)
+    return m+chr(16-len(m) % 16)*(16-len(m) % 16)
 
 
 def get_cur_timestamp() -> int:
     return int(datetime.now().timestamp() * 1000)
 
 
 def get_gid() -> str:
```

### Comparing `qdata-0.2.3/qdata/baidu_login/config.py` & `qdata-0.2.4/qdata/baidu_login/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,2 +1,3 @@
 # 猜测这个东西是写死的
+# pylint: disable=line-too-long
 EXIN_TOKEN = """eyJkYXRhIjoiY2E0NzE1ZDhhNTgxZTljNmE0NzQxYjJkNTJmMzIwYjRkYWYwZGMzYzIzZTk5YmE0MGY1NzRjMjVkNzkyOGMxZjkxZDRlMDU0ZTY4Mzg3ZjEyZDYzNTQ1ODU2MDRhZGZkY2NmMzlmY2NhYjkzYTYyOGZiZjBhNzJlMDJmOWZmMjQ4NDdhM2E1MjA3NTViMjc4NjQ4YWM4OGYwZmI2NTNmYTZhNjgwZGNmZTM4YWEzOGRlMTVjZTg5NTYwZDE4YjY5Y2YyMjc4Mzg5YmMzNGVmMDBmNDMwZWUyMWNhYzE0MDI5MzJmM2JlNzIyNzAwYTliZmM1YjE3OGY1ZjgxYzA2MDFkNDliZjY2ZjM3ODJkOTkzMGNiNzJkYjE3MGVjZjY2MTEyM2NiMTM5MjlmNGIyOWVmYjljM2JlYjlkZjczZDYxNGY2YWViOWNhZjNiMjhmNjE2MDMxMjllYTkyNWY1MzU1ZDAxNjcyZWNjMDYxNTNkOWMzNTJiZTEwYzc2N2E0NjgxMjUzZDQ5MGExZTQxMDVlYWRmMzZlZDM1ZWMyNzY1NjU1ZmFmNjNkNTJjYjIyMzA1NDkzMjk2NWE1MTRiNTc2Mzk0MTMxNDJjNjMyZWFmZmI0NDFiNTVkMTViZjc3N2RiMGFhYzdlNWI5MWZkM2M3MWJkMjFkY2RiZTc5MzljZWI2OGYzOWNiODM4Zjk4NTMzNzFmOGZhNjI0MjQzY2YwYjIyOWJmZmZhYTA3Y2Y2YmVkZGVkZDZkZjgzYzAzZWM4N2Q3Y2Y5MWM4ZTc5Mjc2OWIxN2VjNWI4M2FiMzJiYWI0MTk3ZDUyOTllZWVmNjU0ZTJiN2NlNjVhYTNjNDMyODI3NTMwNWJhNzRhOGFhMmQ0M2VjMTIyNDU0N2U4ZjVkNDc2N2M1ODNhZjViYjAxMjZjYmEwMTI2ZmVjNzMzNjdlZTdjYjExMDgyYzljNTQ2ZDU0YzI4ZDcxMTY5NzBjMDlmYTAzMmI0YjliNTkyZTc5MWUyZDg4ZGEyZDViN2E2YWQwZWI3OTQ0MjBjMTVhMWNiNzk5NjRlNTQzNDkzNjA4YjY2OTc1ZDlmNjRlZDMyZDMyMjE0MWY4ODIzYzNjYmY3ODM5YmU4NDQ5MDYxNjJmNDJkMzkxYTExMzU4Y2MzMjMzOWRkMWY4ZGNlM2VkZjI3YTc1NmNhN2VkMDJiOTUwNjY1NGMwZTFjMDg1Mjk2OGFiYTVlMjhkZjk4MTMzNjczOGNhZTJiZWU5ODVmOTJkMGRiN2NiMDdiMDFjMDc0ZmMzZGMwZTdlMjBjYjUxNzM0MzdiNDUzYzNhYmU1NmQ5NDU4ZDA4MjIzZmQwMGUzNTYxNmI2Zjc0ODI0YWY0Mjc5ZjJiNWU3ZjNjMmUyYTkyMzhhMjFmMjdhY2Y0ZjM0NTYwZDQxNWEwNTFlYTk4YmFkOGVlY2RhMGFlZTg2MmJkMzQyZjJmZGUxNjg0OWM1NzliMGQ0YzdkOTZhNDM3ODMyYTI1M2YzMTAxZDQzODcwZjgxZjFkOWE5YTRjYTZkN2U1ZGMxZDk1ZjhjNDM0Y2RiN2VlNTViZTJjZjM5NGUyODI4NTY3M2IxMjBjMGE1YTdkMjViMjMyMmJmODVkYjY1ODJkZWQ2MzQ0MWFhNzM1NWE1ODgyMzZhMTlmOGY4YjU3MDUyMjA0OTA1NDZmZTc0NDY0ZWMwNzk2Y2JjMmQ0MzQ3MTI1NjA4ZDc2MDViOTYwMTJkMWI1ZTgzYTBmMzdmYmYxNWE2NTYyYTM1NWNiOTk5NTNjZjI0OWIzNGE2OGE5YWVhMTcyODhiODkwZmY0MjhkNWE0NmY3ZTc5YTE3ODYwNTY2YzAxODliNDVhZmFmZDNhNWNkNmYzOTc1NzkxODFiYjYyMzVjZjIyZGI4OTY3ZTI5OTA4ODQ4Yjg2YjgzMTc4YjExMTQ2ZDdmZjEwNTM4YzFmMGRlNjU5N2QyNWQwY2JlZjYyNTkzNjVhNWM4MDY5NDVmMDdmYTQzYWVjZDNkNzg1YzE0MjM5ODNhYTI3Zjk2MzIxZDhjMjc2NTU5MGQ1ZTU2NzU0MGRkODg0YjVmMWQ1MGUzYjM1Y2U5MGVmYmJiYjNjM2RiMTg1NzJjNmIwMTkxNjQxMzc5YzBlYjRkMGI4NTkwMzE0NzllMGEzODVmYzkzNDY3YzJjMzM2MDdjZGY1YzdiZWE4ZjM2ZTYyYWYwMDRkOTQ0N2EyNzcyMGYzNDIzNWRiZWMxOGYzNzNhZmQxMDBmNjlhODM4MTYxMTZhMmZmYzdkZDNlNmMxOWM4MzZmMDJkMzdhZjk4ZjE0MDkwMzJlZTNkZjE2MDU1N2FkZDAzYzdhODcwNmJiZmU0YTk2MDk4MzkyOGExOThhZWM5Yzk2ZWYzNzdjOWRmMDczMzM3ZGIxZTQxMzc5OGExNGRhZTA2M2Y4YjEyZWZkYjY4YmM2ODljY2ZmNTkxMGM1MTI0NzQzZjFlNzkzOGE5MDYwODc5MzgzOTY4NzE3ZTU0Y2I1MDc1NzJiNWI1MmQyM2E3MzU2NTViNWZlNDljMDEyZDE0MThkNmZlMzQxYWZmZTNkN2YzNGMwZDU2MTYzMDY0ODkyNmMwODc2YzJiMGMzZTRiZGQ4Y2ZlZjg0OTk2ZGFjNGIzNmRlODRlMzJmYjM4NTI1YThjMmFhNjljMDhkYmFmNTg5ZTdmNmRjMTkyMjMwZTIxZjgyYTcyNTk3YzJiNzFmNjFlMTVlNjQwYmZlNDhiZGY3MmJlZTMyYWFhMzQ0ZDNlYjRiM2VlZjgwMjYwNDA1ZTNhYTc3OGQxMmEzYmRkNzM2MzQ1NmViZjc1ZjUxNDQzZmU0MjIyYzYyNDM5YWJhNTBhYTBhNWU5ZTkwY2FmMmJmMGJhNjIzNDhjZWMyMjQyNTU5Njk1YWE2MTEyZDI2ZDA0NGMwNjI5YWJiMTc1MDU1ZjBmZGEwNjRlN2JlZGE1YmJiOWUxMzVhZDI4OWJlOWJmOWY2YTBiZTQyZWMzZTJiNjZjNmYxMWUzMmZmODE3ZGU0YTQ5OTVjYTg5MjM5OGI2MGJkMzJkNmUzY2QzNDRjYjc1ZWEzNjdiMDg4ZTdmOWQ0ZjVjZWE4NDQ2MTFhN2QxOWQ5NmRkMDZjYzYxMDJiZDAyZGIyYzNjNzU3YzUxZmRmNDI2M2UxYmE3MmYyZDliY2M0ZWQ0ZmE4ZDA3ZGM0MTAxYjllNmU2YzcwNzlhYTVlNmQwYWIxMjI2NWIyMDM2MmM4ODkzNWZmYTQ4OTMzZDNkZWFhMzUxYzM1YjEzZTI5OTQ1OWY0NzdkN2UzMmJkZDQxMjcwZWY1OTQ3NTY5MDYxYjMzZTMwNmQ1OWY3ZGJmOTZkM2MyNmM3YTc4NjdhMTczNTNjZThjYTUzN2JjNjZkZDkzZDdhODRiNzU4MGQ4ZTUyMmVkMWY1ZmE2MjEwYWRmZTM2NjM3NzRmNWQyMTM0MDgyNmRkYTAxMjM3MWZmY2JkZWRhZGYyOWRmMzIwZGY1MTc3ODU0MzkzNmFjNTZjOGUxZmNiMzZkOWMxZmY2ODNhMjE2ZjUxNzU1NjI0YWQ2YTcxYmViZGYxMjgwNzFkZWU4ZWJkMDE0YmIyZmVkYzdhYWNkY2FiM2Y4ODk1MTg0ZjQwYTdiNWI5ZmQ5NmQ3OWE2YzNmOWJkMzA3NDQ5MGQ3Zjg0MGE3NjVmOTFlNDFjZDE2MDBmYjQ0ODI5ODJmYzA2OTE0YzRlY2M2MzRhZWY1NjM4NDE4MDFjYjM0N2Q5YmU1NThkYmMzMjI1MzY5ODYyODkxMmNmNzVmNjlmOGM2ZDA1YjlkNWQ2ZmZlM2M4MWI0NDZiMWQ1Y2E3ZjVkYTg5NDRjZTcxYWU0OGNmMGJjMTNjNjVmZjAxMTIyZGFiZjcwMDJjMDM3ZDVkMmZjMzg0M2VhN2E4YWFkY2Q2ZTk4MjdkNGIyZDYwMDdiOWQyZWEwZTc0NTU3ODlmODUwNjJjMzMzMWM4YmVkYTQ3NjA2MjYxZmE1NGE1ODVjNjYzNDliYzkzODA0Y2NjYzRlMWI2NWI0OTM4ZjkwOThlYmVmZjU0YjhkYzVjZGRhNTllMjE3NjNhNDYyNzAxZTRlYzUwYmFmNzA4YjI1YzYzMzcxYmZhNmU0NjgiLCJrZXlfaWQiOiI5NWIyYzAzZGJhNWM0M2I0In0="""
```

### Comparing `qdata-0.2.3/qdata/baidu_login/qr_login.py` & `qdata-0.2.4/qdata/baidu_login/qr_login.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,19 @@
     get_cur_timestamp,
     format_callback_resp,
     get_shaone,
     get_sig
 )
 from .config import EXIN_TOKEN
 
+# pylint: disable=line-too-long
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.182 Safari/537.36"
 }
+# pylint: enable=line-too-long
 
 session = requests.session()
 
 
 def get_qrcode_info() -> Tuple[str, str, str]:
     url = 'https://passport.baidu.com/v2/api/getqrcode'
     params = {
@@ -122,34 +124,36 @@
             resp_data['data']['lid'],
             resp_data['data']['ret_code'],
             resp_data['data']['server_time'],
             resp_data['data']['ip'],
             resp_data['sign']
         )
     elif isinstance(resp_data['data'], str):
-        __yjs_st = b64encode(quote("_".join([resp_data['data'], resp_data['key_id'], resp_data['sign']])).encode()).decode()
-        return "; __yjs_st=2_{}".format(__yjs_st)
+        yjs_st = b64encode(
+            quote("_".join([resp_data['data'], resp_data['key_id'], resp_data['sign']])).encode()
+        ).decode()
+        return "; __yjs_st=2_{}".format(yjs_st)
     else:
         raise QdataError(ErrorCode.LOGIN_FAIL)
 
 
 def get_cookie_by_qr_login() -> str:
     print("扫完码记得关闭弹出的图片框...")
 
     try:
         qrcode_link, sign, callback = get_qrcode_info()
         show_qrcode(qrcode_link)
-    except Exception:
-        raise QdataError(ErrorCode.GET_QR_FAIL)
+    except Exception as exc:
+        raise QdataError(ErrorCode.GET_QR_FAIL) from exc
 
     try:
         bduss = get_bduss(sign, callback)
         cookies = get_login_cookie(bduss)
-    except Exception:
-        raise QdataError(ErrorCode.LOGIN_FAIL)
+    except Exception as exc:
+        raise QdataError(ErrorCode.LOGIN_FAIL) from exc
 
     try:
         cookies = cookies + get_exin()
-    except Exception:
-        raise QdataError(ErrorCode.INDEX_LOGIN_FAIL)
+    except Exception as exc:
+        raise QdataError(ErrorCode.INDEX_LOGIN_FAIL) from exc
 
     return cookies
```

### Comparing `qdata-0.2.3/qdata/baidu_search/baidu_search.py` & `qdata-0.2.4/qdata/baidu_search/baidu_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,50 +20,49 @@
     'Accept-Language': 'zh-CN,zh;q=0.9',
 }
 
 
 def get_url(url: str) -> str:
     """extract special url"""
     try:
-        r = requests.get(url, allow_redirects=False)
+        r = requests.get(url, allow_redirects=False, timeout=15)
         if r.status_code == 302 and 'Location' in r.headers.keys():
             return r.headers['Location']
     except Exception:
         pass
     return ''
 
 
-def get_search(*, keyword: str, pn: int, cookies: str, domain: str = None) -> Iterator[Dict]:
+def get_search(*, keyword: str, pn: int, domain: str = None) -> Iterator[Dict]:
     keyword = 'site: {} {}'.format(domain, keyword) if domain else keyword
     params = (
         ('wd', keyword),
         ('pn', (pn - 1) * 10),
         ('oq', keyword),
         ('tn', 'baiduhome_pg'),
         ('ie', 'utf-8'),
         ('rsv_idx', '2'),
         ('rsv_pq', 'd09ea91a000533ad'),
         ('rsv_t', 'a741enhrt8jcViHd/8Q+gb0DnCzjIbctyKmpOkRk6BibYwnyQXvHFSqrZtTKeUHQlE4s'),
     )
-    response = requests.get('https://www.baidu.com/s', headers=headers, params=params)
+    response = requests.get('https://www.baidu.com/s', headers=headers, params=params, timeout=15)
     html = etree.HTML(response.text)
     items = html.xpath('//*/h3/a')
     for item in items:
         title = ''.join(item.xpath('.//text()'))
         href = item.xpath('./@href')[0]
         url = get_url(href)
         if not url:
             continue
         if domain and domain not in url:
             continue
         yield {'title': title, 'url': url}
 
 
-def get_all_search(*, keyword: str, cookies: str, domain: str = None) -> Iterator[Dict]:
+def get_all_search(*, keyword: str, domain: str = None, cookies: str) -> Iterator[Dict]:
     for pn in range(1, 76):
         for item in get_search(
             keyword=keyword,
             pn=pn,
-            cookies=compile,
             domain=domain
         ):
             yield item
```

### Comparing `qdata-0.2.3/qdata/errors.py` & `qdata-0.2.4/qdata/errors.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/tianyancha/base_datas/area.py` & `qdata-0.2.4/qdata/tianyancha/base_datas/area.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/tianyancha/base_datas/category.py` & `qdata-0.2.4/qdata/tianyancha/base_datas/category.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/tianyancha/company_count.py` & `qdata-0.2.4/qdata/tianyancha/company_count.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata/tianyancha/company_filter_options.py` & `qdata-0.2.4/qdata/tianyancha/company_filter_options.py`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/qdata.egg-info/PKG-INFO` & `qdata-0.2.4/qdata.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python SDK for getting data quickly
 Home-page: https://github.com/longxiaofei/spider-BaiduIndex
 Author: longxiaofei
 Author-email: libra.19951002@gmail.com
 License: UNKNOWN
 Description: # Qdata - Python SDK for index and search
         
@@ -58,14 +58,20 @@
         * 2021/04/13 添加天眼查高级搜索公司数数据
         * 2021/05/18 修正打包问题
         * 2022/05/12 百度指数添加Cipher-Text(不确定部分逻辑)
         * 2022/05/16 一些小的改动
         * 2022/05/30 修正百度指数加密逻辑
         * 2022/09/06 添加检查关键词方法、添加最佳实践脚本
         
+        
+        ### Stargazers over time
+        
+        [![Stargazers over time](https://starchart.cc/longxiaofei/spider-BaiduIndex.svg)](https://starchart.cc/longxiaofei/spider-BaiduIndex)
+        
+        
 Keywords: data sdk
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qdata Version: 0.2.3 Summary: Python SDK for
+Metadata-Version: 2.1 Name: qdata Version: 0.2.4 Summary: Python SDK for
 getting data quickly Home-page: https://github.com/longxiaofei/spider-
 BaiduIndex Author: longxiaofei Author-email: libra.19951002@gmail.com License:
 UNKNOWN Description: # Qdata - Python SDK for index and search ###
 ä¸ºä»ä¹ç»é¡¹ç®æ¹äºå *
 æ³åä¸ä¸ªæä¾æ´å¤æ°æ®çSDKå,ä½ä¸ä¸å®ææ¶é´ããã *
 èçä»£ç åå¯ä»¥å¨old_baiduindexéæ¾å° *
 ä¼æ ¹æ®æèªå·±ä¸ªäººçæ°æ®éæ±ï¼å¾éé¢æ·»å ä¸åçæ°æ®æºï¼å¦ææ°å¥½å¸®å©å°ä½ ï¼å¾å¼å¿
@@ -18,13 +18,15 @@
 * å¹¸å¥½å·¥ä½ä¸åç¬è«ï¼å¿å¤ªç´¯äºã #### å¤©ç¼æ¥ `./examples/
 test_tianyancha.py` * èå©åæ±æ¥çæ¥ç¨ ### Changelog * 2021/03/25
 ä¸çº¿ * 2021/03/26 æ´æ°ç¾åº¦ç»å½åè½ * 2021/04/07 ç¾åº¦ææ°æ°å¢:
 å®æ¶ç¾åº¦ææ° * 2021/04/13 æ·»å å¤©ç¼æ¥é«çº§æç´¢å¬å¸æ°æ°æ® *
 2021/05/18 ä¿®æ­£æåé®é¢ * 2022/05/12 ç¾åº¦ææ°æ·»å Cipher-Text
 (ä¸ç¡®å®é¨åé»è¾) * 2022/05/16 ä¸äºå°çæ¹å¨ * 2022/05/30
 ä¿®æ­£ç¾åº¦ææ°å å¯é»è¾ * 2022/09/06
-æ·»å æ£æ¥å³é®è¯æ¹æ³ãæ·»å æä½³å®è·µèæ¬ Keywords: data sdk
-Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
+æ·»å æ£æ¥å³é®è¯æ¹æ³ãæ·»å æä½³å®è·µèæ¬ ### Stargazers over time
+[![Stargazers over time](https://starchart.cc/longxiaofei/spider-
+BaiduIndex.svg)](https://starchart.cc/longxiaofei/spider-BaiduIndex) Keywords:
+data sdk Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python Description-Content-Type: text/markdown
```

### Comparing `qdata-0.2.3/qdata.egg-info/SOURCES.txt` & `qdata-0.2.4/qdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qdata-0.2.3/setup.py` & `qdata-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 import os
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 
 CUR_DIR = os.path.abspath(os.path.dirname(__file__))
 README = os.path.join(CUR_DIR, "README.md")
 with open("README.md", "r") as fd:
     long_description = fd.read()
 
 setuptools.setup(
```

