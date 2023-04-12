# Comparing `tmp/hagworm-5.4.1.tar.gz` & `tmp/hagworm-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.4.1.tar", last modified: Tue Apr 11 10:21:55 2023, max compression
+gzip compressed data, was "hagworm-5.4.2.tar", last modified: Wed Apr 12 09:04:36 2023, max compression
```

## Comparing `hagworm-5.4.1.tar` & `hagworm-5.4.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.691665 hagworm-5.4.1/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.1/LICENSE
--rw-rw-rw-   0        0        0     7509 2023-04-11 10:21:55.690665 hagworm-5.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.589665 hagworm-5.4.1/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.1/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.592665 hagworm-5.4.1/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.597664 hagworm-5.4.1/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.600664 hagworm-5.4.1/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.601665 hagworm-5.4.1/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.602664 hagworm-5.4.1/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.1/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.604664 hagworm-5.4.1/hagworm/
--rw-rw-rw-   0        0        0      510 2023-04-11 09:57:01.000000 hagworm-5.4.1/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.638665 hagworm-5.4.1/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.662665 hagworm-5.4.1/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.1/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.1/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     2967 2023-04-11 09:13:15.000000 hagworm-5.4.1/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.1/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    14359 2023-04-11 09:19:20.000000 hagworm-5.4.1/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    10611 2023-04-11 07:37:23.000000 hagworm-5.4.1/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     3787 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.1/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22499 2023-04-11 09:35:01.000000 hagworm-5.4.1/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1742 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1717 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4205 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2106 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14031 2023-04-08 01:06:26.000000 hagworm-5.4.1/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.1/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     3555 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     6914 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3620 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.666665 hagworm-5.4.1/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.673665 hagworm-5.4.1/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     7853 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.676664 hagworm-5.4.1/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.677665 hagworm-5.4.1/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.681666 hagworm-5.4.1/hagworm/third/aliyun/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/aliyun/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/aliyun/logging.py
--rw-rw-rw-   0        0        0    10135 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/aliyun/rocketmq.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.684665 hagworm-5.4.1/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.689665 hagworm-5.4.1/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.1/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-04-08 01:06:26.000000 hagworm-5.4.1/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:21:55.611665 hagworm-5.4.1/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7509 2023-04-11 10:21:55.000000 hagworm-5.4.1/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2262 2023-04-11 10:21:55.000000 hagworm-5.4.1/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 10:21:55.000000 hagworm-5.4.1/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      707 2023-04-11 10:21:55.000000 hagworm-5.4.1/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 10:21:55.000000 hagworm-5.4.1/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 10:21:55.691665 hagworm-5.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.678876 hagworm-5.4.2/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.2/LICENSE
+-rw-rw-rw-   0        0        0     7509 2023-04-12 09:04:36.677875 hagworm-5.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.541873 hagworm-5.4.2/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.2/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.544873 hagworm-5.4.2/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.550873 hagworm-5.4.2/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.553873 hagworm-5.4.2/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.555873 hagworm-5.4.2/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.557874 hagworm-5.4.2/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.2/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.559873 hagworm-5.4.2/hagworm/
+-rw-rw-rw-   0        0        0      510 2023-04-12 09:01:18.000000 hagworm-5.4.2/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.601873 hagworm-5.4.2/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.636874 hagworm-5.4.2/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.2/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.2/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     3073 2023-04-12 08:05:02.000000 hagworm-5.4.2/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.2/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    14412 2023-04-12 08:15:17.000000 hagworm-5.4.2/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    10611 2023-04-11 07:37:23.000000 hagworm-5.4.2/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     3787 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.2/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22551 2023-04-12 08:21:47.000000 hagworm-5.4.2/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1759 2023-04-12 08:23:58.000000 hagworm-5.4.2/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1699 2023-04-12 08:24:47.000000 hagworm-5.4.2/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4251 2023-04-12 08:28:34.000000 hagworm-5.4.2/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2208 2023-04-12 08:06:38.000000 hagworm-5.4.2/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14060 2023-04-12 08:30:31.000000 hagworm-5.4.2/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.2/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     3555 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     6909 2023-04-12 08:32:50.000000 hagworm-5.4.2/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3620 2023-04-12 08:40:57.000000 hagworm-5.4.2/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.642873 hagworm-5.4.2/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.654876 hagworm-5.4.2/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     7849 2023-04-12 08:55:19.000000 hagworm-5.4.2/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.657876 hagworm-5.4.2/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.659876 hagworm-5.4.2/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.665876 hagworm-5.4.2/hagworm/third/aliyun/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/third/aliyun/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/third/aliyun/logging.py
+-rw-rw-rw-   0        0        0    10141 2023-04-12 08:57:49.000000 hagworm-5.4.2/hagworm/third/aliyun/rocketmq.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.668876 hagworm-5.4.2/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.675876 hagworm-5.4.2/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3437 2023-04-12 09:00:41.000000 hagworm-5.4.2/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.2/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.4.2/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:04:36.567873 hagworm-5.4.2/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7509 2023-04-12 09:04:36.000000 hagworm-5.4.2/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2262 2023-04-12 09:04:36.000000 hagworm-5.4.2/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:04:36.000000 hagworm-5.4.2/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      707 2023-04-12 09:04:36.000000 hagworm-5.4.2/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-12 09:04:36.000000 hagworm-5.4.2/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:04:36.678876 hagworm-5.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.2/setup.py
```

### Comparing `hagworm-5.4.1/LICENSE` & `hagworm-5.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/PKG-INFO` & `hagworm-5.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.1
+Version: 5.4.2
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.1/README.md` & `hagworm-5.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/c_extend/math.c` & `hagworm-5.4.2/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.4.2/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/example/fastapi_demo/main.py` & `hagworm-5.4.2/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/example/fastapi_demo/service/__init__.py` & `hagworm-5.4.2/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/example/fastapi_demo/setting.py` & `hagworm-5.4.2/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/example/main_test.py` & `hagworm-5.4.2/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/base.py` & `hagworm-5.4.2/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/buffer.py` & `hagworm-5.4.2/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/command.py` & `hagworm-5.4.2/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/event.py` & `hagworm-5.4.2/hagworm/extend/asyncio/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,28 +36,34 @@
 
         async for _ in AsyncCirculatorForSecond():
 
             with catch_error():
 
                 receiver = self._redis_client.pubsub(ignore_subscribe_messages=True)
 
