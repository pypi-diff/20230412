# Comparing `tmp/sunyata-0.0.29.tar.gz` & `tmp/sunyata-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.29.tar", last modified: Wed Mar  1 03:16:44 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.30.tar", last modified: Wed Apr 12 05:35:53 2023, max compression
```

## Comparing `sunyata-0.0.29.tar` & `sunyata-0.0.30.tar`

### file list

```diff
@@ -1,57 +1,65 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/
--rw-r--r--   0 root         (0) staff       (20)      636 2023-03-01 03:16:44.000000 sunyata-0.0.29/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      636 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1112 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       57 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/db.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     5416 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      368 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      938 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     3670 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)      256 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-01 03:16:44.000000 sunyata-0.0.29/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    11596 2023-03-01 03:14:41.000000 sunyata-0.0.29/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     8307 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.29/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.29/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.29/README.md
--rwxr-xr-x   0 root         (0) staff       (20)     1110 2023-03-01 03:10:59.000000 sunyata-0.0.29/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-03-01 03:16:44.000000 sunyata-0.0.29/setup.cfg
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/
+-rw-r--r--   0 admin      (501) staff       (20)      636 2023-04-12 05:35:53.000000 sunyata-0.0.30/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      636 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1357 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)       52 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)       57 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       63 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/
+-rw-r--r--   0 admin      (501) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/db.py
+-rwxr-xr-x   0 admin      (501) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/log.py
+-rw-r--r--   0 admin      (501) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/util.py
+-rw-r--r--   0 admin      (501) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/orm.py
+-rwxr-xr-x   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/eventloop.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/cli/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/cli/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/cli/cli.py
+-rw-r--r--   0 admin      (501) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/cli/entry.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/algorithm/
+-rw-r--r--   0 admin      (501) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 admin      (501) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.30/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 admin      (501) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.30/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 admin      (501) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.30/sunyata/algorithm/avltree.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.30/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 admin      (501) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.30/sunyata/algorithm/btree.py
+-rw-r--r--   0 admin      (501) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.30/sunyata/algorithm/bintree.py
+-rw-r--r--   0 admin      (501) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/lru.py
+-rw-r--r--   0 admin      (501) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/algorithm/trie.py
+-rw-r--r--   0 admin      (501) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.30/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 admin      (501) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/redislock.py
+-rw-r--r--   0 admin      (501) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/consul.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/http/
+-rw-r--r--   0 admin      (501) staff       (20)     3333 2023-04-12 02:46:43.000000 sunyata-0.0.30/sunyata/http/server.py
+-rw-r--r--   0 admin      (501) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.30/sunyata/http/request_stream.py
+-rw-r--r--   0 admin      (501) staff       (20)     2375 2023-04-12 01:46:57.000000 sunyata-0.0.30/sunyata/http/transport.py
+-rw-r--r--   0 admin      (501) staff       (20)      368 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/http/request.py
+-rw-r--r--   0 admin      (501) staff       (20)       68 2023-04-12 02:59:45.000000 sunyata-0.0.30/sunyata/http/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      938 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/http/response.py
+-rw-r--r--   0 admin      (501) staff       (20)     3738 2023-04-12 02:47:40.000000 sunyata-0.0.30/sunyata/http/factory.py
+-rw-r--r--   0 admin      (501) staff       (20)      256 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/http/router.py
+-rw-r--r--   0 admin      (501) staff       (20)      663 2023-04-11 12:55:36.000000 sunyata-0.0.30/sunyata/http/status.py
+-rw-r--r--   0 admin      (501) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/cache_wrap.py
+-rw-r--r--   0 admin      (501) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/compress.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/rpc/
+-rw-r--r--   0 admin      (501) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/encrypt.py
+-rw-r--r--   0 admin      (501) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/rpc/serialize.py
+-rw-r--r--   0 admin      (501) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/rpc/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)    11596 2023-04-12 02:59:15.000000 sunyata-0.0.30/sunyata/rpc/server.py
+-rw-r--r--   0 admin      (501) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/discovery.py
+-rw-r--r--   0 admin      (501) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.30/sunyata/rpc/transport.py
+-rw-r--r--   0 admin      (501) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/client.py
+-rw-r--r--   0 admin      (501) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/compress.py
+-rw-r--r--   0 admin      (501) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/method.py
+-rw-r--r--   0 admin      (501) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/protocal.py
+-rw-r--r--   0 admin      (501) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/rpc/const.py
+-rw-r--r--   0 admin      (501) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/table_writer.py
+-rw-r--r--   0 admin      (501) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/wrap.py
+-rw-r--r--   0 admin      (501) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.30/README.md
+-rwxr-xr-x   0 admin      (501) staff       (20)     1110 2023-04-12 03:00:11.000000 sunyata-0.0.30/setup.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-12 05:35:53.000000 sunyata-0.0.30/setup.cfg
```

### Comparing `sunyata-0.0.29/PKG-INFO` & `sunyata-0.0.30/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sunyata
-Version: 0.0.29
+Version: 0.0.30
 Summary: Light, simple, asynchronous RPC framework for Python
 Home-page: UNKNOWN
 Author: tank
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Keywords: sunyata
```

### Comparing `sunyata-0.0.29/sunyata.egg-info/PKG-INFO` & `sunyata-0.0.30/sunyata.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sunyata
-Version: 0.0.29
+Version: 0.0.30
 Summary: Light, simple, asynchronous RPC framework for Python
 Home-page: UNKNOWN
 Author: tank
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Keywords: sunyata
```

### Comparing `sunyata-0.0.29/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.30/sunyata.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -15,24 +15,32 @@
 sunyata.egg-info/PKG-INFO
 sunyata.egg-info/SOURCES.txt
 sunyata.egg-info/dependency_links.txt
 sunyata.egg-info/entry_points.txt
 sunyata.egg-info/requires.txt
 sunyata.egg-info/top_level.txt
 sunyata/algorithm/__init__.py
