# Comparing `tmp/peek-platform-3.3.3.tar.gz` & `tmp/peek-platform-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-platform-3.3.3.tar", last modified: Mon Nov 14 05:36:38 2022, max compression
+gzip compressed data, was "peek-platform-3.4.0.tar", last modified: Wed Apr 12 11:05:24 2023, max compression
```

## Comparing `peek-platform-3.3.3.tar` & `peek-platform-3.4.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.929008 peek-platform-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      353 2022-11-14 05:36:38.929008 peek-platform-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       96 2022-11-14 05:34:28.000000 peek-platform-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.925008 peek-platform-3.3.3/peek_platform/
--rw-r--r--   0 root         (0) root         (0)     4386 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/CeleryPatchToPlPython.py
--rw-r--r--   0 root         (0) root         (0)     7177 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/ConfigCeleryApp.py
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      828 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/WindowsPatch.py
--rw-r--r--   0 root         (0) root         (0)      990 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.926008 peek-platform-3.3.3/peek_platform/file_config/
--rw-r--r--   0 root         (0) root         (0)     3628 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigABC.py
--rw-r--r--   0 root         (0) root         (0)     2475 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py
--rw-r--r--   0 root         (0) root         (0)     2527 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py
--rw-r--r--   0 root         (0) root         (0)      989 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigDocBuildMixin.py
--rw-r--r--   0 root         (0) root         (0)     2041 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py
--rw-r--r--   0 root         (0) root         (0)     1444 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigHttpServerMixin.py
--rw-r--r--   0 root         (0) root         (0)      624 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigOsMixin.py
--rw-r--r--   0 root         (0) root         (0)     8032 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigPlatformMixin.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py
--rw-r--r--   0 root         (0) root         (0)     3428 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigTest.py
--rw-r--r--   0 root         (0) root         (0)     2787 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigWorkerMixin.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/file_config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.926008 peek-platform-3.3.3/peek_platform/platform_init/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/platform_init/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11125 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/platform_init/init_platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.927008 peek-platform-3.3.3/peek_platform/plugin/
--rw-r--r--   0 root         (0) root         (0)    17524 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/plugin/PluginLoaderABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.927008 peek-platform-3.3.3/peek_platform/subproc_plugin_init/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.928008 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4004 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py
--rw-r--r--   0 root         (0) root         (0)     2999 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py
--rw-r--r--   0 root         (0) root         (0)     2161 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py
--rw-r--r--   0 root         (0) root         (0)     3270 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1323 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py
--rw-r--r--   0 root         (0) root         (0)      200 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_constants.py
--rw-r--r--   0 root         (0) root         (0)     7499 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py
--rw-r--r--   0 root         (0) root         (0)      353 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_platform_config_tuple.py
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py
--rw-r--r--   0 root         (0) root         (0)      570 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py
--rw-r--r--   0 root         (0) root         (0)     5294 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py
--rw-r--r--   0 root         (0) root         (0)     4401 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.928008 peek-platform-3.3.3/peek_platform/sw_install/
--rw-r--r--   0 root         (0) root         (0)     9495 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/sw_install/PeekSwInstallManagerABC.py
--rw-r--r--   0 root         (0) root         (0)     8235 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/sw_install/PluginSwInstallManagerABC.py
--rw-r--r--   0 root         (0) root         (0)      162 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/sw_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.928008 peek-platform-3.3.3/peek_platform/sw_version/
--rw-r--r--   0 root         (0) root         (0)     3875 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/sw_version/PeekSwVersionPollHandler.py
--rw-r--r--   0 root         (0) root         (0)      332 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/sw_version/PeekSwVersionTuple.py
--rw-r--r--   0 root         (0) root         (0)      162 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/sw_version/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.929008 peek-platform-3.3.3/peek_platform/util/
--rw-r--r--   0 root         (0) root         (0)     2500 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/util/LogUtil.py
--rw-r--r--   0 root         (0) root         (0)     1719 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/util/ManHoleUtil.py
--rw-r--r--   0 root         (0) root         (0)     8893 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/util/MemUtil.py
--rw-r--r--   0 root         (0) root         (0)     7221 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/util/PtyUtil.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2676 2022-11-14 05:34:28.000000 peek-platform-3.3.3/peek_platform/winsvc_peek_restarter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:38.925008 peek-platform-3.3.3/peek_platform.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2857 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      530 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-14 05:36:38.000000 peek-platform-3.3.3/peek_platform.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-14 05:36:38.929008 peek-platform-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4754 2022-11-14 05:36:38.000000 peek-platform-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.636206 peek-platform-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-12 11:05:24.636206 peek-platform-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-12 11:03:19.000000 peek-platform-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.633206 peek-platform-3.4.0/peek_platform/
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/CeleryPatchToPlPython.py
+-rw-r--r--   0 root         (0) root         (0)     7177 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/ConfigCeleryApp.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/WindowsPatch.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.634206 peek-platform-3.4.0/peek_platform/file_config/
+-rw-r--r--   0 root         (0) root         (0)     3628 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigABC.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigDocBuildMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigHttpServerMixin.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigOsMixin.py
+-rw-r--r--   0 root         (0) root         (0)     8032 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigPlatformMixin.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigWorkerMixin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/file_config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.634206 peek-platform-3.4.0/peek_platform/platform_init/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/platform_init/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11125 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/platform_init/init_platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.634206 peek-platform-3.4.0/peek_platform/plugin/
+-rw-r--r--   0 root         (0) root         (0)    17891 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/plugin/PluginLoaderABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.635206 peek-platform-3.4.0/peek_platform/subproc_plugin_init/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.635206 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_constants.py
+-rw-r--r--   0 root         (0) root         (0)     7744 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_platform_config_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      570 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.635206 peek-platform-3.4.0/peek_platform/sw_install/
+-rw-r--r--   0 root         (0) root         (0)     9495 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/sw_install/PeekSwInstallManagerABC.py
+-rw-r--r--   0 root         (0) root         (0)     8235 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/sw_install/PluginSwInstallManagerABC.py
+-rw-r--r--   0 root         (0) root         (0)      162 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/sw_install/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.635206 peek-platform-3.4.0/peek_platform/sw_version/
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/sw_version/PeekSwVersionPollHandler.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/sw_version/PeekSwVersionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      162 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/sw_version/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.636206 peek-platform-3.4.0/peek_platform/util/
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/util/LogUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/util/ManHoleUtil.py
+-rw-r--r--   0 root         (0) root         (0)     8893 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/util/MemUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/util/PtyUtil.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2023-04-12 11:03:19.000000 peek-platform-3.4.0/peek_platform/winsvc_peek_restarter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:24.634206 peek-platform-3.4.0/peek_platform.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      530 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-12 11:05:24.000000 peek-platform-3.4.0/peek_platform.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 11:05:24.636206 peek-platform-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4754 2023-04-12 11:05:24.000000 peek-platform-3.4.0/setup.py
```

### Comparing `peek-platform-3.3.3/peek_platform/CeleryPatchToPlPython.py` & `peek-platform-3.4.0/peek_platform/CeleryPatchToPlPython.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/ConfigCeleryApp.py` & `peek-platform-3.4.0/peek_platform/ConfigCeleryApp.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/WindowsPatch.py` & `peek-platform-3.4.0/peek_platform/WindowsPatch.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/__init__.py` & `peek-platform-3.4.0/peek_platform/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import WindowsPatch
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 class PeekPlatformConfig:
     """Peek Platform Config
 
     This is really a GLOBAL pettern, It should be replaced at some stage.
     (Maybe named as a factory?)
```

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigABC.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigABC.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 from jsoncfg.value_mappers import require_bool
 from jsoncfg.value_mappers import require_string, require_integer
 
 from peek_platform.file_config.PeekFileConfigPlatformMixin import (
     PeekFileConfigPlatformMixin,
 )
+from peek_plugin_base.PeekPlatformServerInfoHookABC import (
+    PeekPlatformServerInfoHookABC,
+)
 
 
-class PeekFileConfigDataExchangeClientMixin(metaclass=ABCMeta):
+class PeekFileConfigDataExchangeClientMixin(PeekPlatformServerInfoHookABC):
     def __init__(self, config: PeekFileConfigPlatformMixin):
         self._config = config
 
     ### SERVER SECTION ###
     @property
     def peekServerHttpPort(self) -> int:
         with self._config._cfg as c:
@@ -22,15 +25,19 @@
 
     @property
     def peekServerHost(self) -> str:
         with self._config._cfg as c:
             return c.dataExchange.host("localhost", require_string)
 
     @property
-    def peekServerUseSSL(self) -> int:
+    def peekServerSSL(self) -> bool:
+        return self.peekServerUseSSL
+
+    @property
+    def peekServerUseSSL(self) -> bool:
         with self._config._cfg as c:
             return c.dataExchange.useSsl(False, require_bool)
 
     @property
     def peekServerSSLEnableMutualTLS(self) -> int:
         with self._config._cfg as c:
             return c.dataExchange.sslEnableMutualTLS(False, require_bool)
```

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigDocBuildMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigDocBuildMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigHttpServerMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigHttpServerMixin.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,14 +33,21 @@
 
     @property
     def useSsl(self) -> bool:
         with self._config._cfg as c:
             return c.httpServer[self._name].useSsl(False, require_bool)
 
     @property
+    def concurrentPeerIpConnectionLimit(self) -> int:
+        with self._config._cfg as c:
+            return c.httpServer[self._name].concurrentPeerIpConnectionLimit(
+                5, require_integer
+            )
+
+    @property
     def sslBundleFilePath(self) -> Optional[str]:
         default = os.path.join(self._config._homePath, "key-cert-cachain.pem")
         with self._config._cfg as c:
             file = c.httpServer[self._name].sslBundleFilePath(
                 default, require_string
             )
             if os.path.exists(file):
```

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigOsMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigOsMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigPlatformMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigPlatformMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,8 +28,12 @@
             val = c.sqlalchemy.engineArgs(default, require_dict)
             # Upgrade depreciated psycopg setting.
             if val.get("use_batch_mode") == True:
                 del val["use_batch_mode"]
                 val["executemany_mode"] = "batch"
                 c.sqlalchemy.engineArgs = val
 
+            if "client_encoding" not in val:
+                val["client_encoding"] = "utf8"
+                c.sqlalchemy.engineArgs = val
+
             return val
```

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigTest.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/file_config/PeekFileConfigWorkerMixin.py` & `peek-platform-3.4.0/peek_platform/file_config/PeekFileConfigWorkerMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/platform_init/init_platform.py` & `peek-platform-3.4.0/peek_platform/platform_init/init_platform.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/plugin/PluginLoaderABC.py` & `peek-platform-3.4.0/peek_platform/plugin/PluginLoaderABC.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import os
 import sys
 from abc import ABCMeta
 from abc import abstractmethod
 from abc import abstractproperty
 from collections import defaultdict
 from importlib.util import find_spec
-from typing import Any
 from typing import Optional
 from typing import Tuple
 from typing import Type
 
 from jsoncfg.value_mappers import require_array
 from jsoncfg.value_mappers import require_string
+from twisted.internet.defer import maybeDeferred
+from vortex.DeferUtil import vortexLogFailure
+
 from peek_platform import PeekPlatformConfig
 from twisted.internet.defer import inlineCallbacks
 
 from peek_platform.subproc_plugin_init.plugin_subproc.plugin_subproc_platform_config_tuple import (
     PluginSubprocPlatformConfigTuple,
 )
 from peek_platform.subproc_plugin_init.plugin_subproc.plugin_subproc_vortex_msg_tuple import (
@@ -206,15 +208,17 @@
             if not issubclass(RealEntryHookClass, self._entryHookClassType):
                 raise Exception(
                     "%s load error, Excpected %s, received %s"
                     % (pluginName, self._entryHookClassType, RealEntryHookClass)
                 )
 
             # Are we going to run this plugin in a subprocess?
-            if runInSubprocess:
+            if False:  # runInSubprocess:
+                pass
+                """
                 from peek_platform.subproc_plugin_init.plugin_subproc_parent_main import (
                     PluginSubprocParentMain,
                 )
 
                 # We can run multiple plugins in one group
                 # Have we already created this group?
                 if subprocessGroup in self._loadedSubprocessGroups:
