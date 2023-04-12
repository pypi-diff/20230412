# Comparing `tmp/glustercli-0.8.3.tar.gz` & `tmp/glustercli-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glustercli-0.8.3.tar", last modified: Mon May 23 15:16:26 2022, max compression
+gzip compressed data, was "glustercli-0.8.4.tar", last modified: Wed Apr 12 16:12:29 2023, max compression
```

## Comparing `glustercli-0.8.3.tar` & `glustercli-0.8.4.tar`

### file list

```diff
@@ -1,40 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 15:16:26.904582 glustercli-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-05-23 15:16:18.000000 glustercli-0.8.3/COPYING-GPLV2
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-05-23 15:16:18.000000 glustercli-0.8.3/COPYING-LGPLV3
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-05-23 15:16:18.000000 glustercli-0.8.3/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-05-23 15:16:18.000000 glustercli-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-05-23 15:16:26.900582 glustercli-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-05-23 15:16:18.000000 glustercli-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 15:16:26.896582 glustercli-0.8.3/glustercli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 15:16:26.900582 glustercli-0.8.3/glustercli/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/bitrot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3867 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/bricks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8171 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/georep.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/gluster_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/heal.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/nfs_ganesha.py
--rw-r--r--   0 runner    (1001) docker     (121)    27409 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/peer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4725 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/quota.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/rebalance.py
--rw-r--r--   0 runner    (1001) docker     (121)     5029 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6660 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11053 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/cli/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 15:16:26.900582 glustercli-0.8.3/glustercli/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/metrics/cmdlineparser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3876 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/metrics/diskstats.py
--rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/metrics/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/metrics/utilization.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-05-23 15:16:18.000000 glustercli-0.8.3/glustercli/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 15:16:26.896582 glustercli-0.8.3/glustercli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-05-23 15:16:26.000000 glustercli-0.8.3/glustercli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-05-23 15:16:26.000000 glustercli-0.8.3/glustercli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 15:16:26.000000 glustercli-0.8.3/glustercli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-23 15:16:26.000000 glustercli-0.8.3/glustercli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-23 15:16:26.000000 glustercli-0.8.3/glustercli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-23 15:16:26.904582 glustercli-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-05-23 15:16:18.000000 glustercli-0.8.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-23 15:16:18.000000 glustercli-0.8.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.187635 glustercli-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.179635 glustercli-0.8.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 16:12:20.000000 glustercli-0.8.4/.github/workflows/on-release-tag.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 16:12:20.000000 glustercli-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-12 16:12:20.000000 glustercli-0.8.4/COPYING-GPLV2
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-12 16:12:20.000000 glustercli-0.8.4/COPYING-LGPLV3
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 16:12:20.000000 glustercli-0.8.4/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-12 16:12:20.000000 glustercli-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-12 16:12:20.000000 glustercli-0.8.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-12 16:12:29.187635 glustercli-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 16:12:20.000000 glustercli-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/debian/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/changelog
+-rwxr-xr-x   0 runner    (1001) docker     (123)        3 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/compat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/debian/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/source/format
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-12 16:12:20.000000 glustercli-0.8.4/debian/source/options
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/bitrot.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/bricks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/georep.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/heal.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/local_diskstats.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/local_processes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/local_utilization.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/nfs_ganesha.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/peer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/quota.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/rebalance.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/snapshot.md
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-04-12 16:12:20.000000 glustercli-0.8.4/docs/volume.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/glustercli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.187635 glustercli-0.8.4/glustercli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/bitrot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/georep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/gluster_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/heal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/nfs_ganesha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27409 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/rebalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/cli/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.187635 glustercli-0.8.4/glustercli/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/cmdlineparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/diskstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 16:12:20.000000 glustercli-0.8.4/glustercli/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:12:29.183635 glustercli-0.8.4/glustercli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 16:12:29.000000 glustercli-0.8.4/glustercli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-12 16:12:20.000000 glustercli-0.8.4/pydocmd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 16:12:20.000000 glustercli-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:12:29.187635 glustercli-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-12 16:12:20.000000 glustercli-0.8.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 16:12:20.000000 glustercli-0.8.4/tox.ini
```

### Comparing `glustercli-0.8.3/COPYING-GPLV2` & `glustercli-0.8.4/COPYING-GPLV2`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/COPYING-LGPLV3` & `glustercli-0.8.4/COPYING-LGPLV3`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/MAINTAINERS` & `glustercli-0.8.4/MAINTAINERS`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/PKG-INFO` & `glustercli-0.8.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: glustercli
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python bindings for GlusterFS CLI and Metrics collection
 Home-page: https://github.com/gluster/glustercli-python
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: GPLv2 or LGPLv3+
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -18,10 +17,7 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Filesystems
 License-File: COPYING-GPLV2
 License-File: COPYING-LGPLV3
-
-UNKNOWN
-
```

