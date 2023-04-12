# Comparing `tmp/peek-plugin-base-3.3.3.tar.gz` & `tmp/peek-plugin-base-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-base-3.3.3.tar", last modified: Mon Nov 14 05:36:34 2022, max compression
+gzip compressed data, was "peek-plugin-base-3.4.0.tar", last modified: Wed Apr 12 11:05:19 2023, max compression
```

## Comparing `peek-plugin-base-3.3.3.tar` & `peek-plugin-base-3.4.0.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.227039 peek-plugin-base-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      365 2022-11-14 05:36:34.227039 peek-plugin-base-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.223039 peek-plugin-base-3.3.3/peek_plugin_base/
--rw-r--r--   0 root         (0) root         (0)      871 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/LoopingCallUtil.py
--rw-r--r--   0 root         (0) root         (0)      703 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/PeekPlatformCommonHookABC.py
--rw-r--r--   0 root         (0) root         (0)      830 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/PeekPlatformFileStorageHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1807 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/PeekPlatformServerInfoHookABC.py
--rw-r--r--   0 root         (0) root         (0)      976 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/PeekVortexUtil.py
--rw-r--r--   0 root         (0) root         (0)     1765 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/PluginCommonEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)     2094 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/PluginPackageFileConfig.py
--rw-r--r--   0 root         (0) root         (0)      106 2022-11-14 05:36:33.000000 peek-plugin-base-3.3.3/peek_plugin_base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.224039 peek-plugin-base-3.3.3/peek_plugin_base/agent/
--rw-r--r--   0 root         (0) root         (0)      462 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/agent/PeekAgentPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1200 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1481 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/agent/PluginAgentEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.224039 peek-plugin-base-3.3.3/peek_plugin_base/client/
--rw-r--r--   0 root         (0) root         (0)      705 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/client/PeekClientPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1660 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1668 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     2581 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/client/PluginClientEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.224039 peek-plugin-base-3.3.3/peek_plugin_base/server/
--rw-r--r--   0 root         (0) root         (0)     1660 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1594 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1060 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/PeekServerPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)     2017 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/PluginLogicEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1006 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py
--rw-r--r--   0 root         (0) root         (0)     2972 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/PluginServerStorageEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)      146 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/PluginServerWorkerEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.225039 peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2610 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3063 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py
--rw-r--r--   0 root         (0) root         (0)      416 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/simple_subproc_task_call_tuple.py
--rw-r--r--   0 root         (0) root         (0)      369 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/simple_subproc_task_constructor_tuple.py
--rw-r--r--   0 root         (0) root         (0)      483 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/simple_subproc_task_result_tuple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.225039 peek-plugin-base-3.3.3/peek_plugin_base/storage/
--rw-r--r--   0 root         (0) root         (0)     2613 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/storage/AlembicEnvBase.py
--rw-r--r--   0 root         (0) root         (0)    10178 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/storage/DbConnection.py
--rw-r--r--   0 root         (0) root         (0)     1253 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/storage/LoadPayloadPgUtil.py
--rw-r--r--   0 root         (0) root         (0)     1002 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/storage/RunPyInPg.py
--rw-r--r--   0 root         (0) root         (0)     1863 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/storage/StorageUtil.py
--rw-r--r--   0 root         (0) root         (0)      292 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/storage/TypeDecorators.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.225039 peek-plugin-base-3.3.3/peek_plugin_base/util/
--rw-r--r--   0 root         (0) root         (0)     1251 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/PeekPsUtil.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.226039 peek-plugin-base-3.3.3/peek_plugin_base/util/build_common/
--rw-r--r--   0 root         (0) root         (0)     3744 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_common/BuilderABC.py
--rw-r--r--   0 root         (0) root         (0)     2023 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_common/BuilderOsCmd.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.226039 peek-plugin-base-3.3.3/peek_plugin_base/util/build_doc/
--rw-r--r--   0 root         (0) root         (0)     3656 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_doc/DocBuilder.py
--rw-r--r--   0 root         (0) root         (0)     7496 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_doc/DocBuilderABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.226039 peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/
--rw-r--r--   0 root         (0) root         (0)     5184 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py
--rw-r--r--   0 root         (0) root         (0)    22377 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py
--rw-r--r--   0 root         (0) root         (0)    14140 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/FrontendFileSync.py
--rw-r--r--   0 root         (0) root         (0)     9870 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/WebBuilder.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.226039 peek-plugin-base-3.3.3/peek_plugin_base/worker/
--rw-r--r--   0 root         (0) root         (0)       57 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/worker/CeleryApp.py
--rw-r--r--   0 root         (0) root         (0)     2855 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/worker/CeleryDbConn.py
--rw-r--r--   0 root         (0) root         (0)     1781 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/worker/CeleryDbConnInit.py
--rw-r--r--   0 root         (0) root         (0)      152 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/worker/PeekWorkerPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)      991 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/worker/PluginWorkerEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-plugin-base-3.3.3/peek_plugin_base/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:34.223039 peek-plugin-base-3.3.3/peek_plugin_base.egg-info/
--rw-r--r--   0 root         (0) root         (0)      365 2022-11-14 05:36:34.000000 peek-plugin-base-3.3.3/peek_plugin_base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3074 2022-11-14 05:36:34.000000 peek-plugin-base-3.3.3/peek_plugin_base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:34.000000 peek-plugin-base-3.3.3/peek_plugin_base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:34.000000 peek-plugin-base-3.3.3/peek_plugin_base.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      264 2022-11-14 05:36:34.000000 peek-plugin-base-3.3.3/peek_plugin_base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-14 05:36:34.000000 peek-plugin-base-3.3.3/peek_plugin_base.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:36:34.227039 peek-plugin-base-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2665 2022-11-14 05:36:33.000000 peek-plugin-base-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.367206 peek-plugin-base-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-04-12 11:05:19.367206 peek-plugin-base-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.364206 peek-plugin-base-3.4.0/peek_plugin_base/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/LoopingCallUtil.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/PeekPlatformCommonHookABC.py
+-rw-r--r--   0 root         (0) root         (0)      830 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/PeekPlatformFileStorageHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/PeekPlatformServerInfoHookABC.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/PeekVortexUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/PluginCommonEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/PluginPackageFileConfig.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.364206 peek-plugin-base-3.4.0/peek_plugin_base/agent/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/agent/PeekAgentPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/agent/PluginAgentEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.365206 peek-plugin-base-3.4.0/peek_plugin_base/client/
+-rw-r--r--   0 root         (0) root         (0)      705 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/client/PeekClientPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/client/PluginClientEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.365206 peek-plugin-base-3.4.0/peek_plugin_base/server/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/PeekServerPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/PluginLogicEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/PluginServerStorageEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/PluginServerWorkerEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.365206 peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/simple_subproc_task_call_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/simple_subproc_task_constructor_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/simple_subproc_task_result_tuple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.366206 peek-plugin-base-3.4.0/peek_plugin_base/storage/
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/storage/AlembicEnvBase.py
+-rw-r--r--   0 root         (0) root         (0)    11090 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/storage/DbConnection.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/storage/LoadPayloadPgUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/storage/RunPyInPg.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/storage/StorageUtil.py
+-rw-r--r--   0 root         (0) root         (0)      292 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/storage/TypeDecorators.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.366206 peek-plugin-base-3.4.0/peek_plugin_base/util/
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/PeekPsUtil.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.366206 peek-plugin-base-3.4.0/peek_plugin_base/util/build_common/
+-rw-r--r--   0 root         (0) root         (0)     3744 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_common/BuilderABC.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_common/BuilderOsCmd.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.366206 peek-plugin-base-3.4.0/peek_plugin_base/util/build_doc/
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_doc/DocBuilder.py
+-rw-r--r--   0 root         (0) root         (0)     7496 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_doc/DocBuilderABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_doc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.366206 peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/
+-rw-r--r--   0 root         (0) root         (0)     5184 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py
+-rw-r--r--   0 root         (0) root         (0)    22377 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py
+-rw-r--r--   0 root         (0) root         (0)    14140 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/FrontendFileSync.py
+-rw-r--r--   0 root         (0) root         (0)     9870 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/WebBuilder.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.367206 peek-plugin-base-3.4.0/peek_plugin_base/worker/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/CeleryApp.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/CeleryDbConn.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/CeleryDbConnInit.py
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/CeleryFileStorageConfig.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/CeleryLogicServerInfoConfig.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/PeekWorkerPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/PluginWorkerEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-plugin-base-3.4.0/peek_plugin_base/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:19.364206 peek-plugin-base-3.4.0/peek_plugin_base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/peek_plugin_base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/peek_plugin_base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/peek_plugin_base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/peek_plugin_base.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      264 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/peek_plugin_base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/peek_plugin_base.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:05:19.367206 peek-plugin-base-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-04-12 11:05:19.000000 peek-plugin-base-3.4.0/setup.py
```

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/LoopingCallUtil.py` & `peek-plugin-base-3.4.0/peek_plugin_base/LoopingCallUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/PeekPlatformCommonHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/PeekPlatformCommonHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/PeekPlatformFileStorageHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/PeekPlatformFileStorageHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/PeekPlatformServerInfoHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/PeekPlatformServerInfoHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/PeekVortexUtil.py` & `peek-plugin-base-3.4.0/peek_plugin_base/PeekVortexUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/PlatformDependencyTest.py` & `peek-plugin-base-3.4.0/peek_plugin_base/PlatformDependencyTest.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/PluginCommonEntryHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/PluginCommonEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/PluginPackageFileConfig.py` & `peek-plugin-base-3.4.0/peek_plugin_base/PluginPackageFileConfig.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/agent/PluginAgentEntryHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/agent/PluginAgentEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/client/PeekClientPlatformHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/client/PeekClientPlatformHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/client/PluginClientEntryHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/client/PluginClientEntryHookABC.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,21 +56,24 @@
         """
         relDir = self._packageCfg.config.plugin.title(require_string)
         dir = os.path.join(self._pluginRoot, relDir)
         if not os.path.isdir(dir):
             raise NotADirectoryError(dir)
         return dir
 
+    # TODO: Remove this, Plugins should access platform config via self.platform
     @property
     def platformConfig(self):
         return PeekPlatformConfig.config
 
+    # TODO, Remove this
     def copyFolder(self, srcDir: Path, dstDir: Path):
         shutil.copytree(srcDir, dstDir, dirs_exist_ok=True)
 
+    # TODO, Move this to PeekClientPlatformHookABC
     def createProxy(self) -> HttpResourceProxy:
         return HttpResourceProxy(
             self.platform.peekServerHost,
             self.platform.peekServerHttpPort,
             useSsl=self.platform.peekServerSSL,
             sslEnableMutualTLS=self.platform.peekServerSSLEnableMutualTLS,
             sslClientCertificateBundleFilePath=self.platform.peekServerSSLClientBundleFilePath,
```

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/server/PeekServerPlatformHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/server/PeekServerPlatformHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/server/PluginLogicEntryHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/server/PluginLogicEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py` & `peek-plugin-base-3.4.0/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/server/PluginServerStorageEntryHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/server/PluginServerStorageEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py` & `peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py` & `peek-plugin-base-3.4.0/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/storage/AlembicEnvBase.py` & `peek-plugin-base-3.4.0/peek_plugin_base/storage/AlembicEnvBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/storage/DbConnection.py` & `peek-plugin-base-3.4.0/peek_plugin_base/storage/DbConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
+import traceback
 from io import StringIO
 from textwrap import dedent
 from threading import Lock
 from typing import Optional, Dict, Union, Callable, Iterable
 
 import sqlalchemy_utils
