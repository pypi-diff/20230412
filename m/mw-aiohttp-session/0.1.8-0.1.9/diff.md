# Comparing `tmp/mw-aiohttp-session-0.1.8.tar.gz` & `tmp/mw-aiohttp-session-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mw-aiohttp-session-0.1.8.tar", last modified: Thu Jul  9 06:56:43 2020, max compression
+gzip compressed data, was "dist\mw-aiohttp-session-0.1.9.tar", last modified: Mon May 10 02:53:28 2021, max compression
```

## Comparing `mw-aiohttp-session-0.1.8.tar` & `mw-aiohttp-session-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/
--rw-rw-rw-   0        0        0       23 2020-07-09 06:55:37.000000 mw-aiohttp-session-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      827 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      215 2020-07-09 06:44:55.000000 mw-aiohttp-session-0.1.8/README.md
--rw-rw-rw-   0        0        0      193 2020-06-30 01:21:20.000000 mw-aiohttp-session-0.1.8/README.rst
-drwxrwxrwx   0        0        0        0 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session/
--rw-rw-rw-   0        0        0      100 2018-10-09 08:30:34.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session/__init__.py
--rw-rw-rw-   0        0        0     4983 2020-06-29 08:17:09.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session/redis_storage.py
-drwxrwxrwx   0        0        0        0 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session.egg-info/
--rw-rw-rw-   0        0        0      827 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/mw_aiohttp_session.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-07-09 06:56:43.000000 mw-aiohttp-session-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1005 2020-07-09 06:56:37.000000 mw-aiohttp-session-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-10 02:53:28.000000 mw-aiohttp-session-0.1.9/
+-rw-rw-rw-   0        0        0       23 2021-05-10 02:50:50.000000 mw-aiohttp-session-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      827 2021-05-10 02:53:28.000000 mw-aiohttp-session-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2018-10-30 09:50:37.000000 mw-aiohttp-session-0.1.9/README.md
+-rw-rw-rw-   0        0        0      193 2021-05-10 02:50:50.000000 mw-aiohttp-session-0.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2021-05-10 02:53:28.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session/
+-rw-rw-rw-   0        0        0      100 2018-10-09 08:20:57.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session/__init__.py
+-rw-rw-rw-   0        0        0     5048 2021-05-10 02:33:37.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session/redis_storage.py
+drwxrwxrwx   0        0        0        0 2021-05-10 02:53:28.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session.egg-info/
+-rw-rw-rw-   0        0        0      827 2021-05-10 02:53:27.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2021-05-10 02:53:28.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-10 02:53:27.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2021-05-10 02:53:27.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2021-05-10 02:53:27.000000 mw-aiohttp-session-0.1.9/mw_aiohttp_session.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-05-10 02:53:28.000000 mw-aiohttp-session-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2021-05-10 02:53:03.000000 mw-aiohttp-session-0.1.9/setup.py
```

### Comparing `mw-aiohttp-session-0.1.8/PKG-INFO` & `mw-aiohttp-session-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mw-aiohttp-session
-Version: 0.1.8
+Version: 0.1.9
 Summary: maxwin aiohttp-session 
 Home-page: https://bitbucket.org/maxwin-inc/mw-aiohttp-session/src
 Author: candyabc
 Author-email: hfcandyabc@163.com
 License: UNKNOWN
 Description: ###产生分发包
         ``
```

### Comparing `mw-aiohttp-session-0.1.8/mw_aiohttp_session/redis_storage.py` & `mw-aiohttp-session-0.1.9/mw_aiohttp_session/redis_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if isinstance(redis_pool, aioredis.pool.ConnectionsPool):
             warnings.warn(
                 "using a pool created with aioredis.create_pool is deprecated"
                 "please use a pool created with aioredis.create_redis_pool",
                 DeprecationWarning
             )
             redis_pool = aioredis.commands.Redis(redis_pool)
-        elif not isinstance(redis_pool, aioredis.commands.Redis):
+        elif not isinstance(redis_pool, aioredis.commands.Redis) and not isinstance(redis_pool, aioredis.sentinel.RedisSentinel) :
             raise TypeError("Expexted aioredis.commands.Redis got {}".format(
                     type(redis_pool)))
         self._redis = redis_pool
 
     def load_cookie(self, request):
         # 如果有jwt，优先判断jwt，避免cookie与jwt不一致
         cookie = request.query.get('jwt')
```

### Comparing `mw-aiohttp-session-0.1.8/mw_aiohttp_session.egg-info/PKG-INFO` & `mw-aiohttp-session-0.1.9/mw_aiohttp_session.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mw-aiohttp-session
-Version: 0.1.8
+Version: 0.1.9
 Summary: maxwin aiohttp-session 
 Home-page: https://bitbucket.org/maxwin-inc/mw-aiohttp-session/src
 Author: candyabc
 Author-email: hfcandyabc@163.com
 License: UNKNOWN
 Description: ###产生分发包
         ``
```

### Comparing `mw-aiohttp-session-0.1.8/setup.py` & `mw-aiohttp-session-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
-# from codecs import open
+from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='mw-aiohttp-session',
-    version='0.1.8',
+    version='0.1.9',
     description='maxwin aiohttp-session ',
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://bitbucket.org/maxwin-inc/mw-aiohttp-session/src',  # Optional
     author='candyabc',  # Optional
     author_email='hfcandyabc@163.com',  # Optional
     packages=find_packages(),  # Required
```

