# Comparing `tmp/peek-abstract-chunked-index-3.3.3.tar.gz` & `tmp/peek-abstract-chunked-index-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-abstract-chunked-index-3.3.3.tar", last modified: Mon Nov 14 05:35:02 2022, max compression
+gzip compressed data, was "peek-abstract-chunked-index-3.4.0.tar", last modified: Wed Apr 12 11:03:50 2023, max compression
```

## Comparing `peek-abstract-chunked-index-3.3.3.tar` & `peek-abstract-chunked-index-3.4.0.tar`

### file list

```diff
@@ -1,74 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.508642 peek-abstract-chunked-index-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      408 2022-11-14 05:35:02.508642 peek-abstract-chunked-index-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.505642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/
--rw-r--r--   0 root         (0) root         (0)      614 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:35:02.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.506642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      530 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts
--rw-r--r--   0 root         (0) root         (0)      920 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts
--rw-r--r--   0 root         (0) root         (0)      963 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts
--rw-r--r--   0 root         (0) root         (0)      565 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.506642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      501 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/PluginNames.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.506642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/admin/
--rw-r--r--   0 root         (0) root         (0)      513 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.506642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/
--rw-r--r--   0 root         (0) root         (0)      394 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexEncodedChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    21045 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      546 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      610 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      342 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/index.ts
--rw-r--r--   0 root         (0) root         (0)     2838 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts
--rw-r--r--   0 root         (0) root         (0)      253 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.506642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      334 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/tuples/OfflineConfigTuple.ts
--rw-r--r--   0 root         (0) root         (0)      307 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.506642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.507642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.507642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/controller/
--rw-r--r--   0 root         (0) root         (0)    19915 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/controller/ACICacheControllerABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.507642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     7689 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.507642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1223 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo
--rw-r--r--   0 root         (0) root         (0)     2330 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.507642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.507642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     6099 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py
--rw-r--r--   0 root         (0) root         (0)     5406 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkUpdateHandlerABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.507642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/
--rw-r--r--   0 root         (0) root         (0)    18352 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py
--rw-r--r--   0 root         (0) root         (0)     1552 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py
--rw-r--r--   0 root         (0) root         (0)     1906 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.508642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/
--rw-r--r--   0 root         (0) root         (0)     3071 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py
--rw-r--r--   0 root         (0) root         (0)     1175 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py
--rw-r--r--   0 root         (0) root         (0)     1710 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py
--rw-r--r--   0 root         (0) root         (0)      254 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/ChunkedIndexQueueStatusTupleABC.py_abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.508642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.508642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     6206 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo
--rw-r--r--   0 root         (0) root         (0)     9317 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo
--rw-r--r--   0 root         (0) root         (0)      274 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexRemover.py_abctodo
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:26.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:02.506642 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2022-11-14 05:35:02.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3670 2022-11-14 05:35:02.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:02.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-14 05:35:02.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-11-14 05:35:02.000000 peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:35:02.508642 peek-abstract-chunked-index-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2022-11-14 05:35:02.000000 peek-abstract-chunked-index-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.843218 peek-abstract-chunked-index-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-12 11:03:50.843218 peek-abstract-chunked-index-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.840218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/
+-rw-r--r--   0 root         (0) root         (0)      614 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:50.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      530 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      920 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      565 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/PluginNames.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/admin/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexEncodedChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    20958 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      610 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      342 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/index.ts
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/tuples/OfflineConfigTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.842218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)    12460 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/ACICacheControllerABC.py
+-rw-r--r--   0 root         (0) root         (0)     8543 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/ACICacheControllerLoadFromLogicMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/ACICacheControllerNotifyMixin.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/ACICacheControllerOfflineIndexMixin.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteAppDbMixin.py
+-rw-r--r--   0 root         (0) root         (0)     6349 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteCacheMixin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.842218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     9390 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.842218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.842218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.842218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkUpdateHandlerABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.843218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)    18313 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.843218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/ChunkedIndexQueueStatusTupleABC.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.843218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.843218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)     9317 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)      274 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexRemover.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)      631 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:17.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:03:50.841218 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-12 11:03:50.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4023 2023-04-12 11:03:50.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:03:50.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:03:50.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-12 11:03:50.000000 peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:03:50.844218 peek-abstract-chunked-index-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-04-12 11:03:50.000000 peek-abstract-chunked-index-3.4.0/setup.py
```

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/PlatformDependencyTest.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/PlatformDependencyTest.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,23 @@
     TupleStorageBatchSaveArguments,
 } from "@synerty/vortexjs";
 import { ChunkedIndexEncodedChunkTuple } from "./ChunkedIndexEncodedChunkTuple";
 import { ChunkedIndexUpdateDateTuple } from "./ChunkedIndexUpdateDateTuple";
 import { ChunkedTuple } from "../../ChunkedTuple";
 import { ChunkedIndexTupleService } from "../index-blueprint-tuple.service";
 import { ChunkedTypeTuple } from "../../ChunkedTypeTuple";
-import { ChunkedIndexLoaderStatusTuple } from "./ChunkedIndexLoaderStatusTuple";
 import { ChunkedIndexModelSetTuple } from "../../ChunkedIndexModelSetTuple";
 import {
     chunkedIndexCacheStorageName,
     chunkedIndexFilt,
     chunkedIndexTuplePrefix,
 } from "../PluginNames";
 import {
     DeviceOfflineCacheService,
-    OfflineCacheStatusTuple,
+    OfflineCacheLoaderStatusTuple,
 } from "@peek/peek_core_device";
 
 // ----------------------------------------------------------------------------
 
 export interface ChunkedIndexResultI {
     [key: string]: ChunkedTuple;
 }
@@ -125,24 +124,24 @@
 
     // Every 100 chunks from the server
     private SAVE_POINT_ITERATIONS = 100;
 
     // Saving the cache after each chunk is so expensive, we only do it every 20 or so
     private chunksSavedSinceLastIndexSave = 0;
 
-    private index = new ChunkedIndexUpdateDateTuple();
+    private index: ChunkedIndexUpdateDateTuple | null = null;
     private askServerChunks: ChunkedIndexUpdateDateTuple[] = [];
 
     private _hasLoaded = false;
 
     private _hasLoadedSubject = new Subject<void>();
     private storage: TupleOfflineStorageService;
 
-    private _statusSubject = new Subject<ChunkedIndexLoaderStatusTuple>();
-    private _status = new ChunkedIndexLoaderStatusTuple();
+    private _statusSubject = new Subject<OfflineCacheLoaderStatusTuple>();
+    private _status = new OfflineCacheLoaderStatusTuple();
 
     private objectTypesByIds: { [id: number]: ChunkedTypeTuple } = {};
     private _hasDocTypeLoaded = false;
 
     private modelSetByIds: { [id: number]: ChunkedIndexModelSetTuple } = {};
     private _hasModelSetLoaded = false;
 
@@ -151,14 +150,17 @@
         private vortexStatusService: VortexStatusService,
         storageFactory: TupleStorageFactoryService,
         private tupleService: ChunkedIndexTupleService,
         private deviceCacheControllerService: DeviceOfflineCacheService
     ) {
         super();
 
+        this._status.pluginName = "Chunked Loader";
+        this._status.indexName = "Abstract Index";
+
         let objTypeTs = new TupleSelector(ChunkedTypeTuple.tupleName, {});
         this.tupleService.offlineObserver
             .subscribeToTupleSelector(objTypeTs)
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((tuples: ChunkedTypeTuple[]) => {
                 this.objectTypesByIds = {};
                 for (let chunked of tuples) {
@@ -186,38 +188,53 @@
 
         this.storage = new TupleOfflineStorageService(
             storageFactory,
             new TupleOfflineStorageNameService(chunkedIndexCacheStorageName)
         );
 
         this.setupVortexSubscriptions();
-        this._notifyStatus();
 
-        this.deviceCacheControllerService.triggerCachingObservable
+        this.deviceCacheControllerService.offlineModeEnabled$
             .pipe(takeUntil(this.onDestroyEvent))
             .pipe(filter((v) => v))
+            .pipe(first())
             .subscribe(() => {
                 this.initialLoad();
+            });
+
+        this.deviceCacheControllerService.triggerCachingStartObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+            .pipe(filter((v) => v))
+            .subscribe(() => {
+                this.askServerForUpdates();
+                this._notifyStatus();
+            });
+
+        this.deviceCacheControllerService.triggerCachingResumeObservable
+            .pipe(takeUntil(this.onDestroyEvent))
+
+            .subscribe(() => {
                 this._notifyStatus();
+                this.askServerForNextUpdateChunk();
             });
     }
 
     isReady(): boolean {
         return this._hasLoaded;
     }
 
     isReadyObservable(): Observable<void> {
         return this._hasLoadedSubject;
     }
 
-    statusObservable(): Observable<ChunkedIndexLoaderStatusTuple> {
+    statusObservable(): Observable<OfflineCacheLoaderStatusTuple> {
         return this._statusSubject;
     }
 
-    status(): ChunkedIndexLoaderStatusTuple {
+    status(): OfflineCacheLoaderStatusTuple {
         return this._status;
     }
 
     /** Get ChunkedIndexs
      *
      * Get the objects with matching keywords from the index..
      *
@@ -279,81 +296,67 @@
             this._hasDocTypeLoaded &&
             this._hasModelSetLoaded &&
             this._hasLoaded
         )
             this._hasLoadedSubject.next();
     }
 
-    private _notifyStatus(): void {
-        this._status.cacheForOfflineEnabled =
-            this.deviceCacheControllerService.cachingEnabled;
-        this._status.initialLoadComplete = this.index.initialLoadComplete;
-
-        this._status.loadProgress = Object.keys(
-            this.index.updateDateByChunkKey
-        ).length;
-        for (let chunk of this.askServerChunks)
-            this._status.loadProgress -= Object.keys(
+    private _notifyStatus(paused: boolean = false): void {
+        this._status.lastCheckDate = new Date();
+        this._status.paused = paused;
+        this._status.initialFullLoadComplete = this.index.initialLoadComplete;
+
+        this._status.loadingQueueCount = 0;
+        for (let chunk of this.askServerChunks) {
+            this._status.loadingQueueCount += Object.keys(
                 chunk.updateDateByChunkKey
             ).length;
+        }
 
         this._statusSubject.next(this._status);
-
-        const status = new OfflineCacheStatusTuple();
-        status.pluginName = "Chunked Loader";
-        status.indexName = "Abstract Index";
-        status.loadingQueueCount = this._status.loadProgress;
-        status.totalLoadedCount = this._status.loadTotal;
-        status.lastCheckDate = new Date();
-        status.initialFullLoadComplete = this._status.initialLoadComplete;
-        this.deviceCacheControllerService.updateCachingStatus(status);
+        this.deviceCacheControllerService.updateLoaderCachingStatus(
+            this._status
+        );
     }
 
     /** Initial load
      *
      * Load the dates of the index buckets and ask the server if it has any updates.
      */
     private initialLoad(): void {
         this.storage
             .loadTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any[]) => {
                 let tuples: ChunkedIndexUpdateDateTuple[] = tuplesAny;
-                if (tuples.length != 0) {
+                if (tuples.length === 0) {
+                    this.index = new ChunkedIndexUpdateDateTuple();
+                } else {
                     this.index = tuples[0];
 
                     if (this.index.initialLoadComplete) {
                         this._hasLoaded = true;
                         this._notifyReady();
                     }
                 }
 
-                this.askServerForUpdates();
                 this._notifyStatus();
             });
-
-        this._notifyStatus();
     }
 
     private setupVortexSubscriptions(): void {
         // Services don't have destructors, I'm not sure how to unsubscribe.
         this.vortexService
             .createEndpointObservable(
                 this,
                 clientChunkedIndexWatchUpdateFromDeviceFilt
             )
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((payloadEnvelope: PayloadEnvelope) => {
                 this.processChunksFromServer(payloadEnvelope);
             });
-
-        // If the vortex service comes back online, update the watch grids.
-        this.vortexStatusService.isOnline
-            .pipe(filter((isOnline) => isOnline == true))
-            .pipe(takeUntil(this.onDestroyEvent))
-            .subscribe(() => this.askServerForUpdates());
     }
 
     private areWeTalkingToTheServer(): boolean {
         return (
             this.deviceCacheControllerService.offlineModeEnabled &&
             this.vortexStatusService.snapshot.isOnline
         );
@@ -377,15 +380,15 @@
         this.tupleService.observer
             .pollForTuples(new UpdateDateTupleSelector())
             .then((tuplesAny: any) => {
                 let serverIndex: ChunkedIndexUpdateDateTuple = tuplesAny[0];
                 let keys = Object.keys(serverIndex.updateDateByChunkKey);
                 let keysNeedingUpdate: string[] = [];
 
-                this._status.loadTotal = keys.length;
+                this._status.totalLoadedCount = keys.length;
 
                 // Tuples is an array of strings
                 for (let chunkKey of keys) {
                     if (
                         !this.index.updateDateByChunkKey.hasOwnProperty(
                             chunkKey
                         )
@@ -426,38 +429,38 @@
             }
         }
 
         if (count) this.askServerChunks.push(indexChunk);
 
         this.askServerForNextUpdateChunk();
 
-        this._status.lastCheck = new Date();
+        this._status.lastCheckDate = new Date();
     }
 
     private askServerForNextUpdateChunk() {
         if (!this.areWeTalkingToTheServer()) return;
 
         if (this.askServerChunks.length == 0) return;
 
-        this.deviceCacheControllerService //
-            .waitForGarbageCollector()
-            .then(() => {
-                let indexChunk: ChunkedIndexUpdateDateTuple =
-                    this.askServerChunks.pop();
-                let filt = extend(
-                    {},
-                    clientChunkedIndexWatchUpdateFromDeviceFilt
-                );
-                filt[cacheAll] = true;
-                let pl = new Payload(filt, [indexChunk]);
-                this.vortexService.sendPayload(pl);
+        if (this.deviceCacheControllerService.isOfflineCachingPaused) {
+            this.saveChunkCacheIndex(true) //
+                .catch((e) => console.log(`ERROR saveChunkCacheIndex: ${e}`));
+            this._notifyStatus(true);
+            return;
+        }
 
-                this._status.lastCheck = new Date();
-                this._notifyStatus();
-            });
+        let indexChunk: ChunkedIndexUpdateDateTuple =
+            this.askServerChunks.pop();
+        let filt = extend({}, clientChunkedIndexWatchUpdateFromDeviceFilt);
+        filt[cacheAll] = true;
+        let pl = new Payload(filt, [indexChunk]);
+        this.vortexService.sendPayload(pl);
+
+        this._status.lastCheckDate = new Date();
+        this._notifyStatus();
     }
 
     /** Process ChunkedIndexes From Server
      *
      * Process the grids the server has sent us.
      */
     private async processChunksFromServer(
```

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 import logging
 from abc import ABCMeta
 from collections import defaultdict
