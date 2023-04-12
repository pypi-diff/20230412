# Comparing `tmp/kwil-0.0.1.tar.gz` & `tmp/kwil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwil-0.0.1.tar", last modified: Wed Apr 12 18:58:22 2023, max compression
+gzip compressed data, was "kwil-0.0.2.tar", last modified: Wed Apr 12 20:54:09 2023, max compression
```

## Comparing `kwil-0.0.1.tar` & `kwil-0.0.2.tar`

### file list

```diff
@@ -1,63 +1,71 @@
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.200755 kwil-0.0.1/
--rw-r--r--   0 gavin      (501) staff       (20)     1005 2023-04-12 18:58:22.200593 kwil-0.0.1/PKG-INFO
--rw-r--r--   0 gavin      (501) staff       (20)      360 2023-04-12 18:40:46.000000 kwil-0.0.1/README.md
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.188302 kwil-0.0.1/kwil/
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.192406 kwil-0.0.1/kwil/_utils/
--rw-r--r--   0 gavin      (501) staff       (20)        0 2023-04-03 19:04:31.000000 kwil-0.0.1/kwil/_utils/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     1555 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/action.py
--rw-r--r--   0 gavin      (501) staff       (20)      346 2023-04-10 22:57:27.000000 kwil-0.0.1/kwil/_utils/dataset.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.193040 kwil-0.0.1/kwil/_utils/grpc/
--rw-r--r--   0 gavin      (501) staff       (20)       56 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/grpc/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     2936 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/grpc/client.py
--rw-r--r--   0 gavin      (501) staff       (20)     2183 2023-04-12 15:56:08.000000 kwil-0.0.1/kwil/_utils/method_formatters.py
--rw-r--r--   0 gavin      (501) staff       (20)      719 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/naming_converter.py
--rw-r--r--   0 gavin      (501) staff       (20)     2796 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/request.py
--rw-r--r--   0 gavin      (501) staff       (20)      504 2023-04-09 22:05:10.000000 kwil-0.0.1/kwil/_utils/rpcs.py
--rw-r--r--   0 gavin      (501) staff       (20)     1812 2023-04-12 15:15:10.000000 kwil-0.0.1/kwil/_utils/signature.py
--rw-r--r--   0 gavin      (501) staff       (20)      185 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/signing.py
--rw-r--r--   0 gavin      (501) staff       (20)     1210 2023-04-12 14:59:57.000000 kwil-0.0.1/kwil/_utils/transaction.py
--rw-r--r--   0 gavin      (501) staff       (20)      419 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/utils.py
--rw-r--r--   0 gavin      (501) staff       (20)     3566 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/_utils/validation.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.193894 kwil-0.0.1/kwil/kwil.egg-info/
--rw-r--r--   0 gavin      (501) staff       (20)     1005 2023-04-12 18:58:22.000000 kwil-0.0.1/kwil/kwil.egg-info/PKG-INFO
--rw-r--r--   0 gavin      (501) staff       (20)     1326 2023-04-12 18:58:22.000000 kwil-0.0.1/kwil/kwil.egg-info/SOURCES.txt
--rw-r--r--   0 gavin      (501) staff       (20)        1 2023-04-12 18:58:22.000000 kwil-0.0.1/kwil/kwil.egg-info/dependency_links.txt
--rw-r--r--   0 gavin      (501) staff       (20)      306 2023-04-12 18:58:22.000000 kwil-0.0.1/kwil/kwil.egg-info/requires.txt
--rw-r--r--   0 gavin      (501) staff       (20)       42 2023-04-12 18:58:22.000000 kwil-0.0.1/kwil/kwil.egg-info/top_level.txt
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.194282 kwil-0.0.1/kwil/kwil_typing/
--rw-r--r--   0 gavin      (501) staff       (20)       81 2023-04-12 15:29:41.000000 kwil-0.0.1/kwil/kwil_typing/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)      148 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/kwil_typing/kvm.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.194744 kwil-0.0.1/kwil/kwil_utils/
--rw-r--r--   0 gavin      (501) staff       (20)      129 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/kwil_utils/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     1065 2023-04-05 19:34:56.000000 kwil-0.0.1/kwil/kwil_utils/types.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.195782 kwil-0.0.1/kwil/provider/
--rw-r--r--   0 gavin      (501) staff       (20)      167 2023-04-12 15:29:34.000000 kwil-0.0.1/kwil/provider/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     2074 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/provider/auto.py
--rw-r--r--   0 gavin      (501) staff       (20)     2344 2023-04-12 15:25:27.000000 kwil-0.0.1/kwil/provider/base.py
--rw-r--r--   0 gavin      (501) staff       (20)     1634 2023-04-11 19:46:10.000000 kwil-0.0.1/kwil/provider/grpc.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.196109 kwil-0.0.1/kwil/tx/
--rw-r--r--   0 gavin      (501) staff       (20)        0 2023-04-12 15:23:06.000000 kwil-0.0.1/kwil/tx/__init__.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 18:58:22.200363 kwil-0.0.1/kwil/tx/v1/
--rw-r--r--   0 gavin      (501) staff       (20)        0 2023-03-30 22:48:39.000000 kwil-0.0.1/kwil/tx/v1/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     1511 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/account_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/account_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1388 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/broadcast_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/broadcast_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1360 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/config_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/config_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     3435 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/dataset_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/dataset_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/list_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/list_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1219 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/ping_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/ping_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1375 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/price_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/price_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/query_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/query_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     4479 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/service_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)    14437 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/service_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     2062 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/tx_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-11 20:04:35.000000 kwil-0.0.1/kwil/tx/v1/tx_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1468 2023-04-12 15:13:17.000000 kwil-0.0.1/pyproject.toml
--rw-r--r--   0 gavin      (501) staff       (20)       38 2023-04-12 18:58:22.200798 kwil-0.0.1/setup.cfg
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.191761 kwil-0.0.2/
+-rw-r--r--   0 gavin      (501) staff       (20)     1020 2023-04-12 20:54:09.191630 kwil-0.0.2/PKG-INFO
+-rw-r--r--   0 gavin      (501) staff       (20)      360 2023-04-12 18:40:46.000000 kwil-0.0.2/README.md
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.182269 kwil-0.0.2/kwil/
+-rw-r--r--   0 gavin      (501) staff       (20)       87 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/__about__.py
+-rw-r--r--   0 gavin      (501) staff       (20)      322 2023-04-12 20:39:28.000000 kwil-0.0.2/kwil/__init__.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.186215 kwil-0.0.2/kwil/_utils/
+-rw-r--r--   0 gavin      (501) staff       (20)        0 2023-04-03 19:04:31.000000 kwil-0.0.2/kwil/_utils/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1555 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/action.py
+-rw-r--r--   0 gavin      (501) staff       (20)      346 2023-04-10 22:57:27.000000 kwil-0.0.2/kwil/_utils/dataset.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.186610 kwil-0.0.2/kwil/_utils/grpc/
+-rw-r--r--   0 gavin      (501) staff       (20)       56 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/grpc/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2935 2023-04-12 20:45:39.000000 kwil-0.0.2/kwil/_utils/grpc/client.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2183 2023-04-12 15:56:08.000000 kwil-0.0.2/kwil/_utils/method_formatters.py
+-rw-r--r--   0 gavin      (501) staff       (20)      719 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/naming_converter.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2796 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/request.py
+-rw-r--r--   0 gavin      (501) staff       (20)      504 2023-04-09 22:05:10.000000 kwil-0.0.2/kwil/_utils/rpcs.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1807 2023-04-12 20:01:31.000000 kwil-0.0.2/kwil/_utils/signature.py
+-rw-r--r--   0 gavin      (501) staff       (20)      185 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/signing.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1210 2023-04-12 14:59:57.000000 kwil-0.0.2/kwil/_utils/transaction.py
+-rw-r--r--   0 gavin      (501) staff       (20)      419 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/utils.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3566 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/_utils/validation.py
+-rw-r--r--   0 gavin      (501) staff       (20)      404 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/exceptions.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1436 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/kwild.py
+-rw-r--r--   0 gavin      (501) staff       (20)     4341 2023-04-12 16:17:47.000000 kwil-0.0.2/kwil/main.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1774 2023-04-12 15:18:49.000000 kwil-0.0.2/kwil/manager.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1808 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/method.py
+-rw-r--r--   0 gavin      (501) staff       (20)      783 2023-04-12 15:19:39.000000 kwil-0.0.2/kwil/middleware.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1014 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/module.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.187491 kwil-0.0.2/kwil/provider/
+-rw-r--r--   0 gavin      (501) staff       (20)      167 2023-04-12 15:29:34.000000 kwil-0.0.2/kwil/provider/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2074 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/provider/auto.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2344 2023-04-12 15:25:27.000000 kwil-0.0.2/kwil/provider/base.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1634 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil/provider/grpc.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.178865 kwil-0.0.2/kwil/tx/
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.190413 kwil-0.0.2/kwil/tx/v1/
+-rw-r--r--   0 gavin      (501) staff       (20)     1511 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/account_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/account_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1388 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/broadcast_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/broadcast_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1360 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/config_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/config_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3435 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/dataset_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/dataset_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/list_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/list_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1219 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/ping_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/ping_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1375 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/price_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/price_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/query_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/query_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     4479 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/service_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)    14437 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/service_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2062 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/tx_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.2/kwil/tx/v1/tx_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3413 2023-04-12 20:01:31.000000 kwil-0.0.2/kwil/types.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.182946 kwil-0.0.2/kwil.egg-info/
+-rw-r--r--   0 gavin      (501) staff       (20)     1020 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/PKG-INFO
+-rw-r--r--   0 gavin      (501) staff       (20)     1398 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/SOURCES.txt
+-rw-r--r--   0 gavin      (501) staff       (20)        1 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/dependency_links.txt
+-rw-r--r--   0 gavin      (501) staff       (20)      306 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/requires.txt
+-rw-r--r--   0 gavin      (501) staff       (20)       28 2023-04-12 20:54:09.000000 kwil-0.0.2/kwil.egg-info/top_level.txt
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.190836 kwil-0.0.2/kwil_typing/
+-rw-r--r--   0 gavin      (501) staff       (20)       81 2023-04-12 15:29:41.000000 kwil-0.0.2/kwil_typing/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)      148 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil_typing/kvm.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-12 20:54:09.191377 kwil-0.0.2/kwil_utils/
+-rw-r--r--   0 gavin      (501) staff       (20)      129 2023-04-11 19:46:10.000000 kwil-0.0.2/kwil_utils/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1065 2023-04-05 19:34:56.000000 kwil-0.0.2/kwil_utils/types.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1558 2023-04-12 20:52:23.000000 kwil-0.0.2/pyproject.toml
+-rw-r--r--   0 gavin      (501) staff       (20)       38 2023-04-12 20:54:09.191796 kwil-0.0.2/setup.cfg
```

### Comparing `kwil-0.0.1/PKG-INFO` & `kwil-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: kwil
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for interacting with the kwil blockchain
 Author-email: yaiba <4yaiba@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kwilteam/kwil.py