-                with catch_error():
+                try:
 
                     await receiver.subscribe(channel)
 
                     Utils.log.info(f'event bus channel({channel}) receiver created')
 
                     while True:
 
                         message = await receiver.get_message(timeout=10)
 
                         if message:
                             await self._event_assigner(message)
 
-                await receiver.close()
+                except Exception as err:
+
+                    Utils.log.warning(str(err))
+
+                finally:
+
+                    await receiver.close()
 
     async def _event_assigner(self, message):
 
         data = Utils.msgpack_decode(message[r'data'])
 
         _type = data.get(r'type', r'')
         args = data.get(r'args', [])
```

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/file.py` & `hagworm-5.4.2/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/future.py` & `hagworm-5.4.2/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/mail.py` & `hagworm-5.4.2/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/mongo.py` & `hagworm-5.4.2/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/mysql.py` & `hagworm-5.4.2/hagworm/extend/asyncio/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,16 @@
             *, name=None, minsize=8, maxsize=32, echo=False, pool_recycle=21600,
             charset=r'utf8', autocommit=True, cursorclass=aiomysql.DictCursor,
             readonly=False, conn_life=43200,
             **settings
     ):
 
         self._name = name if name is not None else (Utils.uuid1()[:8] + (r'_ro' if readonly else r'_rw'))
-        self._pool = None
-        self._engine = None
+        self._pool: aiomysql.pool.Pool = None
+        self._engine: Engine = None
         self._readonly = readonly
         self._conn_life = conn_life
 
         self._settings = settings
 
         self._settings[r'host'] = host
         self._settings[r'port'] = port
@@ -218,21 +218,21 @@
         return result
 
     async def _check_health(self, pool):
 
         if pool is None:
             return True
 
-        async with pool.get_client() as client:
+        result = False
 
+        async with pool.get_client() as client:
             await client.safe_execute(r'select version();')
+            result = True
 
-            return True
-
-        return False
+        return result
 
     async def reset_mysql_pool(self):
 
         if self._mysql_rw_pool:
             await self._mysql_rw_pool.reset()
 
         if self._mysql_ro_pool:
```

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/net.py` & `hagworm-5.4.2/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/ntp.py` & `hagworm-5.4.2/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/pool.py` & `hagworm-5.4.2/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/redis.py` & `hagworm-5.4.2/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/socket.py` & `hagworm-5.4.2/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/task.py` & `hagworm-5.4.2/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/transaction.py` & `hagworm-5.4.2/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/asyncio/zmq.py` & `hagworm-5.4.2/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/base.py` & `hagworm-5.4.2/hagworm/extend/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 __author__ = r'wsb310@gmail.com'
 
 import os
 import re
 import sys
 import platform
