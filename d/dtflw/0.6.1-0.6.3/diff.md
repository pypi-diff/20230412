# Comparing `tmp/dtflw-0.6.1.tar.gz` & `tmp/dtflw-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtflw-0.6.1.tar", last modified: Mon Mar 27 10:34:11 2023, max compression
+gzip compressed data, was "dtflw-0.6.3.tar", last modified: Wed Apr 12 17:47:57 2023, max compression
```

## Comparing `dtflw-0.6.1.tar` & `dtflw-0.6.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:34:11.980608 dtflw-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-27 10:33:57.000000 dtflw-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-27 10:34:11.980608 dtflw-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-27 10:33:57.000000 dtflw-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-27 10:33:57.000000 dtflw-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-27 10:34:11.980608 dtflw-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-27 10:33:57.000000 dtflw-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:34:11.976608 dtflw-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:34:11.976608 dtflw-0.6.1/src/dtflw/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/com.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/flow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/input_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/lazy_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/output_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:34:11.980608 dtflw-0.6.1/src/dtflw/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/storage/dbfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-27 10:33:57.000000 dtflw-0.6.1/src/dtflw/tables_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:34:11.980608 dtflw-0.6.1/src/dtflw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-27 10:34:11.000000 dtflw-0.6.1/src/dtflw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-27 10:34:11.000000 dtflw-0.6.1/src/dtflw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:34:11.000000 dtflw-0.6.1/src/dtflw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 10:34:11.000000 dtflw-0.6.1/src/dtflw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 10:34:11.000000 dtflw-0.6.1/src/dtflw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:34:11.980608 dtflw-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_com.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_input_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_lazy_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_output_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_pipeline_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-27 10:33:57.000000 dtflw-0.6.1/tests/test_tables_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-12 17:47:47.000000 dtflw-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-12 17:47:57.637840 dtflw-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-04-12 17:47:47.000000 dtflw-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-12 17:47:47.000000 dtflw-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 17:47:57.641840 dtflw-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-12 17:47:47.000000 dtflw-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.633840 dtflw-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/src/dtflw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/com.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/flow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/input_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/lazy_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/output_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/src/dtflw/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/dbfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-12 17:47:47.000000 dtflw-0.6.3/src/dtflw/tables_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/src/dtflw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 17:47:57.000000 dtflw-0.6.3/src/dtflw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:47:57.637840 dtflw-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_com.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_input_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_lazy_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_output_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_pipeline_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-12 17:47:47.000000 dtflw-0.6.3/tests/test_tables_repository.py
```

### Comparing `dtflw-0.6.1/LICENSE` & `dtflw-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/PKG-INFO` & `dtflw-0.6.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtflw
-Version: 0.6.1
+Version: 0.6.3
 Summary: dtflw is a Python framework for building modular data pipelines based on Databricks dbutils.notebook API.
 Home-page: https://github.com/SoleyIo/dtflw
 Author: Soley GmbH
 Author-email: codeofconduct@soley.io
 Project-URL: Bug Reports, https://github.com/SoleyIo/dtflw/issues
 Project-URL: Source, https://github.com/SoleyIo/dtflw
 Keywords: databricks,data pipelines,etl,data engineering
