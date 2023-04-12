# Comparing `tmp/cxlint-1.0.3.tar.gz` & `tmp/cxlint-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/pmarlow/eng/cxlint/dist/tmppx_0w9t4/cxlint-1.0.3.tar", last modified: Wed Apr 12 03:06:04 2023, max compression
+gzip compressed data, was "/Users/pmarlow/eng/cxlint/dist/tmpwr51zaep/cxlint-1.0.4.tar", last modified: Wed Apr 12 03:57:26 2023, max compression
```

## Comparing `cxlint-1.0.3.tar` & `cxlint-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,99 @@
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 03:06:04.000000 cxlint-1.0.3/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2978 2023-04-12 01:31:40.000000 cxlint-1.0.3/README.md
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1753 2023-04-12 03:05:33.000000 cxlint-1.0.3/setup.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-04-12 03:06:04.000000 cxlint-1.0.3/setup.cfg
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2023-03-01 20:47:23.000000 cxlint-1.0.3/LICENSE.txt
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8160 2023-04-12 03:05:27.000000 cxlint-1.0.3/src/cxlint/cxlint.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint/resources/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3441 2023-04-12 02:20:03.000000 cxlint-1.0.3/src/cxlint/resources/route_groups.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8793 2023-04-12 02:19:51.000000 cxlint-1.0.3/src/cxlint/resources/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6180 2023-04-12 02:19:29.000000 cxlint-1.0.3/src/cxlint/resources/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-26 14:31:21.000000 cxlint-1.0.3/src/cxlint/resources/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7029 2023-04-12 02:20:20.000000 cxlint-1.0.3/src/cxlint/resources/types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1348 2023-04-12 02:19:17.000000 cxlint-1.0.3/src/cxlint/resources/agents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5978 2023-04-12 02:19:59.000000 cxlint-1.0.3/src/cxlint/resources/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13432 2023-04-12 02:19:45.000000 cxlint-1.0.3/src/cxlint/resources/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4160 2023-04-12 02:20:25.000000 cxlint-1.0.3/src/cxlint/resources/webhooks.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9825 2023-04-12 02:20:16.000000 cxlint-1.0.3/src/cxlint/resources/test_cases.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10560 2023-04-12 02:20:10.000000 cxlint-1.0.3/src/cxlint/resources/routes.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1420 2023-03-02 21:47:37.000000 cxlint-1.0.3/src/cxlint/graph.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-09 15:34:14.000000 cxlint-1.0.3/src/cxlint/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7541 2023-04-12 02:17:45.000000 cxlint-1.0.3/src/cxlint/common.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint/rules/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10503 2023-04-12 02:22:04.000000 cxlint-1.0.3/src/cxlint/rules/intents.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6783 2023-04-12 02:21:53.000000 cxlint-1.0.3/src/cxlint/rules/entity_types.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-03-15 21:40:16.000000 cxlint-1.0.3/src/cxlint/rules/__init__.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2804 2023-04-12 02:20:42.000000 cxlint-1.0.3/src/cxlint/rules/logger.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8607 2023-04-12 02:21:44.000000 cxlint-1.0.3/src/cxlint/rules/pages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6155 2023-04-12 02:21:30.000000 cxlint-1.0.3/src/cxlint/rules/flows.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2301 2023-04-12 02:22:14.000000 cxlint-1.0.3/src/cxlint/rules/webhooks.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5370 2023-04-12 02:20:52.000000 cxlint-1.0.3/src/cxlint/rules/response_messages.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4437 2023-04-12 02:20:58.000000 cxlint-1.0.3/src/cxlint/rules/test_cases.py
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2277 2023-03-02 21:47:37.000000 cxlint-1.0.3/src/cxlint/gcs_utils.py
-drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/PKG-INFO
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      911 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/SOURCES.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        7 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/top_level.txt
--rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-04-12 03:06:04.000000 cxlint-1.0.3/src/cxlint.egg-info/dependency_links.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 03:57:26.000000 cxlint-1.0.4/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2978 2023-04-12 01:31:40.000000 cxlint-1.0.4/README.md
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1803 2023-04-12 03:55:03.000000 cxlint-1.0.4/setup.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)       78 2023-04-12 03:57:26.000000 cxlint-1.0.4/setup.cfg
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11357 2023-03-01 20:47:23.000000 cxlint-1.0.4/LICENSE.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    37587 2023-04-12 03:04:48.000000 cxlint-1.0.4/src/logs.txt
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8160 2023-04-12 03:05:27.000000 cxlint-1.0.4/src/cxlint/cxlint.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint/resources/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3441 2023-04-12 02:20:03.000000 cxlint-1.0.4/src/cxlint/resources/route_groups.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8793 2023-04-12 02:19:51.000000 cxlint-1.0.4/src/cxlint/resources/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6180 2023-04-12 02:19:29.000000 cxlint-1.0.4/src/cxlint/resources/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-26 14:31:21.000000 cxlint-1.0.4/src/cxlint/resources/__init__.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7029 2023-04-12 02:20:20.000000 cxlint-1.0.4/src/cxlint/resources/types.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2743 2023-04-12 02:21:47.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/route_groups.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4559 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/route_groups.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3270 2023-04-12 02:22:22.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/webhooks.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5490 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/webhooks.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    11749 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/intents.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7324 2023-04-12 02:21:57.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/intents.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1086 2023-04-12 02:21:21.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/agents.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7561 2023-04-12 02:21:47.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/routes.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12608 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/routes.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1547 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/agents.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8079 2023-04-12 02:21:20.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4581 2023-04-12 02:21:47.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/pages.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8442 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/pages.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12330 2023-04-12 02:42:08.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/types.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5052 2023-04-12 02:21:47.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/entity_types.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8198 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/entity_types.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    16354 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/flows.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10901 2023-04-12 02:21:21.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/flows.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      167 2023-04-12 02:42:08.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12145 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/test_cases.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7131 2023-04-12 02:22:22.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/test_cases.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      144 2023-01-26 16:47:13.000000 cxlint-1.0.4/src/cxlint/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1348 2023-04-12 02:19:17.000000 cxlint-1.0.4/src/cxlint/resources/agents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5978 2023-04-12 02:19:59.000000 cxlint-1.0.4/src/cxlint/resources/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    13432 2023-04-12 02:19:45.000000 cxlint-1.0.4/src/cxlint/resources/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4160 2023-04-12 02:20:25.000000 cxlint-1.0.4/src/cxlint/resources/webhooks.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9825 2023-04-12 02:20:16.000000 cxlint-1.0.4/src/cxlint/resources/test_cases.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10560 2023-04-12 02:20:10.000000 cxlint-1.0.4/src/cxlint/resources/routes.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1420 2023-03-02 21:47:37.000000 cxlint-1.0.4/src/cxlint/graph.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-01-09 15:34:14.000000 cxlint-1.0.4/src/cxlint/__init__.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint/__pycache__/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      139 2023-04-12 02:35:23.000000 cxlint-1.0.4/src/cxlint/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5937 2023-04-12 02:35:23.000000 cxlint-1.0.4/src/cxlint/__pycache__/cxlint.cpython-39.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8991 2023-04-12 02:42:08.000000 cxlint-1.0.4/src/cxlint/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5879 2023-04-12 02:17:49.000000 cxlint-1.0.4/src/cxlint/__pycache__/common.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2294 2023-04-12 02:42:08.000000 cxlint-1.0.4/src/cxlint/__pycache__/graph.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1546 2023-04-12 02:18:40.000000 cxlint-1.0.4/src/cxlint/__pycache__/graph.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3193 2023-04-12 02:42:08.000000 cxlint-1.0.4/src/cxlint/__pycache__/gcs_utils.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1901 2023-04-12 02:18:40.000000 cxlint-1.0.4/src/cxlint/__pycache__/gcs_utils.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10757 2023-04-12 02:42:08.000000 cxlint-1.0.4/src/cxlint/__pycache__/cxlint.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6089 2023-04-12 03:05:14.000000 cxlint-1.0.4/src/cxlint/__pycache__/cxlint.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      157 2023-04-12 02:42:08.000000 cxlint-1.0.4/src/cxlint/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      141 2023-04-12 02:16:34.000000 cxlint-1.0.4/src/cxlint/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4237 2023-03-31 20:05:56.000000 cxlint-1.0.4/src/cxlint/.cxlintrc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7541 2023-04-12 02:17:45.000000 cxlint-1.0.4/src/cxlint/common.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint/rules/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    10503 2023-04-12 02:22:04.000000 cxlint-1.0.4/src/cxlint/rules/intents.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6783 2023-04-12 02:21:53.000000 cxlint-1.0.4/src/cxlint/rules/entity_types.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        0 2023-03-15 21:40:16.000000 cxlint-1.0.4/src/cxlint/rules/__init__.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5703 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/response_messages.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3455 2023-04-12 02:21:47.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/response_messages.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1852 2023-04-12 02:22:22.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/webhooks.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2713 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/webhooks.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)    12532 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/intents.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3054 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1970 2023-04-12 02:21:34.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7583 2023-04-12 02:22:22.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/intents.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5276 2023-04-12 02:21:47.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/pages.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     9683 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/pages.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4514 2023-04-12 02:21:57.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/entity_types.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7780 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/entity_types.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     7229 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/flows.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3734 2023-04-12 02:21:34.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/flows.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      163 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5228 2023-04-12 02:42:45.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/test_cases.cpython-311.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3263 2023-04-12 02:22:22.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/test_cases.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)      140 2023-03-16 16:05:06.000000 cxlint-1.0.4/src/cxlint/rules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2804 2023-04-12 02:20:42.000000 cxlint-1.0.4/src/cxlint/rules/logger.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     8607 2023-04-12 02:21:44.000000 cxlint-1.0.4/src/cxlint/rules/pages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     6155 2023-04-12 02:21:30.000000 cxlint-1.0.4/src/cxlint/rules/flows.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2301 2023-04-12 02:22:14.000000 cxlint-1.0.4/src/cxlint/rules/webhooks.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     5370 2023-04-12 02:20:52.000000 cxlint-1.0.4/src/cxlint/rules/response_messages.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     4437 2023-04-12 02:20:58.000000 cxlint-1.0.4/src/cxlint/rules/test_cases.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     2277 2023-03-02 21:47:37.000000 cxlint-1.0.4/src/cxlint/gcs_utils.py
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)   221959 2023-04-12 03:05:35.000000 cxlint-1.0.4/src/lint-scratch.ipynb
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     1866 2023-03-31 20:05:05.000000 cxlint-1.0.4/src/main_scratch.py
+drwxr-xr-x   0 pmarlow  (802654) primarygroup (89939)        0 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint.egg-info/
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3835 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint.egg-info/PKG-INFO
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)     3806 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint.egg-info/SOURCES.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        7 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint.egg-info/top_level.txt
+-rw-r--r--   0 pmarlow  (802654) primarygroup (89939)        1 2023-04-12 03:57:26.000000 cxlint-1.0.4/src/cxlint.egg-info/dependency_links.txt
```

### Comparing `cxlint-1.0.3/PKG-INFO` & `cxlint-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxlint
-Version: 1.0.3
+Version: 1.0.4
 Summary: A static code analyzer that provides automated quality       control for Dialogflow CX Agents
 Home-page: https://github.com/GoogleCloudPlatform/cxlint
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,linter,dfcx
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cxlint Version: 1.0.3 Summary: A static code
+Metadata-Version: 2.1 Name: cxlint Version: 1.0.4 Summary: A static code
 analyzer that provides automated quality control for Dialogflow CX Agents Home-
 page: https://github.com/GoogleCloudPlatform/cxlint Author: Patrick Marlow
 Author-email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,linter,dfcx Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