### Comparing `glustercli-0.8.3/README.md` & `glustercli-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/__init__.py` & `glustercli-0.8.4/glustercli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/bitrot.py` & `glustercli-0.8.4/glustercli/cli/bitrot.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/bricks.py` & `glustercli-0.8.4/glustercli/cli/bricks.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/georep.py` & `glustercli-0.8.4/glustercli/cli/georep.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/heal.py` & `glustercli-0.8.4/glustercli/cli/heal.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/nfs_ganesha.py` & `glustercli-0.8.4/glustercli/cli/nfs_ganesha.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/parsers.py` & `glustercli-0.8.4/glustercli/cli/parsers.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/peer.py` & `glustercli-0.8.4/glustercli/cli/peer.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/quota.py` & `glustercli-0.8.4/glustercli/cli/quota.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/rebalance.py` & `glustercli-0.8.4/glustercli/cli/rebalance.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/snapshot.py` & `glustercli-0.8.4/glustercli/cli/snapshot.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/utils.py` & `glustercli-0.8.4/glustercli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/cli/volume.py` & `glustercli-0.8.4/glustercli/cli/volume.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/metrics/cmdlineparser.py` & `glustercli-0.8.4/glustercli/metrics/cmdlineparser.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/metrics/diskstats.py` & `glustercli-0.8.4/glustercli/metrics/diskstats.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/metrics/process.py` & `glustercli-0.8.4/glustercli/metrics/process.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/metrics/utilization.py` & `glustercli-0.8.4/glustercli/metrics/utilization.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli/metrics/utils.py` & `glustercli-0.8.4/glustercli/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `glustercli-0.8.3/glustercli.egg-info/PKG-INFO` & `glustercli-0.8.4/glustercli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: glustercli
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python bindings for GlusterFS CLI and Metrics collection
 Home-page: https://github.com/gluster/glustercli-python
 Author: Aravinda Vishwanathapura
 Author-email: aravinda@kadalu.io
 License: GPLv2 or LGPLv3+
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -18,10 +17,7 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Filesystems
 License-File: COPYING-GPLV2
 License-File: COPYING-LGPLV3
-
-UNKNOWN
-
```

### Comparing `glustercli-0.8.3/setup.py` & `glustercli-0.8.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
 import re
 from setuptools import setup
+from importlib.metadata import version, PackageNotFoundError
 
-VERSION = os.environ.get("VERSION", "master")
-
+try:
+    __version__ = version('glustercli')
+except PackageNotFoundError:
+    __version__ = "unknown"
 
 setup(
     name='glustercli',
-    version=VERSION,
+    version=__version__,
     description='Python bindings for GlusterFS CLI and Metrics collection',
     license='GPLv2 or LGPLv3+',
     author='Aravinda Vishwanathapura',
     author_email='aravinda@kadalu.io',
     url='https://github.com/gluster/glustercli-python',
     packages=["glustercli", "glustercli.cli", "glustercli.metrics"],
     install_requires=["paramiko"],
```