+Keywords: kwil
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
```

### Comparing `kwil-0.0.1/kwil/_utils/action.py` & `kwil-0.0.2/kwil/_utils/action.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/_utils/grpc/client.py` & `kwil-0.0.2/kwil/_utils/grpc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import grpc
 
 from kwil.types import TxParams, DBIdentifier, HexAddress
 from kwil.tx.v1 import (
-    service_pb2_grpc,
     ping_pb2,
     query_pb2,
     broadcast_pb2,
     account_pb2,
     config_pb2,
     price_pb2,
     dataset_pb2,
     tx_pb2,
     list_pb2,
+    service_pb2_grpc
 )
 
 # timeout in seconds
 READY_TIMEOUT = 3
 REQUEST_TIMEOUT = 2
```

### Comparing `kwil-0.0.1/kwil/_utils/method_formatters.py` & `kwil-0.0.2/kwil/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/_utils/naming_converter.py` & `kwil-0.0.2/kwil/_utils/naming_converter.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/_utils/request.py` & `kwil-0.0.2/kwil/_utils/request.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/_utils/signature.py` & `kwil-0.0.2/kwil/_utils/signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from eth_account import Account
 from eth_utils import to_bytes, keccak as eth_utils_keccak
 from hexbytes import (
     HexBytes,
 )
 
