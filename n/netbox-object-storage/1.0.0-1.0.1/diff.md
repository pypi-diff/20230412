# Comparing `tmp/netbox-object-storage-1.0.0.tar.gz` & `tmp/netbox-object-storage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-object-storage-1.0.0.tar", last modified: Tue Apr 11 15:35:30 2023, max compression
+gzip compressed data, was "netbox-object-storage-1.0.1.tar", last modified: Wed Apr 12 15:08:41 2023, max compression
```

## Comparing `netbox-object-storage-1.0.0.tar` & `netbox-object-storage-1.0.1.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.308000 netbox-object-storage-1.0.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-07 09:10:48.000000 netbox-object-storage-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-07 17:50:35.000000 netbox-object-storage-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-11 15:35:30.308000 netbox-object-storage-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1880 2023-04-08 03:02:21.000000 netbox-object-storage-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.298000 netbox-object-storage-1.0.0/netbox_object_storage/
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.300000 netbox-object-storage-1.0.0/netbox_object_storage/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/api/urls.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/api/views.py
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.301000 netbox-object-storage-1.0.0/netbox_object_storage/filtersets/
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/filtersets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1294 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/filtersets/bucket.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/filtersets/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/filtersets/pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.302000 netbox-object-storage-1.0.0/netbox_object_storage/forms/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/forms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/forms/assginment.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/forms/bucket.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/forms/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/forms/pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.303000 netbox-object-storage-1.0.0/netbox_object_storage/migrations/
--rw-r--r--   0 root         (0) root         (0)     5564 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/migrations/0002_remove_pool_contact_remove_s3cluster_contact_and_more.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.304000 netbox-object-storage-1.0.0/netbox_object_storage/models/
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/models/bucket.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/models/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/models/pool.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-11 15:27:52.000000 netbox-object-storage-1.0.0/netbox_object_storage/navigation.py
--rw-r--r--   0 root         (0) root         (0)     4446 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/tables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.296000 netbox-object-storage-1.0.0/netbox_object_storage/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.305000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/base.html
--rw-r--r--   0 root         (0) root         (0)      971 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/cluster_add_devices.html
--rw-r--r--   0 root         (0) root         (0)      970 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/cluster_add_virtualmachine.html
--rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/device.html
--rw-r--r--   0 root         (0) root         (0)      594 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/device_base.html
--rw-r--r--   0 root         (0) root         (0)      920 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/virtualmachine.html
--rw-r--r--   0 root         (0) root         (0)      611 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/virtualmachine_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.306000 netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/
--rw-r--r--   0 root         (0) root         (0)     1666 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/bucket.html
--rw-r--r--   0 root         (0) root         (0)     2254 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/bucket_edit.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.306000 netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/generic/
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/generic/bulk_remove.html
--rw-r--r--   0 root         (0) root         (0)     1380 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/pool.html
--rw-r--r--   0 root         (0) root         (0)     3249 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/s3cluster.html
--rw-r--r--   0 root         (0) root         (0)     2938 2023-04-11 15:27:50.000000 netbox-object-storage-1.0.0/netbox_object_storage/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.307000 netbox-object-storage-1.0.0/netbox_object_storage/views/
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/views/bucket.py
--rw-r--r--   0 root         (0) root         (0)     1348 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/views/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/views/cluster_device.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/views/cluster_vm.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-04-11 15:27:51.000000 netbox-object-storage-1.0.0/netbox_object_storage/views/pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 15:35:30.299000 netbox-object-storage-1.0.0/netbox_object_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-11 15:35:30.000000 netbox-object-storage-1.0.0/netbox_object_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2427 2023-04-11 15:35:30.000000 netbox-object-storage-1.0.0/netbox_object_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 15:35:30.000000 netbox-object-storage-1.0.0/netbox_object_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-11 15:35:30.000000 netbox-object-storage-1.0.0/netbox_object_storage.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 15:35:30.000000 netbox-object-storage-1.0.0/netbox_object_storage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 15:35:30.000000 netbox-object-storage-1.0.0/netbox_object_storage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 15:35:30.308000 netbox-object-storage-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-07 17:50:52.000000 netbox-object-storage-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.324586 netbox-object-storage-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-12 15:08:41.324586 netbox-object-storage-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.312586 netbox-object-storage-1.0.1/netbox_object_storage/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-12 15:08:35.000000 netbox-object-storage-1.0.1/netbox_object_storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.316586 netbox-object-storage-1.0.1/netbox_object_storage/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-04-12 14:12:12.000000 netbox-object-storage-1.0.1/netbox_object_storage/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/api/views.py
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-11 14:20:45.000000 netbox-object-storage-1.0.1/netbox_object_storage/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.316586 netbox-object-storage-1.0.1/netbox_object_storage/filtersets/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/filtersets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-12 14:14:00.000000 netbox-object-storage-1.0.1/netbox_object_storage/filtersets/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-11 14:39:58.000000 netbox-object-storage-1.0.1/netbox_object_storage/filtersets/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-04-11 14:51:29.000000 netbox-object-storage-1.0.1/netbox_object_storage/filtersets/pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.316586 netbox-object-storage-1.0.1/netbox_object_storage/forms/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/forms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-04-12 14:20:28.000000 netbox-object-storage-1.0.1/netbox_object_storage/forms/assginment.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-04-12 14:02:03.000000 netbox-object-storage-1.0.1/netbox_object_storage/forms/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-04-12 15:05:00.000000 netbox-object-storage-1.0.1/netbox_object_storage/forms/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-04-11 14:48:51.000000 netbox-object-storage-1.0.1/netbox_object_storage/forms/pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.320586 netbox-object-storage-1.0.1/netbox_object_storage/migrations/
+-rw-r--r--   0 root         (0) root         (0)     5564 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/migrations/0002_remove_pool_contact_remove_s3cluster_contact_and_more.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-04-12 14:42:03.000000 netbox-object-storage-1.0.1/netbox_object_storage/migrations/0003_remove_s3cluster_s3device_count_and_more.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.320586 netbox-object-storage-1.0.1/netbox_object_storage/models/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-04-12 14:54:53.000000 netbox-object-storage-1.0.1/netbox_object_storage/models/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-04-12 15:03:25.000000 netbox-object-storage-1.0.1/netbox_object_storage/models/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-04-10 09:18:31.000000 netbox-object-storage-1.0.1/netbox_object_storage/models/pool.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-10 05:42:47.000000 netbox-object-storage-1.0.1/netbox_object_storage/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     4674 2023-04-12 13:59:01.000000 netbox-object-storage-1.0.1/netbox_object_storage/tables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.312586 netbox-object-storage-1.0.1/netbox_object_storage/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.320586 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-04-11 15:07:41.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/base.html
+-rw-r--r--   0 root         (0) root         (0)      971 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/cluster_add_devices.html
+-rw-r--r--   0 root         (0) root         (0)      970 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/cluster_add_virtualmachine.html
+-rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 15:08:18.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/device.html
+-rw-r--r--   0 root         (0) root         (0)      594 2023-04-10 09:13:21.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/device_base.html
+-rw-r--r--   0 root         (0) root         (0)      920 2023-04-11 15:08:26.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/virtualmachine.html
+-rw-r--r--   0 root         (0) root         (0)      611 2023-04-10 09:12:16.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/virtualmachine_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.324586 netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-04-12 14:06:40.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/bucket.html
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-04-12 14:03:54.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/bucket_edit.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.324586 netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/generic/
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/generic/bulk_remove.html
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-04-11 14:28:18.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/pool.html
+-rw-r--r--   0 root         (0) root         (0)     3249 2023-04-11 15:10:55.000000 netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/s3cluster.html
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-04-10 09:10:22.000000 netbox-object-storage-1.0.1/netbox_object_storage/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.324586 netbox-object-storage-1.0.1/netbox_object_storage/views/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-10 05:33:19.000000 netbox-object-storage-1.0.1/netbox_object_storage/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-04-10 09:17:57.000000 netbox-object-storage-1.0.1/netbox_object_storage/views/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-04-11 12:35:04.000000 netbox-object-storage-1.0.1/netbox_object_storage/views/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-04-10 09:17:48.000000 netbox-object-storage-1.0.1/netbox_object_storage/views/cluster_device.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-04-10 09:17:40.000000 netbox-object-storage-1.0.1/netbox_object_storage/views/cluster_vm.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-10 05:37:13.000000 netbox-object-storage-1.0.1/netbox_object_storage/views/pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:08:41.316586 netbox-object-storage-1.0.1/netbox_object_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-12 15:08:41.000000 netbox-object-storage-1.0.1/netbox_object_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-04-12 15:08:41.000000 netbox-object-storage-1.0.1/netbox_object_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 15:08:41.000000 netbox-object-storage-1.0.1/netbox_object_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-12 15:08:41.000000 netbox-object-storage-1.0.1/netbox_object_storage.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 05:33:58.000000 netbox-object-storage-1.0.1/netbox_object_storage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-12 15:08:41.000000 netbox-object-storage-1.0.1/netbox_object_storage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 15:08:41.324586 netbox-object-storage-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      470 2023-04-12 15:08:16.000000 netbox-object-storage-1.0.1/setup.py
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/api/serializers.py` & `netbox-object-storage-1.0.1/netbox_object_storage/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,17 @@
     )
     assigned_object = serializers.SerializerMethodField(read_only=True)
 
     class Meta:
         model = Bucket
         fields = fields = (
             'id', 'url', 'display', 'name', 'capacity', 'credential', 'contact',
-            'url', 'access','assigned_object_type', 'assigned_object_id', 'assigned_object', 
-            'description', 'comments', 'tags', 'custom_fields', 'created', 'last_updated'
+            'issue_date', 'expiration_date', 'url', 'access','assigned_object_type', 
+            'assigned_object_id', 'assigned_object', 'description', 'comments', 'tags', 
+            'custom_fields', 'created', 'last_updated'
         )
 
     @swagger_serializer_method(serializer_or_field=serializers.JSONField)
     def get_assigned_object(self, instance):
         if instance.assigned_object is None:
             raise ValidationError('Assigned Storage is None')
         serializer = get_serializer_for_model(instance.assigned_object, prefix=NESTED_SERIALIZER_PREFIX)
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/api/views.py` & `netbox-object-storage-1.0.1/netbox_object_storage/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/filtersets/bucket.py` & `netbox-object-storage-1.0.1/netbox_object_storage/filtersets/bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             'capacity', 
             'contact', 
             'credential', 
             'url',
             'access',
             'assigned_object_type_id'
         )
