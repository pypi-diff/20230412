# Comparing `tmp/watchtower_browser_testing-0.2.7.tar.gz` & `tmp/watchtower_browser_testing-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.2.7.tar", last modified: Wed Apr 12 13:37:21 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.2.9.tar", last modified: Wed Apr 12 13:40:30 2023, max compression
```

## Comparing `watchtower_browser_testing-0.2.7.tar` & `watchtower_browser_testing-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 13:37:21.465509 watchtower_browser_testing-0.2.7/
--rw-rw-rw-   0        0        0      310 2023-04-12 13:37:21.465509 watchtower_browser_testing-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 13:37:21.465509 watchtower_browser_testing-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:37:21.450165 watchtower_browser_testing-0.2.7/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0    11527 2023-04-12 13:37:02.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-12 13:37:11.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 13:37:21.464982 watchtower_browser_testing-0.2.7/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-12 13:37:21.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-04-12 13:37:21.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 13:37:21.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 13:37:21.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-12 13:37:21.000000 watchtower_browser_testing-0.2.7/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 13:40:30.564026 watchtower_browser_testing-0.2.9/
+-rw-rw-rw-   0        0        0      310 2023-04-12 13:40:30.564026 watchtower_browser_testing-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 13:40:30.564026 watchtower_browser_testing-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:40:30.548401 watchtower_browser_testing-0.2.9/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0    11551 2023-04-12 13:40:18.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-12 13:40:18.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:40:30.548401 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-12 13:40:30.000000 watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.2.7/setup.py` & `watchtower_browser_testing-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.7/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.2.9/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.7/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.2.9/watchtower_browser_testing/testsuite.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,20 +227,21 @@
         return self.__class__.__name__
 
     @classmethod
     def scen_methods(cls):
 
         return [x for x in dir(cls) if x.startswith(config.SCENARIO_METHOD_PREFIX)]
 
-    def md_description(self):
+    @classmethod
+    def md_description(cls):
 
         md = markdown.parse(self.__doc__ or '')
 
-        for scenario_method in self.scen_methods():
-            md.children.extend(markdown.parse(getattr(self, scenario_method).__doc__ or '').children)
+        for scenario_method in cls.scen_methods():
+            md.children.extend(markdown.parse(getattr(cls, scenario_method).__doc__ or '').children)
 
         return md
 
 
 class MeasurementPlan(object):
 
     def __init__(self,
@@ -334,13 +335,13 @@
     def md_description(self):
 
         tests = self.get_tests()
 
         md = markdown.parse(self.__doc__ or '')
 
         for test in tests:
-            md.children.extend(test.md_description().children)
+            md.children.extend(test['class'].md_description().children)
 
         return md
```

### Comparing `watchtower_browser_testing-0.2.7/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.2.9/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.7/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.2.9/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

