# Comparing `tmp/lavacli-1.7.tar.gz` & `tmp/lavacli-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavacli-1.7.tar", last modified: Fri Apr  7 12:41:44 2023, max compression
+gzip compressed data, was "lavacli-1.8.tar", last modified: Wed Apr 12 15:50:06 2023, max compression
```

## Comparing `lavacli-1.7.tar` & `lavacli-1.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 12:41:44.641114 lavacli-1.7/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-1.7/.coveragerc
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2506 2023-03-17 09:18:40.000000 lavacli-1.7/.gitlab-ci.yml
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-1.7/LICENSE
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-1.7/MANIFEST.in
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-07 12:41:44.641114 lavacli-1.7/PKG-INFO
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 12:41:44.637114 lavacli-1.7/doc/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-1.7/doc/Makefile
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-1.7/doc/conf.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-1.7/doc/configuration.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-1.7/doc/index.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      721 2019-04-24 15:25:09.000000 lavacli-1.7/doc/install.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-1.7/doc/usage.rst
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 12:41:44.641114 lavacli-1.7/lavacli/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1344 2023-04-07 12:35:31.000000 lavacli-1.7/lavacli/__about__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9098 2023-04-07 07:01:47.000000 lavacli-1.7/lavacli/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-1.7/lavacli/__main__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-1.7/lavacli/colors.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 12:41:44.641114 lavacli-1.7/lavacli/commands/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-1.7/lavacli/commands/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-1.7/lavacli/commands/aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-1.7/lavacli/commands/device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-1.7/lavacli/commands/devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-1.7/lavacli/commands/events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-1.7/lavacli/commands/groups.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-1.7/lavacli/commands/identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-04-07 07:01:47.000000 lavacli-1.7/lavacli/commands/jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    33394 2023-04-07 12:33:18.000000 lavacli-1.7/lavacli/commands/lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-1.7/lavacli/commands/results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-1.7/lavacli/commands/system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-1.7/lavacli/commands/tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11204 2023-04-07 12:33:18.000000 lavacli-1.7/lavacli/commands/users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-1.7/lavacli/commands/utils.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-1.7/lavacli/commands/workers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-1.7/lavacli/utils.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 12:41:44.641114 lavacli-1.7/lavacli.egg-info/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-07 12:41:44.000000 lavacli-1.7/lavacli.egg-info/PKG-INFO
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1242 2023-04-07 12:41:44.000000 lavacli-1.7/lavacli.egg-info/SOURCES.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-07 12:41:44.000000 lavacli-1.7/lavacli.egg-info/dependency_links.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-04-07 12:41:44.000000 lavacli-1.7/lavacli.egg-info/entry_points.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-04-07 12:41:44.000000 lavacli-1.7/lavacli.egg-info/requires.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-04-07 12:41:44.000000 lavacli-1.7/lavacli.egg-info/top_level.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-07 12:41:44.000000 lavacli-1.7/lavacli.egg-info/zip-safe
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-03-17 09:09:30.000000 lavacli-1.7/requirements.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-04-07 12:41:44.641114 lavacli-1.7/setup.cfg
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2417 2023-03-17 09:10:17.000000 lavacli-1.7/setup.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 12:41:44.641114 lavacli-1.7/share/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-1.7/share/lavacli.yaml
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 12:41:44.641114 lavacli-1.7/tests/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-1.7/tests/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-1.7/tests/conftest.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_helpers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-1.7/tests/test_jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    76698 2023-04-07 12:33:18.000000 lavacli-1.7/tests/test_lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_lavacli.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-1.7/tests/test_tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4743 2023-04-07 12:33:18.000000 lavacli-1.7/tests/test_users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-1.7/tests/test_workers.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.877318 lavacli-1.8/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-1.8/.coveragerc
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2506 2023-03-17 09:18:40.000000 lavacli-1.8/.gitlab-ci.yml
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-1.8/LICENSE
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-1.8/MANIFEST.in
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-12 15:50:06.877318 lavacli-1.8/PKG-INFO
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.869318 lavacli-1.8/doc/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-1.8/doc/Makefile
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-1.8/doc/conf.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-1.8/doc/configuration.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-1.8/doc/index.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      721 2019-04-24 15:25:09.000000 lavacli-1.8/doc/install.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-1.8/doc/usage.rst
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.869318 lavacli-1.8/lavacli/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1344 2023-04-12 15:49:32.000000 lavacli-1.8/lavacli/__about__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9098 2023-04-12 15:39:30.000000 lavacli-1.8/lavacli/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/__main__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-1.8/lavacli/colors.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.873318 lavacli-1.8/lavacli/commands/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-1.8/lavacli/commands/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-1.8/lavacli/commands/device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-1.8/lavacli/commands/devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-1.8/lavacli/commands/events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-1.8/lavacli/commands/groups.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-04-07 07:01:47.000000 lavacli-1.8/lavacli/commands/jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    33751 2023-04-12 15:39:33.000000 lavacli-1.8/lavacli/commands/lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-1.8/lavacli/commands/system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-1.8/lavacli/commands/tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11354 2023-04-12 15:39:33.000000 lavacli-1.8/lavacli/commands/users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-1.8/lavacli/commands/utils.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-1.8/lavacli/commands/workers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-1.8/lavacli/utils.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.869318 lavacli-1.8/lavacli.egg-info/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/PKG-INFO
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1242 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/SOURCES.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/dependency_links.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/entry_points.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/requires.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/top_level.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-12 15:50:06.000000 lavacli-1.8/lavacli.egg-info/zip-safe
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-03-17 09:09:30.000000 lavacli-1.8/requirements.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-04-12 15:50:06.877318 lavacli-1.8/setup.cfg
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2417 2023-03-17 09:10:17.000000 lavacli-1.8/setup.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.873318 lavacli-1.8/share/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-1.8/share/lavacli.yaml
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-12 15:50:06.873318 lavacli-1.8/tests/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-1.8/tests/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-1.8/tests/conftest.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_helpers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-1.8/tests/test_jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    78667 2023-04-12 15:39:33.000000 lavacli-1.8/tests/test_lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_lavacli.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-1.8/tests/test_tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5479 2023-04-12 15:39:33.000000 lavacli-1.8/tests/test_users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-1.8/tests/test_workers.py
```

### Comparing `lavacli-1.7/.gitlab-ci.yml` & `lavacli-1.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/LICENSE` & `lavacli-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/PKG-INFO` & `lavacli-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 1.7
+Version: 1.8
 Summary: LAVA XML-RPC command line interface
 Home-page: https://git.lavasoftware.org/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
 Project-URL: Bug Tracker, https://git.lavasoftware.org/lava/lavacli/issues/
 Project-URL: Documentation, https://docs.lavasoftware.org/lavacli/