### Comparing `cxlint-1.0.3/README.md` & `cxlint-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/setup.py` & `cxlint-1.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='cxlint',
-    version='1.0.3',
+    version='1.0.4',
     description='A static code analyzer that provides automated quality \
       control for Dialogflow CX Agents',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/cxlint',
     author='Patrick Marlow',
     author_email='pmarlow@google.com',
@@ -40,9 +40,12 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='dialogflow, cx, google, bot, chatbot, linter, dfcx',
     package_dir={'':'src'},
     packages=find_packages(where='src'),
+    package_data={
+      '': ['.cxlintrc']
+    },
     python_requires='>=3.6, <4',
 )
```

### Comparing `cxlint-1.0.3/LICENSE.txt` & `cxlint-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/cxlint.py` & `cxlint-1.0.4/src/cxlint/cxlint.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/route_groups.py` & `cxlint-1.0.4/src/cxlint/resources/route_groups.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/intents.py` & `cxlint-1.0.4/src/cxlint/resources/intents.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/entity_types.py` & `cxlint-1.0.4/src/cxlint/resources/entity_types.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/types.py` & `cxlint-1.0.4/src/cxlint/resources/types.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/agents.py` & `cxlint-1.0.4/src/cxlint/resources/agents.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/pages.py` & `cxlint-1.0.4/src/cxlint/resources/pages.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/flows.py` & `cxlint-1.0.4/src/cxlint/resources/flows.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/webhooks.py` & `cxlint-1.0.4/src/cxlint/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/test_cases.py` & `cxlint-1.0.4/src/cxlint/resources/test_cases.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/resources/routes.py` & `cxlint-1.0.4/src/cxlint/resources/routes.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/graph.py` & `cxlint-1.0.4/src/cxlint/graph.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/common.py` & `cxlint-1.0.4/src/cxlint/common.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/intents.py` & `cxlint-1.0.4/src/cxlint/rules/intents.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/entity_types.py` & `cxlint-1.0.4/src/cxlint/rules/entity_types.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/logger.py` & `cxlint-1.0.4/src/cxlint/rules/logger.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/pages.py` & `cxlint-1.0.4/src/cxlint/rules/pages.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/flows.py` & `cxlint-1.0.4/src/cxlint/rules/flows.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/webhooks.py` & `cxlint-1.0.4/src/cxlint/rules/webhooks.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/response_messages.py` & `cxlint-1.0.4/src/cxlint/rules/response_messages.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/rules/test_cases.py` & `cxlint-1.0.4/src/cxlint/rules/test_cases.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint/gcs_utils.py` & `cxlint-1.0.4/src/cxlint/gcs_utils.py`

 * *Files identical despite different names*

### Comparing `cxlint-1.0.3/src/cxlint.egg-info/PKG-INFO` & `cxlint-1.0.4/src/cxlint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxlint
-Version: 1.0.3
+Version: 1.0.4
 Summary: A static code analyzer that provides automated quality       control for Dialogflow CX Agents
 Home-page: https://github.com/GoogleCloudPlatform/cxlint
 Author: Patrick Marlow
 Author-email: pmarlow@google.com
 License: UNKNOWN
 Keywords: dialogflow,cx,google,bot,chatbot,linter,dfcx
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cxlint Version: 1.0.3 Summary: A static code
+Metadata-Version: 2.1 Name: cxlint Version: 1.0.4 Summary: A static code
 analyzer that provides automated quality control for Dialogflow CX Agents Home-
 page: https://github.com/GoogleCloudPlatform/cxlint Author: Patrick Marlow
 Author-email: pmarlow@google.com License: UNKNOWN Keywords:
 dialogflow,cx,google,bot,chatbot,linter,dfcx Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Communications :: Chat Classifier: Topic ::
```

