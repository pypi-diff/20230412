# Comparing `tmp/testit-python-commons-2.1.5.tar.gz` & `tmp/testit-python-commons-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-python-commons-2.1.5.tar", last modified: Tue Apr  4 07:02:47 2023, max compression
+gzip compressed data, was "testit-python-commons-2.1.6.tar", last modified: Wed Apr 12 09:36:34 2023, max compression
```

## Comparing `testit-python-commons-2.1.5.tar` & `testit-python-commons-2.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:47.499274 testit-python-commons-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 07:02:47.499274 testit-python-commons-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:02:47.499274 testit-python-commons-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:47.495274 testit-python-commons-2.1.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:47.495274 testit-python-commons-2.1.5/src/testit_python_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/app_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:47.499274 testit-python-commons-2.1.5/src/testit_python_commons/client/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/client/client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/client/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/dynamic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:47.499274 testit-python-commons-2.1.5/src/testit_python_commons/models/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/models/adapter_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/models/link_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/models/outcome_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:47.499274 testit-python-commons-2.1.5/src/testit_python_commons/services/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/services/adapter_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/services/adapter_manager_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/services/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-04 07:02:08.000000 testit-python-commons-2.1.5/src/testit_python_commons/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:02:47.499274 testit-python-commons-2.1.5/src/testit_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-04 07:02:47.000000 testit-python-commons-2.1.5/src/testit_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-04 07:02:47.000000 testit-python-commons-2.1.5/src/testit_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:02:47.000000 testit-python-commons-2.1.5/src/testit_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-04 07:02:47.000000 testit-python-commons-2.1.5/src/testit_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-04 07:02:47.000000 testit-python-commons-2.1.5/src/testit_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.529741 testit-python-commons-2.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.529741 testit-python-commons-2.1.6/src/testit_python_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/app_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/src/testit_python_commons/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/client/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/dynamic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/src/testit_python_commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/adapter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/models/outcome_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.533742 testit-python-commons-2.1.6/src/testit_python_commons/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-12 09:35:58.000000 testit-python-commons-2.1.6/src/testit_python_commons/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:36:34.529741 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-12 09:36:34.000000 testit-python-commons-2.1.6/src/testit_python_commons.egg-info/top_level.txt
```

### Comparing `testit-python-commons-2.1.5/PKG-INFO` & `testit-python-commons-2.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.5/setup.py` & `testit-python-commons-2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-python-commons',
-    version='2.1.5',
+    version='2.1.6',
     description='Python commons for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit-python-commons-2.1.5/src/testit.py` & `testit-python-commons-2.1.6/src/testit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from testit_python_commons.decorators import (
+    className,
     description,
     displayName,
-    nameSpace,
-    className,
     externalID,
     externalId,
     labels,
     link,
     links,
+    nameSpace,
     title,
     workItemID,
     workItemIds
 )
 from testit_python_commons.dynamic_methods import (
     addAttachments,
     addLink,
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/app_properties.py` & `testit-python-commons-2.1.6/src/testit_python_commons/app_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,16 @@
         if f'{cls.__env_prefix}_ADAPTER_MODE' in os.environ.keys():
             env_properties['adaptermode'] = os.environ.get(f'{cls.__env_prefix}_ADAPTER_MODE')
 
         if f'{cls.__env_prefix}_CERT_VALIDATION' in os.environ.keys():
             env_properties['certvalidation'] = os.environ.get(f'{cls.__env_prefix}_CERT_VALIDATION')
 
         if f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES' in os.environ.keys():
-            env_properties['automaticcreationtestcases'] = os.environ.get(f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')
+            env_properties['automaticcreationtestcases'] = os.environ.get(
+                f'{cls.__env_prefix}_AUTOMATIC_CREATION_TEST_CASES')
 
         return env_properties
 
     @staticmethod
     def __check_properties(properties: dict):
         adapter_mode = properties.get('adaptermode')
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/client/api_client.py` & `testit-python-commons-2.1.6/src/testit_python_commons/client/api_client.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/client/client_configuration.py` & `testit-python-commons-2.1.6/src/testit_python_commons/client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/client/converter.py` & `testit-python-commons-2.1.6/src/testit_python_commons/client/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from testit_api_client.models import (
-    AutoTestStepModel,
-    AvailableTestResultOutcome,
     AttachmentPutModelAutoTestStepResultsModel,
     AutoTestPostModel,
     AutoTestPutModel,
     AutoTestResultsForTestRunModel,
+    AutoTestStepModel,
+    AvailableTestResultOutcome,
     LinkPostModel,
     LinkPutModel,
     LinkType,
     TestRunV2PostShortModel
 )
+
 from testit_python_commons.services.logger import adapter_logger
 
 
 class Converter:
     @classmethod
     @adapter_logger
     def test_run_to_test_run_short_model(cls, project_id, name):
@@ -263,16 +264,15 @@
             outcome: str,
             description: str = None,
             duration: str = None,
             parameters: list = None,
             attachments: list = None,
             started_on: str = None,
             completed_on: str = None,
-            step_results: list = None
-            ):
+            step_results: list = None):
         return AttachmentPutModelAutoTestStepResultsModel(
             title=title,
             outcome=AvailableTestResultOutcome(outcome),
             description=description,
             duration=duration,
             parameters=parameters,
             attachments=attachments,
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/decorators.py` & `testit-python-commons-2.1.6/src/testit_python_commons/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import types
 from functools import wraps
 
 from testit_python_commons.services.logger import adapter_logger
 from testit_python_commons.services.utils import Utils
 
 
@@ -144,13 +145,13 @@
                     function.test_links.append(
                         {'url': link['url'],
                          'title': link['title'] if 'title' in link else None,
                          'type': link['type'] if 'type' in link else None,
                          'description': link['description'] if 'description' in link else None}
                     )
                 else:
-                    print(f'Link ({link}) can\'t be processed!')
+                    logging.warning(f'Link ({link}) can\'t be processed!')
         else:
-            print(f'Links for {function.__name__} can\'t be processed!\nPlease, set "url" or "links"!')
+            logging.warning(f'Links for {function.__name__} can\'t be processed!\nPlease, set "url" or "links"!')
         return inner(function)
 
     return outer
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/dynamic_methods.py` & `testit-python-commons-2.1.6/src/testit_python_commons/dynamic_methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from testit_python_commons.services import TmsPluginManager
 from testit_python_commons.services.logger import adapter_logger
 from testit_python_commons.services.utils import Utils
 from testit_python_commons.step import Step
 
 
 @Utils.deprecated('Use "addLinks" instead.')
@@ -35,17 +37,17 @@
             )
         elif links and (isinstance(links, list) or isinstance(links, tuple)):
             for link in links:
                 if isinstance(link, dict) and 'url' in link:
                     TmsPluginManager.get_plugin_manager().hook \
                         .add_link(link=link)
                 else:
-                    print(f'Link ({link}) can\'t be processed!')
+                    logging.warning(f'Link ({link}) can\'t be processed!')
         else:
-            print("Links can't be processed!\nPlease, set 'url' or 'links'!")
+            logging.warning("Links can't be processed!\nPlease, set 'url' or 'links'!")
 
 
 @Utils.deprecated('Use "addMessage" instead.')
 @adapter_logger
 def message(test_message: str):
     if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_message'):
         TmsPluginManager.get_plugin_manager().hook \
@@ -79,15 +81,15 @@
                 name)
         else:
             if isinstance(data, str):
                 Step.add_attachments([data])
             elif isinstance(data, tuple) or isinstance(data, list):
                 Step.add_attachments(data)
             else:
-                print(f'File ({data}) not found!')
+                logging.warning(f'File ({data}) not found!')
     else:
         if is_text and hasattr(TmsPluginManager.get_plugin_manager().hook, 'create_attachment'):
             Step.create_attachment(str(data), name)
             TmsPluginManager.get_plugin_manager().hook \
                 .create_attachment(
                 body=str(data),
                 name=name)
@@ -95,8 +97,8 @@
             if isinstance(data, str):
                 TmsPluginManager.get_plugin_manager().hook \
                     .add_attachments(attach_paths=[data])
             elif isinstance(data, tuple) or isinstance(data, list):
                 TmsPluginManager.get_plugin_manager().hook \
                     .add_attachments(attach_paths=data)
             else:
-                print(f'({data}) is not path!')
+                logging.warning(f'({data}) is not path!')
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/services/adapter_manager.py` & `testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import uuid
 
 from testit_python_commons.client.api_client import ApiClientWorker
 from testit_python_commons.client.client_configuration import ClientConfiguration
-from testit_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
 from testit_python_commons.models.adapter_mode import AdapterMode
+from testit_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
 from testit_python_commons.services.logger import adapter_logger
 
 
 class AdapterManager:
     def __init__(
             self,
             adapter_configuration: AdapterManagerConfiguration,
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/services/adapter_manager_configuration.py` & `testit-python-commons-2.1.6/src/testit_python_commons/services/adapter_manager_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/services/logger.py` & `testit-python-commons-2.1.6/src/testit_python_commons/services/logger.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-
 from functools import wraps
 
 from testit_python_commons.services.plugin_manager import TmsPluginManager
 
 
 def adapter_logger(function):
     @wraps(function)
@@ -27,14 +26,15 @@
             message += f' with result: {result}'
 
         logger.debug(message)
 
         return result
     return wrapper
 
+
 def get_function_parameters(function, *args, **kwargs):
     parameters = {}
     args_default_values = inspect.getfullargspec(function).defaults
 
     if args or args_default_values:
         all_keys = inspect.getfullargspec(function).args
         all_args = list(args)
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/services/plugin_manager.py` & `testit-python-commons-2.1.6/src/testit_python_commons/services/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/services/utils.py` & `testit-python-commons-2.1.6/src/testit_python_commons/services/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import hashlib
+import inspect
 import logging
 import re
 import warnings
-import inspect
 
 from testit_python_commons.services.logger import adapter_logger
 
 
 class Utils:
     @staticmethod
     def uuid_check(uuid: str):
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons/step.py` & `testit-python-commons-2.1.6/src/testit_python_commons/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import wraps
 
 from testit_python_commons.services import (
     TmsPluginManager,
     Utils
 )
 
+
 class Step:
     step_stack = []
     steps_data = []
     steps_data_results = []
     attachments = []
 
     def __init__(self, *args, **kwargs):
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons.egg-info/PKG-INFO` & `testit-python-commons-2.1.6/src/testit_python_commons.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.5/src/testit_python_commons.egg-info/SOURCES.txt` & `testit-python-commons-2.1.6/src/testit_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

