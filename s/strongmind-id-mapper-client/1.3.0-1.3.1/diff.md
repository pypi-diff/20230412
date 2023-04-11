# Comparing `tmp/StrongMind-id-mapper-client-1.3.0.tar.gz` & `tmp/strongmind-id-mapper-client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StrongMind-id-mapper-client-1.3.0.tar", last modified: Mon Mar 20 20:09:34 2023, max compression
+gzip compressed data, was "strongmind-id-mapper-client-1.3.1.tar", last modified: Tue Apr 11 23:42:27 2023, max compression
```

## Comparing `StrongMind-id-mapper-client-1.3.0.tar` & `strongmind-id-mapper-client-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:09:34.512692 StrongMind-id-mapper-client-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-20 20:09:34.512692 StrongMind-id-mapper-client-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:09:34.512692 StrongMind-id-mapper-client-1.3.0/StrongMind_id_mapper_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-20 20:09:34.000000 StrongMind-id-mapper-client-1.3.0/StrongMind_id_mapper_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-20 20:09:34.000000 StrongMind-id-mapper-client-1.3.0/StrongMind_id_mapper_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 20:09:34.000000 StrongMind-id-mapper-client-1.3.0/StrongMind_id_mapper_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-20 20:09:34.000000 StrongMind-id-mapper-client-1.3.0/StrongMind_id_mapper_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:09:34.512692 StrongMind-id-mapper-client-1.3.0/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/mapper/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/mapper/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/mapper/partner.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 20:09:34.516692 StrongMind-id-mapper-client-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:09:34.512692 StrongMind-id-mapper-client-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/test/test_identifier_mapper_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/test/test_partner_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/test/test_post_pairs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-20 20:09:10.000000 StrongMind-id-mapper-client-1.3.0/test/test_uuid_link_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:42:27.547218 strongmind-id-mapper-client-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 23:42:27.547218 strongmind-id-mapper-client-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:42:27.543218 strongmind-id-mapper-client-1.3.1/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/mapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/mapper/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/mapper/partner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:42:27.547218 strongmind-id-mapper-client-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:42:27.547218 strongmind-id-mapper-client-1.3.1/strongmind_id_mapper_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 23:42:27.000000 strongmind-id-mapper-client-1.3.1/strongmind_id_mapper_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-11 23:42:27.000000 strongmind-id-mapper-client-1.3.1/strongmind_id_mapper_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:42:27.000000 strongmind-id-mapper-client-1.3.1/strongmind_id_mapper_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 23:42:27.000000 strongmind-id-mapper-client-1.3.1/strongmind_id_mapper_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:42:27.547218 strongmind-id-mapper-client-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/test/test_identifier_mapper_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/test/test_partner_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/test/test_post_pairs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-11 23:41:59.000000 strongmind-id-mapper-client-1.3.1/test/test_uuid_link_api.py
```

### Comparing `StrongMind-id-mapper-client-1.3.0/mapper/client.py` & `strongmind-id-mapper-client-1.3.1/mapper/client.py`

 * *Files identical despite different names*

### Comparing `StrongMind-id-mapper-client-1.3.0/mapper/errors.py` & `strongmind-id-mapper-client-1.3.1/mapper/errors.py`

 * *Files identical despite different names*

### Comparing `StrongMind-id-mapper-client-1.3.0/test/test_identifier_mapper_client.py` & `strongmind-id-mapper-client-1.3.1/test/test_identifier_mapper_client.py`

 * *Files identical despite different names*

### Comparing `StrongMind-id-mapper-client-1.3.0/test/test_partner_api.py` & `strongmind-id-mapper-client-1.3.1/test/test_partner_api.py`

 * *Files identical despite different names*

### Comparing `StrongMind-id-mapper-client-1.3.0/test/test_post_pairs_api.py` & `strongmind-id-mapper-client-1.3.1/test/test_post_pairs_api.py`

 * *Files identical despite different names*

### Comparing `StrongMind-id-mapper-client-1.3.0/test/test_uuid_link_api.py` & `strongmind-id-mapper-client-1.3.1/test/test_uuid_link_api.py`

 * *Files identical despite different names*

