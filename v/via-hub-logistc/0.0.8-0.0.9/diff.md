# Comparing `tmp/via-hub-logistc-0.0.8.tar.gz` & `tmp/via-hub-logistc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "via-hub-logistc-0.0.8.tar", max compression
+gzip compressed data, was "via-hub-logistc-0.0.9.tar", max compression
```

## Comparing `via-hub-logistc-0.0.8.tar` & `via-hub-logistc-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      434 2023-03-04 01:39:19.331745 via-hub-logistc-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1568 2023-03-03 21:35:57.553317 via-hub-logistc-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-03-03 16:57:28.713969 via-hub-logistc-0.0.8/via_hub_logistc/__init__.py
--rw-r--r--   0        0        0      671 2023-03-04 01:33:48.330516 via-hub-logistc-0.0.8/via_hub_logistc/core/via_atlassian.py
--rw-r--r--   0        0        0     1788 2023-03-04 01:34:08.362573 via-hub-logistc-0.0.8/via_hub_logistc/core/via_azure.py
--rw-r--r--   0        0        0     1141 2023-03-04 01:10:40.466266 via-hub-logistc-0.0.8/via_hub_logistc/core/via_file.py
--rw-r--r--   0        0        0      409 2023-03-04 01:33:59.718219 via-hub-logistc-0.0.8/via_hub_logistc/core/via_scenario.py
--rw-r--r--   0        0        0      597 2023-03-04 01:09:25.003935 via-hub-logistc-0.0.8/via_hub_logistc/core/via_timer.py
--rw-r--r--   0        0        0     2865 2023-03-04 01:23:06.852797 via-hub-logistc-0.0.8/via_hub_logistc/core/via_zephry.py
--rw-r--r--   0        0        0     1143 2023-03-04 01:20:18.640682 via-hub-logistc-0.0.8/via_hub_logistc/model/zephry.py
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 via-hub-logistc-0.0.8/setup.py
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 via-hub-logistc-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-03-04 02:38:25.977047 via-hub-logistc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1568 2023-03-03 21:35:57.553317 via-hub-logistc-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-03 16:57:28.713969 via-hub-logistc-0.0.9/via_hub_logistc/__init__.py
+-rw-r--r--   0        0        0      671 2023-03-04 01:33:48.330516 via-hub-logistc-0.0.9/via_hub_logistc/core/via_atlassian.py
+-rw-r--r--   0        0        0     1788 2023-03-04 01:34:08.362573 via-hub-logistc-0.0.9/via_hub_logistc/core/via_azure.py
+-rw-r--r--   0        0        0     1141 2023-03-04 01:10:40.466266 via-hub-logistc-0.0.9/via_hub_logistc/core/via_file.py
+-rw-r--r--   0        0        0      409 2023-03-04 01:33:59.718219 via-hub-logistc-0.0.9/via_hub_logistc/core/via_scenario.py
+-rw-r--r--   0        0        0      597 2023-03-04 01:09:25.003935 via-hub-logistc-0.0.9/via_hub_logistc/core/via_timer.py
+-rw-r--r--   0        0        0     2892 2023-03-04 02:27:35.419563 via-hub-logistc-0.0.9/via_hub_logistc/core/via_zephry.py
+-rw-r--r--   0        0        0     1143 2023-03-04 01:20:18.640682 via-hub-logistc-0.0.9/via_hub_logistc/model/zephry.py
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 via-hub-logistc-0.0.9/setup.py
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 via-hub-logistc-0.0.9/PKG-INFO
```

### Comparing `via-hub-logistc-0.0.8/README.md` & `via-hub-logistc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-0.0.8/via_hub_logistc/core/via_atlassian.py` & `via-hub-logistc-0.0.9/via_hub_logistc/core/via_atlassian.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-0.0.8/via_hub_logistc/core/via_azure.py` & `via-hub-logistc-0.0.9/via_hub_logistc/core/via_azure.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-0.0.8/via_hub_logistc/core/via_file.py` & `via-hub-logistc-0.0.9/via_hub_logistc/core/via_file.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-0.0.8/via_hub_logistc/core/via_timer.py` & `via-hub-logistc-0.0.9/via_hub_logistc/core/via_timer.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-0.0.8/via_hub_logistc/core/via_zephry.py` & `via-hub-logistc-0.0.9/via_hub_logistc/core/via_zephry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import requests
 
 from base64 import b64encode
 