+from vortex.DeferUtil import isMainThread
+
 from peek_plugin_base.storage.AlembicEnvBase import (
     ensureSchemaExists,
     isMssqlDialect,
     isPostGreSQLDialect,
 )
 from pytmpdir.directory_ import Directory
 from sqlalchemy import create_engine, Integer
@@ -68,15 +71,27 @@
         """
         self._dbConnectString = dbConnectString
         self._metadata = metadata
         self._alembicDir = alembicDir
 
         self._dbEngine = None
         self._ScopedSession = None
-        self._dbEngineArgs = dbEngineArgs if dbEngineArgs else {"echo": False}
+        self._dbEngineArgs = (
+            dbEngineArgs
+            if dbEngineArgs
+            else {
+                "client_encoding": "utf8",
+                "echo": False,
+                "executemany_mode": "batch",
+                "max_overflow": 50,
+                "pool_recycle": 3540,
+                "pool_size": 5,
+                "pool_timeout": 60,
+            }
+        )
 
         self._sequenceMutex = Lock()
 
         self._enableForeignKeys = enableForeignKeys
         self._enableCreateAll = enableCreateAll
 
     def closeAllSessions(self):
@@ -86,14 +101,32 @@
 
         """
         self.ormSessionCreator()  # Ensure we have a session maker and session
         self._ScopedSession.close_all()
 
     @property
     def ormSessionCreator(self) -> DbSessionCreator:
