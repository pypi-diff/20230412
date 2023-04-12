# Comparing `tmp/axterdb-1.2.tar.gz` & `tmp/axterdb-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axterdb-1.2.tar", last modified: Wed Apr 12 09:39:07 2023, max compression
+gzip compressed data, was "axterdb-1.2.1.tar", last modified: Wed Apr 12 11:27:56 2023, max compression
```

## Comparing `axterdb-1.2.tar` & `axterdb-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 09:39:07.206225 axterdb-1.2/
--rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.2/.gitignore
--rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.2/.readthedocs
--rw-rw-rw-   0        0        0     1794 2023-04-12 09:39:07.205226 axterdb-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 09:39:07.062222 axterdb-1.2/axterdb/
--rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.2/axterdb/__init__.py
--rw-rw-rw-   0        0        0    11776 2023-04-12 09:02:08.000000 axterdb-1.2/axterdb/client.py
--rw-rw-rw-   0        0        0     2279 2023-04-12 08:59:15.000000 axterdb-1.2/axterdb/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:39:07.089221 axterdb-1.2/axterdb.egg-info/
--rw-rw-rw-   0        0        0     1794 2023-04-12 09:39:06.000000 axterdb-1.2/axterdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-04-12 09:39:07.000000 axterdb-1.2/axterdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 09:39:06.000000 axterdb-1.2/axterdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 09:39:06.000000 axterdb-1.2/axterdb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 09:39:07.171235 axterdb-1.2/docs/
--rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.2/docs/Makefile
--rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.2/docs/clients.rst
--rw-rw-rw-   0        0        0     2003 2023-04-12 09:17:49.000000 axterdb-1.2/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-12 09:39:07.173226 axterdb-1.2/docs/images/
--rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.2/docs/images/axterdb_logo.ico
--rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.2/docs/images/axterdb_logo.png
--rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.2/docs/index.rst
--rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.2/docs/installing.rst
--rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.2/docs/make.bat
--rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.2/docs/quickstart.rst
--rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 09:39:07.204230 axterdb-1.2/examples/
--rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.2/examples/basic.py
--rw-rw-rw-   0        0        0     1741 2023-04-12 09:38:19.000000 axterdb-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 09:39:07.206225 axterdb-1.2/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:27:56.315995 axterdb-1.2.1/
+-rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.2.1/.gitignore
+-rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.2.1/.readthedocs
+-rw-rw-rw-   0        0        0     1796 2023-04-12 11:27:56.307967 axterdb-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 11:27:56.083231 axterdb-1.2.1/axterdb/
+-rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.2.1/axterdb/__init__.py
+-rw-rw-rw-   0        0        0    11778 2023-04-12 11:25:40.000000 axterdb-1.2.1/axterdb/client.py
+-rw-rw-rw-   0        0        0     2279 2023-04-12 08:59:15.000000 axterdb-1.2.1/axterdb/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:27:56.138209 axterdb-1.2.1/axterdb.egg-info/
+-rw-rw-rw-   0        0        0     1796 2023-04-12 11:27:55.000000 axterdb-1.2.1/axterdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-12 11:27:55.000000 axterdb-1.2.1/axterdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 11:27:55.000000 axterdb-1.2.1/axterdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-12 11:27:55.000000 axterdb-1.2.1/axterdb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 11:27:56.234073 axterdb-1.2.1/docs/
+-rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.2.1/docs/clients.rst
+-rw-rw-rw-   0        0        0     2003 2023-04-12 11:26:14.000000 axterdb-1.2.1/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-12 11:27:56.248693 axterdb-1.2.1/docs/images/
+-rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.2.1/docs/images/axterdb_logo.ico
+-rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.2.1/docs/images/axterdb_logo.png
+-rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.2.1/docs/index.rst
+-rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.2.1/docs/installing.rst
+-rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.2.1/docs/make.bat
+-rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.2.1/docs/quickstart.rst
+-rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.2.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 11:27:56.304969 axterdb-1.2.1/examples/
+-rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.2.1/examples/basic.py
+-rw-rw-rw-   0        0        0     1743 2023-04-12 11:26:07.000000 axterdb-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 11:27:56.316970 axterdb-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.2.1/setup.py
```

### Comparing `axterdb-1.2/.gitignore` & `axterdb-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/PKG-INFO` & `axterdb-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.2
+Version: 1.2.1
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.2/README.rst` & `axterdb-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/axterdb/client.py` & `axterdb-1.2.1/axterdb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,17 +214,17 @@
             Not connected to the database.
         InvalidColumn
             Invalid column provided.
         """
         if not self._connected:
             raise NotConnected()
         data = data
-        headers = self.headers
+        headers = self._headers
         headers["table"] = table
-        async with self._session.get(self.route(f"/database/{self.name}/insert"), headers=self.headers, json=data) as response:
+        async with self._session.get(self.route(f"/database/{self.name}/insert"), headers=self._headers, json=data) as response:
             if response.status == 200:
                 return True
             elif response.status == 422:
                 data = await response.json()
                 raise InvalidColumn(data["detail"].split(' ').pop(0))
             raise UnknownError(response.status)
             # TODO: Add errors from status codes.
```

### Comparing `axterdb-1.2/axterdb/errors.py` & `axterdb-1.2.1/axterdb/errors.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/axterdb.egg-info/PKG-INFO` & `axterdb-1.2.1/axterdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.2
+Version: 1.2.1
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.2/docs/Makefile` & `axterdb-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/docs/conf.py` & `axterdb-1.2.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 import os
 
 project = 'AxterDB'
 copyright = '2023, AxterDB'
 author = 'ItsNeil'
-release = '1.0'
+release = '1.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 sys.path.insert(0, os.path.abspath(".."))
 sys.path.append(os.path.abspath("extensions"))
```

### Comparing `axterdb-1.2/docs/images/axterdb_logo.ico` & `axterdb-1.2.1/docs/images/axterdb_logo.ico`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/docs/images/axterdb_logo.png` & `axterdb-1.2.1/docs/images/axterdb_logo.png`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/docs/index.rst` & `axterdb-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/docs/installing.rst` & `axterdb-1.2.1/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/docs/make.bat` & `axterdb-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/docs/quickstart.rst` & `axterdb-1.2.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/examples/basic.py` & `axterdb-1.2.1/examples/basic.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.2/pyproject.toml` & `axterdb-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=62.6,<66",
     "setuptools-scm>=6.2,<8",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axterdb"
-version = "1.2"
+version = "1.2.1"
 authors = [
     {name = "AxterDB Development"}
 ]
 description = "A Python wrapper for AxterDB"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

