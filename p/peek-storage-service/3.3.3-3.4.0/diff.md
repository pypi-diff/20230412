# Comparing `tmp/peek-storage-service-3.3.3.tar.gz` & `tmp/peek-storage-service-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-storage-service-3.3.3.tar", last modified: Mon Nov 14 05:36:44 2022, max compression
+gzip compressed data, was "peek-storage-service-3.4.0.tar", last modified: Wed Apr 12 11:05:29 2023, max compression
```

## Comparing `peek-storage-service-3.3.3.tar` & `peek-storage-service-3.4.0.tar`

### file list

```diff
@@ -1,63 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.128974 peek-storage-service-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      381 2022-11-14 05:36:44.128974 peek-storage-service-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      238 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.124974 peek-storage-service-3.3.3/peek_storage_service/
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-11-14 05:36:43.000000 peek-storage-service-3.3.3/peek_storage_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.125974 peek-storage-service-3.3.3/peek_storage_service/_private/
--rw-r--r--   0 root         (0) root         (0)     1987 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/StorageInit.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.126974 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)     2516 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      505 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.126974 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2145 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/12a0ab3826f3_add_run_generic_python.py
--rw-r--r--   0 root         (0) root         (0)      679 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py
--rw-r--r--   0 root         (0) root         (0)     2606 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/34490abd765c_add_pg_load_payload_tuples.py
--rw-r--r--   0 root         (0) root         (0)     3263 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/51e48a6594d5_up1_run_generic_py.py
--rw-r--r--   0 root         (0) root         (0)     4139 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/72518909970f_add_run_worker_plpy.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      473 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/bab14faf0cd7_add_timescale.py
--rw-r--r--   0 root         (0) root         (0)      189 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.127974 peek-storage-service-3.3.3/peek_storage_service/_private/plugin/
--rw-r--r--   0 root         (0) root         (0)     1791 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py
--rw-r--r--   0 root         (0) root         (0)     3826 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/plugin/StoragePluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1617 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.127974 peek-storage-service-3.3.3/peek_storage_service/_private/service/
--rw-r--r--   0 root         (0) root         (0)      988 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/PeekStorageConfig.py
--rw-r--r--   0 root         (0) root         (0)      675 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/StorageSiteResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.127974 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_download/
--rw-r--r--   0 root         (0) root         (0)     1616 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py
--rw-r--r--   0 root         (0) root         (0)     2350 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py
--rw-r--r--   0 root         (0) root         (0)      141 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_download/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.127974 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      790 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.128974 peek-storage-service-3.3.3/peek_storage_service/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      453 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     8581 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)      797 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.128974 peek-storage-service-3.3.3/peek_storage_service/_private/test/
--rw-r--r--   0 root         (0) root         (0)     1276 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/test/StorageTestMixin.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/_private/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.128974 peek-storage-service-3.3.3/peek_storage_service/plpython/
--rw-r--r--   0 root         (0) root         (0)     1678 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/plpython/LoadPayloadPgUtil.py
--rw-r--r--   0 root         (0) root         (0)     1952 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/plpython/RunPyInPg.py
--rw-r--r--   0 root         (0) root         (0)     1827 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/plpython/RunPyInPgTest.py
--rw-r--r--   0 root         (0) root         (0)     1353 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/plpython/RunWorkerTaskPyInPg.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/plpython/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6313 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/run_peek_storage_service.py
--rw-r--r--   0 root         (0) root         (0)     1460 2022-11-14 05:34:28.000000 peek-storage-service-3.3.3/peek_storage_service/winsvc_peek_storage_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:36:44.125974 peek-storage-service-3.3.3/peek_storage_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      381 2022-11-14 05:36:44.000000 peek-storage-service-3.3.3/peek_storage_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2627 2022-11-14 05:36:44.000000 peek-storage-service-3.3.3/peek_storage_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:44.000000 peek-storage-service-3.3.3/peek_storage_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      281 2022-11-14 05:36:44.000000 peek-storage-service-3.3.3/peek_storage_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:36:44.000000 peek-storage-service-3.3.3/peek_storage_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-14 05:36:44.000000 peek-storage-service-3.3.3/peek_storage_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-14 05:36:44.000000 peek-storage-service-3.3.3/peek_storage_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-14 05:36:44.129974 peek-storage-service-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3071 2022-11-14 05:36:43.000000 peek-storage-service-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.856205 peek-storage-service-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-12 11:05:29.856205 peek-storage-service-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.854205 peek-storage-service-3.4.0/peek_storage_service/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.854205 peek-storage-service-3.4.0/peek_storage_service/_private/
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/StorageInit.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.854205 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.855205 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/object_load_paylaod_tuples.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/object_run_generic_python.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/object_run_worker_task_python.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.855205 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/12a0ab3826f3_add_run_generic_python.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/34490abd765c_add_pg_load_payload_tuples.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/51e48a6594d5_up1_run_generic_py.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/72518909970f_add_run_worker_plpy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/bab14faf0cd7_add_timescale.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.855205 peek-storage-service-3.4.0/peek_storage_service/_private/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/plugin/StoragePluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.855205 peek-storage-service-3.4.0/peek_storage_service/_private/service/
+-rw-r--r--   0 root         (0) root         (0)      988 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/PeekStorageConfig.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/StorageSiteResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.856205 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_download/
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_download/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.856205 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      790 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_install/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.856205 peek-storage-service-3.4.0/peek_storage_service/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      453 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     8581 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)      810 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.856205 peek-storage-service-3.4.0/peek_storage_service/_private/test/
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/test/StorageTestMixin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/_private/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.856205 peek-storage-service-3.4.0/peek_storage_service/plpython/
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/plpython/LoadPayloadPgUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/plpython/RunPyInPg.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/plpython/RunPyInPgTest.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/plpython/RunWorkerTaskPyInPg.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/plpython/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6313 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/run_peek_storage_service.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-04-12 11:03:19.000000 peek-storage-service-3.4.0/peek_storage_service/winsvc_peek_storage_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:05:29.854205 peek-storage-service-3.4.0/peek_storage_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      281 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/peek_storage_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 11:05:29.857205 peek-storage-service-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-04-12 11:05:29.000000 peek-storage-service-3.4.0/setup.py
```

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/StorageInit.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/StorageInit.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,32 @@
     def __init__(self, dbConnection: DbConnection):
         self._dbConnection = dbConnection
 
     def runPreMigrate(self):
         self._upgradeTimescaleDbExtension()
 
     def runPostMigrate(self):
-        pass
+        from .alembic.objects import object_load_paylaod_tuples
+        from .alembic.objects import object_run_generic_python
+        from .alembic.objects import object_run_worker_task_python
+
+        session = self._dbConnection.ormSessionCreator()
+
+        objects = (
+            object_load_paylaod_tuples,
+            object_run_generic_python,
+            object_run_worker_task_python,
+        )
+
+        for obj in objects:
+            logger.debug("(Re)creating object %s", obj.__name__)
+            session.execute(obj.sql)
+
+        session.commit()
+        session.close()
 
     def _upgradeTimescaleDbExtension(self):
         rawConn = self._dbConnection.dbEngine.raw_connection()
         rawConn.set_isolation_level(ISOLATION_LEVEL_AUTOCOMMIT)
         cursor = rawConn.cursor()
         try:
```

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/alembic/env.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/alembic/env.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/12a0ab3826f3_add_run_generic_python.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/object_load_paylaod_tuples.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,91 @@
-"""add run_generic_python
-
-Revision ID: 12a0ab3826f3
-Revises: 34490abd765c
-Create Date: 2020-04-25 15:28:50.279318
-
-"""
-
-# revision identifiers, used by Alembic.
-revision = "12a0ab3826f3"
-down_revision = "34490abd765c"
-branch_labels = None
-depends_on = None
-
-from alembic import op
-
-
-def upgrade():
-    sql = """
-CREATE OR REPLACE FUNCTION peek_storage_service.run_generic_python(
-    args_json character varying,
-    kwargs_json character varying,
-    class_method_to_run_str_ character varying,
-    python_path character varying)
+sql = """
+CREATE OR REPLACE FUNCTION peek_storage_service.load_paylaod_tuples(
+	sql_qry_ character varying,
+	payload_filt_ character varying,
+	loader_module_class_method_ character varying,
+	python_path character varying,
+	fetch_size_ integer DEFAULT 50)
     RETURNS character varying
     LANGUAGE 'plpython3u'
 
     COST 100
     VOLATILE 
     
 AS $BODY$
 
 import json
 from base64 import b64decode
