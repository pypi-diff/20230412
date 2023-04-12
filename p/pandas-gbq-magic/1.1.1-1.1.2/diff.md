# Comparing `tmp/pandas_gbq_magic-1.1.1.tar.gz` & `tmp/pandas_gbq_magic-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_gbq_magic-1.1.1.tar", last modified: Mon Apr  3 19:07:15 2023, max compression
+gzip compressed data, was "pandas_gbq_magic-1.1.2.tar", last modified: Wed Apr 12 04:18:07 2023, max compression
```

## Comparing `pandas_gbq_magic-1.1.1.tar` & `pandas_gbq_magic-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 19:07:15.351776 pandas_gbq_magic-1.1.1/
--rw-rw-rw-   0        0        0     1084 2023-04-03 17:31:18.000000 pandas_gbq_magic-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2197 2023-04-03 19:07:15.350775 pandas_gbq_magic-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1656 2023-04-03 18:48:49.000000 pandas_gbq_magic-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 19:07:15.336438 pandas_gbq_magic-1.1.1/pandas_gbq_magic/
--rw-rw-rw-   0        0        0        0 2023-04-03 19:06:22.000000 pandas_gbq_magic-1.1.1/pandas_gbq_magic/__init__.py
--rw-rw-rw-   0        0        0     2523 2023-04-03 17:28:18.000000 pandas_gbq_magic-1.1.1/pandas_gbq_magic/magic.py
-drwxrwxrwx   0        0        0        0 2023-04-03 19:07:15.350775 pandas_gbq_magic-1.1.1/pandas_gbq_magic.egg-info/
--rw-rw-rw-   0        0        0     2197 2023-04-03 19:07:15.000000 pandas_gbq_magic-1.1.1/pandas_gbq_magic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-04-03 19:07:15.000000 pandas_gbq_magic-1.1.1/pandas_gbq_magic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 19:07:15.000000 pandas_gbq_magic-1.1.1/pandas_gbq_magic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-03 19:07:15.000000 pandas_gbq_magic-1.1.1/pandas_gbq_magic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 19:07:15.351776 pandas_gbq_magic-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      971 2023-04-03 19:06:48.000000 pandas_gbq_magic-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 04:18:07.649158 pandas_gbq_magic-1.1.2/
+-rw-rw-rw-   0        0        0     1084 2023-04-03 17:31:18.000000 pandas_gbq_magic-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2345 2023-04-12 04:18:07.648159 pandas_gbq_magic-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1806 2023-04-12 04:13:42.000000 pandas_gbq_magic-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 04:18:07.636129 pandas_gbq_magic-1.1.2/pandas_gbq_magic/
+-rw-rw-rw-   0        0        0        0 2023-04-03 19:06:22.000000 pandas_gbq_magic-1.1.2/pandas_gbq_magic/__init__.py
+-rw-rw-rw-   0        0        0     2523 2023-04-03 17:28:18.000000 pandas_gbq_magic-1.1.2/pandas_gbq_magic/magic.py
+drwxrwxrwx   0        0        0        0 2023-04-12 04:18:07.648159 pandas_gbq_magic-1.1.2/pandas_gbq_magic.egg-info/
+-rw-rw-rw-   0        0        0     2345 2023-04-12 04:18:07.000000 pandas_gbq_magic-1.1.2/pandas_gbq_magic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-12 04:18:07.000000 pandas_gbq_magic-1.1.2/pandas_gbq_magic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 04:18:07.000000 pandas_gbq_magic-1.1.2/pandas_gbq_magic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-12 04:18:07.000000 pandas_gbq_magic-1.1.2/pandas_gbq_magic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 04:18:07.649158 pandas_gbq_magic-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      971 2023-04-12 04:16:22.000000 pandas_gbq_magic-1.1.2/setup.py
```

### Comparing `pandas_gbq_magic-1.1.1/LICENSE.txt` & `pandas_gbq_magic-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pandas_gbq_magic-1.1.1/PKG-INFO` & `pandas_gbq_magic-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 Metadata-Version: 2.1
 Name: pandas_gbq_magic
-Version: 1.1.1
+Version: 1.1.2
 Summary: The package provides as magic on top of Pandas GBQ to make querying in Jupter envioronment easy and user  friendly
 Home-page: https://github.com/PulakSachdeva52/Big-Query-Magic/
 Author: Pulak JS
 Author-email: pulaksachdeva@gmail.com
 Project-URL: Bug Tracker, https://github.com/PulakSachdeva52/Big-Query-Magic/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # Big-Query-Magic
 