-        
+
     def search(self, queryset, name, value):
         query = Q(
             Q(name__icontains=value) |
             Q(contact__name__icontains=value) |
             Q(capacity__icontains=value) |
             Q(credential__icontains=value) |
             Q(access__icontains=value) |
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/filtersets/cluster.py` & `netbox-object-storage-1.0.1/netbox_object_storage/filtersets/cluster.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/filtersets/pool.py` & `netbox-object-storage-1.0.1/netbox_object_storage/filtersets/pool.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/forms/assginment.py` & `netbox-object-storage-1.0.1/netbox_object_storage/forms/assginment.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
 
 # VM ADD
 class ClusterAddVMsForm(BootstrapMixin, forms.Form):
     virtualmachine = DynamicModelMultipleChoiceField(
         queryset=VirtualMachine.objects.all(),
     )
+    
     class Meta:
         fields = [
             'cluster', 'virtualmachine'
         ]
 
     def __init__(self, *args, **kwargs):
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/forms/bucket.py` & `netbox-object-storage-1.0.1/netbox_object_storage/forms/bucket.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         queryset=Tag.objects.all(),
         required=False
     )
 
     class Meta:
         model = Bucket
         fields = (
-            'name', 'capacity', 'credential', 'url', 
+            'name', 'capacity', 'credential', 'url',
+            'contact', 'issue_date', 'expiration_date',
             'access', 'description', 'comments', 'tags'
             )
     def __init__(self, *args, **kwargs):
         instance = kwargs.get('instance')
         initial = kwargs.get('initial', {}).copy()
 
         if instance:
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/forms/cluster.py` & `netbox-object-storage-1.0.1/netbox_object_storage/forms/cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     contact = DynamicModelChoiceField(
         queryset=Contact.objects.all(),
         required=False
     )
 
     raw_size = forms.IntegerField(
         required=False,
-        label='Raw Size',
+        label='Raw Size (GB)',
     )
 
     used_size = forms.IntegerField(
         required=False,
-        label='Used Size',
+        label='Used Size (GB)',
     )
 
     comments = CommentField()
 
     tags = DynamicModelMultipleChoiceField(
         queryset=Tag.objects.all(),
         required=False
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/forms/pool.py` & `netbox-object-storage-1.0.1/netbox_object_storage/forms/pool.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/migrations/0001_initial.py` & `netbox-object-storage-1.0.1/netbox_object_storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/migrations/0002_remove_pool_contact_remove_s3cluster_contact_and_more.py` & `netbox-object-storage-1.0.1/netbox_object_storage/migrations/0002_remove_pool_contact_remove_s3cluster_contact_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/models/bucket.py` & `netbox-object-storage-1.0.1/netbox_object_storage/models/bucket.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,15 +74,27 @@
         default=None
     )
 
     assigned_object = GenericForeignKey(
         ct_field='assigned_object_type',
         fk_field='assigned_object_id'
     )