```

### Comparing `lavacli-1.7/doc/Makefile` & `lavacli-1.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/doc/conf.py` & `lavacli-1.8/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/doc/configuration.rst` & `lavacli-1.8/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/doc/install.rst` & `lavacli-1.8/doc/install.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/doc/usage.rst` & `lavacli-1.8/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/__about__.py` & `lavacli-1.8/lavacli/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 
 
 __author__ = "Rémi Duraffort"
 __author_email__ = "remi.duraffort@linaro.org"
 __description__ = "LAVA XML-RPC command line interface"
 __license__ = "AGPLv3+"
 __url__ = "https://git.lavasoftware.org/lava/lavacli"
-__version__ = "1.7"
+__version__ = "1.8"
```

### Comparing `lavacli-1.7/lavacli/__init__.py` & `lavacli-1.8/lavacli/__init__.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/__main__.py` & `lavacli-1.8/lavacli/__main__.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/aliases.py` & `lavacli-1.8/lavacli/commands/aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/device_types.py` & `lavacli-1.8/lavacli/commands/device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/devices.py` & `lavacli-1.8/lavacli/commands/devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/events.py` & `lavacli-1.8/lavacli/commands/events.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/groups.py` & `lavacli-1.8/lavacli/commands/groups.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/identities.py` & `lavacli-1.8/lavacli/commands/identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/jobs.py` & `lavacli-1.8/lavacli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/lab.py` & `lavacli-1.8/lavacli/commands/lab.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,25 +224,34 @@
     username: str
     last_name: str = ""
     first_name: str = ""
     email: str = ""
     is_superuser: bool = False
     is_staff: bool = False
     is_active: bool = True
+    ldap: bool = False
     groups: Set[str] = field(default_factory=set)
     permissions: Set[Permission] = field(default_factory=set)
 
     def __post_init__(self):
         self.groups = set(self.groups)
         self.permissions = set([Permission.from_str(p) for p in self.permissions])
 
     def diff(self, data: Dict[str, Any]) -> List[str]:
         data = data.copy()
         data["groups"] = set(data["groups"])
