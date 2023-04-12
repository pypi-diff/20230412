# Comparing `tmp/pyicat-plus-0.1.2.tar.gz` & `tmp/pyicat-plus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyicat-plus-0.1.2.tar", last modified: Wed Jan  4 10:42:29 2023, max compression
+gzip compressed data, was "dist/pyicat-plus-0.1.3.tar", last modified: Wed Apr 12 09:40:33 2023, max compression
```

## Comparing `pyicat-plus-0.1.2.tar` & `pyicat-plus-0.1.3.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     7560 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1648 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/apps/store_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/apps/store_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2639 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/apps/store_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/archive.py
--rw-rw-rw-   0 root         (0) root         (0)     7613 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     3110 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/interface.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/investigation.py
--rw-rw-rw-   0 root         (0) root         (0)    12903 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3597 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2280 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/null.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/client/xmlns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/concurrency/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/concurrency/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/concurrency/query_pool/
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/concurrency/query_pool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/concurrency/query_pool/gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/concurrency/query_pool/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10040 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/metadata/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)   107517 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/metadata/hdf5_cfg.xml
--rw-rw-rw-   0 root         (0) root         (0)     1775 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/metadata/namespace_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/metadata/nexus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9106 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/icat.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/proc.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/activemq_rest_server.py
--rw-rw-rw-   0 root         (0) root         (0)     8429 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/icatplus_server.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/stomp_publisher.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/stomp_subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_mockup.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)     4610 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_query_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/test_url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/tests/utils/compare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-04 10:42:24.000000 pyicat-plus-0.1.2/src/pyicat_plus/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/utils/maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-01-04 10:40:14.000000 pyicat-plus-0.1.2/src/pyicat_plus/utils/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1648 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2419 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      307 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-04 10:42:29.000000 pyicat-plus-0.1.2/src/pyicat_plus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/apps/store_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/apps/store_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/apps/store_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     7677 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     3110 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     6121 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/investigation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12840 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/null.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/client/xmlns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/concurrency/
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/concurrency/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/concurrency/query_pool/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/concurrency/query_pool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/concurrency/query_pool/gevent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3565 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/concurrency/query_pool/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10117 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/metadata/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)   108391 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/metadata/hdf5_cfg.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/metadata/namespace_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/metadata/nexus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9106 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/icat.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/proc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/activemq_rest_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8429 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/icatplus_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/stomp_publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/stomp_subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_mockup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4610 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_query_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/test_url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/tests/utils/compare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 09:40:27.000000 pyicat-plus-0.1.3/src/pyicat_plus/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/utils/maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-04-12 09:38:19.000000 pyicat-plus-0.1.3/src/pyicat_plus/utils/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 09:40:33.000000 pyicat-plus-0.1.3/src/pyicat_plus.egg-info/top_level.txt
```

### Comparing `pyicat-plus-0.1.2/LICENSE.md` & `pyicat-plus-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/PKG-INFO` & `pyicat-plus-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat-plus-0.1.2/README.md` & `pyicat-plus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/setup.cfg` & `pyicat-plus-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/apps/store_from_file.py` & `pyicat-plus-0.1.3/src/pyicat_plus/apps/store_from_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import sys
 import argparse
 from glob import glob
 from ..client.main import IcatClient
+from ..client import defaults
 
 
 def main(argv=None):
     if argv is None:
         argv = sys.argv
 
     parser = argparse.ArgumentParser(description="Register stored data with ICAT")
@@ -24,21 +25,21 @@
 def add_store_parameters(parser):
     parser.add_argument("filter", help="File search filter")
 
     parser.add_argument(
         "--queue",
         dest="metadata_urls",
         action="append",
-        help="ActiveMQ queue URLS. Example: bcu-mq-01.esrf.fr:61613",
+        help="ActiveMQ queue URLS",
         default=[],
     )
 
 
 def apply_store_parameters(args):
     args.files = sorted(glob(args.filter), key=os.path.getmtime)
 
     if not args.metadata_urls:
-        args.metadata_urls = ["bcu-mq-01.esrf.fr:61613", "bcu-mq-02.esrf.fr:61613"]
+        args.metadata_urls = defaults.METADATA_BROKERS
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/apps/store_processed.py` & `pyicat-plus-0.1.3/src/pyicat_plus/apps/store_processed.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/apps/store_raw.py` & `pyicat-plus-0.1.3/src/pyicat_plus/apps/store_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import json
 import argparse
 from configparser import RawConfigParser
 from typing import Any, Tuple
 from ..client.main import IcatClient
+from ..client import defaults
 
 
 def main(argv=None):
     if argv is None:
         argv = sys.argv
 
     parser = argparse.ArgumentParser(description="Register processed data with ICAT")
@@ -22,15 +23,14 @@
         dataset=args.dataset,
         path=args.path,
         metadata=args.metadata,
     )
 
 
 def add_store_parameters(parser):
-
     parser.add_argument("--beamline", required=True, help="Beamline name")
 
     parser.add_argument("--proposal", required=True, help="Proposal name")
 
     parser.add_argument("--dataset", required=True, help="Dataset name")
 
     parser.add_argument("--sample", required=True, help="Sample name")
@@ -54,15 +54,15 @@
         help="ICAT metadata names and values (overwrite metadata from file)",
     )
 
     parser.add_argument(
         "--queue",
         dest="metadata_urls",
         action="append",
-        help="ActiveMQ queue URLS. Example: bcu-mq-01.esrf.fr:61613",
+        help="ActiveMQ queue URLS",
         default=[],
     )
 
 
 def apply_store_parameters(args):
     if args.metadatafile:
         parameters = _parameters_from_file()
@@ -71,15 +71,15 @@
     if args.parameters:
         parameters.update(_parse_parameter(s) for s in args.parameters)
     if args.sample:
         parameters["Sample_name"] = args.sample
     args.metadata = parameters
 
     if not args.metadata_urls:
-        args.metadata_urls = ["bcu-mq-01.esrf.fr:61613", "bcu-mq-02.esrf.fr:61613"]
+        args.metadata_urls = defaults.METADATA_BROKERS
 
 
 def _parse_parameter(parameter: str) -> Tuple[str, str]:
     name, _, value = parameter.partition("=")
     return name, _parse_value(value)
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/elogbook.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/elogbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import socket
 from urllib.parse import urljoin
 from typing import Optional, Iterable, List
 import logging
 
 from ..utils.url import normalize_url
 from .. import __version__