+sunyata/algorithm/avlsearchtree.py
+sunyata/algorithm/avltree.py
+sunyata/algorithm/binsearchtree.py
+sunyata/algorithm/bintree.py
 sunyata/algorithm/bloomfilter.py
+sunyata/algorithm/bplustree.py
+sunyata/algorithm/btree.py
 sunyata/algorithm/hashtable.py
 sunyata/algorithm/lru.py
+sunyata/algorithm/rbtree.py
 sunyata/algorithm/trie.py
 sunyata/cli/__init__.py
 sunyata/cli/cli.py
 sunyata/cli/entry.py
 sunyata/http/__init__.py
 sunyata/http/factory.py
 sunyata/http/request.py
+sunyata/http/request_stream.py
 sunyata/http/response.py
 sunyata/http/router.py
 sunyata/http/server.py
 sunyata/http/status.py
 sunyata/http/transport.py
 sunyata/rpc/__init__.py
 sunyata/rpc/client.py
```

### Comparing `sunyata-0.0.29/sunyata/db.py` & `sunyata-0.0.30/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/log.py` & `sunyata-0.0.30/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/orm.py` & `sunyata-0.0.30/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/cli/cli.py` & `sunyata-0.0.30/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.30/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/lru.py` & `sunyata-0.0.30/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/trie.py` & `sunyata-0.0.30/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/algorithm/hashtable.py` & `sunyata-0.0.30/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/redislock.py` & `sunyata-0.0.30/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/consul.py` & `sunyata-0.0.30/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/http/transport.py` & `sunyata-0.0.30/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/http/response.py` & `sunyata-0.0.30/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/http/factory.py` & `sunyata-0.0.30/sunyata/http/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,19 +50,19 @@
                 reqBody = line
             elif index > 0 and line != b'':
                 reqHeaders.append(line)
         return reqLine, reqHeaders, reqBody
         '''
         
     @classmethod
-    def genHttpRequest(cls, linesStr, conn):
+    async def genHttpRequest(cls, requestStream):
+        linesStr = await requestStream.reader.read(requestStream.bufsize)
         req = HttpRequest()
         lines = linesStr.split(b"\r\n")
         reqLine, reqHeaders, reqBody = cls.genLineHeaderBody(lines)
-    
         method, uri, httpVersion = reqLine.split(b' ')
         req.method = bytes2str(method)
         req.httpVersion = bytes2str(httpVersion)
         req.uri = bytes2str( uri.split(b'?')[0] )
         req.body = reqBody
         for header in reqHeaders:
             if header == b'':
@@ -83,22 +83,21 @@
             try:
                 kvPairs = uri.split(b'?')[1].split(b'&')
                 for kvPair in kvPairs:
                     k, v = kvPair.split(b'=')
                     req.data[bytes2str(k)] = bytes2str(v)
             except:
                 pass
-        contentLength = int(req.headers.get('Content-Length'))
+        contentLength = int(req.headers.get('Content-Length', 0))
         #if contentLength > cls.maxContentLength:
         #    raise Exception('content-length over')
         hasRead = len(req.body)
         toRead = contentLength - hasRead
-        bufsize = 1024 
         while toRead:
-            rdata = conn.recv(bufsize)
+            rdata = requestStream.reader.read(toRead)
             if not rdata:
                 raise Exception('peer closed')
             req.body = req.body + rdata
             hasRead = hasRead + len(rdata)
             toRead = contentLength - hasRead
         return req
```

### Comparing `sunyata-0.0.29/sunyata/http/status.py` & `sunyata-0.0.30/sunyata/http/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class HttpStatus403(HttpStatus):
     code = 403
     msg = 'Forbidden'
 
 
 class HttpStatus404(HttpStatus):
-    code = 403
+    code = 404
     msg = 'Not Found'
 
 
 class HttpStatus405(HttpStatus):
     code = 405
     msg = 'Method Not Allowed'
```

### Comparing `sunyata-0.0.29/sunyata/cache_wrap.py` & `sunyata-0.0.30/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/serialize.py` & `sunyata-0.0.30/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/server.py` & `sunyata-0.0.30/sunyata/rpc/server.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/discovery.py` & `sunyata-0.0.30/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/transport.py` & `sunyata-0.0.30/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/client.py` & `sunyata-0.0.30/sunyata/rpc/client.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/method.py` & `sunyata-0.0.30/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/rpc/protocal.py` & `sunyata-0.0.30/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/table_writer.py` & `sunyata-0.0.30/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/sunyata/wrap.py` & `sunyata-0.0.30/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/README.md` & `sunyata-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.29/setup.py` & `sunyata-0.0.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFINE_VERSION = '0.0.29'
+DEFINE_VERSION = '0.0.30'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
     'requests==2.25.1',
     'PyMySQL==0.10.1',
     'DBUtils==1.3',
```