-#### The package has been created for Mac OS 
+#### The package has been created for Mac OS
 #### Requirements
-It is assumed that you have basic packages like pandas installed 
-Install Auth2client and pandas_gbq 
-Ensure that you can query data using pandas gbq 
+It is assumed that you have basic packages like pandas installed
+Install Auth2client and pandas_gbq
+Ensure that you can query data using pandas gbq
 <hr>
 
 This packacge installs a magic in your startup directory which makes querying in jupyter environment more user friendly and easier to use.Post intallation simply type %%BQSQL and write your query
-example 
+example
 ```python
 %%BQSQL
-SELECT * 
-FROM table 
-LIMIT 10; 
+SELECT *
+FROM table
+LIMIT 10;
 ```
 
 <b>There are other features also present which makes it even more user friendly which can be explained with help of the argument this magic can take</b>
 
--job [Y or None] If Y is passed as job argument this will run just the query but will not pull the out put, this is useful when one is creating a large temp table during the workflow and does not want to download and load it in python, the existing pandas_gbq does not offer that 
+-job [Y or None] If Y is passed as job argument this will run just the query but will not pull the out put, this is useful when one is creating a large temp table during the workflow and does not want to download and load it in python, the existing pandas_gbq does not offer that
 
 -save_to [Table Name] Pass a variable in which the output needs to be store
 
-Note Do not pass both the arguments at the same time 
+Note Do not pass both the arguments at the same time
 
 -para [Y or None] If Y is passed the query will look if parameters or python variables are used in the query. Yes this is one of the best features of this magic you can use python variables directly in your query
 
-example 
+example
 ```python
-x = ['user1','user2']
+x = ['user1','user2']```
 
+```python
 %%BQSQL -para Y -job Y
-SELECT * 
-FROM table 
-WHERE user_id IN @x 
+SELECT *
+FROM table
+WHERE user_id IN @x
+```
+Currently string int and list of these two can be passed as a parameter. Note parameter needs to be preceded by <b><u> @ </u></b> in case one was planning to use @ just as character in that case please avoid using parameter
+
+#### Installation
+Run
+```python
+from pandas_gbq_magic import magic
+magic.install('You Bigquery Project name')
 ```
-Currently string int and list of these two can be passed as a parameter. Note parameter needs to be preceeded by <b><u>@</u></b> in case one was planning to use @ just as character in that case please avaoid using parameter 
+Restart Jupyter notebook
```

### Comparing `pandas_gbq_magic-1.1.1/README.md` & `pandas_gbq_magic-1.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 # Big-Query-Magic
 
-#### The package has been created for Mac OS 
+#### The package has been created for Mac OS
 #### Requirements
-It is assumed that you have basic packages like pandas installed 
-Install Auth2client and pandas_gbq 
-Ensure that you can query data using pandas gbq 
+It is assumed that you have basic packages like pandas installed
+Install Auth2client and pandas_gbq
+Ensure that you can query data using pandas gbq
 <hr>
 
 This packacge installs a magic in your startup directory which makes querying in jupyter environment more user friendly and easier to use.Post intallation simply type %%BQSQL and write your query
-example 
+example
 ```python
 %%BQSQL
-SELECT * 
-FROM table 
-LIMIT 10; 
+SELECT *
+FROM table
+LIMIT 10;
 ```
 
 <b>There are other features also present which makes it even more user friendly which can be explained with help of the argument this magic can take</b>
 
--job [Y or None] If Y is passed as job argument this will run just the query but will not pull the out put, this is useful when one is creating a large temp table during the workflow and does not want to download and load it in python, the existing pandas_gbq does not offer that 
+-job [Y or None] If Y is passed as job argument this will run just the query but will not pull the out put, this is useful when one is creating a large temp table during the workflow and does not want to download and load it in python, the existing pandas_gbq does not offer that
 
 -save_to [Table Name] Pass a variable in which the output needs to be store
 
-Note Do not pass both the arguments at the same time 
+Note Do not pass both the arguments at the same time
 
 -para [Y or None] If Y is passed the query will look if parameters or python variables are used in the query. Yes this is one of the best features of this magic you can use python variables directly in your query
 
-example 
+example
 ```python
-x = ['user1','user2']
+x = ['user1','user2']```
 