-
+    
+    issue_date = models.DateField(
+        help_text='The date on which this bucket was issued',
+        blank=True,
+        default=None,
+        null=True,
+    )
+    expiration_date = models.DateField(
+        help_text='The date on which this bucket expires',
+        blank=True,
+        default=None,
+        null=True,
+    )
     description = models.CharField(
         max_length=500,
         blank=True
     )
 
     comments = models.TextField(
         blank=True
@@ -94,17 +106,20 @@
 
     class Meta:
         ordering = ('name',)
         verbose_name = 'Bucket'
 
     def __str__(self):
         if self.pk is not None:
-            return f'{self.assigned_object} <> {self.name}'
+            return f'{self.name}'
         return super().__str__()
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_object_storage:bucket', args=[self.pk])
 
     def clean(self):
         # Check if name is existed, raise Validation Error
         if Bucket.objects.filter(name=self.name).exclude(pk=self.pk).exists():
-            raise ValidationError('A bucket with this name already exists.')
+            raise ValidationError('A bucket with this name already exists.')
+        if self.expiration_date and self.issue_date:
+            if self.expiration_date <= self.issue_date:
+                raise ValidationError('Expiration date must be after issue date.')
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/models/cluster.py` & `netbox-object-storage-1.0.1/netbox_object_storage/models/cluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,28 +45,14 @@
         on_delete=models.SET_NULL, 
         null=True,
         blank=True,
         default=None,
         related_name='s3cluster_contact',
     )
 