@@ -227,14 +231,15 @@
                     self._loadedSubprocessGroups[
                         subprocessGroup
                     ] = subprocParentMain
 
                 # Return the subprocParentMain, it has a __call__ method
                 # to simulate the plugin class constructor
                 EntryHookClass = subprocParentMain
+                """
 
             else:
                 EntryHookClass = RealEntryHookClass
 
             ### Perform the loading of the plugin
             yield self._loadPluginThrows(
                 pluginName,
@@ -424,46 +429,53 @@
     # ---------------
     # Util methods Plugins
 
     @inlineCallbacks
     def _tryStart(self, pluginName):
         plugin = self._loadedPlugins[pluginName]
         try:
-            yield plugin.start()
+            d = plugin.start()
+            if d:
+                d.addErrback(vortexLogFailure, logger)
+                yield d
 
         except Exception as e:
             logger.error(
-                "An exception occured while starting plugin %s,"
+                "An exception occurred while starting plugin %s,"
                 " starting continues" % pluginName
             )
-            logger.exception(e)
 
     @inlineCallbacks
     def _tryStop(self, pluginName):
         plugin = self._loadedPlugins[pluginName]
         try:
-            yield plugin.stop()
+            d = plugin.stop()
+            if d:
+                d.addErrback(vortexLogFailure, logger)
+                yield d
 
         except Exception as e:
             logger.error(
-                "An exception occured while stopping plugin %s,"
+                "An exception occurred while stopping plugin %s,"
                 " stopping continues" % pluginName
             )
-            logger.exception(e)
 
     @inlineCallbacks
     def _unloadPluginPackage(self, pluginName):
 
         oldLoadedPlugin = self._loadedPlugins.get(pluginName)
 
         # Stop and remove the Plugin
         del self._loadedPlugins[pluginName]
 
         try:
-            yield oldLoadedPlugin.unload()
+            d = oldLoadedPlugin.unload()
+            if d:
+                d.addErrback(vortexLogFailure, logger)
+                yield d
 
         except Exception as e:
             logger.error(
                 "An exception occured while unloading plugin %s,"
                 " unloading continues" % pluginName
             )
             logger.exception(e)
```

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 logger = logging.getLogger(__name__)
 
 
 class PluginSubprocParentProtocol(protocol.ProcessProtocol):
     VORTEX_UUID_UPDATE_PERIOD = 30
 
     def __init__(self, subprocessGroupName):
-        self._data = b""
+        self._dataBytesArray = bytearray()
         self._logData = b""
         self._pluginStateData = b""
 
         self._vortexUpdateLoopingCall = task.LoopingCall(
             self._sendUpdatedVortexUuids
         )
 
@@ -126,23 +126,33 @@
                 elif severity == "ERROR":
                     self._loggerForChild.error(logMsg)
                 else:
                     self._loggerForChild.error(message)
 
     @inlineCallbacks
     def outReceived(self, data):
-        self._data += data
+        self._dataBytesArray.append(data)
 
-        while b"." in self._data:
-            message, self._data = self._data.split(b".", 1)
+        if b"." not in data:
+            return
+
+        # Avoid accidentally referencing this
+        del data
+
+        joinedData = bytes(self._dataBytesArray)
+
+        while b"." in joinedData:
+            message, joinedData = joinedData.split(b".", 1)
             if not message:
                 continue
 
             yield self._sendVortexMsgFromChild(message)
 
+        self._dataArray = bytearray(joinedData)
+
     @inlineCallbacks
     def _sendVortexMsgFromChild(self, message: bytes):
         vortexMsgTuple = yield self._decodeVortexMsgTuple(message)
 
         yield VortexFactory.sendVortexMsg(
             vortexMsgs=vortexMsgTuple.vortexMsgs,
             destVortexUuid=vortexMsgTuple.vortexUuid,
```

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py` & `peek-platform-3.4.0/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/sw_install/PeekSwInstallManagerABC.py` & `peek-platform-3.4.0/peek_platform/sw_install/PeekSwInstallManagerABC.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/sw_install/PluginSwInstallManagerABC.py` & `peek-platform-3.4.0/peek_platform/sw_install/PluginSwInstallManagerABC.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/sw_version/PeekSwVersionPollHandler.py` & `peek-platform-3.4.0/peek_platform/sw_version/PeekSwVersionPollHandler.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/util/LogUtil.py` & `peek-platform-3.4.0/peek_platform/util/LogUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,15 @@
             while data:
                 f.write(data)
                 data = sf.read(READ_CHUNK)
     os.remove(source)
 
 
 def updatePeekLoggerHandlers(
-    serviceName: Optional[str] = None,
-    daysToKeep=28,
-    logToStdout=True,
+    serviceName: Optional[str] = None, daysToKeep=28, logToStdout=True
 ):
     rootLogger = logging.getLogger()
     logFormatter = logging.Formatter(LOG_FORMAT, DATE_FORMAT)
 
     for handler in list(rootLogger.handlers):
         if isinstance(handler, TimedRotatingFileHandler):
             # Setup the file logging output
@@ -60,15 +58,17 @@
             logger.info(
                 "Logging to stdout disabled, see 'logToStdout' in config.json"
             )
             rootLogger.removeHandler(handler)
 
     fileName = str(Path.home() / ("%s.log" % serviceName))
 
-    fh = TimedRotatingFileHandler(fileName, when="midnight", backupCount=daysToKeep)
+    fh = TimedRotatingFileHandler(
+        fileName, when="midnight", backupCount=daysToKeep
+    )
     fh.setFormatter(logFormatter)
     fh.rotator = _rotator
     fh.namer = _namer
     rootLogger.addHandler(fh)
 
 
 def setupLoggingToSyslogServer(host: str, port: int, facility: str):
```

### Comparing `peek-platform-3.3.3/peek_platform/util/ManHoleUtil.py` & `peek-platform-3.4.0/peek_platform/util/ManHoleUtil.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/util/MemUtil.py` & `peek-platform-3.4.0/peek_platform/util/MemUtil.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/util/PtyUtil.py` & `peek-platform-3.4.0/peek_platform/util/PtyUtil.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform/winsvc_peek_restarter.py` & `peek-platform-3.4.0/peek_platform/winsvc_peek_restarter.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform.egg-info/SOURCES.txt` & `peek-platform-3.4.0/peek_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-platform-3.3.3/peek_platform.egg-info/requires.txt` & `peek-platform-3.4.0/peek_platform.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 alembic>=0.8.7
 python-dateutil>=2.6.0
 Pygments>=2.0.1
 watchdog>=0.8.3
 pycryptodome
 cryptography<38.0.0
 flower<1.0.0
-peek-plugin-base==3.3.*,>=3.3.3
-peek-core-device==3.3.*,>=3.3.3
-peek-core-email==3.3.*,>=3.3.3
+peek-plugin-base==3.4.*,>=3.4.0
+peek-core-device==3.4.*,>=3.4.0
+peek-core-email==3.4.*,>=3.4.0
 psutil
 pexpect<5.0,>=4.8.0
 Shapely>=1.5.16
 pymssql
 future
 celery[auth,redis]<5.0.0
 coverage>=4.2
```

### Comparing `peek-platform-3.3.3/setup.py` & `peek-platform-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_platform"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Platform."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
@@ -89,15 +89,15 @@
 
 win_dependencies = [
     # "pymssql >= 2.1.3",  # DB-API interface to Microsoft SQL Server, requires FreeTDS
     "pycparser >= 2.17",
     "cffi >= 1.9.1",
     "cryptography <= 3.1.1",  # PEEK-1136
     "pytest >= 3.0.5",
-    "wheel >= 0.33.3.3",
+    "wheel >= 0.33.4.0",
     "virtualenv >= 15.1.0",
     # Celery 4 is not supported on windows
     "celery[redis,auth]<4.0.0",
     # Service support for windows
     "pypiwin32",
 ]
```