+```python
 %%BQSQL -para Y -job Y
-SELECT * 
-FROM table 
-WHERE user_id IN @x 
+SELECT *
+FROM table
+WHERE user_id IN @x
+```
+Currently string int and list of these two can be passed as a parameter. Note parameter needs to be preceded by <b><u> @ </u></b> in case one was planning to use @ just as character in that case please avoid using parameter
+
+#### Installation
+Run
+```python
+from pandas_gbq_magic import magic
+magic.install('You Bigquery Project name')
 ```
-Currently string int and list of these two can be passed as a parameter. Note parameter needs to be preceeded by <b><u>@</u></b> in case one was planning to use @ just as character in that case please avaoid using parameter 
+Restart Jupyter notebook
```

### Comparing `pandas_gbq_magic-1.1.1/pandas_gbq_magic/magic.py` & `pandas_gbq_magic-1.1.2/pandas_gbq_magic/magic.py`

 * *Files identical despite different names*

### Comparing `pandas_gbq_magic-1.1.1/pandas_gbq_magic.egg-info/PKG-INFO` & `pandas_gbq_magic-1.1.2/pandas_gbq_magic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 Metadata-Version: 2.1
 Name: pandas-gbq-magic
-Version: 1.1.1
+Version: 1.1.2
 Summary: The package provides as magic on top of Pandas GBQ to make querying in Jupter envioronment easy and user  friendly
 Home-page: https://github.com/PulakSachdeva52/Big-Query-Magic/
 Author: Pulak JS
 Author-email: pulaksachdeva@gmail.com
 Project-URL: Bug Tracker, https://github.com/PulakSachdeva52/Big-Query-Magic/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # Big-Query-Magic
 
-#### The package has been created for Mac OS 
+#### The package has been created for Mac OS
 #### Requirements
-It is assumed that you have basic packages like pandas installed 
-Install Auth2client and pandas_gbq 
-Ensure that you can query data using pandas gbq 
+It is assumed that you have basic packages like pandas installed
+Install Auth2client and pandas_gbq
+Ensure that you can query data using pandas gbq
 <hr>
 
 This packacge installs a magic in your startup directory which makes querying in jupyter environment more user friendly and easier to use.Post intallation simply type %%BQSQL and write your query
-example 
+example
 ```python
 %%BQSQL
-SELECT * 
-FROM table 
-LIMIT 10; 
+SELECT *
+FROM table
+LIMIT 10;
 ```
 
 <b>There are other features also present which makes it even more user friendly which can be explained with help of the argument this magic can take</b>
 
--job [Y or None] If Y is passed as job argument this will run just the query but will not pull the out put, this is useful when one is creating a large temp table during the workflow and does not want to download and load it in python, the existing pandas_gbq does not offer that 
+-job [Y or None] If Y is passed as job argument this will run just the query but will not pull the out put, this is useful when one is creating a large temp table during the workflow and does not want to download and load it in python, the existing pandas_gbq does not offer that
 
 -save_to [Table Name] Pass a variable in which the output needs to be store
 
-Note Do not pass both the arguments at the same time 
+Note Do not pass both the arguments at the same time
 
 -para [Y or None] If Y is passed the query will look if parameters or python variables are used in the query. Yes this is one of the best features of this magic you can use python variables directly in your query
 
-example 
+example
 ```python
-x = ['user1','user2']
+x = ['user1','user2']```
 
+```python
 %%BQSQL -para Y -job Y
-SELECT * 
-FROM table 
-WHERE user_id IN @x 
+SELECT *
+FROM table
+WHERE user_id IN @x
+```
+Currently string int and list of these two can be passed as a parameter. Note parameter needs to be preceded by <b><u> @ </u></b> in case one was planning to use @ just as character in that case please avoid using parameter
+
+#### Installation
+Run
+```python
+from pandas_gbq_magic import magic
+magic.install('You Bigquery Project name')
 ```
-Currently string int and list of these two can be passed as a parameter. Note parameter needs to be preceeded by <b><u>@</u></b> in case one was planning to use @ just as character in that case please avaoid using parameter 
+Restart Jupyter notebook
```

### Comparing `pandas_gbq_magic-1.1.1/setup.py` & `pandas_gbq_magic-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name="pandas_gbq_magic",
-    version="1.1.1",
+    version="1.1.2",
     author="Pulak JS",
     author_email="pulaksachdeva@gmail.com",
     description="The package provides as magic on top of Pandas GBQ to make querying in Jupter envioronment easy and user  friendly",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PulakSachdeva52/Big-Query-Magic/",
     project_urls={
```