+from . import defaults
 
 logger = logging.getLogger(__name__)
 
 MessageCategory = Enum("MessageCategory", "debug info error commandLine comment")
 MessageType = Enum("MessageType", "annotation notification")
 
 MessageCategoryMapping = {
@@ -48,18 +49,20 @@
     """
 
     DEFAULT_SCHEME = "https"
 
     def __init__(
         self,
         url: str,
-        api_key: str = "elogbook-00000000-0000-0000-0000-000000000000",
+        api_key: Optional[str] = None,
         timeout: Optional[float] = None,
         **payload,
     ):
+        if api_key is None:
+            api_key = defaults.ELOGBOOK_TOKEN
         url = normalize_url(url, default_scheme=self.DEFAULT_SCHEME)
 
         path = f"dataacquisition/{api_key}/notification"
         self._message_url = urljoin(url, path)
 
         path = f"dataacquisition/{api_key}/base64"
         self._data_url = urljoin(url, path)
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/interface.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/interface.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/investigation.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/investigation.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy
 import logging
 
 from ..concurrency.query_pool import QueryPool
 from .interface import DatasetId
 from ..utils.maxsizedict import MaxSizeDict
 from ..utils.url import normalize_url
+from . import defaults
 
 logger = logging.getLogger(__name__)
 
 
 def arg_smallest_positive(arr: numpy.ndarray) -> Optional[int]:
     condition = arr >= 0
     if condition.any():
@@ -34,17 +35,19 @@
     """
 
     DEFAULT_SCHEME = "https"
 
     def __init__(
         self,
         url: str,
-        api_key: str = "elogbook-00000000-0000-0000-0000-000000000000",
+        api_key: Optional[str] = None,
         timeout: Optional[float] = None,
     ):
+        if api_key is None:
+            api_key = defaults.ELOGBOOK_TOKEN
         url = normalize_url(url, default_scheme=self.DEFAULT_SCHEME)
 
         path = f"dataacquisition/{api_key}/investigation"
         query = (
             "?instrumentName={beamline}&investigationName={proposal}&sortBy=startdate"
         )
         self._investigation_url = urljoin(url, path + query)
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/main.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 
 class IcatClient(IcatClientInterface):
     """Direct communication with ICAT: e-logbook, metadata and archive status"""
 
     def __init__(
         self,
-        metadata_urls: Optional[list] = None,
+        metadata_urls: Optional[List[str]] = None,
         elogbook_url: Optional[str] = None,
-        elogbook_token: Optional[str] = "elogbook-00000000-0000-0000-0000-000000000000",
-        metadata_queue: Optional[str] = "icatIngest",
+        elogbook_token: Optional[str] = None,
+        metadata_queue: Optional[str] = None,
         metadata_queue_monitor_port: Optional[int] = None,
         elogbook_timeout: Optional[float] = None,
         feedback_timeout: Optional[float] = None,
         queue_timeout: Optional[float] = None,
         beamline: Optional[str] = None,
         proposal: Optional[str] = None,
         elogbook_metadata: Optional[Mapping] = None,
-        archive_urls: Optional[list] = None,
-        archive_queue: Optional[str] = "icatArchiveRestoreStatus",
+        archive_urls: Optional[List[str]] = None,
+        archive_queue: Optional[str] = None,
         archive_queue_monitor_port: Optional[int] = None,
     ):
         self.current_proposal = proposal
         self.current_beamline = beamline
         self.current_dataset = None
         self.current_path = None
         self.current_dataset_metadata = None
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/messaging.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/messaging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import base64
 import requests
-from typing import Optional
+from typing import Optional, List
 
 from stompest.config import StompConfig
 from stompest.protocol import StompSpec
 from stompest.protocol import StompSession
 from stompest.sync import Stomp
+from stompest.error import StompConnectionError
 
 from ..utils.url import normalize_url
 
 
 class IcatMessagingClient:
     """Client for the ICAT message broker.
 
@@ -23,33 +24,33 @@
     MONITOR_SCHEME = "http"
     DEFAULT_MONITOR_PORT = 8778
     MONITOR_USER = "user"
     MONITOR_PWD = "user"
 
     def __init__(
         self,
-        queue_urls: list,
+        queue_urls: List[str],
         queue_name: str,
         monitor_port: Optional[int] = None,
         timeout: Optional[float] = None,
     ):
         urls = [
             normalize_url(
                 url, default_scheme=self.DEFAULT_SCHEME, default_port=self.DEFAULT_PORT
             )
             for url in queue_urls
         ]
         failover = ",".join(urls)
         url = f"failover:({failover})?maxReconnectAttempts=3,initialReconnectDelay=250,maxReconnectDelay=1000"
         self.__max_version = StompSpec.VERSION_1_1
         self.__client = Stomp(StompConfig(url, version=self.__max_version))
-        self.socket_timeout = None
+        self._socket_timeout = None
         if timeout is None:
             timeout = 1
-        self.connect_timeout = timeout
+        self._connect_timeout = timeout
 
         self.__send_destination = "/queue/" + queue_name
         self.__send_headers = {
             "persistent": "true",
             StompSpec.ACK_HEADER: StompSpec.ACK_CLIENT_INDIVIDUAL,
         }
 
@@ -57,32 +58,43 @@
             monitor_port = self.DEFAULT_MONITOR_PORT
         self.__consumer_count_url = f"{self.MONITOR_SCHEME}://{{host}}:{monitor_port}/api/jolokia/read/org.apache.activemq:type=Broker,brokerName=metadata,destinationType=Queue,destinationName={queue_name}/ConsumerCount"
         self.__jolokia_headers = {
             "Authorization": b"Basic "
             + base64.b64encode(f"{self.MONITOR_USER}:{self.MONITOR_PWD}".encode())
         }
 
-    def close(self):
-        self.__client.close()
+    def reconnect(self):
+        self.__client.disconnect()
+        self._connect()
+
+    def _connect(self):
+        self.__client.connect(
+            versions=[self.__max_version],
+            connectTimeout=self._socket_timeout,
+            connectedTimeout=self._connect_timeout,
+        )
 
     @property
     def _connected_client(self):
         if self.__client.session.state != StompSession.CONNECTED:
-            self.__client.connect(
-                versions=[self.__max_version],
-                connectTimeout=self.socket_timeout,
-                connectedTimeout=self.connect_timeout,
-            )
+            self._connect()
         return self.__client
 
     @property
     def _host(self):
         return self._connected_client._transport.host
 
     def send(self, data: bytes):
+        try:
+            self._send(data)
+        except StompConnectionError:
+            self.reconnect()
+            self._send(data)
+
+    def _send(self, data: bytes):
         self._connected_client.send(
             self.__send_destination, body=data, headers=self.__send_headers
         )
 
     @property
     def _consumer_count(self):
         url = self.__consumer_count_url.format(host=self._host)
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/metadata.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import os
-from typing import Optional
+from typing import Optional, List
 import xml.etree.ElementTree as etree
 
 from .xmlns import dataset_as_xml
 from .xmlns import investigation_as_xml
 from .messaging import IcatMessagingClient
+from . import defaults
 
 
 class IcatMetadataClient:
     """Client for storing dataset metadata in ICAT."""
 
     def __init__(
         self,
-        queue_urls: list,
-        queue_name: str = "icatIngest",
+        queue_urls: Optional[List[str]] = None,
+        queue_name: Optional[str] = None,
         monitor_port: Optional[int] = None,
         timeout: Optional[float] = None,
     ):
+        if queue_urls is None:
+            defaults.METADATA_BROKERS
+        if queue_name is None:
+            queue_name = defaults.METADATA_QUEUE
         self._client = IcatMessagingClient(
             queue_urls, queue_name, monitor_port=monitor_port, timeout=timeout
         )
 
     def send_metadata(
         self,
         beamline: str,
@@ -71,12 +76,13 @@
             payload = f.read()
         self._client.send(payload)
 
     def start_investigation(self, beamline: str, proposal: str, start_datetime=None):
         root = investigation_as_xml(
             beamline=beamline, proposal=proposal, start_datetime=start_datetime
         )
+        self._client.reconnect()
         self._client.send(etree.tostring(root))
 
     def check_health(self):
         """Raises an exception when not healthy"""
         self._client.check_health()
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/null.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/null.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/serialize.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/client/xmlns.py` & `pyicat-plus-0.1.3/src/pyicat_plus/client/xmlns.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/concurrency/__init__.py` & `pyicat-plus-0.1.3/src/pyicat_plus/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/concurrency/query_pool/gevent.py` & `pyicat-plus-0.1.3/src/pyicat_plus/concurrency/query_pool/gevent.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/concurrency/query_pool/threading.py` & `pyicat-plus-0.1.3/src/pyicat_plus/concurrency/query_pool/threading.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/metadata/definitions.py` & `pyicat-plus-0.1.3/src/pyicat_plus/metadata/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,17 @@
                 return value
             else:
                 return getter(value.info.field_name)
 
         cls = type(self)
         for k, v in self.items():
             if isinstance(v, cls):
-                adict[k] = v.namespace(getter=getter, setter=setter)
+                adict[k] = v.namespace(
+                    getter=getter, setter=setter, property_decorator=property_decorator
+                )
             else:
                 adict[k] = v
         return NamespaceWrapper(
             property_names=list(adict),
             property_decorator=property_decorator,
             getter=wrap_getter,
             setter=wrap_setter,
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/metadata/hdf5_cfg.xml` & `pyicat-plus-0.1.3/src/pyicat_plus/metadata/hdf5_cfg.xml`

 * *Files 2% similar despite different names*

#### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/metadata/hdf5_cfg.xml` & `pyicat-plus-0.1.3/src/pyicat_plus/metadata/hdf5_cfg.xml`

```diff
@@ -88,26 +88,26 @@
     <amplitude_contrast ESRF_description="Amplitude contrast" NAPItype="NX_CHAR">${EM_amplitude_contrast}</amplitude_contrast>
     <sampling_rate ESRF_description="samplingRate" NAPItype="NX_CHAR">${EM_sampling_rate}</sampling_rate>
   </group>
   <group NX_class="NXsubentry" groupName="PTYCHO">
     <propagation record="final" ESRF_description="Propagation may be near or far" NAPItype="NX_CHAR">${PTYCHO_propagation}</propagation>
     <beamSize record="final" ESRF_description="Beam size on the sample in microns" NAPItype="NX_FLOAT" units="micron">${PTYCHO_beamSize}</beamSize>
     <stepSize record="final" ESRF_description="Step size during scan" NAPItype="NX_FLOAT" units="micron">${PTYCHO_stepSize}</stepSize>
-    <focusToDetectorDistance record="final" ESRF_description="Step size during scan" NAPItype="NX_FLOAT" units="mm">${PTYCHO_focusToDetectorDistance}</focusToDetectorDistance>
+    <focusToDetectorDistance record="final" ESRF_description="Focus to detector distance" NAPItype="NX_FLOAT" units="mm">${PTYCHO_focusToDetectorDistance}</focusToDetectorDistance>
     <countTime record="final" ESRF_description="Step size during scan" NAPItype="NX_FLOAT" units="s">${PTYCHO_countTime}</countTime>
     <parameters record="final" ESRF_description="Ptycho parameters" NAPItype="NX_CHAR">${PTYCHO_parameters}</parameters>
     <refN record="final" ESRF_description="Ptycho parameters" NAPItype="NX_FLOAT">${PTYCHO_refN}</refN>
     <darkN record="final" ESRF_description="Ptycho parameters" NAPItype="NX_FLOAT">${PTYCHO_darkN}</darkN>
     <pixelSize record="final" ESRF_description="Ptycho parameters" NAPItype="NX_CHAR" units="micron">${PTYCHO_pixelSize}</pixelSize>
     <group NX_class="NXcollection" groupName="Axis1">
       <name ESRF_description="Scan motor in the horizontal direction" NAPItype="NX_CHAR">${PTYCHO_Axis1_name}</name>
       <range ESRF_description="Range of the moves in microns" NAPItype="NX_FLOAT" units="micron">${PTYCHO_Axis1_range}</range>
     </group>
     <group NX_class="NXcollection" groupName="Axis2">
-      <name ESRF_description="Scan motor in the horizontal direction" NAPItype="NX_CHAR">${PTYCHO_Axis2_name}</name>
+      <name ESRF_description="Scan motor in the vertical direction" NAPItype="NX_CHAR">${PTYCHO_Axis2_name}</name>
       <range ESRF_description="Range of the moves in microns" NAPItype="NX_FLOAT" units="micron">${PTYCHO_Axis2_range}</range>
     </group>
   </group>
   <group NX_class="NXsubentry" groupName="FLUO">
     <pixelSize record="final" ESRF_description="" NAPItype="NX_FLOAT" units="micron">${FLUO_pixelSize}</pixelSize>
     <dwellTime record="final" ESRF_description="" NAPItype="NX_FLOAT" units="s">${FLUO_dwellTime}</dwellTime>
     <scanDim_1 record="final" ESRF_description="" NAPItype="NX_FLOAT">${FLUO_scanDim1}</scanDim_1>
@@ -275,14 +275,22 @@
   </group>
   <group NX_class="NXsubentry" groupName="HTXRPD">
     <energy ESRF_description="Beam energy" NAPItype="NX_FLOAT" units="keV">${HTXRPD_energy}</energy>
     <exposureTime ESRF_description="Requested exposure time per diffraction pattern" NAPItype="NX_FLOAT" units="s">${HTXRPD_exposureTime}</exposureTime>
     <distance ESRF_description="The perpendicular sample-detector distance" NAPItype="NX_FLOAT" units="mm">${HTXRPD_distance}</distance>
     <sampleVibration ESRF_description="The vibration speed of the powder sample (0-100 %)" NAPItype="NX_FLOAT" units="">${HTXRPD_sampleVibration}</sampleVibration>
   </group>
+  <group NX_class="NXsubentry" groupName="SXDM">
+    <beamSizeVertical record="final" ESRF_description="Vertical beam size on the sample in microns" NAPItype="NX_FLOAT" units="micron">${SXDM_beamSizeVertical}</beamSizeVertical>
+    <beamSizeHorizontal record="final" ESRF_description="Horizontal beam size on the sample in microns" NAPItype="NX_FLOAT" units="micron">${SXDM_beamSizeHorizontal}</beamSizeHorizontal>
+  </group>
+  <group NX_class="NXsubentry" groupName="BCDI">
+    <beamSizeVertical record="final" ESRF_description="Vertical beam size on the sample in microns" NAPItype="NX_FLOAT" units="micron">${BCDI_beamSizeVertical}</beamSizeVertical>
+    <beamSizeHorizontal record="final" ESRF_description="Horizontal beam size on the sample in microns" NAPItype="NX_FLOAT" units="micron">${BCDI_beamSizeHorizontal}</beamSizeHorizontal>
+  </group>
   <group NX_class="NXsample" groupName="sample">
     <name record="final" ESRF_description="Name of the sample" ESRF_mandatory="Mandatory" NAPItype="NX_CHAR">${Sample_name}</name>
     <description record="final" ESRF_description="Description of the sample" NAPItype="NX_CHAR">${Sample_description}</description>
     <distance record="final" ESRF_description="Translation of the sample along the Z-direction of the laboratory coordinate system" NAPItype="NX_CHAR">${Sample_distance}</distance>
     <group NX_class="NXnote" groupName="notes">
       <notes record="final" NAPItype="NX_CHAR">${Sample_notes}</notes>
     </group>
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/metadata/namespace_wrapper.py` & `pyicat-plus-0.1.3/src/pyicat_plus/metadata/namespace_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import partial
 from typing import Callable, Iterable, Optional
 
 
-class NamespaceWrapper(object):
+class NamespaceWrapper:
     """Namespace which delegates attribute getting and setting to a getter and setter method."""
 
     def __new__(
         cls,
         property_names: Iterable[str],
         getter: Callable,
         setter: Optional[Callable] = None,
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/metadata/nexus.py` & `pyicat-plus-0.1.3/src/pyicat_plus/metadata/nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/icat.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/icat.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/proc.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/proc.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/fixtures/tcp.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/fixtures/tcp.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/activemq_rest_server.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/activemq_rest_server.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/icatplus_server.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/icatplus_server.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/stomp_publisher.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/stomp_publisher.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/stomp_subscriber.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/stomp_subscriber.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/servers/utils.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/servers/utils.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_cli.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_elogbook.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_archive.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_archive.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_datasets.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_datasets.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_definitions.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_nexus.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_icat_serialize.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_icat_serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_query_pool.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_query_pool.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/test_url_utils.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/test_url_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/tests/utils/compare.py` & `pyicat-plus-0.1.3/src/pyicat_plus/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/utils/maxsizedict.py` & `pyicat-plus-0.1.3/src/pyicat_plus/utils/maxsizedict.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus/utils/url.py` & `pyicat-plus-0.1.3/src/pyicat_plus/utils/url.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus.egg-info/PKG-INFO` & `pyicat-plus-0.1.3/src/pyicat_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat-plus-0.1.2/src/pyicat_plus.egg-info/SOURCES.txt` & `pyicat-plus-0.1.3/src/pyicat_plus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/pyicat_plus.egg-info/top_level.txt
 src/pyicat_plus/apps/__init__.py
 src/pyicat_plus/apps/store_from_file.py
 src/pyicat_plus/apps/store_processed.py
 src/pyicat_plus/apps/store_raw.py
 src/pyicat_plus/client/__init__.py
 src/pyicat_plus/client/archive.py
+src/pyicat_plus/client/defaults.py
 src/pyicat_plus/client/elogbook.py
 src/pyicat_plus/client/interface.py
 src/pyicat_plus/client/investigation.py
 src/pyicat_plus/client/main.py
 src/pyicat_plus/client/messaging.py
 src/pyicat_plus/client/metadata.py
 src/pyicat_plus/client/null.py
```

