# Comparing `tmp/morphqs-0.1.22.tar.gz` & `tmp/morphqs-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphqs-0.1.22.tar", last modified: Tue Apr 11 14:28:42 2023, max compression
+gzip compressed data, was "morphqs-0.1.23.tar", last modified: Wed Apr 12 16:53:34 2023, max compression
```

## Comparing `morphqs-0.1.22.tar` & `morphqs-0.1.23.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.148152 morphqs-0.1.22/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.22/LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-11 14:28:42.146829 morphqs-0.1.22/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.22/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.080416 morphqs-0.1.22/morphqs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      201 2023-04-07 16:34:53.000000 morphqs-0.1.22/morphqs/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.131799 morphqs-0.1.22/morphqs/components/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.22/morphqs/components/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.22/morphqs/components/ansible.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3444 2023-04-07 16:04:30.000000 morphqs-0.1.22/morphqs/components/integrations.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.22/morphqs/components/uchigheredmsp.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-04-07 16:15:46.000000 morphqs-0.1.22/morphqs/components/usecasedeployment.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.142191 morphqs-0.1.22/morphqs/logging/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.22/morphqs/logging/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.22/morphqs/logging/loghandler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.22/morphqs/morphclass.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-11 14:28:42.105519 morphqs-0.1.22/morphqs.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-11 14:28:41.000000 morphqs-0.1.22/morphqs.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-11 14:28:42.148900 morphqs-0.1.22/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-11 14:28:41.000000 morphqs-0.1.22/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 16:53:34.913651 morphqs-0.1.23/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.23/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-12 16:53:34.912350 morphqs-0.1.23/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.23/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 16:53:34.848194 morphqs-0.1.23/morphqs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      201 2023-04-07 16:34:53.000000 morphqs-0.1.23/morphqs/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 16:53:34.898579 morphqs-0.1.23/morphqs/components/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.23/morphqs/components/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.23/morphqs/components/ansible.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3479 2023-04-12 16:52:21.000000 morphqs-0.1.23/morphqs/components/integrations.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.23/morphqs/components/uchigheredmsp.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2023-04-07 16:15:46.000000 morphqs-0.1.23/morphqs/components/usecasedeployment.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 16:53:34.908004 morphqs-0.1.23/morphqs/logging/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.23/morphqs/logging/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.23/morphqs/logging/loghandler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.23/morphqs/morphclass.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 16:53:34.874547 morphqs-0.1.23/morphqs.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-12 16:53:34.000000 morphqs-0.1.23/morphqs.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-12 16:53:34.000000 morphqs-0.1.23/morphqs.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-12 16:53:34.000000 morphqs-0.1.23/morphqs.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-12 16:53:34.000000 morphqs-0.1.23/morphqs.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-12 16:53:34.000000 morphqs-0.1.23/morphqs.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-12 16:53:34.914409 morphqs-0.1.23/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-12 16:53:30.000000 morphqs-0.1.23/setup.py
```

### Comparing `morphqs-0.1.22/LICENSE.txt` & `morphqs-0.1.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.22/PKG-INFO` & `morphqs-0.1.23/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.22
+Version: 0.1.23
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.22/morphqs/components/ansible.py` & `morphqs-0.1.23/morphqs/components/ansible.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.22/morphqs/components/integrations.py` & `morphqs-0.1.23/morphqs/components/integrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..morphclass import RequestsApi
 import morphqs.logging.loghandler as loghandler
 import json
 import urllib
 import sys
+import time
 
 def add_integration(default_branch, repo_url, integration_name):
     """
     The add_integration function is used to create a new integration in Morpheus.
         It takes three arguments: 
             1) default_branch - the branch that will be checked out by default when cloning the repo (defaults to master)
             2) repo_url - The URL of the repository you want to integrate with Morpheus. This can be any valid git url, including SSH and HTTP(S). 
@@ -51,14 +52,15 @@
                                     "cacheEnabled": False
                                 },
                                 "name": integration_name, #"Morpheus Quickshots Base Repo",
                                 "serviceUrl": repo_url #"https://gitlab.com/jaredlutgen/morpheus_quickshots.git"
                             }}
         logger.debug(f"Creating integration {integration_name} with payload {root_int_payload}")
         cl.post("/api/integrations", data = json.dumps(root_int_payload)).json()
+        time.sleep(10)
         intid = cl.get(f"/api/integrations?name={integrationname}").json()
         try: 
             intid = intid["integrations"][0]["id"]
         except IndexError as e:
             intid = None
         coderepoId = cl.get(f"/api/options/codeRepositories?integrationId={intid}").json()
         logger.debug(coderepoId)
```

### Comparing `morphqs-0.1.22/morphqs/components/uchigheredmsp.py` & `morphqs-0.1.23/morphqs/components/uchigheredmsp.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.22/morphqs/components/usecasedeployment.py` & `morphqs-0.1.23/morphqs/components/usecasedeployment.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.22/morphqs/logging/loghandler.py` & `morphqs-0.1.23/morphqs/logging/loghandler.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.22/morphqs/morphclass.py` & `morphqs-0.1.23/morphqs/morphclass.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.22/morphqs.egg-info/PKG-INFO` & `morphqs-0.1.23/morphqs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.22
+Version: 0.1.23
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.22/setup.py` & `morphqs-0.1.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Jared Lutgen",
     author_email="jlutgen@morpheusdata.com",
     name='morphqs',
     license="MIT",
     description='Tool utilized to deploy some basic concepts for the Morpheus Data Platform',
-    version='v0.1.22',
+    version='v0.1.23',
     long_description=README,
     url='https://gitlab.com/jaredlutgen/morphqs',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['requests'],
     classifiers=[
         # Trove classifiers
```

