# Comparing `tmp/talisman-interfaces-0.3.2.tar.gz` & `tmp/talisman-interfaces-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-interfaces-0.3.2.tar", last modified: Mon Mar 27 12:26:15 2023, max compression
+gzip compressed data, was "talisman-interfaces-0.4.0.tar", last modified: Wed Apr 12 08:26:31 2023, max compression
```

## Comparing `talisman-interfaces-0.3.2.tar` & `talisman-interfaces-0.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:15.002267 talisman-interfaces-0.3.2/
--rw-r--r--   0 root         (0) root         (0)      698 2023-03-27 12:26:15.002267 talisman-interfaces-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-03-27 11:09:35.000000 talisman-interfaces-0.3.2/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 12:26:15.002267 talisman-interfaces-0.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-03-27 11:09:35.000000 talisman-interfaces-0.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.946267 talisman-interfaces-0.3.2/talisman_interfaces.egg-info/
--rw-r--r--   0 root         (0) root         (0)      698 2023-03-27 12:26:14.000000 talisman-interfaces-0.3.2/talisman_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1913 2023-03-27 12:26:14.000000 talisman-interfaces-0.3.2/talisman_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 12:26:14.000000 talisman-interfaces-0.3.2/talisman_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-03-27 12:26:14.000000 talisman-interfaces-0.3.2/talisman_interfaces.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-27 12:26:14.000000 talisman-interfaces-0.3.2/talisman_interfaces.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.946267 talisman-interfaces-0.3.2/tp_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.966267 talisman-interfaces-0.3.2/tp_interfaces/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.974267 talisman-interfaces-0.3.2/tp_interfaces/abstract/configuration/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/configuration/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.978267 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/composite.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/constructable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.978267 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/merge/
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      733 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/merge/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-03-27 12:26:08.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/model/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.990267 talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2688 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/category.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2023-03-27 11:09:35.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-03-27 12:26:08.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.994267 talisman-interfaces-0.3.2/tp_interfaces/abstract/updatable/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/updatable/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1249 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/updatable/model.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/updatable/update.py
--rw-rw-rw-   0 root         (0) root         (0)     1296 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/abstract/updatable/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.994267 talisman-interfaces-0.3.2/tp_interfaces/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/helpers/batch.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/helpers/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/helpers/tar_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.998267 talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7608 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3482 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/kb_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     7744 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/readers.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/stub_kb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.998267 talisman-interfaces-0.3.2/tp_interfaces/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/logging/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.998267 talisman-interfaces-0.3.2/tp_interfaces/processors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/processors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4100 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/processors/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/processors/updatable_composite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.998267 talisman-interfaces-0.3.2/tp_interfaces/readers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-03-27 12:26:08.000000 talisman-interfaces-0.3.2/tp_interfaces/readers/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:14.998267 talisman-interfaces-0.3.2/tp_interfaces/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-03-22 12:10:58.000000 talisman-interfaces-0.3.2/tp_interfaces/serializers/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:15.002267 talisman-interfaces-0.3.2/tp_interfaces/trainer_cache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:09.000000 talisman-interfaces-0.3.2/tp_interfaces/trainer_cache/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-03-27 12:26:08.000000 talisman-interfaces-0.3.2/tp_interfaces/trainer_cache/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2554 2023-03-27 12:26:08.000000 talisman-interfaces-0.3.2/tp_interfaces/trainer_cache/manipulations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-04-11 11:40:07.000000 talisman-interfaces-0.4.0/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-04-11 11:40:07.000000 talisman-interfaces-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/configuration/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-04 13:33:04.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/constructable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2688 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/category.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-04-11 11:40:07.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/update.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/tar_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7608 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3482 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/kb_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7744 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/readers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/stub_kb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/logging/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/processors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/processors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4100 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/processors/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/processors/updatable_composite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/readers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/readers/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/tp_interfaces/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/serializers/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3970 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2554 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/manipulations.py
```

### Comparing `talisman-interfaces-0.3.2/PKG-INFO` & `talisman-interfaces-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-interfaces
-Version: 0.3.2
+Version: 0.4.0
 Summary: Talisman Processor base interfaces
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-interfaces-0.3.2/setup.py` & `talisman-interfaces-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type="text/markdown",
     author='ISPRAS Talisman NLP team',
     author_email='modis@ispras.ru',
     maintainer='Vladimir Mayorov',
     maintainer_email='vmayorov@ispras.ru',
     packages=find_packages(include=['tp_interfaces', 'tp_interfaces.*']),
     install_requires=[
-        'talisman-dm~=1.0.0a3', 'pydantic>=1.9.0', 'more-itertools>=8.12.0'
+        'talisman-dm~=0.7.1', 'pydantic>=1.9.0', 'more-itertools>=8.12.0'
     ],
     extras_require={
         'dvc': ['dvc[s3]>=2.8.1']
     },
     data_files=[('', ['VERSION'])],
     python_requires='>=3.6',
     license='Apache Software License',
