# Comparing `tmp/presencedb-0.1.tar.gz` & `tmp/presencedb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "presencedb-0.1.tar", last modified: Thu Jan 27 19:22:39 2022, max compression
+gzip compressed data, was "presencedb-2.0.0.tar", last modified: Wed Apr 12 02:39:03 2023, max compression
```

## Comparing `presencedb-0.1.tar` & `presencedb-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-01-27 19:22:38.973369 presencedb-0.1/
--rw-rw-rw-   0        0        0      697 2022-01-27 19:22:38.973369 presencedb-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-01-27 19:22:38.884364 presencedb-0.1/presencedb/
--rw-rw-rw-   0        0        0       84 2022-01-27 17:34:05.836615 presencedb-0.1/presencedb/__init__.py
--rw-rw-rw-   0        0        0      472 2022-01-27 18:17:31.648182 presencedb-0.1/presencedb/enums.py
--rw-rw-rw-   0        0        0      299 2022-01-27 16:36:25.945277 presencedb-0.1/presencedb/errors.py
--rw-rw-rw-   0        0        0     2359 2022-01-27 18:16:10.107683 presencedb-0.1/presencedb/models.py
--rw-rw-rw-   0        0        0     1928 2022-01-27 19:21:31.627449 presencedb-0.1/presencedb/presencedb.py
--rw-rw-rw-   0        0        0     1461 2022-01-27 19:19:45.181804 presencedb-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:39:03.772838 presencedb-2.0.0/
+-rw-rw-rw-   0        0        0       75 2023-04-08 15:41:18.000000 presencedb-2.0.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     1083 2022-01-27 14:54:09.000000 presencedb-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      647 2023-04-12 02:39:03.771837 presencedb-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1639 2023-04-12 01:42:39.000000 presencedb-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 02:39:03.725837 presencedb-2.0.0/presencedb/
+-rw-rw-rw-   0        0        0      414 2023-04-12 02:01:27.000000 presencedb-2.0.0/presencedb/__init__.py
+-rw-rw-rw-   0        0        0     2118 2023-04-12 02:18:38.000000 presencedb-2.0.0/presencedb/abc.py
+-rw-rw-rw-   0        0        0     2647 2023-04-12 02:18:41.000000 presencedb-2.0.0/presencedb/activity.py
+-rw-rw-rw-   0        0        0     4888 2023-04-12 02:18:41.000000 presencedb-2.0.0/presencedb/client.py
+-rw-rw-rw-   0        0        0      650 2023-04-08 15:42:21.000000 presencedb-2.0.0/presencedb/constants.py
+-rw-rw-rw-   0        0        0     1119 2023-04-12 01:51:56.000000 presencedb-2.0.0/presencedb/enums.py
+-rw-rw-rw-   0        0        0     2511 2023-04-12 02:16:02.000000 presencedb-2.0.0/presencedb/errors.py
+-rw-rw-rw-   0        0        0     6323 2023-04-12 02:21:18.000000 presencedb-2.0.0/presencedb/user.py
+-rw-rw-rw-   0        0        0     1777 2023-04-12 01:51:57.000000 presencedb-2.0.0/presencedb/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:39:03.765840 presencedb-2.0.0/presencedb.egg-info/
+-rw-rw-rw-   0        0        0      647 2023-04-12 02:39:03.000000 presencedb-2.0.0/presencedb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-12 02:39:03.000000 presencedb-2.0.0/presencedb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 02:39:03.000000 presencedb-2.0.0/presencedb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-12 02:39:03.000000 presencedb-2.0.0/presencedb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-12 02:39:03.000000 presencedb-2.0.0/presencedb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      941 2023-04-12 02:38:52.000000 presencedb-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 02:39:03.773837 presencedb-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-04-12 02:01:14.000000 presencedb-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 02:39:03.769835 presencedb-2.0.0/tests/
+-rw-rw-rw-   0        0        0     1034 2023-04-12 02:18:42.000000 presencedb-2.0.0/tests/test_activities.py
+-rw-rw-rw-   0        0        0      415 2023-04-12 02:18:42.000000 presencedb-2.0.0/tests/test_user.py
```

### Comparing `presencedb-0.1/PKG-INFO` & `presencedb-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: presencedb
-Version: 0.1
-Summary: API wrapper for the presencedb (undocumented) api
+Version: 2.0.0
+Summary: A modern, feature rich, easy to use API wrapper for presencedb
 Home-page: https://github.com/xFGhoul/py-presencedb
-Author: Ghoul
-Author-email: UNKNOWN
+Author: xFGhoul
 License: MIT
-Description: UNKNOWN
-Keywords: discord,api,presencedb
-Platform: UNKNOWN
+Keywords: discord,api,presencedb,discord-api,discord bot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.11
+License-File: LICENSE
+License-File: AUTHORS.md
```

