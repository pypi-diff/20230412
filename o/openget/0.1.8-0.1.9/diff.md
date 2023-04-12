# Comparing `tmp/openget-0.1.8.tar.gz` & `tmp/openget-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openget-0.1.8.tar", last modified: Sun Jan 15 05:54:11 2023, max compression
+gzip compressed data, was "openget-0.1.9.tar", last modified: Wed Apr 12 11:17:24 2023, max compression
```

## Comparing `openget-0.1.8.tar` & `openget-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.428867 openget-0.1.8/
--rw-r--r--   0 dytttf     (501) staff       (20)     1514 2022-07-21 15:26:26.000000 openget-0.1.8/LICENSE
--rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-01-15 05:54:11.428715 openget-0.1.8/PKG-INFO
--rw-r--r--   0 dytttf     (501) staff       (20)      505 2023-01-14 16:55:04.000000 openget-0.1.8/README.md
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.424458 openget-0.1.8/openget/
--rw-r--r--   0 dytttf     (501) staff       (20)       40 2023-01-14 16:55:04.000000 openget-0.1.8/openget/__init__.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.426433 openget-0.1.8/openget/db/
--rw-r--r--   0 dytttf     (501) staff       (20)      125 2023-01-14 16:55:04.000000 openget-0.1.8/openget/db/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     2327 2023-01-14 16:55:04.000000 openget-0.1.8/openget/db/db.py
--rw-r--r--   0 dytttf     (501) staff       (20)    17596 2023-01-15 05:30:00.000000 openget-0.1.8/openget/db/db_mysql.py
--rw-r--r--   0 dytttf     (501) staff       (20)    12619 2023-01-14 16:55:04.000000 openget-0.1.8/openget/db/db_oracle.py
--rw-r--r--   0 dytttf     (501) staff       (20)    38448 2023-01-14 16:55:04.000000 openget-0.1.8/openget/db/db_oss.py
--rw-r--r--   0 dytttf     (501) staff       (20)     3229 2023-01-14 16:55:04.000000 openget-0.1.8/openget/db/db_redis.py
--rw-r--r--   0 dytttf     (501) staff       (20)    14416 2023-01-14 16:55:04.000000 openget-0.1.8/openget/db/db_sqlite.py
--rw-r--r--   0 dytttf     (501) staff       (20)      837 2023-01-14 16:55:04.000000 openget-0.1.8/openget/db/util.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1765 2023-01-14 16:55:04.000000 openget-0.1.8/openget/env.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.427142 openget-0.1.8/openget/network/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.8/openget/network/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)    17631 2023-01-14 16:55:04.000000 openget-0.1.8/openget/network/downloader.py
--rw-r--r--   0 dytttf     (501) staff       (20)    25746 2023-01-14 16:55:04.000000 openget-0.1.8/openget/network/proxy.py
--rw-r--r--   0 dytttf     (501) staff       (20)      811 2023-01-14 16:55:04.000000 openget-0.1.8/openget/network/request.py
--rw-r--r--   0 dytttf     (501) staff       (20)     3533 2023-01-14 16:55:04.000000 openget-0.1.8/openget/network/response.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1354 2023-01-14 16:55:04.000000 openget-0.1.8/openget/setting.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.427787 openget-0.1.8/openget/spiders/
--rw-r--r--   0 dytttf     (501) staff       (20)      522 2023-01-14 16:55:04.000000 openget-0.1.8/openget/spiders/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)    15507 2023-01-14 16:55:04.000000 openget-0.1.8/openget/spiders/base.py
--rw-r--r--   0 dytttf     (501) staff       (20)    54681 2023-01-14 16:55:04.000000 openget-0.1.8/openget/spiders/batch_spider.py
--rw-r--r--   0 dytttf     (501) staff       (20)    38777 2023-01-14 16:55:04.000000 openget-0.1.8/openget/util.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.428177 openget-0.1.8/openget/utils/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.8/openget/utils/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     2605 2023-01-14 16:55:04.000000 openget-0.1.8/openget/utils/log.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.428454 openget-0.1.8/openget/utils/message/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.8/openget/utils/message/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1842 2023-01-14 16:55:04.000000 openget-0.1.8/openget/utils/message/dingtalk.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-01-15 05:54:11.425028 openget-0.1.8/openget.egg-info/
--rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-01-15 05:54:11.000000 openget-0.1.8/openget.egg-info/PKG-INFO
--rw-r--r--   0 dytttf     (501) staff       (20)      776 2023-01-15 05:54:11.000000 openget-0.1.8/openget.egg-info/SOURCES.txt
--rw-r--r--   0 dytttf     (501) staff       (20)        1 2023-01-15 05:54:11.000000 openget-0.1.8/openget.egg-info/dependency_links.txt
--rw-r--r--   0 dytttf     (501) staff       (20)      101 2023-01-15 05:54:11.000000 openget-0.1.8/openget.egg-info/requires.txt
--rw-r--r--   0 dytttf     (501) staff       (20)        8 2023-01-15 05:54:11.000000 openget-0.1.8/openget.egg-info/top_level.txt
--rw-r--r--   0 dytttf     (501) staff       (20)      809 2023-01-14 16:55:04.000000 openget-0.1.8/pyproject.toml
--rw-r--r--   0 dytttf     (501) staff       (20)       38 2023-01-15 05:54:11.428913 openget-0.1.8/setup.cfg
--rw-r--r--   0 dytttf     (501) staff       (20)     1015 2023-01-14 16:55:04.000000 openget-0.1.8/setup.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.865245 openget-0.1.9/
+-rw-r--r--   0 dytttf     (501) staff       (20)     1514 2022-07-21 15:26:26.000000 openget-0.1.9/LICENSE
+-rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-12 11:17:24.865134 openget-0.1.9/PKG-INFO
+-rw-r--r--   0 dytttf     (501) staff       (20)      505 2023-01-14 16:55:04.000000 openget-0.1.9/README.md
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.861880 openget-0.1.9/openget/
+-rw-r--r--   0 dytttf     (501) staff       (20)       40 2023-04-12 11:16:05.000000 openget-0.1.9/openget/__init__.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.863428 openget-0.1.9/openget/db/
+-rw-r--r--   0 dytttf     (501) staff       (20)      125 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     2327 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    17596 2023-04-12 11:15:21.000000 openget-0.1.9/openget/db/db_mysql.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    12619 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_oracle.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    38448 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_oss.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     3229 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_redis.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    14416 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_sqlite.py
+-rw-r--r--   0 dytttf     (501) staff       (20)      837 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/util.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1765 2023-01-14 16:55:04.000000 openget-0.1.9/openget/env.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864057 openget-0.1.9/openget/network/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    17631 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/downloader.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    25746 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/proxy.py
+-rw-r--r--   0 dytttf     (501) staff       (20)      811 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/request.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     3533 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/response.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1354 2023-01-14 16:55:04.000000 openget-0.1.9/openget/setting.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864501 openget-0.1.9/openget/spiders/
+-rw-r--r--   0 dytttf     (501) staff       (20)      522 2023-01-14 16:55:04.000000 openget-0.1.9/openget/spiders/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    15507 2023-01-14 16:55:04.000000 openget-0.1.9/openget/spiders/base.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    54681 2023-01-14 16:55:04.000000 openget-0.1.9/openget/spiders/batch_spider.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    38777 2023-01-14 16:55:04.000000 openget-0.1.9/openget/util.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864773 openget-0.1.9/openget/utils/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     2605 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/log.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864966 openget-0.1.9/openget/utils/message/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/message/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1842 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/message/dingtalk.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.862452 openget-0.1.9/openget.egg-info/
+-rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/PKG-INFO
+-rw-r--r--   0 dytttf     (501) staff       (20)      776 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/SOURCES.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)        1 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/dependency_links.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)       89 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/requires.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)        8 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/top_level.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)      810 2023-04-12 11:15:21.000000 openget-0.1.9/pyproject.toml
+-rw-r--r--   0 dytttf     (501) staff       (20)       38 2023-04-12 11:17:24.865275 openget-0.1.9/setup.cfg
+-rw-r--r--   0 dytttf     (501) staff       (20)     1017 2023-04-12 11:15:21.000000 openget-0.1.9/setup.py
```

### Comparing `openget-0.1.8/LICENSE` & `openget-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/PKG-INFO` & `openget-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openget
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Spider FrameWork
 Home-page: https://github.com/dytttf/openget
 Author: Dytttf
 Author-email: dytttf@foxmail.com
 License: BSD
 Keywords: openget,spider,batch-spider
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openget-0.1.8/openget/db/db.py` & `openget-0.1.9/openget/db/db.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/db/db_mysql.py` & `openget-0.1.9/openget/db/db_mysql.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/db/db_oracle.py` & `openget-0.1.9/openget/db/db_oracle.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/db/db_oss.py` & `openget-0.1.9/openget/db/db_oss.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/db/db_redis.py` & `openget-0.1.9/openget/db/db_redis.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/db/db_sqlite.py` & `openget-0.1.9/openget/db/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/db/util.py` & `openget-0.1.9/openget/db/util.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/env.py` & `openget-0.1.9/openget/env.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/network/downloader.py` & `openget-0.1.9/openget/network/downloader.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/network/proxy.py` & `openget-0.1.9/openget/network/proxy.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/network/request.py` & `openget-0.1.9/openget/network/request.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/network/response.py` & `openget-0.1.9/openget/network/response.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/setting.py` & `openget-0.1.9/openget/setting.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/spiders/__init__.py` & `openget-0.1.9/openget/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/spiders/base.py` & `openget-0.1.9/openget/spiders/base.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/spiders/batch_spider.py` & `openget-0.1.9/openget/spiders/batch_spider.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/util.py` & `openget-0.1.9/openget/util.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/utils/log.py` & `openget-0.1.9/openget/utils/log.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget/utils/message/dingtalk.py` & `openget-0.1.9/openget/utils/message/dingtalk.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/openget.egg-info/PKG-INFO` & `openget-0.1.9/openget.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openget
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Spider FrameWork
 Home-page: https://github.com/dytttf/openget
 Author: Dytttf
 Author-email: dytttf@foxmail.com
 License: BSD
 Keywords: openget,spider,batch-spider
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openget-0.1.8/openget.egg-info/SOURCES.txt` & `openget-0.1.9/openget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openget-0.1.8/pyproject.toml` & `openget-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 python = "^3.8"
 urllib3 = "^1.26.7"
 gevent = "^21.8.0"
 pymysql = "^1.0.2"
 redis = "^3.5.3"
 better-exceptions = "^0.3.3"
 tqdm = "^4.62.3"
-mysqlclient = "^2.0.3"
+#mysqlclient = "^2.0.3"
 httpx = {extras = ["http2"], version = "^0.20.0"}
 user-agent2 = "^2021.11.1"
 crontab = "^0.23.0"
 oss2 = "^2.15.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.3.0"
```

### Comparing `openget-0.1.8/setup.py` & `openget-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author="Dytttf",
     author_email="dytttf@foxmail.com",
     url="https://github.com/dytttf/openget",
     packages=find_packages(),
     install_requires=[
         "gevent",
         "pymysql",
-        "mysqlclient",
+        # "mysqlclient",
         "redis>=3.0.0",
         "better-exceptions",
         "tqdm",
         "httpx[http2]",
         "user-agent2",
         "urllib3",
         "oss2",
```