-from kwil.kwil_typing import HexStr
+from kwil_typing import HexStr
 from kwil.types import Signature, SignatureType
 
 
 def keccak(
     primitive: Union[bytes, int, bool, None] = None,
     text: Optional[str] = None,
     hexstr: Optional[HexStr] = None,
```

### Comparing `kwil-0.0.1/kwil/_utils/transaction.py` & `kwil-0.0.2/kwil/_utils/transaction.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/_utils/validation.py` & `kwil-0.0.2/kwil/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/kwil.egg-info/PKG-INFO` & `kwil-0.0.2/kwil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: kwil
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for interacting with the kwil blockchain
 Author-email: yaiba <4yaiba@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/kwilteam/kwil.py
+Keywords: kwil
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
```

### Comparing `kwil-0.0.1/kwil/kwil.egg-info/SOURCES.txt` & `kwil-0.0.2/kwil.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 README.md
 pyproject.toml
+kwil/__about__.py
+kwil/__init__.py
+kwil/exceptions.py
+kwil/kwild.py
+kwil/main.py
+kwil/manager.py
+kwil/method.py
+kwil/middleware.py
+kwil/module.py
+kwil/types.py
+kwil.egg-info/PKG-INFO
+kwil.egg-info/SOURCES.txt
+kwil.egg-info/dependency_links.txt
+kwil.egg-info/requires.txt
+kwil.egg-info/top_level.txt
 kwil/_utils/__init__.py
 kwil/_utils/action.py
 kwil/_utils/dataset.py
 kwil/_utils/method_formatters.py
 kwil/_utils/naming_converter.py
 kwil/_utils/request.py
 kwil/_utils/rpcs.py
 kwil/_utils/signature.py
 kwil/_utils/signing.py
 kwil/_utils/transaction.py
 kwil/_utils/utils.py
 kwil/_utils/validation.py
 kwil/_utils/grpc/__init__.py
 kwil/_utils/grpc/client.py
-kwil/kwil.egg-info/PKG-INFO
-kwil/kwil.egg-info/SOURCES.txt
-kwil/kwil.egg-info/dependency_links.txt
-kwil/kwil.egg-info/requires.txt
-kwil/kwil.egg-info/top_level.txt
-kwil/kwil_typing/__init__.py
-kwil/kwil_typing/kvm.py
-kwil/kwil_utils/__init__.py
-kwil/kwil_utils/types.py
 kwil/provider/__init__.py
 kwil/provider/auto.py
 kwil/provider/base.py
 kwil/provider/grpc.py
-kwil/tx/__init__.py
-kwil/tx/v1/__init__.py
 kwil/tx/v1/account_pb2.py
 kwil/tx/v1/account_pb2_grpc.py
 kwil/tx/v1/broadcast_pb2.py
 kwil/tx/v1/broadcast_pb2_grpc.py
 kwil/tx/v1/config_pb2.py
 kwil/tx/v1/config_pb2_grpc.py
 kwil/tx/v1/dataset_pb2.py
@@ -44,8 +48,12 @@
 kwil/tx/v1/price_pb2.py
 kwil/tx/v1/price_pb2_grpc.py
 kwil/tx/v1/query_pb2.py
 kwil/tx/v1/query_pb2_grpc.py
 kwil/tx/v1/service_pb2.py
 kwil/tx/v1/service_pb2_grpc.py
 kwil/tx/v1/tx_pb2.py
-kwil/tx/v1/tx_pb2_grpc.py
+kwil/tx/v1/tx_pb2_grpc.py
+kwil_typing/__init__.py
+kwil_typing/kvm.py
+kwil_utils/__init__.py
+kwil_utils/types.py
```

### Comparing `kwil-0.0.1/kwil/kwil_utils/types.py` & `kwil-0.0.2/kwil_utils/types.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/provider/auto.py` & `kwil-0.0.2/kwil/provider/auto.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/provider/base.py` & `kwil-0.0.2/kwil/provider/base.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/provider/grpc.py` & `kwil-0.0.2/kwil/provider/grpc.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/account_pb2.py` & `kwil-0.0.2/kwil/tx/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/broadcast_pb2.py` & `kwil-0.0.2/kwil/tx/v1/broadcast_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/config_pb2.py` & `kwil-0.0.2/kwil/tx/v1/config_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/dataset_pb2.py` & `kwil-0.0.2/kwil/tx/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/list_pb2.py` & `kwil-0.0.2/kwil/tx/v1/list_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/ping_pb2.py` & `kwil-0.0.2/kwil/tx/v1/ping_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/price_pb2.py` & `kwil-0.0.2/kwil/tx/v1/price_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/query_pb2.py` & `kwil-0.0.2/kwil/tx/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/service_pb2.py` & `kwil-0.0.2/kwil/tx/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/service_pb2_grpc.py` & `kwil-0.0.2/kwil/tx/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/kwil/tx/v1/tx_pb2.py` & `kwil-0.0.2/kwil/tx/v1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.1/pyproject.toml` & `kwil-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=67.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kwil"
 description = 'Library for interacting with the kwil blockchain'
-version = "0.0.1"
+version = "0.0.2"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT License"}
-keywords = []
+keywords = ["kwil"]
 authors = [
   { name = "yaiba", email = "4yaiba@gmail.com" },
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: Implementation :: CPython",
@@ -65,8 +65,10 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.setuptools.packages.find]
-where = ["kwil"]
+where = ["."]
+exclude = ["tests*"]
+include = ["kwil_proto*", "kwil_typing*", "kwil_utils*", "kwil*"]
```