+from datetime import datetime
 from typing import Dict
 from typing import List
 
-from twisted.internet.defer import Deferred
-from twisted.internet.defer import DeferredList
-from twisted.internet.defer import inlineCallbacks
-from vortex.DeferUtil import vortexLogFailure
-from vortex.PayloadEndpoint import PayloadEndpoint
-from vortex.PayloadEnvelope import PayloadEnvelope
-from vortex.VortexABC import SendVortexMsgResponseCallable
-from vortex.VortexFactory import VortexFactory
-
+import pytz
 from peek_abstract_chunked_index.private.client.controller.ACICacheControllerABC import (
     ACICacheControllerABC,
 )
 
 # ModelSet HANDLER
 from peek_abstract_chunked_index.private.tuples.ACIUpdateDateTupleABC import (
     ACIUpdateDateTupleABC,
 )
-from peek_plugin_base.PeekVortexUtil import peekServerName
+from twisted.internet.defer import DeferredSemaphore
+from twisted.internet.defer import inlineCallbacks
+from txhttputil.util.DeferUtil import vortexLogFailure
+from vortex.PayloadEndpoint import PayloadEndpoint
+from vortex.PayloadEnvelope import PayloadEnvelope
+from vortex.VortexABC import SendVortexMsgResponseCallable
+from vortex.VortexFactory import NoVortexException
+from vortex.VortexFactory import VortexFactory
+from vortex.VortexUtil import limitConcurrency
+
+cacheHandlerLogger = logging.getLogger(__name__)
+
+
+def _dedupOACICacheHandlerABCCallKeys(
+    payloadEnvelope: PayloadEnvelope, vortexUuid: str, *args, **kwargs
+):
+
+    filt = payloadEnvelope.filt.copy()
+    filt.pop(PayloadResponse.MESSAGE_ID_KEY, None)
+    return vortexUuid, str(filt)
 
 
 class ACICacheHandlerABC(metaclass=ABCMeta):
     _UpdateDateTuple: ACIUpdateDateTupleABC = None
     _updateFromDeviceFilt: Dict = None
     _updateFromLogicFilt: Dict = None
     _logger: logging.Logger = None
 