-        return super().diff(data)
+        diff = super().diff(data)
+        # ldap is user add only.
+        if "ldap" in diff:
+            diff.remove("ldap")
+        # Don't update first_name, last_name and email for ldap user.
+        if self.ldap:
+            diff = [d for d in diff if d not in ["first_name", "last_name", "email"]]
+
+        return diff
 
     def dump(self):
         defaults = {f.name: f.default for f in fields(self) if f.default != MISSING}
         data = {}
         for k, v in asdict(self).items():
             if k in defaults and v == defaults[k]:
                 continue
@@ -324,17 +333,17 @@
         )
 
 
 @dataclass
 class Config:
     device_types: Dict[str, DeviceType]
     devices: Dict[str, Device]
-    groups: Dict[str, Group]
-    users: Dict[str, User]
     workers: Dict[str, Worker]
+    groups: Dict[str, Group] = field(default_factory=dict)
+    users: Dict[str, User] = field(default_factory=dict)
 
     def __post_init__(self):
         self.devices = {n: Device(hostname=n, **d) for n, d in self.devices.items()}
         self.device_types = {
             n: DeviceType(name=n, **(dt if dt is not None else {}))
             for n, dt in self.device_types.items()
         }
@@ -450,66 +459,67 @@
                         user.username,
                         user.first_name or None,
                         user.last_name or None,
                         user.email or None,
                         user.is_active,
                         user.is_staff,
                         user.is_superuser,
+                        user.ldap,
                     )
 
             data = proxy.auth.users.show(user.username)
             data["permissions"] = set(
                 [Permission.from_str(p) for p in data["permissions"]]
             )
             diff = user.diff(data)
-            for name in (n for n in diff if n not in ["groups", "permissions"]):
-                print(
-                    f"    {colors.yellow}-> {name}: '{data[name]}' => '{getattr(user, name)}'{colors.reset}"
-                )
-
-            if diff:
+            update_diff = [n for n in diff if n not in ["groups", "permissions"]]
+            if update_diff:
+                for name in update_diff:
+                    print(
+                        f"    {colors.yellow}-> {name}: '{data[name]}' => '{getattr(user, name)}'{colors.reset}"
+                    )
                 if not options.dry_run:
                     proxy.auth.users.update(
                         user.username,
                         user.first_name if "first_name" in diff else None,
                         user.last_name if "last_name" in diff else None,
                         user.email if "email" in diff else None,
                         user.is_active if "is_active" in diff else None,
                         user.is_staff if "is_staff" in diff else None,
                         user.is_superuser if "is_superuser" in diff else None,
                     )