+        sessionCreator = self.__ormSessionCreator
+
+        def call():
+            if isMainThread():
+                logger.warning(
+                    "This plugin has called"
+                    " SQLAlchemy code in the main thread,"
+                    " this is very bad"
+                )
+                for line in traceback.format_stack():
+                    logger.debug(line.strip().replace("\n", ""))
+
+            return sessionCreator()
+
+        return call
+
+    @property
+    def __ormSessionCreator(self) -> DbSessionCreator:
         """Get Orm Session
 
         :return: A SQLAlchemy session scoped for the callers thread..
         """
         assert self._dbConnectString
 
         if self._ScopedSession:
```

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/storage/LoadPayloadPgUtil.py` & `peek-plugin-base-3.4.0/peek_plugin_base/storage/LoadPayloadPgUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/storage/RunPyInPg.py` & `peek-plugin-base-3.4.0/peek_plugin_base/storage/RunPyInPg.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/storage/StorageUtil.py` & `peek-plugin-base-3.4.0/peek_plugin_base/storage/StorageUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_common/BuilderABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_common/BuilderABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_common/BuilderOsCmd.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_common/BuilderOsCmd.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_doc/DocBuilder.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_doc/DocBuilder.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_doc/DocBuilderABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_doc/DocBuilderABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/FrontendFileSync.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/FrontendFileSync.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/util/build_frontend/WebBuilder.py` & `peek-plugin-base-3.4.0/peek_plugin_base/util/build_frontend/WebBuilder.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/worker/CeleryDbConn.py` & `peek-plugin-base-3.4.0/peek_plugin_base/worker/CeleryDbConn.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,26 +31,30 @@
     global _dbEngineArgs
     from peek_platform.file_config.PeekFileConfigABC import PeekFileConfigABC
     from peek_platform.file_config.PeekFileConfigSqlAlchemyMixin import (
         PeekFileConfigSqlAlchemyMixin,
     )
     from peek_platform import PeekPlatformConfig
 
-    class _WorkerTaskConfigMixin(PeekFileConfigABC, PeekFileConfigSqlAlchemyMixin):
+    class _WorkerTaskConfigMixin(
+        PeekFileConfigABC, PeekFileConfigSqlAlchemyMixin
+    ):
         pass
 
     PeekPlatformConfig.componentName = peekWorkerName
 
     _dbConnectString = _WorkerTaskConfigMixin().dbConnectString
     _dbEngineArgs = _WorkerTaskConfigMixin().dbEngineArgs
 
 
 # For celery, an engine is created per worker
 def getDbEngine():
     global __dbEngine
+    global _dbConnectString
+    global _dbEngineArgs
 
     if _dbConnectString is None:
         if _isWindows:
             from peek_platform.ConfigCeleryApp import configureCeleryLogging
 
             configureCeleryLogging()
             setConnStringForWindows()
```

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/worker/CeleryDbConnInit.py` & `peek-plugin-base-3.4.0/peek_plugin_base/worker/CeleryDbConnInit.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base/worker/PluginWorkerEntryHookABC.py` & `peek-plugin-base-3.4.0/peek_plugin_base/worker/PluginWorkerEntryHookABC.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from abc import abstractproperty
 
 from celery.app.base import Celery
 from peek_plugin_base.PluginCommonEntryHookABC import PluginCommonEntryHookABC