-import traceback
 import uuid
 import time
 import math
 import string
 import random
 import hashlib
 import base64
@@ -681,18 +680,21 @@
     def jwt_encode(cls, val, key, algorithms=r'HS256'):
 
         result = jwt.encode(val, key, algorithms)
 
         return cls.basestring(result)
 
     @classmethod
-    def jwt_decode(cls, val, key, algorithms=[r'HS256']):
+    def jwt_decode(cls, val, key, algorithms=None):
 
         val = cls.utf8(val)
 
+        if algorithms is None:
+            algorithms = [r'HS256']
+
         return jwt.decode(val, key, algorithms)
 
     @classmethod
     def yaml_encode(cls, data, stream=None):
 
         return yaml.safe_dump(data, stream)
 
@@ -995,16 +997,16 @@
         self._callables = set()
 
     def __call__(self, *args, **kwargs):
 
         for func in self._callables:
             try:
                 func(*args, **kwargs)
-            except:
-                Utils.log.error(traceback.format_exc())
+            except Exception as err:
+                Utils.log.exception(str(err))
 
     @property
     def is_valid(self):
 
         return len(self._callables) > 0
 
     def add(self, func):
```

### Comparing `hagworm-5.4.1/hagworm/extend/cache.py` & `hagworm-5.4.2/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/compile.py` & `hagworm-5.4.2/hagworm/extend/compile.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import argparse
 import py_compile
 
 from .base import Utils
 
 
-def compile(file_path, cfile_path=None, exclude=None):
+def compile_pyc(file_path, pyc_file_path=None, exclude=None):
     """PYC编译函数
     """
 
     if exclude:
         exclude = [os.path.join(file_path, val) for val in Utils.split_str(exclude, r'|')]
     else:
         exclude = []
@@ -32,21 +32,21 @@
             for _file in files:
 
                 _, ext_name = os.path.splitext(_file)
 
                 if ext_name != r'.py':
                     continue
 
-                if cfile_path is None:
+                if pyc_file_path is None:
 
                     dest_path = file_path
 
                 else:
 
-                    dest_path = root.replace(file_path, cfile_path)
+                    dest_path = root.replace(file_path, pyc_file_path)
 
                     if not os.path.exists(dest_path):
                         os.makedirs(dest_path)
 
                 ori_path = os.path.join(root, _file)
                 dest_path = os.path.join(dest_path, _file) + r'c'
 
@@ -64,15 +64,15 @@
     parser.add_argument(r'-i', r'--input', default=r'./', dest=r'input')
     parser.add_argument(r'-o', r'--output', default=None, dest=r'output')
     parser.add_argument(r'-e', r'--exclude', default=None, dest=r'exclude')
 
     args = parser.parse_args()
 
     try:
-        compile(args.input, args.output, args.exclude)
+        compile_pyc(args.input, args.output, args.exclude)
     except Exception as error:
         sys.stderr.write(f'{error}\n')
 
     return result
 
 
 if __name__ == r'__main__':
```

### Comparing `hagworm-5.4.1/hagworm/extend/config.py` & `hagworm-5.4.2/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/crypto.py` & `hagworm-5.4.2/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/error.py` & `hagworm-5.4.2/hagworm/extend/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
 
 __author__ = r'wsb310@gmail.com'
 
-import traceback
-
 from contextlib import contextmanager
 
 from .base import Utils
 
 
 # 基础异常
 class BaseError(Exception):
```

### Comparing `hagworm-5.4.1/hagworm/extend/event.py` & `hagworm-5.4.2/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/igraph.py` & `hagworm-5.4.2/hagworm/extend/igraph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 __author__ = r'wsb310@gmail.com'
 
-from typing import List, Tuple, Dict
+from typing import Union, List, Tuple, Dict
 from igraph import Graph as _Graph, Vertex, VertexSeq, Edge, EdgeSeq
 
 
 class Graph:
 
     def __init__(self, directed: bool, name: str):
 
@@ -68,15 +68,15 @@
 
         return vertex
 
     def init_edges(self, edges: List[Tuple[Vertex]]):
 
         self._graph.add_edges(edges)
 