-    s3device_count = models.IntegerField(
-        null=True, 
-        blank=True, 
-        default=None,
-        verbose_name = 'Device Count'
-    )
-
-    s3vm_count = models.IntegerField(
-        null=True, 
-        blank=True,
-        default=None,
-        verbose_name = 'VM Count'
-    )
-
     raw_size = models.IntegerField(
         null=True, 
         blank=True, 
         default=None,
         verbose_name = 'Raw Size'
     )
 
@@ -94,8 +80,11 @@
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_object_storage:s3cluster', args=[self.pk])
 
     def clean(self):
         # Check if name is existed, raise Validation Error
         if S3Cluster.objects.filter(name=self.name).exclude(pk=self.pk).exists():
-            raise ValidationError('A cluster with this name already exists.')
+            raise ValidationError('A cluster with this name already exists.')
+        if self.raw_size and self.used_size:
+            if self.raw_size <= self.used_size:
+                raise ValidationError('Used size must less than Raw Size')
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/models/pool.py` & `netbox-object-storage-1.0.1/netbox_object_storage/models/pool.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/navigation.py` & `netbox-object-storage-1.0.1/netbox_object_storage/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/tables.py` & `netbox-object-storage-1.0.1/netbox_object_storage/tables.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
     credential = tables.Column()
 
     url = tables.Column()
 
     access = ChoiceFieldColumn()
 
