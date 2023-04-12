# Comparing `tmp/watchtower_browser_testing-0.2.4.tar.gz` & `tmp/watchtower_browser_testing-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.2.4.tar", last modified: Wed Apr 12 13:23:30 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.2.5.tar", last modified: Wed Apr 12 13:29:57 2023, max compression
```

## Comparing `watchtower_browser_testing-0.2.4.tar` & `watchtower_browser_testing-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/
--rw-rw-rw-   0        0        0      310 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0    11517 2023-04-12 13:23:18.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-12 13:23:18.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 13:29:57.108620 watchtower_browser_testing-0.2.5/
+-rw-rw-rw-   0        0        0      310 2023-04-12 13:29:57.108620 watchtower_browser_testing-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 13:29:57.108620 watchtower_browser_testing-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:29:57.092985 watchtower_browser_testing-0.2.5/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0    11517 2023-04-12 13:23:18.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:29:57.108620 watchtower_browser_testing-0.2.5/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-12 13:29:56.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-12 13:29:56.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:29:56.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 13:29:56.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-12 13:29:56.000000 watchtower_browser_testing-0.2.5/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.2.4/setup.py` & `watchtower_browser_testing-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.4/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.2.5/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.4/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.2.5/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.4/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.2.5/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.2.5/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

