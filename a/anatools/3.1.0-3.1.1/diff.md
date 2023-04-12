# Comparing `tmp/anatools-3.1.0.tar.gz` & `tmp/anatools-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anatools-3.1.0.tar", last modified: Fri Apr  7 14:28:10 2023, max compression
+gzip compressed data, was "anatools-3.1.1.tar", last modified: Wed Apr 12 17:25:47 2023, max compression
```

## Comparing `anatools-3.1.0.tar` & `anatools-3.1.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.392023 anatools-3.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-07 14:27:54.000000 anatools-3.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-07 14:27:54.000000 anatools-3.1.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-04-07 14:28:10.392023 anatools-3.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6585 2023-04-07 14:27:54.000000 anatools-3.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.380023 anatools-3.1.0/anatools/
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-07 14:27:57.000000 anatools-3.1.0/anatools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.384024 anatools-3.1.0/anatools/anaclient/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11167 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/anaclient.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)    11005 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/annotations.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.384024 anatools-3.1.0/anatools/anaclient/api/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)     9403 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    10389 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     8002 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)    10116 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     4206 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     5334 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/limits.py
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/members.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/umap.py
--rw-rw-rw-   0 root         (0) root         (0)     8958 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/api/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)    18408 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     9145 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     9573 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     9386 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/umap.py
--rw-rw-rw-   0 root         (0) root         (0)    17861 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/anaclient/workspaces.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.388023 anatools-3.1.0/anatools/annotations/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/convert_coco.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/convert_kitti.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/convert_pascal.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/convert_sagemaker.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/convert_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/annotations/draw.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.388023 anatools-3.1.0/anatools/bin/
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/bin/ana
--rw-rw-rw-   0 root         (0) root         (0)     9659 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/bin/anadeploy
--rw-rw-rw-   0 root         (0) root         (0)     7692 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/bin/anamount
--rw-rw-rw-   0 root         (0) root         (0)     4524 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/bin/anautils
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.388023 anatools-3.1.0/anatools/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6974 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/ana_object.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/bbox.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/blender_main.py
--rw-rw-rw-   0 root         (0) root         (0)     4923 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/camera_checks.py
--rw-rw-rw-   0 root         (0) root         (0)    14524 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1777 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/context.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/download.py
--rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/file_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     9556 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5727 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/interp.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/load.py
--rw-rw-rw-   0 root         (0) root         (0)    10556 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/node.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/object_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/package_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/print.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/python_main.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/rigged_object.py
--rw-rw-rw-   0 root         (0) root         (0)     8111 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/scene.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/lib/search_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.392023 anatools-3.1.0/anatools/nodes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/constants.yml
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/generators.yml
--rw-rw-rw-   0 root         (0) root         (0)     1592 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/logic.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/logic.yml
--rw-rw-rw-   0 root         (0) root         (0)     5381 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/random_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     8429 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/random_generator.yml
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/sweep_arange.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/sweep_arange.yml
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/sweep_linspace.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/sweep_linspace.yml
--rw-rw-rw-   0 root         (0) root         (0)     1224 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/vectors.yml
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/volume_file.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-04-07 14:27:54.000000 anatools-3.1.0/anatools/nodes/volume_file.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.380023 anatools-3.1.0/anatools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6975 2023-04-07 14:28:10.000000 anatools-3.1.0/anatools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2555 2023-04-07 14:28:10.000000 anatools-3.1.0/anatools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-07 14:28:10.000000 anatools-3.1.0/anatools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-04-07 14:28:10.000000 anatools-3.1.0/anatools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-07 14:28:10.000000 anatools-3.1.0/anatools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-07 14:27:54.000000 anatools-3.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-07 14:27:54.000000 anatools-3.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-07 14:28:10.392023 anatools-3.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-04-07 14:27:54.000000 anatools-3.1.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 14:28:10.392023 anatools-3.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-04-07 14:27:54.000000 anatools-3.1.0/tests/test_bbox.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.742206 anatools-3.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-12 17:25:26.000000 anatools-3.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-12 17:25:26.000000 anatools-3.1.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6975 2023-04-12 17:25:47.742206 anatools-3.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6585 2023-04-12 17:25:26.000000 anatools-3.1.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.730206 anatools-3.1.1/anatools/
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-12 17:25:30.000000 anatools-3.1.1/anatools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.734206 anatools-3.1.1/anatools/anaclient/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11167 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/anaclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)    11005 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/annotations.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.734206 anatools-3.1.1/anatools/anaclient/api/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)     9403 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4454 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10389 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10116 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4206 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5334 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/limits.py
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/members.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)     8958 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/api/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    18408 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     9145 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9386 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)    17861 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/anaclient/workspaces.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.738206 anatools-3.1.1/anatools/annotations/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/convert_coco.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/convert_kitti.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/convert_pascal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/convert_sagemaker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/convert_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/annotations/draw.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.738206 anatools-3.1.1/anatools/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/bin/ana
+-rw-rw-rw-   0 root         (0) root         (0)     9659 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/bin/anadeploy
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/bin/anamount
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/bin/anautils
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.742206 anatools-3.1.1/anatools/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6974 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/ana_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/bbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/blender_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4923 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/camera_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14524 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/context.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/file_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     9556 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5727 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/interp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/load.py
+-rw-rw-rw-   0 root         (0) root         (0)    10556 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/object_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/package_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/print.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/python_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/rigged_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     8111 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/lib/search_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.742206 anatools-3.1.1/anatools/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/constants.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/generators.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/logic.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5381 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/random_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8429 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/random_generator.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/sweep_arange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/sweep_arange.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/sweep_linspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/sweep_linspace.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/vectors.yml
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/volume_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-04-12 17:25:26.000000 anatools-3.1.1/anatools/nodes/volume_file.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.730206 anatools-3.1.1/anatools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6975 2023-04-12 17:25:47.000000 anatools-3.1.1/anatools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2023-04-12 17:25:47.000000 anatools-3.1.1/anatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-12 17:25:47.000000 anatools-3.1.1/anatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-04-12 17:25:47.000000 anatools-3.1.1/anatools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-12 17:25:47.000000 anatools-3.1.1/anatools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-12 17:25:26.000000 anatools-3.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-12 17:25:26.000000 anatools-3.1.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-12 17:25:47.742206 anatools-3.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-04-12 17:25:26.000000 anatools-3.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 17:25:47.742206 anatools-3.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-04-12 17:25:26.000000 anatools-3.1.1/tests/test_bbox.py
```

### Comparing `anatools-3.1.0/LICENSE` & `anatools-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/PKG-INFO` & `anatools-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.1.0
+Version: 3.1.1
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.1.0/README.md` & `anatools-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/__init__.py` & `anatools-3.1.1/anatools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         https://support.rendered.ai/gc/Introduction-to-Rendered.ai.1577812005.html
 
 """
 
 from .anaclient.anaclient import client
 from .annotations.annotations import annotations
 
-__version__ = '3.1.0'
+__version__ = '3.1.1'
```

### Comparing `anatools-3.1.0/anatools/anaclient/anaclient.py` & `anatools-3.1.1/anatools/anaclient/anaclient.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/analytics.py` & `anatools-3.1.1/anatools/anaclient/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/annotations.py` & `anatools-3.1.1/anatools/anaclient/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/analytics.py` & `anatools-3.1.1/anatools/anaclient/api/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/annotations.py` & `anatools-3.1.1/anatools/anaclient/api/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/api.py` & `anatools-3.1.1/anatools/anaclient/api/api.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/channels.py` & `anatools-3.1.1/anatools/anaclient/api/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/datasets.py` & `anatools-3.1.1/anatools/anaclient/api/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/gan.py` & `anatools-3.1.1/anatools/anaclient/api/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/graphs.py` & `anatools-3.1.1/anatools/anaclient/api/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/handlers.py` & `anatools-3.1.1/anatools/anaclient/api/handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/limits.py` & `anatools-3.1.1/anatools/anaclient/api/limits.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/members.py` & `anatools-3.1.1/anatools/anaclient/api/members.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/organizations.py` & `anatools-3.1.1/anatools/anaclient/api/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/umap.py` & `anatools-3.1.1/anatools/anaclient/api/umap.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
         json = {
             "operationName": "getUMAP",
             "variables": {
                 "workspaceId": workspaceId,
                 "umapId": umapId
             },
             "query": """query 