-args = json.loads(args_json)
-kwargs = json.loads(kwargs_json)
-classMethodToRunStr = class_method_to_run_str_
+sqlQry = sql_qry_
+payloadFilt = json.loads(payload_filt_)
+loaderModuleClassMethod = loader_module_class_method_
 pythonPath = json.loads(python_path)
+fetchSize = fetch_size_
 
 # ---------------
 # Setup to use the virtual environment
 import sys
 
 sys.path.extend(pythonPath)
 
 # ---------------
 # Dynamically load the tuple create method
 
 from importlib.util import find_spec, module_from_spec
 
-modName, className, methodName = classMethodToRunStr.rsplit('.',2)
+modName, className, methodName = loaderModuleClassMethod.rsplit('.',2)
 
 if modName in sys.modules:
-    package_ = sys.modules[modName]
+	tuple_package = sys.modules[modName]
 
 else:
-    modSpec = find_spec(modName)
-    if not modSpec:
-         raise Exception("Failed to find package %s,"
-                           " is the python package installed?" % modName)
-    package_ = modSpec.loader.load_module()
+	modSpec = find_spec(modName)
+	if not modSpec:
+		 raise Exception("Failed to find package %s,"
+						   " is the python package installed?" % modName)
+	tuple_package = modSpec.loader.load_module()
 