-from model.zephry import TestFolder, TestCycle
+from via_hub_logistc.model.zephry import TestFolder, TestCycle
 
 
 class TestRunner():
     def __init__(self, url, usr, pwd):
         self.url = url
         self.user = usr
         self.pwd = pwd
 
     ###Create new folder for test regression ###
     def regression_create_folder(self, date_run: str, projectKey: str):
         uri = self.url + "folder"
 
         headers = {
-            "Authorization": b64encode(f"{self.user}:{self.pwd}".encode('utf-8')).decode("ascii")
+            "Authorization": "Basic " + b64encode(f"{self.user}:{self.pwd}".encode('utf-8')).decode("ascii")
         }
 
         payload = TestFolder(
             projectKey, f"/ViaOps/{date_run}", "TEST_RUN").__dict__
 
         response = requests.request("POST", uri, json=payload, headers=headers)
```

### Comparing `via-hub-logistc-0.0.8/via_hub_logistc/model/zephry.py` & `via-hub-logistc-0.0.9/via_hub_logistc/model/zephry.py`

 * *Files identical despite different names*

### Comparing `via-hub-logistc-0.0.8/setup.py` & `via-hub-logistc-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['via_hub_logistc', 'via_hub_logistc.core', 'via_hub_logistc.model']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'via-hub-logistc',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'This project is intended to be a facilitator for new developments for test automation',
     'long_description': 'Introduction\n------------\n\nvia-hub-logistic is a library with testing utilities for robotframework that uses a set of python frameworks internally. The project is hosted on GitHub and downloads can be found on PyPI.\n\n\nKeyword Documentation\n---------------------\nSee `keyword documentation`_ for available keywords and more information\nabout the library in general.\n\n\nInstallation\n------------\n\nThe recommended installation method is using pip_::\n\n    pip install --upgrade via-hub-logistc\n\n\nTo install the last legacy via-hub-logistc version, use this command instead::\n\n    pip install via-hub-logistc==1.8.0\n\n\nUsage\n-----\n\nTo use via-hub-logistc in Robot Framework tests, the library needs to\nfirst be imported using the ``Library`` setting as any other library.\nThe library accepts some import time arguments, which are documented\nin the `keyword documentation`_ along with all the keywords provided\nby the library.\n\n\n.. code:: robotframework\n\n    *** Settings ***\n    Documentation     Simple example using via-hub-logistc.\n    Library           via-hub-logistc.Blob\n\n    *** Variables ***\n    ${URL}      http://localhost:7272\n    ${USER}     user\n    ${PWD}      password\n\n    *** Test Cases ***\n    Conect azure blob service\n        Connect azure blob   ${URL}   ${USER}    ${PWD}\n\n    *** Keywords ***\n    Connect azure blob\n        [Arguments]    ${url}    ${user}   ${pwd}\n        ${conn}=        connect     ${url}    ${user}   ${pwd}\n\n\n\nCommunity\n---------\n\nVersions\n--------\n\nHistory\n-------',
     'author': 'Jaderson Macedo',
     'author_email': 'jaderson.macedo@viavarejo.com.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `via-hub-logistc-0.0.8/PKG-INFO` & `via-hub-logistc-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: via-hub-logistc
-Version: 0.0.8
+Version: 0.0.9
 Summary: This project is intended to be a facilitator for new developments for test automation
 Author: Jaderson Macedo
 Author-email: jaderson.macedo@viavarejo.com.br
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