-                getUMAP($workspaceId: String!, $umapId: String) {
+                getUMAP($workspaceId: String!, $umapId: String!) {
                     getUMAP(workspaceId: $workspaceId, umapId: $umapId){
                         datasets
                         samples
                         seed
                         status
                         results {
                             id
-                            featuresize
+                            featureSize
                             datasets {
                                 datasetId
                                 datasetName
                                 points {
                                     image
                                     x
                                     y
```

### Comparing `anatools-3.1.0/anatools/anaclient/api/volumes.py` & `anatools-3.1.1/anatools/anaclient/api/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/api/workspaces.py` & `anatools-3.1.1/anatools/anaclient/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/channels.py` & `anatools-3.1.1/anatools/anaclient/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/datasets.py` & `anatools-3.1.1/anatools/anaclient/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/gan.py` & `anatools-3.1.1/anatools/anaclient/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/graphs.py` & `anatools-3.1.1/anatools/anaclient/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/organizations.py` & `anatools-3.1.1/anatools/anaclient/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/umap.py` & `anatools-3.1.1/anatools/anaclient/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/volumes.py` & `anatools-3.1.1/anatools/anaclient/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/anaclient/workspaces.py` & `anatools-3.1.1/anatools/anaclient/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/annotations/annotations.py` & `anatools-3.1.1/anatools/annotations/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/annotations/convert_coco.py` & `anatools-3.1.1/anatools/annotations/convert_coco.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/annotations/convert_kitti.py` & `anatools-3.1.1/anatools/annotations/convert_kitti.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/annotations/convert_pascal.py` & `anatools-3.1.1/anatools/annotations/convert_pascal.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/annotations/convert_sagemaker.py` & `anatools-3.1.1/anatools/annotations/convert_sagemaker.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/annotations/convert_yolo.py` & `anatools-3.1.1/anatools/annotations/convert_yolo.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/annotations/draw.py` & `anatools-3.1.1/anatools/annotations/draw.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/bin/ana` & `anatools-3.1.1/anatools/bin/ana`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/bin/anadeploy` & `anatools-3.1.1/anatools/bin/anadeploy`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/bin/anamount` & `anatools-3.1.1/anatools/bin/anamount`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/bin/anautils` & `anatools-3.1.1/anatools/bin/anautils`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/ana_object.py` & `anatools-3.1.1/anatools/lib/ana_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/bbox.py` & `anatools-3.1.1/anatools/lib/bbox.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/blender_main.py` & `anatools-3.1.1/anatools/lib/blender_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/camera_checks.py` & `anatools-3.1.1/anatools/lib/camera_checks.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/channel.py` & `anatools-3.1.1/anatools/lib/channel.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/context.py` & `anatools-3.1.1/anatools/lib/context.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/file_handlers.py` & `anatools-3.1.1/anatools/lib/file_handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/generator.py` & `anatools-3.1.1/anatools/lib/generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/interp.py` & `anatools-3.1.1/anatools/lib/interp.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/load.py` & `anatools-3.1.1/anatools/lib/load.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/node.py` & `anatools-3.1.1/anatools/lib/node.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/object_utils.py` & `anatools-3.1.1/anatools/lib/object_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/package_utils.py` & `anatools-3.1.1/anatools/lib/package_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/python_main.py` & `anatools-3.1.1/anatools/lib/python_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/rigged_object.py` & `anatools-3.1.1/anatools/lib/rigged_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/scene.py` & `anatools-3.1.1/anatools/lib/scene.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/lib/search_utils.py` & `anatools-3.1.1/anatools/lib/search_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/constants.py` & `anatools-3.1.1/anatools/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/constants.yml` & `anatools-3.1.1/anatools/nodes/constants.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/generators.py` & `anatools-3.1.1/anatools/nodes/generators.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/generators.yml` & `anatools-3.1.1/anatools/nodes/generators.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/logic.py` & `anatools-3.1.1/anatools/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/logic.yml` & `anatools-3.1.1/anatools/nodes/logic.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/random_generator.py` & `anatools-3.1.1/anatools/nodes/random_generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/random_generator.yml` & `anatools-3.1.1/anatools/nodes/random_generator.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/sweep_arange.py` & `anatools-3.1.1/anatools/nodes/sweep_arange.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/sweep_arange.yml` & `anatools-3.1.1/anatools/nodes/sweep_arange.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/sweep_linspace.py` & `anatools-3.1.1/anatools/nodes/sweep_linspace.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/sweep_linspace.yml` & `anatools-3.1.1/anatools/nodes/sweep_linspace.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/vectors.py` & `anatools-3.1.1/anatools/nodes/vectors.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/vectors.yml` & `anatools-3.1.1/anatools/nodes/vectors.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/volume_file.py` & `anatools-3.1.1/anatools/nodes/volume_file.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools/nodes/volume_file.yml` & `anatools-3.1.1/anatools/nodes/volume_file.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/anatools.egg-info/PKG-INFO` & `anatools-3.1.1/anatools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.1.0
+Version: 3.1.1
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.1.0/anatools.egg-info/SOURCES.txt` & `anatools-3.1.1/anatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/setup.py` & `anatools-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `anatools-3.1.0/tests/test_bbox.py` & `anatools-3.1.1/tests/test_bbox.py`

 * *Files identical despite different names*