+    _DEBUG_LOGGING = False
+
     def __init__(self, cacheController: ACICacheControllerABC, clientId: str):
         """App ChunkedIndex Handler
 
-        This class handles the custom needs of the desktop/mobile apps observing chunkedIndexs.
+        This class handles the custom needs of the desktop/mobile apps
+         observing chunkedIndexes.
 
         """
         self._cacheController = cacheController
         self._clientId = clientId
 
         self._epObserve = PayloadEndpoint(
-            self._updateFromDeviceFilt, self._processObserve
+            self._updateFromDeviceFilt, self._processObserveLimited
         )
 
         self._uuidsObserving = set()
 
-        # If the vortex goes online, check the cache.
-        # Before this line of code, the vortex is already online.
-        (
-            VortexFactory.subscribeToVortexStatusChange(peekServerName)
-            .filter(lambda online: online is True)
-            .subscribe(on_next=self._startObserving)
-        )
-
-    def _startObserving(self, *args):
-        # Tell the logic service that this vortexUuid is interested in its data
-        VortexFactory.sendVortexMsg(
-            vortexMsgs=PayloadEnvelope(
-                filt=self._updateFromLogicFilt
-            ).toVortexMsg(),
-            destVortexName=peekServerName,
-        )
-
     @inlineCallbacks
     def start(self):