-    def get_edge(self, source: Vertex, target: Vertex) -> Edge:
+    def get_edge(self, source: Vertex, target: Vertex) -> Union[Edge, None]:
 
         eid = self._graph.get_eid(source[r'name'], target[r'name'], error=False)
 
         if eid < 0:
             return None
 
         return self._graph.es[eid]
@@ -126,24 +126,24 @@
 
 class DiGraph(Graph):
 
     def __init__(self, name: str):
 
         super().__init__(True, name)
 
-    def find_in(self, name: str) -> List[Vertex]:
+    def find_in(self, name: str) -> Union[List[Vertex], None]:
 
         vertex = self.find_vertex(name)
 
         if vertex is None:
             return None
 
         return vertex.predecessors()
 
-    def find_out(self, name: str) -> List[Vertex]:
+    def find_out(self, name: str) -> Union[List[Vertex], None]:
 
         vertex = self.find_vertex(name)
 
         if vertex is None:
             return None
 
         return vertex.successors()
```

### Comparing `hagworm-5.4.1/hagworm/extend/interface.py` & `hagworm-5.4.2/hagworm/extend/interface.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,45 +8,45 @@
 from .error import Ignore
 
 
 class FunctorInterface:
     """仿函数接口定义
     """
 
-    def __call__(self):
+    def __call__(self, *args, **kwargs):
         raise NotImplementedError()
 
 
 class RunnableInterface:
     """Runnable接口定义
     """
 
-    def run(self):
+    def run(self, *args, **kwargs):
         raise NotImplementedError()
 
 
 class TaskInterface:
     """Task接口定义
     """
 
-    def start(self):
+    def start(self, *args, **kwargs):
         raise NotImplementedError()
 
-    def stop(self):
+    def stop(self, *args, **kwargs):
         raise NotImplementedError()
 
-    def is_running(self):
+    def is_running(self, *args, **kwargs):
         raise NotImplementedError()
 
 
 class ObjectFactoryInterface:
     """对象工厂类接口定义
     """
 
