# Comparing `tmp/morphqs-0.1.24.tar.gz` & `tmp/morphqs-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphqs-0.1.24.tar", last modified: Wed Apr 12 21:46:23 2023, max compression
+gzip compressed data, was "morphqs-0.1.25.tar", last modified: Wed Apr 12 21:47:11 2023, max compression
```

## Comparing `morphqs-0.1.24.tar` & `morphqs-0.1.25.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:46:23.490286 morphqs-0.1.24/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.24/LICENSE.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-12 21:46:23.488754 morphqs-0.1.24/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.24/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:46:23.425132 morphqs-0.1.24/morphqs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      201 2023-04-07 16:34:53.000000 morphqs-0.1.24/morphqs/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:46:23.477653 morphqs-0.1.24/morphqs/components/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.24/morphqs/components/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.24/morphqs/components/ansible.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3479 2023-04-12 16:52:21.000000 morphqs-0.1.24/morphqs/components/integrations.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.24/morphqs/components/uchigheredmsp.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10348 2023-04-12 21:46:04.000000 morphqs-0.1.24/morphqs/components/usecasedeployment.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:46:23.485205 morphqs-0.1.24/morphqs/logging/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.24/morphqs/logging/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.24/morphqs/logging/loghandler.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.24/morphqs/morphclass.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:46:23.455239 morphqs-0.1.24/morphqs.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-12 21:46:23.000000 morphqs-0.1.24/morphqs.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-12 21:46:23.000000 morphqs-0.1.24/morphqs.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-12 21:46:23.000000 morphqs-0.1.24/morphqs.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-12 21:46:23.000000 morphqs-0.1.24/morphqs.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-12 21:46:23.000000 morphqs-0.1.24/morphqs.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-12 21:46:23.491167 morphqs-0.1.24/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-12 21:46:20.000000 morphqs-0.1.24/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:47:11.960582 morphqs-0.1.25/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1072 2023-03-29 01:49:10.000000 morphqs-0.1.25/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-12 21:47:11.959182 morphqs-0.1.25/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      206 2023-03-29 01:54:53.000000 morphqs-0.1.25/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:47:11.865300 morphqs-0.1.25/morphqs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      201 2023-04-07 16:34:53.000000 morphqs-0.1.25/morphqs/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:47:11.940229 morphqs-0.1.25/morphqs/components/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-29 02:36:46.000000 morphqs-0.1.25/morphqs/components/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1253 2023-04-07 14:03:43.000000 morphqs-0.1.25/morphqs/components/ansible.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3479 2023-04-12 16:52:21.000000 morphqs-0.1.25/morphqs/components/integrations.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6366 2023-04-05 12:30:10.000000 morphqs-0.1.25/morphqs/components/uchigheredmsp.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10308 2023-04-12 21:46:59.000000 morphqs-0.1.25/morphqs/components/usecasedeployment.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:47:11.954833 morphqs-0.1.25/morphqs/logging/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-28 19:26:20.000000 morphqs-0.1.25/morphqs/logging/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1959 2023-03-28 19:26:20.000000 morphqs-0.1.25/morphqs/logging/loghandler.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3034 2023-03-28 19:51:08.000000 morphqs-0.1.25/morphqs/morphclass.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 21:47:11.901981 morphqs-0.1.25/morphqs.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      925 2023-04-12 21:47:11.000000 morphqs-0.1.25/morphqs.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      456 2023-04-12 21:47:11.000000 morphqs-0.1.25/morphqs.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-12 21:47:11.000000 morphqs-0.1.25/morphqs.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-04-12 21:47:11.000000 morphqs-0.1.25/morphqs.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-04-12 21:47:11.000000 morphqs-0.1.25/morphqs.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-04-12 21:47:11.961616 morphqs-0.1.25/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1025 2023-04-12 21:47:10.000000 morphqs-0.1.25/setup.py
```

### Comparing `morphqs-0.1.24/LICENSE.txt` & `morphqs-0.1.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.24/PKG-INFO` & `morphqs-0.1.25/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.24
+Version: 0.1.25
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.24/morphqs/components/ansible.py` & `morphqs-0.1.25/morphqs/components/ansible.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.24/morphqs/components/integrations.py` & `morphqs-0.1.25/morphqs/components/integrations.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.24/morphqs/components/uchigheredmsp.py` & `morphqs-0.1.25/morphqs/components/uchigheredmsp.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.24/morphqs/components/usecasedeployment.py` & `morphqs-0.1.25/morphqs/components/usecasedeployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,29 +149,27 @@
     logger.info("Creating role: MultiTenantRole")
     resp = cl.post("/api/roles", data = json.dumps(payload)).json()
     if resp["success"] == True:
         logger.info("Successfully created role")
     else:
         logger.error("Failed to create role")
         logger.error(resp)
-        sys.exit(1)
     logger.info("Creating role: BaseTenantRole")
     payload = {"role": {
         "roleType": "account",
         "authority": "BaseTenantRole",
         "description": "Setup by the Installer - used for the MSP Use Case",
         "baseRoleId": role_id
     }}
     resp = cl.post("/api/roles", data = json.dumps(payload)).json()
     if resp["success"] == True:
         logger.info("Successfully created role")
     else:
         logger.error("Failed to create role")
         logger.error(resp)
-        sys.exit(1)
     
     
 
     
     
     
    # task_name = "Higher Education MSP Setup"
```

### Comparing `morphqs-0.1.24/morphqs/logging/loghandler.py` & `morphqs-0.1.25/morphqs/logging/loghandler.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.24/morphqs/morphclass.py` & `morphqs-0.1.25/morphqs/morphclass.py`

 * *Files identical despite different names*

### Comparing `morphqs-0.1.24/morphqs.egg-info/PKG-INFO` & `morphqs-0.1.25/morphqs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphqs
-Version: 0.1.24
+Version: 0.1.25
 Summary: Tool utilized to deploy some basic concepts for the Morpheus Data Platform
 Home-page: https://gitlab.com/jaredlutgen/morphqs
 Author: Jared Lutgen
 Author-email: jlutgen@morpheusdata.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `morphqs-0.1.24/setup.py` & `morphqs-0.1.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Jared Lutgen",
     author_email="jlutgen@morpheusdata.com",
     name='morphqs',
     license="MIT",
     description='Tool utilized to deploy some basic concepts for the Morpheus Data Platform',
-    version='v0.1.24',
+    version='v0.1.25',
     long_description=README,
     url='https://gitlab.com/jaredlutgen/morphqs',
     packages=setuptools.find_packages(),
     python_requires=">=3.5",
     install_requires=['requests'],
     classifiers=[
         # Trove classifiers
```