-                if "groups" in diff:
-                    print(f"    {colors.yellow}-> groups{colors.reset}")
-                    missing = user.groups.difference(set(data["groups"]))
-                    for grp in missing:
-                        print(f"      {colors.green}+ {grp}{colors.reset}")
-                        if not options.dry_run:
-                            proxy.auth.users.groups.add(user.username, grp)
-                    missing = set(data["groups"]).difference(user.groups)
-                    for grp in missing:
-                        print(f"      {colors.red}- {grp}{colors.reset}")
-                        if not options.dry_run:
-                            proxy.auth.users.groups.delete(user.username, grp)
-
-                if "permissions" in diff:
-                    print(f"    {colors.yellow}-> permissions{colors.reset}")
-                    missing = user.permissions.difference(set(data["permissions"]))
-                    for perm in missing:
-                        print(f"      {colors.green}+ {perm}{colors.reset}")
-                        if not options.dry_run:
-                            proxy.auth.users.perms.add(
-                                user.username, perm.app, perm.model, perm.codename
-                            )
-                    missing = set(data["permissions"]).difference(user.permissions)
-                    for perm in missing:
-                        print(f"      {colors.red}- {perm}{colors.reset}")
-                        if not options.dry_run:
-                            proxy.auth.users.perms.delete(
-                                user.username, perm.app, perm.model, perm.codename
-                            )
+            if "groups" in diff:
+                print(f"    {colors.yellow}-> groups{colors.reset}")
+                missing = user.groups.difference(set(data["groups"]))
+                for grp in missing:
+                    print(f"      {colors.green}+ {grp}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.auth.users.groups.add(user.username, grp)
+                missing = set(data["groups"]).difference(user.groups)
+                for grp in missing:
+                    print(f"      {colors.red}- {grp}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.auth.users.groups.delete(user.username, grp)
+
+            if "permissions" in diff:
+                print(f"    {colors.yellow}-> permissions{colors.reset}")
+                missing = user.permissions.difference(set(data["permissions"]))
+                for perm in missing:
+                    print(f"      {colors.green}+ {perm}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.auth.users.perms.add(
+                            user.username, perm.app, perm.model, perm.codename
+                        )
+                missing = set(data["permissions"]).difference(user.permissions)
+                for perm in missing:
+                    print(f"      {colors.red}- {perm}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.auth.users.perms.delete(
+                            user.username, perm.app, perm.model, perm.codename
+                        )
 
     print(f"{colors.cyan}> device-types{colors.reset}")
     if "device-types" not in options.resources:
         print(f"  {colors.yellow}-> SKIP{colors.reset}")
     else:
         device_types = [dt["name"] for dt in proxy.scheduler.device_types.list(False)]
         for dt in lab.device_types.values():
```

### Comparing `lavacli-1.7/lavacli/commands/results.py` & `lavacli-1.8/lavacli/commands/results.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/system.py` & `lavacli-1.8/lavacli/commands/system.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/tags.py` & `lavacli-1.8/lavacli/commands/tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/users.py` & `lavacli-1.8/lavacli/commands/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,20 @@
     users_add.add_argument(
         "--superuser",
         action="store_true",
         dest="is_superuser",
         default=False,
         help="superuser",
     )
+    users_add.add_argument(
+        "--ldap",
+        action="store_true",
+        dest="ldap",
+        help="ldap user",
+    )
 
     # "delete"
     users_del = sub.add_parser("delete", help="delete a user")
     users_del.add_argument("username", help="username")
 
     # "groups"
     users_groups = sub.add_parser("groups", help="manage user groups")
@@ -231,14 +237,15 @@
         options.username,
         options.first_name,
         options.last_name,
         options.email,
         options.is_active,
         options.is_staff,
         options.is_superuser,
+        options.ldap,
     )
     return 0
 
 
 def handle_delete(proxy, options, _):
     proxy.auth.users.delete(options.username)
     return 0
```

### Comparing `lavacli-1.7/lavacli/commands/utils.py` & `lavacli-1.8/lavacli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/commands/workers.py` & `lavacli-1.8/lavacli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli/utils.py` & `lavacli-1.8/lavacli/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/lavacli.egg-info/PKG-INFO` & `lavacli-1.8/lavacli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 1.7
+Version: 1.8
 Summary: LAVA XML-RPC command line interface
 Home-page: https://git.lavasoftware.org/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
 Project-URL: Bug Tracker, https://git.lavasoftware.org/lava/lavacli/issues/
 Project-URL: Documentation, https://docs.lavasoftware.org/lavacli/
```

### Comparing `lavacli-1.7/lavacli.egg-info/SOURCES.txt` & `lavacli-1.8/lavacli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/setup.py` & `lavacli-1.8/setup.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/share/lavacli.yaml` & `lavacli-1.8/share/lavacli.yaml`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/conftest.py` & `lavacli-1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_aliases.py` & `lavacli-1.8/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_device_types.py` & `lavacli-1.8/tests/test_device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_devices.py` & `lavacli-1.8/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_events.py` & `lavacli-1.8/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_helpers.py` & `lavacli-1.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_identities.py` & `lavacli-1.8/tests/test_identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_jobs.py` & `lavacli-1.8/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_lab.py` & `lavacli-1.8/tests/test_lab.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,31 @@
                     "is_staff": False,
                     "is_superuser": False,
                     "last_login": None,
                     "last_name": "",
                     "username": "user3",
                 },
             }
+            self.auth_users_show_user3_ldap = {
+                "request": "auth.users.show",
+                "args": ("user3",),
+                "ret": {
+                    "email": "first.last@linaro,org",
+                    "first_name": "First",
+                    "groups": ["group3"],
+                    "permissions": [],
+                    "id": 14,
+                    "is_active": True,
+                    "is_staff": False,
+                    "is_superuser": False,
+                    "last_login": None,
+                    "last_name": "Last",
+                    "username": "user3",
+                },
+            }
             self.scheduler_device_types_list_empty = {
                 "request": "scheduler.device_types.list",
                 "args": (False,),
                 "ret": [],
             }
             self.scheduler_device_types_list = {
                 "request": "scheduler.device_types.list",
@@ -557,15 +574,20 @@
             self.auth_groups_perms_delete_group1 = {
                 "request": "auth.groups.perms.delete",
                 "args": ("group1", "auth", "user", "add_user"),
                 "ret": None,
             }
             self.auth_users_add_user3 = {
                 "request": "auth.users.add",
-                "args": ("user3", None, None, None, True, False, False),
+                "args": ("user3", None, None, None, True, False, False, False),
+                "ret": None,
+            }
+            self.auth_users_add_user3_ldap = {
+                "request": "auth.users.add",
+                "args": ("user3", None, None, None, True, False, False, True),
                 "ret": None,
             }
             self.auth_users_perms_add_user1 = {
                 "request": "auth.users.perms.add",
                 "args": ("user1", "lava_scheduler_app", "device", "delete_device"),
                 "ret": None,
             }
@@ -1132,14 +1154,48 @@
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_users_add_ldap(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "users", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.auth_users_list,
+            mock_get.auth_users_show_user1,
+            mock_get.auth_users_show_user2,
+            mock_post.auth_users_add_user3_ldap,
+            mock_get.auth_users_show_user3_ldap,
+        ],
+    )
+
+    yaml = ruamel.yaml.YAML(typ="safe")
+    data = yaml.load(config_def)
+    data["users"]["user3"] = {"ldap": True, "groups": ["group3"], "permissions": []}
+    with open(config_file, "w") as f:
+        yaml.dump(data, f)
+    expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[32m* user1\x1b[0m\n  \x1b[32m* user2\x1b[0m\n  \x1b[33m* user3\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == expected_out
+    assert err == ""
+
+
 def test_lab_apply_users_update(
     setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
 ):
     monkeypatch.setattr(
         sys,
         "argv",
         ["lavacli", "lab", "apply", "--resource", "users", str(config_file)],
@@ -1185,15 +1241,14 @@
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
             mock_get.auth_users_list,
             mock_get.auth_users_show_user1,
-            mock_post.auth_users_update_user1,
             mock_post.auth_users_groups_add_user1_group2,
             mock_get.auth_users_show_user2,
         ],
     )
 
     yaml = ruamel.yaml.YAML(typ="safe")
     data = yaml.load(config_def)
@@ -1219,15 +1274,14 @@
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
             mock_get.auth_users_list,
             mock_get.auth_users_show_user1,
-            mock_post.auth_users_update_user1,
             mock_post.auth_users_groups_delete_user1_group1,
             mock_get.auth_users_show_user2,
         ],
     )
 
     yaml = ruamel.yaml.YAML(typ="safe")
     data = yaml.load(config_def)
@@ -1253,15 +1307,14 @@
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
             mock_get.auth_users_list,
             mock_get.auth_users_show_user1,
-            mock_post.auth_users_update_user1,
             mock_post.auth_users_perms_add_user1,
             mock_get.auth_users_show_user2,
         ],
     )
 
     yaml = ruamel.yaml.YAML(typ="safe")
     data = yaml.load(config_def)
@@ -1289,15 +1342,14 @@
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
             mock_get.auth_users_list,
             mock_get.auth_users_show_user1,
-            mock_post.auth_users_update_user1,
             mock_post.auth_users_perms_delete_user1,
             mock_get.auth_users_show_user2,
         ],
     )
 
     yaml = ruamel.yaml.YAML(typ="safe")
     data = yaml.load(config_def)
```

### Comparing `lavacli-1.7/tests/test_lavacli.py` & `lavacli-1.8/tests/test_lavacli.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_results.py` & `lavacli-1.8/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_system.py` & `lavacli-1.8/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_tags.py` & `lavacli-1.8/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.7/tests/test_users.py` & `lavacli-1.8/tests/test_users.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             {"request": "system.version", "args": (), "ret": version},
             {
                 "request": "auth.users.add",
-                "args": ("user1", None, None, None, True, True, True),
+                "args": ("user1", None, None, None, True, True, True, False),
                 "ret": None,
             },
         ],
     )
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == ""
@@ -70,15 +70,46 @@
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             {"request": "system.version", "args": (), "ret": version},
             {
                 "request": "auth.users.add",
-                "args": ("user1", None, None, None, False, False, False),
+                "args": ("user1", None, None, None, False, False, False, False),
+                "ret": None,
+            },
+        ],
+    )
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert out == ""
+    assert err == ""
+
+
+def test_users_add_ldap(setup, monkeypatch, capsys):
+    version = "2023.03"
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        [
+            "lavacli",
+            "users",
+            "add",
+            "--ldap",
+            "user1",
+        ],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            {"request": "system.version", "args": (), "ret": version},
+            {
+                "request": "auth.users.add",
+                "args": ("user1", None, None, None, True, False, False, True),
                 "ret": None,
             },
         ],
     )
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == ""
```

### Comparing `lavacli-1.7/tests/test_workers.py` & `lavacli-1.8/tests/test_workers.py`

 * *Files identical despite different names*

