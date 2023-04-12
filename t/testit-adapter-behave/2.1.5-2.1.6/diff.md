# Comparing `tmp/testit-adapter-behave-2.1.5.tar.gz` & `tmp/testit-adapter-behave-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-behave-2.1.5.tar", last modified: Tue Apr  4 07:02:20 2023, max compression
+gzip compressed data, was "testit-adapter-behave-2.1.6.tar", last modified: Wed Apr 12 09:36:08 2023, max compression
```

## Comparing `testit-adapter-behave-2.1.5.tar` & `testit-adapter-behave-2.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:20.694879 testit-adapter-behave-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-04 07:02:20.694879 testit-adapter-behave-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:02:20.694879 testit-adapter-behave-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:20.694879 testit-adapter-behave-2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:20.694879 testit-adapter-behave-2.1.5/src/testit_adapter_behave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:20.694879 testit-adapter-behave-2.1.5/src/testit_adapter_behave/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/models/label.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/models/option.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/models/test_result_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/models/url_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/scenario_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/tags_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-04 07:02:08.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:20.694879 testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-04 07:02:20.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-04 07:02:20.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:02:20.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-04 07:02:20.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 07:02:20.000000 testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:08.685394 testit-adapter-behave-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-12 09:36:08.685394 testit-adapter-behave-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:36:08.685394 testit-adapter-behave-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:08.681394 testit-adapter-behave-2.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:08.681394 testit-adapter-behave-2.1.6/src/testit_adapter_behave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:08.685394 testit-adapter-behave-2.1.6/src/testit_adapter_behave/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/models/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/models/test_result_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/models/url_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/scenario_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/tags_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-12 09:35:58.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:08.685394 testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-12 09:36:08.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-12 09:36:08.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:36:08.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 09:36:08.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 09:36:08.000000 testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/top_level.txt
```

### Comparing `testit-adapter-behave-2.1.5/PKG-INFO` & `testit-adapter-behave-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 2.1.5
+Version: 2.1.6
 Summary: Behave adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-behave-2.1.5/README.md` & `testit-adapter-behave-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.5/setup.py` & `testit-adapter-behave-2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-behave',
-    version='2.1.5',
+    version='2.1.6',
     description='Behave adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_behave'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'behave',
-        'testit-python-commons==2.1.5',
+        'testit-python-commons==2.1.6',
         'attrs'],
 )
```

### Comparing `testit-adapter-behave-2.1.5/src/testit_adapter_behave/formatter.py` & `testit-adapter-behave-2.1.6/src/testit_adapter_behave/formatter.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.5/src/testit_adapter_behave/listener.py` & `testit-adapter-behave-2.1.6/src/testit_adapter_behave/listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 
     def get_step_parameters(self, match):
         scope = self.get_scope()
 
         executable_step = get_test_result_step_model()
 
         for argument in match.arguments:
-            executable_step['description'] += f'{argument.name} = {argument.original} '
-            executable_step['parameters'][argument.name] = argument.original
+            name = argument.name if argument.name else 'param' + str(match.arguments.index(argument))
+            executable_step['description'] += f'{name} = {argument.original} '
+            executable_step['parameters'][name] = argument.original
 
         self.__executable_test[scope].append(executable_step)
 
     def get_step_result(self, result):
         scope = self.get_scope()
         outcome = parse_status(result.status)
```

### Comparing `testit-adapter-behave-2.1.5/src/testit_adapter_behave/scenario_parser.py` & `testit-adapter-behave-2.1.6/src/testit_adapter_behave/scenario_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 def get_scenario_namespace(scenario):
     return scenario.feature.filename
 
 
 def get_scenario_parameters(scenario):
     row = scenario._row
 
-    return {name: value for name, value in zip(row.headings, row.cells)} if row else None
+    return {name: value for name, value in zip(row.headings, row.cells)} if row else {}
 
 
 def get_scenario_status(scenario):
     for step in scenario.all_steps:
         if get_step_status(step) != 'passed':
             return get_step_status(step)
     return OutcomeType.PASSED
```

### Comparing `testit-adapter-behave-2.1.5/src/testit_adapter_behave/tags_parser.py` & `testit-adapter-behave-2.1.6/src/testit_adapter_behave/tags_parser.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.5/src/testit_adapter_behave/utils.py` & `testit-adapter-behave-2.1.6/src/testit_adapter_behave/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/PKG-INFO` & `testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 2.1.5
+Version: 2.1.6
 Summary: Behave adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-behave-2.1.5/src/testit_adapter_behave.egg-info/SOURCES.txt` & `testit-adapter-behave-2.1.6/src/testit_adapter_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