@@ -13,10 +13,11 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: local
 License-File: LICENSE
 
 See [the home page](https://github.com/SoleyIo/dtflw/blob/main/README.md) of the project for details.
```

### Comparing `dtflw-0.6.1/README.md` & `dtflw-0.6.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,17 @@
 - To start using on Databricks: see [Installing](#installing) below. 
 
 ### Installing
 
 `dtflw` is available on [PyPi](https://pypi.org/project/dtflw/).
 See [how to get it on Databricks](https://docs.databricks.com/libraries/index.html#libraries). 
 
+To use `dtflw` on the local environment you need to have `pyspark` installed. You can either install it manually
+or you can run `pip install dtflw[local]` to install `pyspark` as an extra dependency.
+
 ## Changes
 
 Please, refer to [the log of changes](CHANGES.md). Here we record all notable changes made to the codebase in every version.
 
 ## Built With
 
 `dtflw` is implemented using [dbutils](https://docs.databricks.com/dev-tools/databricks-utils.html).
```

### Comparing `dtflw-0.6.1/setup.py` & `dtflw-0.6.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="dtflw",
-    version="0.6.1",
+    version="0.6.3",
 
     description="dtflw is a Python framework for building modular data pipelines based on Databricks dbutils.notebook API.",
     long_description="See [the home page](https://github.com/SoleyIo/dtflw/blob/main/README.md) of the project for details.",
     long_description_content_type="text/markdown",
 
     url="https://github.com/SoleyIo/dtflw",
 
@@ -29,16 +29,19 @@
     package_dir={"": "src"},
     packages=find_packages(where="src"),
 
     python_requires=">=3.8",
 
     install_requires=[
         "ddt>=1.5.0",
-        "databricks-connect",
         "setuptools"
     ],
 
+    extras_require = {
+        "local": ["pyspark"]
+    },
+
     project_urls={
         "Bug Reports": "https://github.com/SoleyIo/dtflw/issues",
         "Source": "https://github.com/SoleyIo/dtflw"
     },
 )
```

### Comparing `dtflw-0.6.1/src/dtflw/__init__.py` & `dtflw-0.6.3/src/dtflw/__init__.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/arguments.py` & `dtflw-0.6.3/src/dtflw/arguments.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/assertions.py` & `dtflw-0.6.3/src/dtflw/assertions.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/com.py` & `dtflw-0.6.3/src/dtflw/com.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/databricks.py` & `dtflw-0.6.3/src/dtflw/databricks.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/display.py` & `dtflw-0.6.3/src/dtflw/display.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/flow.py` & `dtflw-0.6.3/src/dtflw/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,23 +48,22 @@
         path: str
             Path to a notebook.
         """
         new_nb = LazyNotebook(path, self.__ctx)
 
         # Attach plugin actions to a notebook.
         for plugin in self.__nb_plugins.values():
-            
-            p = partial(plugin.act, new_nb, self)
             setattr(
                 new_nb,
                 plugin.action_name,
-                types.MethodType(
-                    partial(plugin.act, new_nb),
-                    new_nb
-                ))
+                partial(
+                    types.MethodType(plugin.act, new_nb), 
+                    self
+                )
+            )
 
         return new_nb
 
     def show(self):
         """
         Prints the current state.
         """
```

### Comparing `dtflw-0.6.1/src/dtflw/flow_context.py` & `dtflw-0.6.3/src/dtflw/flow_context.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/input_table.py` & `dtflw-0.6.3/src/dtflw/input_table.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/lazy_notebook.py` & `dtflw-0.6.3/src/dtflw/lazy_notebook.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/logger.py` & `dtflw-0.6.3/src/dtflw/logger.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/output_table.py` & `dtflw-0.6.3/src/dtflw/output_table.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/pipeline.py` & `dtflw-0.6.3/src/dtflw/pipeline.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/plugin.py` & `dtflw-0.6.3/src/dtflw/plugin.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/storage/azure.py` & `dtflw-0.6.3/src/dtflw/storage/azure.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/storage/dbfs.py` & `dtflw-0.6.3/src/dtflw/storage/dbfs.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/storage/fs.py` & `dtflw-0.6.3/src/dtflw/storage/fs.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw/tables_repo.py` & `dtflw-0.6.3/src/dtflw/tables_repo.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/src/dtflw.egg-info/PKG-INFO` & `dtflw-0.6.3/src/dtflw.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtflw
-Version: 0.6.1
+Version: 0.6.3
 Summary: dtflw is a Python framework for building modular data pipelines based on Databricks dbutils.notebook API.
 Home-page: https://github.com/SoleyIo/dtflw
 Author: Soley GmbH
 Author-email: codeofconduct@soley.io
 Project-URL: Bug Reports, https://github.com/SoleyIo/dtflw/issues
 Project-URL: Source, https://github.com/SoleyIo/dtflw
 Keywords: databricks,data pipelines,etl,data engineering
@@ -13,10 +13,11 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: local
 License-File: LICENSE
 
 See [the home page](https://github.com/SoleyIo/dtflw/blob/main/README.md) of the project for details.
```

### Comparing `dtflw-0.6.1/src/dtflw.egg-info/SOURCES.txt` & `dtflw-0.6.3/src/dtflw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_arguments.py` & `dtflw-0.6.3/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_assertions.py` & `dtflw-0.6.3/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_com.py` & `dtflw-0.6.3/tests/test_com.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_databricks.py` & `dtflw-0.6.3/tests/test_databricks.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_flow.py` & `dtflw-0.6.3/tests/test_flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,42 +13,70 @@
     def action_name(self):
         return "do_new_stuff"
 
     def act(self, flow: Flow, name):
         """
         Greets.
         """
+        assert isinstance(flow, Flow)
+
         return f"Hello: {name}"
 
 
 class TestNotebookPlugin(NotebookPluginBase):
 
     @property
     def action_name(self):
         return "get_arg_value"
 
     def act(self, notebook: LazyNotebook, flow: Flow, arg_name: str):
         """
         Returns arg name.
         """
+        assert isinstance(notebook, LazyNotebook)
+        assert isinstance(flow, Flow)
+
         return notebook.get_args()[arg_name]
 
+
 class TestNotebookPlugin2(NotebookPluginBase):
 
     @property
     def action_name(self):
         return "get_args_count"
 
-    def act(self, notebook: LazyNotebook, flow: Flow, arg_name: str):
+    def act(self, notebook: LazyNotebook, flow: Flow):
         """
-        Returns arg name.
+        Returns number of arguments of the notebook.
         """
+        assert isinstance(notebook, LazyNotebook)
+        assert isinstance(flow, Flow)
+
         return len(notebook.get_args())
 
 
+class TestNotebookPluginFlowCtxTablesCount(NotebookPluginBase):
+
+    @property
+    def action_name(self):
+        return "get_tables_count"
+
+    def act(self, notebook: LazyNotebook, flow: Flow):
+        """
+        Returns count of tables in flow.ctx.tables_repo.
+        """
+        assert isinstance(notebook, LazyNotebook)
+        assert isinstance(flow, Flow)
+
+        return self.plugin_len_method(flow.ctx.tables_repo.tables)
+
+    def plugin_len_method(self, lst: list):
+        return len(lst)
+
+
 class FlowTestCase(unittest.TestCase):
 
     def test_install_flow_plugin(self):
 
         # Arrange
         ctx = FlowContext(None, None, None, DefaultLogger())
         flow = Flow(ctx)
@@ -129,24 +157,41 @@
         flow = Flow(ctx)
 
         flow.install(nb_plg1)
         flow.install(nb_plg2)
 
         # Act
         expected1 = "foo"
-        expected2 = 1
+        expected2 = 2
 
         actual1 = (
             flow.notebook("import_data")
                 .args({"a": expected1})
                 .get_arg_value("a")
         )
 
         actual2 = (
             flow.notebook("import_data")
-                .args({"a": expected2})
-                .get_args_count("a")
+                .args({"a": "123", "b": "321"})
+                .get_args_count()
         )
 
         # Assert
         self.assertEqual(expected1, actual1)
         self.assertEqual(expected2, actual2)
+
+    def test_insall_notebook_plugins_with_use_of_flow_param(self):
+        # Arrange
+        nb_plg = TestNotebookPluginFlowCtxTablesCount()
+        ctx = FlowContext(None, None, None, DefaultLogger())
+        flow = Flow(ctx)
+
+        flow.install(nb_plg)
+
+        # Act
+        actual = (
+            flow.notebook("import_data")
+                .get_tables_count()
+        )
+
+        # Assert
+        self.assertEqual(0, actual)
```

### Comparing `dtflw-0.6.1/tests/test_input_table.py` & `dtflw-0.6.3/tests/test_input_table.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_lazy_notebook.py` & `dtflw-0.6.3/tests/test_lazy_notebook.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_logger.py` & `dtflw-0.6.3/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_output_table.py` & `dtflw-0.6.3/tests/test_output_table.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_pipeline_state.py` & `dtflw-0.6.3/tests/test_pipeline_state.py`

 * *Files identical despite different names*

### Comparing `dtflw-0.6.1/tests/test_tables_repository.py` & `dtflw-0.6.3/tests/test_tables_repository.py`

 * *Files identical despite different names*