-Class_ = getattr(package_, className)
-classMethodToRun = getattr(Class_, methodName)
+TupleClass = getattr(tuple_package, className)
+tupleLoaderMethod = getattr(TupleClass, methodName)
 
-result = classMethodToRun(plpy, *args, **kwargs)
+# ---------------
+# Turn a row["val"] into a row.val
+class Wrap:
+    row = None
+    def __getattr__(self, name):
+        return self.row[name]
+
+wrap = Wrap()
+
+# ---------------
+# Iterate through and load the tuples
+results = []
+
+cursor = plpy.cursor(sqlQry)
+while True:
+    rows = cursor.fetch(max(500,fetchSize))
+    if not rows:
+        break
+    for row in rows:
+        wrap.row = row
+        results.append(tupleLoaderMethod(wrap))
+
+# ---------------
+# Convert it to a payload
+
+from vortex.Payload import Payload
+encodedPayload = Payload(filt=payloadFilt, tuples=results) \
+                        .toEncodedPayload() \
+                        if results else None
 
 return json.dumps({
-    'result': result
+    'count': len(results),
+    'encodedPayload': encodedPayload
 })
 
 $BODY$;
 
-ALTER FUNCTION peek_storage_service.run_generic_python(character varying, character varying, character varying, character varying)
+ALTER FUNCTION peek_storage_service.load_paylaod_tuples(character varying, character varying, character varying, character varying, integer)
     OWNER TO peek;
 
 
-          """
-    op.execute(sql)
-
-
-def downgrade():
-    sql = """DROP FUNCTION peek_storage_service.run_generic_python(character varying, 
-                                                            character varying, 
-                                                            character varying, 
-                                                            character varying);"""
-    op.execute(sql)
+"""
```

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/51e48a6594d5_up1_run_generic_py.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/object_run_generic_python.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,8 @@
-"""up1_run_generic_py
-
-Revision ID: 51e48a6594d5
-Revises: 72518909970f
-Create Date: 2020-06-02 22:27:48.650874
-
-"""
-
-# revision identifiers, used by Alembic.
-revision = "51e48a6594d5"
-down_revision = "72518909970f"
-branch_labels = None
-depends_on = None
-
-from alembic import op
-
-
-def upgrade():
-    sql = """
+sql = """
 
 DROP FUNCTION IF EXISTS
               peek_storage_service.run_generic_python(character varying,
                                               character varying,
                                               character varying,
                                               character varying);
 
@@ -112,13 +94,8 @@
 ALTER FUNCTION peek_storage_service.run_generic_python(character varying,
                                                character varying,
                                                character varying,
                                                character varying)
     OWNER TO peek;
 
 
-          """
-    op.execute(sql)
-
-
-def downgrade():
-    pass
+"""
```

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/alembic/versions/72518909970f_add_run_worker_plpy.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/alembic/objects/object_run_worker_task_python.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,8 @@
-"""add run worker plpy
-
-Revision ID: 72518909970f
-Revises: bab14faf0cd7
-Create Date: 2020-05-20 20:13:19.092876
-
-"""
-
-# revision identifiers, used by Alembic.
-
-revision = "72518909970f"
-down_revision = "bab14faf0cd7"
-branch_labels = None
-depends_on = None
-
-from alembic import op
-
-
-def upgrade():
-    sql = """
+sql = """
 CREATE OR REPLACE FUNCTION peek_storage_service.run_worker_task_python(
     sqla_url character varying,
     args_json character varying,
     class_method_to_run_str_ character varying,
     python_path character varying)
     RETURNS character varying
     LANGUAGE 'plpython3u'