```

### Comparing `talisman-interfaces-0.3.2/talisman_interfaces.egg-info/PKG-INFO` & `talisman-interfaces-0.4.0/talisman_interfaces.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-interfaces
-Version: 0.3.2
+Version: 0.4.0
 Summary: Talisman Processor base interfaces
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-interfaces-0.3.2/talisman_interfaces.egg-info/SOURCES.txt` & `talisman-interfaces-0.4.0/talisman_interfaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/__init__.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/model/merge/models.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/models.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/model/model.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/model/model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/model/wrapper.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/category.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/category.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/processor.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from abc import ABCMeta, abstractmethod
 from functools import partial
 from itertools import chain
 from typing import Generic, Iterator, Sequence, Tuple, Type, TypeVar
 
 from more_itertools import ichunked
 from tdm.abstract.datamodel import AbstractTreeDocumentContent
-from tdm.datamodel import TalismanDocument as LegacyDocument
-from tdm.future.abstract.datamodel import TalismanDocument
+from tdm.datamodel import TalismanDocument
 
 from tp_interfaces.abstract.model import AbstractModel
 from tp_interfaces.abstract.schema import ImmutableBaseModel
 from tp_interfaces.logging.context import with_log_extras
 
 _DocumentContent = TypeVar('_DocumentContent', bound=AbstractTreeDocumentContent)
 _Config = TypeVar('_Config', bound=ImmutableBaseModel)
 
-_Document = LegacyDocument[_DocumentContent] | TalismanDocument
-
 
 class AbstractDocumentProcessor(AbstractModel, Generic[_Config, _DocumentContent], metaclass=ABCMeta):
 
     @abstractmethod
-    def process_doc(self, document: _Document, config: _Config) -> _Document:
+    def process_doc(self, document: TalismanDocument[_DocumentContent], config: _Config) -> TalismanDocument[_DocumentContent]:
         pass
 
-    def process_docs(self, documents: Sequence[_Document], config: _Config) \
-            -> Tuple[_Document, ...]:
+    def process_docs(self, documents: Sequence[TalismanDocument[_DocumentContent]], config: _Config) \
+            -> Tuple[TalismanDocument[_DocumentContent], ...]:
         log_extras = with_log_extras(doc_id=lambda kwargs: kwargs['document'].doc_id)
         return tuple(map(partial(log_extras(self.process_doc), config=config), documents))
 
-    def process_stream(self, documents: Iterator[_Document], config: _Config, batch_size: int) \
-            -> Iterator[LegacyDocument[_DocumentContent]]:
+    def process_stream(self, documents: Iterator[TalismanDocument[_DocumentContent]], config: _Config, batch_size: int) \
+            -> Iterator[TalismanDocument[_DocumentContent]]:
         return chain.from_iterable(map(partial(self.process_docs, config=config), map(tuple, ichunked(documents, batch_size))))
 
     @property
     @abstractmethod
     def config_type(self) -> Type[_Config]:
         pass
```

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/processor/trainer.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/trainer.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/updatable/model.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/abstract/updatable/wrapper.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/wrapper.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/helpers/batch.py` & `talisman-interfaces-0.4.0/tp_interfaces/helpers/batch.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/helpers/io.py` & `talisman-interfaces-0.4.0/tp_interfaces/helpers/io.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/helpers/tar_model.py` & `talisman-interfaces-0.4.0/tp_interfaces/helpers/tar_model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/interfaces.py` & `talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/interfaces.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/kb_schema.py` & `talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/kb_schema.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/manager.py` & `talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/manager.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/readers.py` & `talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/readers.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/knowledge_base/stub_kb.py` & `talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/stub_kb.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/logging/context.py` & `talisman-interfaces-0.4.0/tp_interfaces/logging/context.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/processors/composite.py` & `talisman-interfaces-0.4.0/tp_interfaces/processors/composite.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/processors/updatable_composite.py` & `talisman-interfaces-0.4.0/tp_interfaces/processors/updatable_composite.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/readers/abstract.py` & `talisman-interfaces-0.4.0/tp_interfaces/readers/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/serializers/abstract.py` & `talisman-interfaces-0.4.0/tp_interfaces/serializers/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/trainer_cache/base.py` & `talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 @dataclass(frozen=True)
 class Cache(Picklable):
     trainer_config: dict
     git_revision: str = field(default=None, init=False)
     match_fields: Tuple[Tuple[str, Any], ...] = field(default=(('$', None),), init=False)  # pairs of (jsonpath pattern, default value)
     match_env: Tuple[Tuple[str, str], ...] = field(default=tuple(os.environ.items()), init=False)  # pairs of (var name, default var value)
-    path: Optional[Path] = field(init=False)
+    path: Optional[Path] = field(init=False, default=None)
     precomputed_hash: Optional[int] = field(init=False)
 
     def __post_init__(self):
         current_envs = []
         for env_name, default_env_value in self.match_env:
             current_envs.append((env_name, os.environ.get(env_name, default_env_value)))
```

### Comparing `talisman-interfaces-0.3.2/tp_interfaces/trainer_cache/manipulations.py` & `talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/manipulations.py`

 * *Files identical despite different names*