-        yield self._startObserving()
+        yield None
 
     def shutdown(self):
         self._epObserve.shutdown()
         self._epObserve = None
 
     def _filterOutOfflineVortexes(self):
         # TODO, Change this to observe offline vortexes
@@ -79,23 +77,34 @@
             set(VortexFactory.getRemoteVortexUuids()) & self._uuidsObserving
         )
         self._uuidsObserving = vortexUuids
 
     # ---------------
     # Process update from the server
 
+    def notifyOfUpdateBeforeSemaphore(self, chunkKeys: list[str]):
+        return self._notifyOfUpdateLimitedDecorated(chunkKeys)
+
+    @limitConcurrency(cacheHandlerLogger, 10)
+    def _notifyOfUpdateLimitedDecorated(self, *args, **kwargs):
+        return self.notifyOfUpdate(*args, **kwargs)
+
+    @inlineCallbacks
     def notifyOfUpdate(self, chunkKeys: List[str]):
         """Notify of ChunkedIndex Updates
 
-        This method is called by the client.ChunkedIndexCacheController when it receives updates
-        from the server.
+        This method is called by the client.ChunkedIndexCacheController
+         when it receives updates from the server.
 
         """
         self._filterOutOfflineVortexes()
 
+        if not self._uuidsObserving:
+            return
+
         def cratePayloadEnvelope():
             payloadEnvelope = PayloadEnvelope()
             payloadEnvelope.data = []
             return payloadEnvelope
 
         payloadsByVortexUuid = defaultdict(cratePayloadEnvelope)
 