@@ -147,17 +128,8 @@
 $BODY$;
 
 ALTER FUNCTION peek_storage_service.run_worker_task_python(character varying, character varying,
                                                    character varying, character varying)
     OWNER TO peek;
 
 
-          """
-    op.execute(sql)
-
-
-def downgrade():
-    sql = """DROP FUNCTION peek_storage_service.run_worker_task_python(character varying,
-                                                               character varying,
-                                                               character varying,
-                                                               character varying);"""
-    op.execute(sql)
+"""
```

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/plugin/StoragePluginLoader.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/plugin/StoragePluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/service/PeekStorageConfig.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/service/PeekStorageConfig.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/service/StorageSiteResource.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/service/StorageSiteResource.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/storage/Setting.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/storage/__init__.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/storage/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
 logger = logging.getLogger(__name__)
 
 dbConn = None
 
 
 def setupDbConn(
-    dbConnectString: str, metadata: MetaData, alembicDir: str, dbEngineArgs: Dict
+    dbConnectString: str,
+    metadata: MetaData,
+    alembicDir: str,
+    dbEngineArgs: Dict,
 ):
     global dbConn
     dbConn = DbConnection(
         dbConnectString=dbConnectString,
         metadata=metadata,
         alembicDir=alembicDir,
         dbEngineArgs=dbEngineArgs,
```

### Comparing `peek-storage-service-3.3.3/peek_storage_service/_private/test/StorageTestMixin.py` & `peek-storage-service-3.4.0/peek_storage_service/_private/test/StorageTestMixin.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/plpython/LoadPayloadPgUtil.py` & `peek-storage-service-3.4.0/peek_storage_service/plpython/LoadPayloadPgUtil.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,16 +46,12 @@
             payloadFileJson,
             loaderModuleClassMethodStr,
             __sysPathsJson,
             fetchSize,
         )
 
         resultJsonStr: str = next(session.execute(sqlFunc))[0]
-
         resultJson: Dict = json.loads(resultJsonStr)
-        if resultJson["encodedPayload"]:
-            resultJson["encodedPayload"] = resultJson["encodedPayload"].encode()
-
         return _LoadPayloadTupleResult(**resultJson)
 
     finally:
         session.close()
```

### Comparing `peek-storage-service-3.3.3/peek_storage_service/plpython/RunPyInPg.py` & `peek-storage-service-3.4.0/peek_storage_service/plpython/RunPyInPg.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/plpython/RunPyInPgTest.py` & `peek-storage-service-3.4.0/peek_storage_service/plpython/RunPyInPgTest.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/plpython/RunWorkerTaskPyInPg.py` & `peek-storage-service-3.4.0/peek_storage_service/plpython/RunWorkerTaskPyInPg.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/run_peek_storage_service.py` & `peek-storage-service-3.4.0/peek_storage_service/run_peek_storage_service.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service/winsvc_peek_storage_service.py` & `peek-storage-service-3.4.0/peek_storage_service/winsvc_peek_storage_service.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.3.3/peek_storage_service.egg-info/SOURCES.txt` & `peek-storage-service-3.4.0/peek_storage_service.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 peek_storage_service.egg-info/requires.txt
 peek_storage_service.egg-info/top_level.txt
 peek_storage_service/_private/StorageInit.py
 peek_storage_service/_private/__init__.py
 peek_storage_service/_private/alembic.ini
 peek_storage_service/_private/alembic/env.py
 peek_storage_service/_private/alembic/script.py.mako
+peek_storage_service/_private/alembic/objects/__init__.py
+peek_storage_service/_private/alembic/objects/object_load_paylaod_tuples.py
+peek_storage_service/_private/alembic/objects/object_run_generic_python.py
+peek_storage_service/_private/alembic/objects/object_run_worker_task_python.py
 peek_storage_service/_private/alembic/versions/12a0ab3826f3_add_run_generic_python.py
 peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py
 peek_storage_service/_private/alembic/versions/34490abd765c_add_pg_load_payload_tuples.py
 peek_storage_service/_private/alembic/versions/51e48a6594d5_up1_run_generic_py.py
 peek_storage_service/_private/alembic/versions/72518909970f_add_run_worker_plpy.py
 peek_storage_service/_private/alembic/versions/__init__.py
 peek_storage_service/_private/alembic/versions/bab14faf0cd7_add_timescale.py
```

### Comparing `peek-storage-service-3.3.3/setup.py` & `peek-storage-service-3.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_storage_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Storage Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