-    def create(self):
+    def create(self, *args, **kwargs):
         raise NotImplementedError()
 
 
 class ContextManager:
     """上下文资源管理器
 
     子类通过实现_context_release接口，方便的实现with语句管理上下文资源释放
```

### Comparing `hagworm-5.4.1/hagworm/extend/logging.py` & `hagworm-5.4.2/hagworm/extend/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 
         try:
 
             if message.record[r'thread'].id == self._task.ident:
                 return
 
             log_extra = message.record[r'extra']
+            trace_id = None
 
             if r'trace_id' not in log_extra and (trace_id := get_trace_id()) is not None:
                 log_extra[r'trace_id'] = trace_id
 
             self._buffer.put_nowait(message)
 
         except queue.Full as _:
```

### Comparing `hagworm-5.4.1/hagworm/extend/media.py` & `hagworm-5.4.2/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/metaclass.py` & `hagworm-5.4.2/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/process.py` & `hagworm-5.4.2/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/qrcode.py` & `hagworm-5.4.2/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/struct.py` & `hagworm-5.4.2/hagworm/extend/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,22 @@
 from io import BytesIO
 
 
 class Enum(_Enum):
 
     @classmethod
     def items(cls):
-
         return cls.to_dict().items()
 
     @classmethod
     def keys(cls):
-
         return cls.to_dict().keys()
 
     @classmethod
     def values(cls):
-
         return cls.to_dict().values()
 
     @classmethod
     def to_dict(cls):
 
         if not hasattr(cls, r'_to_dict'):
             setattr(cls, r'_to_dict', {item.name: item.value for item in cls})
@@ -49,20 +46,18 @@
         if not hasattr(cls, r'_to_values_dict'):
             setattr(cls, r'_to_values_dict', {item.value: item for item in cls})
 
         return getattr(cls, r'_to_values_dict')
 
     @classmethod
     def has_key(cls, key):
-
         return key in cls.to_keys_dict()
 
     @classmethod
     def has_value(cls, value):
-
         return value in cls.to_values_dict()
 
 
 class IntEnum(int, _Enum):
     pass
```

### Comparing `hagworm-5.4.1/hagworm/extend/text.py` & `hagworm-5.4.2/hagworm/extend/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,17 @@
         self._automaton.clear()
 
         for val in words:
             self._automaton.add_word(val, val)
 
         self._automaton.make_automaton()
 
-    def find_all(self, content: str) -> Tuple[int]:
+    def find_all(self, content: str) -> List[Tuple]:
 
-        return tuple(self._automaton.iter_long(content))
+        return list(self._automaton.iter_long(content))
 
     def replace_all(self, content: str, _chars: str = r'*') -> str:
 
         words = {item[1] for item in self.find_all(content)}
 
         for key in words:
             content = content.replace(key, _chars * len(key))
```

### Comparing `hagworm-5.4.1/hagworm/extend/trace.py` & `hagworm-5.4.2/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/transaction.py` & `hagworm-5.4.2/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/extend/validator.py` & `hagworm-5.4.2/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/frame/fastapi/base.py` & `hagworm-5.4.2/hagworm/frame/fastapi/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,17 +97,17 @@
 
         func = self.get_route_handler()
 
         is_coroutine = iscoroutinefunction_or_partial(func)
 
         async def app(scope: Scope, receive: Receive, send: Send) -> None:
 
-            try:
+            request = Request(scope, receive, send, self)
 
-                request = Request(scope, receive, send, self)
+            try:
 
                 trace_id = refresh_trace_id(request.get_header(r'x-request-id', None))
 
                 request_time = time.time() * 1000
 
                 await self.prepare(request)
```

### Comparing `hagworm-5.4.1/hagworm/frame/fastapi/field.py` & `hagworm-5.4.2/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/frame/fastapi/model.py` & `hagworm-5.4.2/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/frame/fastapi/response.py` & `hagworm-5.4.2/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/frame/gunicorn.py` & `hagworm-5.4.2/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/frame/stress_tests.py` & `hagworm-5.4.2/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/static/cacert.pem` & `hagworm-5.4.2/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/third/aliyun/logging.py` & `hagworm-5.4.2/hagworm/third/aliyun/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/third/aliyun/rocketmq.py` & `hagworm-5.4.2/hagworm/third/aliyun/rocketmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
 
 
 class MQCycleTransProducer(MQTransProducer, _TaskMixin):
 
     def __init__(self, message_handler, instance_id, topic_name, group_id, mq_client, debug=False):
 
         MQTransProducer.__init__(self, instance_id, topic_name, group_id, mq_client, debug)
-        _TaskMixin.__init__(message_handler)
+        _TaskMixin.__init__(self, message_handler)
 
         self._client_batch_size = 1
         self._client_wait_seconds = CLIENT_WAIT_TIMEOUT
 
     def set_client_batch_size(self, val):
 
         self._client_batch_size = val
```

### Comparing `hagworm-5.4.1/hagworm/third/consul/config.py` & `hagworm-5.4.2/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/third/rabbitmq/consume.py` & `hagworm-5.4.2/hagworm/third/rabbitmq/consume.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import aio_pika
 
 
 class RabbitMQConsumer(aio_pika.RobustConnection):
     """RabbitMQ消费者
     """
 
-    def __init__(self, url, **kwargs):
+    def __init__(self, url: str, **kwargs):
 
         super().__init__(url, **kwargs)
 
         self._channel: aio_pika.abc.AbstractRobustChannel = None
         self._queue: aio_pika.abc.AbstractRobustQueue = None
 
         self._channel_qos_config = None
@@ -78,15 +78,15 @@
         await self._queue.get(no_ack=no_ack, timeout=timeout)
 
 
 class RabbitMQConsumerForExchange(RabbitMQConsumer):
     """RabbitMQ注册到交换机的消费者(默认生成排它队列注册)
     """
 
-    def __init__(self, url, **kwargs):
+    def __init__(self, url: str, **kwargs):
         
         super().__init__(url, **kwargs)
 
         self._exchange: aio_pika.abc.AbstractExchange = None
 
         self._exchange_name = None
         self._routing_key = None
```

### Comparing `hagworm-5.4.1/hagworm/third/rabbitmq/publish.py` & `hagworm-5.4.2/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.4.2/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm.egg-info/PKG-INFO` & `hagworm-5.4.2/hagworm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.1
+Version: 5.4.2
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.1/hagworm.egg-info/SOURCES.txt` & `hagworm-5.4.2/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/hagworm.egg-info/requires.txt` & `hagworm-5.4.2/hagworm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.1/setup.py` & `hagworm-5.4.2/setup.py`

 * *Files identical despite different names*