@@ -112,117 +121,173 @@
                     vortexUuid,
                 )
                 payloadsByVortexUuid[vortexUuid].data.append(
                     encodedChunkedIndexChunk
                 )
 
         # Send the updates to the clients
-        dl = []
         for vortexUuid, payloadEnvelope in list(payloadsByVortexUuid.items()):
             payloadEnvelope.filt = self._updateFromDeviceFilt
 
-            # Serialise in thread, and then send.
-            d = payloadEnvelope.toVortexMsgDefer(base64Encode=False)
-            d.addCallback(
-                VortexFactory.sendVortexMsg, destVortexUuid=vortexUuid
+            vortexMsg = yield payloadEnvelope.toVortexMsgDefer(
+                base64Encode=False
             )
-            dl.append(d)
 
-        # Log the errors, otherwise we don't care about them
-        dl = DeferredList(dl, fireOnOneErrback=True)
-        dl.addErrback(vortexLogFailure, self._logger, consumeError=True)
+            try:
+                yield VortexFactory.sendVortexMsg(
+                    vortexMsg, destVortexUuid=vortexUuid
+                )
+
+            except NoVortexException:
+                pass
+
+            except Exception as e:
+                self._logger.exception(e)
 
     # ---------------
     # Process observes from the devices
+
+    def _processObserveLimited(self, *args, **kwargs):
+        d = self._processObserveLimitedDecorated(*args, **kwargs)
+        d.addErrback(vortexLogFailure, self._logger, consumeError=True)
+
+    @limitConcurrency(cacheHandlerLogger, 50)
+    def _processObserveLimitedDecorated(self, *args, **kwargs):
+        return self._processObserve(*args, **kwargs)
+
     @inlineCallbacks
     def _processObserve(
         self,
         payloadEnvelope: PayloadEnvelope,
         vortexUuid: str,
         sendResponse: SendVortexMsgResponseCallable,
-        **kwargs
+        **kwargs,
     ):
+        cacheAll = payloadEnvelope.filt.get("cacheAll") is True
 
         payload = yield payloadEnvelope.decodePayloadDefer()
 
         updateDatesTuples: ACIUpdateDateTupleABC = payload.tuples[0]
 
-        self._uuidsObserving.add(vortexUuid)
+        if updateDatesTuples.ckiUpdateDateByChunkKey is None:
+            self._logger.debug(
+                "BUG: " "updateDatesTuples.ckiUpdateDateByChunkKey is " "None"
+            )
+            return
+
+        if not cacheAll:
+            self._uuidsObserving.add(vortexUuid)
 
         yield self._replyToObserve(
-            payload.filt,
+            payloadEnvelope.filt,
             updateDatesTuples.ckiUpdateDateByChunkKey,
             sendResponse,
-            vortexUuid,
+            vortexUuid=vortexUuid,
+            cacheAll=cacheAll,
         )
 
     # ---------------
     # Reply to device observe
 
     @inlineCallbacks
     def _replyToObserve(
         self,
         filt,
         lastUpdateByChunkedIndexKey: Dict[str, str],
         sendResponse: SendVortexMsgResponseCallable,
         vortexUuid: str,
+        cacheAll=False,
     ) -> None:
         """Reply to Observe
 
-        The client has told us that it's observing a new set of chunkedIndexs, and the lastUpdate
-        it has for each of those chunkedIndexs. We will send them the chunkedIndexs that are out of date
+        The client has told us that it's observing a new set of chunkedIndexes,
+        and the lastUpdate it has for each of those chunkedIndexes. We will
+        send them the chunkedIndexes that are out of date
         or missing.
 
         :param filt: The payload filter to respond to.
-        :param lastUpdateByChunkedIndexKey: The dict of chunkedIndexKey:lastUpdate
+        :param lastUpdateByChunkedIndexKey:
+            The dict of chunkedIndexKey:lastUpdate
         :param sendResponse: The callable provided by the Vortex (handy)
         :returns: None
 
         """
+        startTime = datetime.now(pytz.utc)
         yield None
 
         chunkedIndexTuplesToSend = []
+        updateCount = 0
+        sameCount = 0
+        missingCount = 0
 
         # Check and send any updates
         for chunkedIndexKey, lastUpdate in lastUpdateByChunkedIndexKey.items():
             if vortexUuid not in VortexFactory.getRemoteVortexUuids():
                 self._logger.debug(
                     "Vortex %s is offline, stopping update", vortexUuid
                 )
                 return
 
             # NOTE: lastUpdate can be null.
             encodedChunkedIndexTuple = self._cacheController.encodedChunk(
                 chunkedIndexKey
             )
             if not encodedChunkedIndexTuple:
-                self._logger.debug(
-                    "ChunkedIndex %s is not in the cache" % chunkedIndexKey
-                )
+                missingCount += 1
+                if self._DEBUG_LOGGING:
+                    self._logger.debug(
+                        "ChunkedIndex %s is not in the cache" % chunkedIndexKey
+                    )
                 continue
 
-            # We are king, If it's it's not our version, it's the wrong version ;-)
-            self._logger.debug(
-                "%s, %s,  %s",
-                encodedChunkedIndexTuple.ckiLastUpdate == lastUpdate,
-                encodedChunkedIndexTuple.ckiLastUpdate,
-                lastUpdate,
-            )
-
-            if encodedChunkedIndexTuple.ckiLastUpdate == lastUpdate:
+            # We are king, If it's not our version, it's the wrong version
+            if self._DEBUG_LOGGING:
                 self._logger.debug(
-                    "ChunkedIndex %s matches the cache" % chunkedIndexKey
+                    "%s, %s,  %s",
+                    encodedChunkedIndexTuple.ckiLastUpdate == lastUpdate,
+                    encodedChunkedIndexTuple.ckiLastUpdate,
+                    lastUpdate,
                 )
+
+            if encodedChunkedIndexTuple.ckiLastUpdate == lastUpdate:
+                sameCount += 1
+                if self._DEBUG_LOGGING:
+                    self._logger.debug(
+                        "ChunkedIndex %s matches the cache" % chunkedIndexKey
+                    )
                 continue
 
+            updateCount += 1
             chunkedIndexTuplesToSend.append(encodedChunkedIndexTuple)
-            self._logger.debug(
-                "Sending chunkedIndex %s from the cache" % chunkedIndexKey
-            )
+            if self._DEBUG_LOGGING:
+                self._logger.debug(
+                    "Sending chunkedIndex %s from the cache" % chunkedIndexKey
+                )
 
-        # Send the payload to the frontend
-        payloadEnvelope = PayloadEnvelope(
-            filt=filt, data=chunkedIndexTuplesToSend
+        yield self._sendData(
+            sendResponse, filt, cacheAll, chunkedIndexTuplesToSend
         )
-        d: Deferred = payloadEnvelope.toVortexMsgDefer(base64Encode=False)
-        d.addCallback(sendResponse)
-        d.addErrback(vortexLogFailure, self._logger, consumeError=True)
+
+        self._logger.debug(
+            "Chunk request, %s same, %s not in cache,"
+            " %s updates sent to %s in %s",
+            sameCount,
+            missingCount,
+            updateCount,
+            vortexUuid,
+            datetime.now(pytz.utc) - startTime,
+        )
+
+    @inlineCallbacks
+    def _sendData(
+        self,
+        sendResponse: SendVortexMsgResponseCallable,
+        filt: dict,
+        cacheAll: bool,
+        chunksToSend: list,
+    ):
+        if not chunksToSend and not cacheAll:
+            return
+
+        payloadEnvelope = PayloadEnvelope(filt=filt, data=chunksToSend)
+        vortexMsg = yield payloadEnvelope.toVortexMsgDefer(base64Encode=False)
+        yield sendResponse(vortexMsg)
```

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     ) -> list[Tuple]:
         """Chunked Key Index - Initial Load Chunks Blocking
 
         This method is used to load the initial set of chunks from the server
         to the client.
 
         """
+        chunkKeys = [str(ck) for ck in chunkKeys]
         if sql is None:
             table = Declarative.__table__
             sql = select([table]).where(
                 Declarative.sqlCoreChunkKeyColumn().in_(chunkKeys)
             )
 
         sqlStr = str(
@@ -93,14 +94,15 @@
         )
 
         return runPyInPgBlocking(
             self._dbSessionCreator,
             self._load,
             sqlCoreLoadModStr=sqlCoreLoadModStr,
             sqlStr=sqlStr,
+            chunkKeys=chunkKeys,
         )
 
     @classmethod
     def _loadIndexDelta(
         cls,
         plpy,
         sqlStr: str,
@@ -146,15 +148,15 @@
 
         indexIn.ckiSetUpdateDateByChunkKey(deltas)
         indexIn.ckiSetInitialLoadComplete(False)
 
         return Payload(tuples=[indexIn]).toEncodedPayload()
 
     @classmethod
-    def _load(cls, plpy, sqlStr, sqlCoreLoadModStr):
+    def _load(cls, plpy, sqlStr, sqlCoreLoadModStr, chunkKeys: list[str]):
 
         TupleClass = cls._loadTupleClass(sqlCoreLoadModStr)
         tupleLoaderMethod = TupleClass.sqlCoreLoad
 
         # ---------------
         # Turn a row["val"] into a row.val
         class Wrap:
@@ -174,14 +176,24 @@
             rows = cursor.fetch(500)
             if not rows:
                 break
             for row in rows:
                 wrap.row = row
                 results.append(tupleLoaderMethod(wrap))
 
+        # ---------------
+        # Process the results, create blanks where the chunk has been deleted
+
+        deletedChunkKeys = set(chunkKeys) - set(
+            [r.ckiChunkKey for r in results]
+        )
+
+        for chunkKey in deletedChunkKeys:
+            results.append(TupleClass.ckiCreateDeleteEncodedChunk(chunkKey))
+
         return (
             json.dumps(Payload(tuples=results).toJsonDict())
             if results
             else None
         )
 
     @classmethod
```

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,17 +436,15 @@
                 items.append(item)
                 itemUniqueIds.append(item.ckiUniqueKey)
 
             itemsEncodedPayload = Payload(
                 tuples=[items, queueIds]
             ).toEncodedPayload()
 
-            queueBlocks.append(
-                (queueIds, itemsEncodedPayload.decode(), itemUniqueIds)
-            )
+            queueBlocks.append((queueIds, itemsEncodedPayload, itemUniqueIds))
 
         # Put the oldest queue blocks back at the start
         queueBlocks = list(reversed(queueBlocks))
 
         return queueBlocks
 
     @abstractmethod
```

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from abc import ABCMeta, abstractmethod
+from abc import ABCMeta
+from abc import abstractmethod
 
 
 class ACIProcessorStatusNotifierABC(metaclass=ABCMeta):
     @abstractmethod
     def setProcessorStatus(self, state: bool, queueSize: int):
         """Set Processor Status
```

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.3.3/peek_abstract_chunked_index.egg-info/SOURCES.txt` & `peek-abstract-chunked-index-3.4.0/peek_abstract_chunked_index.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,26 @@
 peek_abstract_chunked_index/plugin-module/index.ts
 peek_abstract_chunked_index/plugin-module/_private/PluginNames.ts
 peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts
 peek_abstract_chunked_index/plugin-module/_private/index.ts
 peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts
 peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexEncodedChunkTuple.ts
 peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts
-peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderStatusTuple.ts
 peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts
 peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/index.ts
 peek_abstract_chunked_index/plugin-module/_private/tuples/OfflineConfigTuple.ts
 peek_abstract_chunked_index/private/__init__.py
 peek_abstract_chunked_index/private/alembic.ini
 peek_abstract_chunked_index/private/client/__init__.py
 peek_abstract_chunked_index/private/client/controller/ACICacheControllerABC.py
+peek_abstract_chunked_index/private/client/controller/ACICacheControllerLoadFromLogicMixin.py
+peek_abstract_chunked_index/private/client/controller/ACICacheControllerNotifyMixin.py
+peek_abstract_chunked_index/private/client/controller/ACICacheControllerOfflineIndexMixin.py
+peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteAppDbMixin.py
+peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteCacheMixin.py
 peek_abstract_chunked_index/private/client/controller/__init__.py
 peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py
 peek_abstract_chunked_index/private/client/handlers/__init__.py
 peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo
 peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo
 peek_abstract_chunked_index/private/client/tuple_providers/__init__.py
 peek_abstract_chunked_index/private/server/__init__.py
```

### Comparing `peek-abstract-chunked-index-3.3.3/setup.py` & `peek-abstract-chunked-index-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_abstract_chunked_index"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Abstract Chunked Index"
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