-from peek_plugin_base.worker.PeekWorkerPlatformHookABC import PeekWorkerPlatformHookABC
+from peek_plugin_base.worker.PeekWorkerPlatformHookABC import (
+    PeekWorkerPlatformHookABC,
+)
 
 
 class PluginWorkerEntryHookABC(PluginCommonEntryHookABC):
     def __init__(
-        self, pluginName: str, pluginRootDir: str, platform: PeekWorkerPlatformHookABC
+        self,
+        pluginName: str,
+        pluginRootDir: str,
+        platform: PeekWorkerPlatformHookABC,
     ):
         PluginCommonEntryHookABC.__init__(
             self, pluginName=pluginName, pluginRootDir=pluginRootDir
         )
         self._platform = platform
 
     @property
     def platform(self) -> PeekWorkerPlatformHookABC:
         return self._platform
 
     @abstractproperty
     def celeryAppIncludes(self) -> [str]:
         """Celery App Includes
 
-        This property returns the absolout package paths to the modules with the tasks
+        This property returns the absolute package paths to the modules with the tasks
         :Example: ["plugin_noop.worker.NoopWorkerTask"]
 
         :return: A list of package+module names that Celery should import.
 
         """
```

### Comparing `peek-plugin-base-3.3.3/peek_plugin_base.egg-info/SOURCES.txt` & `peek-plugin-base-3.4.0/peek_plugin_base.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,10 +57,12 @@
 peek_plugin_base/util/build_frontend/FrontendBuilderABC.py
 peek_plugin_base/util/build_frontend/FrontendFileSync.py
 peek_plugin_base/util/build_frontend/WebBuilder.py
 peek_plugin_base/util/build_frontend/__init__.py
 peek_plugin_base/worker/CeleryApp.py
 peek_plugin_base/worker/CeleryDbConn.py
 peek_plugin_base/worker/CeleryDbConnInit.py
+peek_plugin_base/worker/CeleryFileStorageConfig.py
+peek_plugin_base/worker/CeleryLogicServerInfoConfig.py
 peek_plugin_base/worker/PeekWorkerPlatformHookABC.py
 peek_plugin_base/worker/PluginWorkerEntryHookABC.py
 peek_plugin_base/worker/__init__.py
```

### Comparing `peek-plugin-base-3.3.3/setup.py` & `peek-plugin-base-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_base"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin Base."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