+    issue_date = tables.Column()
+    expiration_date = tables.Column()
+
     description = tables.Column()
 
     assigned_object_type = columns.ContentTypeColumn(
         verbose_name='Storage Backend Type'
     )
     assigned_object = tables.Column(
         linkify=True,
@@ -50,14 +53,16 @@
                   "id", 
                   "name",
                   "access",
                   "contact",
                   "capacity",
                   "url",
                   "credential",
+                  "issue_date",
+                  "expiration_date",
                   "description", 
                   "comments",
                   "tags", 
                   "assigned_object_type",
                   "assigned_object",
                   "created",
                   "last_updated",
@@ -65,14 +70,16 @@
                 )
         default_columns = ("name",
                            "access",
                            "contact",
                            "capacity",
                            "url",
                            "credential",
+                           "issue_date",
+                           "expiration_date",
                            "assigned_object_type",
                            "assigned_object",
                            'actions',
                         )
 
 class PoolTable(NetBoxTable):
     name = tables.Column(
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/base.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/base.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/cluster_add_devices.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/cluster_add_devices.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/cluster_add_virtualmachine.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/cluster_add_virtualmachine.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/device.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/device.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/device_base.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/device_base.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/virtualmachine.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/virtualmachine.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/cluster_assignment/virtualmachine_base.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/cluster_assignment/virtualmachine_base.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/bucket.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/pool.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 {% extends 'generic/object.html' %}
 {% load render_table from django_tables2 %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">Bucket</h5>
+        <h5 class="card-header">Pool</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
               <th scope="row">Name</th>
               <td>{{ object.name|linkify|placeholder }}</td>
             </tr>
             <tr>
-              <th scope="row">Capacity</th>
-              <td>{{ object.capacity }}</td>
+              <th scope="row">Type</th>
+              <td>{{ object.type }}</td>
             </tr>
             <tr>
               <th scope="row">Contact</th>
               <td>{{ object.contact|linkify|placeholder }}</td>
             </tr>
             <tr>
-              <th scope="row">Credential</th>
-              <td>{{ object.credential }}</td>
+              <th scope="row">Size</th>
+              <td>{{ object.size }}</td>
             </tr>
             <tr>
-                <th scope="row">Url</th>
-                <td>{{ object.url }}</td>
+              <th scope="row">S3Cluster</th>
+              <td>{{ object.cluster|linkify|placeholder }}</td>
             </tr>
             <tr>
-                <th scope="row">Access</th>
-                <td>{{ object.access }}</td>
-            </tr>
-            <tr>
-                <th scope="row">Storage Backend</th>
-                <td>{{ object.assigned_object|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-                <th scope="row">Description</th>
-                <td>{{ object.description|placeholder }}</td>
+              <th scope="row">Description</th>
+              <td>{{ object.description|placeholder }}</td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
```

#### html2text {}

```diff
@@ -1,14 +1,12 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
 {% block content %}
-** Bucket **
-Name            {{ object.name|linkify|placeholder }}
-Capacity        {{ object.capacity }}
-Contact         {{ object.contact|linkify|placeholder }}
-Credential      {{ object.credential }}
-Url             {{ object.url }}
-Access          {{ object.access }}
-Storage Backend {{ object.assigned_object|linkify|placeholder }}
-Description     {{ object.description|placeholder }}
+** Pool **
+Name        {{ object.name|linkify|placeholder }}
+Type        {{ object.type }}
+Contact     {{ object.contact|linkify|placeholder }}
+Size        {{ object.size }}
+S3Cluster   {{ object.cluster|linkify|placeholder }}
+Description {{ object.description|placeholder }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/bucket_edit.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/bucket_edit.html`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     </div>
     {% render_field form.name %}
     {% render_field form.capacity %}
     {% render_field form.contact %}
     {% render_field form.credential %}
     {% render_field form.url %}
     {% render_field form.access %}
+    {% render_field form.issue_date %}
+    {% render_field form.expiration_date %}
     {% render_field form.description %}
     {% render_field form.tags %}
   </div>
   <div class="field-group my-5">
     <div class="row mb-2">
       <h5 class="offset-sm-3">Bucket Storage Backend</h5>
     </div>
```

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/generic/bulk_remove.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/generic/bulk_remove.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/templates/netbox_object_storage/s3cluster.html` & `netbox-object-storage-1.0.1/netbox_object_storage/templates/netbox_object_storage/s3cluster.html`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/urls.py` & `netbox-object-storage-1.0.1/netbox_object_storage/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/views/bucket.py` & `netbox-object-storage-1.0.1/netbox_object_storage/views/bucket.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/views/cluster.py` & `netbox-object-storage-1.0.1/netbox_object_storage/views/cluster.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/views/cluster_device.py` & `netbox-object-storage-1.0.1/netbox_object_storage/views/cluster_device.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/views/cluster_vm.py` & `netbox-object-storage-1.0.1/netbox_object_storage/views/cluster_vm.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage/views/pool.py` & `netbox-object-storage-1.0.1/netbox_object_storage/views/pool.py`

 * *Files identical despite different names*

### Comparing `netbox-object-storage-1.0.0/netbox_object_storage.egg-info/SOURCES.txt` & `netbox-object-storage-1.0.1/netbox_object_storage.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-LICENSE
 MANIFEST.in
-README.md
 setup.py
 netbox_object_storage/__init__.py
 netbox_object_storage/constants.py
 netbox_object_storage/navigation.py
 netbox_object_storage/tables.py
 netbox_object_storage/urls.py
 netbox_object_storage.egg-info/PKG-INFO
@@ -24,14 +22,15 @@
 netbox_object_storage/forms/__init__.py
 netbox_object_storage/forms/assginment.py
 netbox_object_storage/forms/bucket.py
 netbox_object_storage/forms/cluster.py
 netbox_object_storage/forms/pool.py
 netbox_object_storage/migrations/0001_initial.py
 netbox_object_storage/migrations/0002_remove_pool_contact_remove_s3cluster_contact_and_more.py
+netbox_object_storage/migrations/0003_remove_s3cluster_s3device_count_and_more.py
 netbox_object_storage/migrations/__init__.py
 netbox_object_storage/models/__init__.py
 netbox_object_storage/models/bucket.py
 netbox_object_storage/models/cluster.py
 netbox_object_storage/models/pool.py
 netbox_object_storage/templates/cluster_assignment/base.html
 netbox_object_storage/templates/cluster_assignment/cluster_add_devices.html
```

