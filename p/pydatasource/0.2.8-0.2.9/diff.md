# Comparing `tmp/pydatasource-0.2.8.tar.gz` & `tmp/pydatasource-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatasource-0.2.8.tar", last modified: Thu Jan 28 11:48:31 2021, max compression
+gzip compressed data, was "dist/pydatasource-0.2.9.tar", last modified: Thu Jan 28 12:27:25 2021, max compression
```

## Comparing `pydatasource-0.2.8.tar` & `pydatasource-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 11:48:31.000000 pydatasource-0.2.8/
--rw-r--r--   0 lucet      (501) staff       (20)      452 2021-01-28 11:48:31.000000 pydatasource-0.2.8/PKG-INFO
--rw-r--r--   0 lucet      (501) staff       (20)     1049 2019-11-10 10:50:59.000000 pydatasource-0.2.8/LICENSE
--rw-r--r--   0 lucet      (501) staff       (20)       15 2019-11-10 10:50:59.000000 pydatasource-0.2.8/MANIFEST.in
-drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource.egg-info/
--rw-r--r--   0 lucet      (501) staff       (20)      452 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource.egg-info/PKG-INFO
--rw-r--r--   0 lucet      (501) staff       (20)      408 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource.egg-info/SOURCES.txt
--rw-r--r--   0 lucet      (501) staff       (20)       78 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource.egg-info/requires.txt
--rw-r--r--   0 lucet      (501) staff       (20)       13 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource.egg-info/top_level.txt
--rw-r--r--   0 lucet      (501) staff       (20)        1 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource.egg-info/dependency_links.txt
--rw-r--r--   0 lucet      (501) staff       (20)      847 2021-01-28 11:47:50.000000 pydatasource-0.2.8/setup.py
--rw-r--r--   0 lucet      (501) staff       (20)       38 2021-01-28 11:48:31.000000 pydatasource-0.2.8/setup.cfg
--rw-r--r--   0 lucet      (501) staff       (20)       13 2019-11-10 10:50:59.000000 pydatasource-0.2.8/README.rst
-drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource/
-drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 11:48:31.000000 pydatasource-0.2.8/pydatasource/core/
--rw-r--r--   0 lucet      (501) staff       (20)      713 2020-08-02 15:45:32.000000 pydatasource-0.2.8/pydatasource/core/documentation.py
--rw-r--r--   0 lucet      (501) staff       (20)      671 2020-12-11 10:25:47.000000 pydatasource-0.2.8/pydatasource/core/environment_comparison.py
--rw-r--r--   0 lucet      (501) staff       (20)        0 2019-11-10 10:50:59.000000 pydatasource-0.2.8/pydatasource/core/__init__.py
--rw-r--r--   0 lucet      (501) staff       (20)     2036 2020-10-18 11:44:08.000000 pydatasource-0.2.8/pydatasource/core/snippet.py
--rw-r--r--   0 lucet      (501) staff       (20)       46 2019-11-10 10:50:59.000000 pydatasource-0.2.8/pydatasource/__init__.py
--rw-r--r--   0 lucet      (501) staff       (20)    17348 2021-01-28 11:47:47.000000 pydatasource-0.2.8/pydatasource/DataSource.py
+drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 12:27:25.000000 pydatasource-0.2.9/
+-rw-r--r--   0 lucet      (501) staff       (20)      452 2021-01-28 12:27:25.000000 pydatasource-0.2.9/PKG-INFO
+-rw-r--r--   0 lucet      (501) staff       (20)     1049 2019-11-10 10:50:59.000000 pydatasource-0.2.9/LICENSE
+-rw-r--r--   0 lucet      (501) staff       (20)       15 2019-11-10 10:50:59.000000 pydatasource-0.2.9/MANIFEST.in
+drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource.egg-info/
+-rw-r--r--   0 lucet      (501) staff       (20)      452 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource.egg-info/PKG-INFO
+-rw-r--r--   0 lucet      (501) staff       (20)      408 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource.egg-info/SOURCES.txt
+-rw-r--r--   0 lucet      (501) staff       (20)       78 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource.egg-info/requires.txt
+-rw-r--r--   0 lucet      (501) staff       (20)       13 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource.egg-info/top_level.txt
+-rw-r--r--   0 lucet      (501) staff       (20)        1 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource.egg-info/dependency_links.txt
+-rw-r--r--   0 lucet      (501) staff       (20)      847 2021-01-28 12:27:10.000000 pydatasource-0.2.9/setup.py
+-rw-r--r--   0 lucet      (501) staff       (20)       38 2021-01-28 12:27:25.000000 pydatasource-0.2.9/setup.cfg
+-rw-r--r--   0 lucet      (501) staff       (20)       13 2019-11-10 10:50:59.000000 pydatasource-0.2.9/README.rst
+drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource/
+drwxr-xr-x   0 lucet      (501) staff       (20)        0 2021-01-28 12:27:25.000000 pydatasource-0.2.9/pydatasource/core/
+-rw-r--r--   0 lucet      (501) staff       (20)      713 2020-08-02 15:45:32.000000 pydatasource-0.2.9/pydatasource/core/documentation.py
+-rw-r--r--   0 lucet      (501) staff       (20)      671 2020-12-11 10:25:47.000000 pydatasource-0.2.9/pydatasource/core/environment_comparison.py
+-rw-r--r--   0 lucet      (501) staff       (20)        0 2019-11-10 10:50:59.000000 pydatasource-0.2.9/pydatasource/core/__init__.py
+-rw-r--r--   0 lucet      (501) staff       (20)     2036 2020-10-18 11:44:08.000000 pydatasource-0.2.9/pydatasource/core/snippet.py
+-rw-r--r--   0 lucet      (501) staff       (20)       46 2019-11-10 10:50:59.000000 pydatasource-0.2.9/pydatasource/__init__.py
+-rw-r--r--   0 lucet      (501) staff       (20)    17333 2021-01-28 12:27:10.000000 pydatasource-0.2.9/pydatasource/DataSource.py
```

### Comparing `pydatasource-0.2.8/LICENSE` & `pydatasource-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatasource-0.2.8/setup.py` & `pydatasource-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst') as f:
     readme = f.read()
 
 setup(
     name='pydatasource',
-    version='0.2.8',  # last version with jinja: 0.2.4 / without jinja: 0.1.11
+    version='0.2.9',  # last version with jinja: 0.2.4 / without jinja: 0.1.11
     description='Easily manage a dataflow',
     long_description=readme,
     author='Dacker',
     author_email='hello@dacker.co',
     url='https://github.com/dacker-team/pydatasource',
     keywords='easily manage dataflow',
     packages=find_packages(exclude=('tests', 'docs')),
```

### Comparing `pydatasource-0.2.8/pydatasource/core/documentation.py` & `pydatasource-0.2.9/pydatasource/core/documentation.py`

 * *Files identical despite different names*

### Comparing `pydatasource-0.2.8/pydatasource/core/environment_comparison.py` & `pydatasource-0.2.9/pydatasource/core/environment_comparison.py`

 * *Files identical despite different names*

### Comparing `pydatasource-0.2.8/pydatasource/core/snippet.py` & `pydatasource-0.2.9/pydatasource/core/snippet.py`

 * *Files identical despite different names*

### Comparing `pydatasource-0.2.8/pydatasource/DataSource.py` & `pydatasource-0.2.9/pydatasource/DataSource.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     today = datetime.datetime.today()
     # today = datetime.date(2020, 2, 29)
     if isinstance(date_range, dict):
         if period is not None:
             try:
                 date_range = date_range[period]
             except KeyError:
-                raise Exception("The daterange params in the config file does not match period ")
+                raise Exception("The period params in the config file does not match period ")
         elif period is None:
             raise Exception("period argument is required due to date_range params in the config file")
     if date_range == "ytd":
         start_date = today.strftime("%Y-01-01")
         end_date = today.strftime("%Y-%m-%d")
     elif date_range == "lytd":
         start_date = (today + relativedelta(years=-1)).strftime("%Y-01-01")
@@ -166,24 +166,24 @@
         dict_params.update(
             treat_all_snippet(
                 datasource_instance=self,
                 query_path=query_path,
                 layer=layer_name,
                 dict_params=dict_params)
         )
-        if query_config.get("daterange"):
+        if query_config.get("period"):
             dict_params.update(date_range_params(
-                date_range=query_config.get("daterange"),
+                date_range=query_config.get("period"),
                 comparison=False,
                 period=period)
             )
 
-        if query_config.get("daterange_comparison"):
+        if query_config.get("period_comparison"):
             dict_params.update(date_range_params(
-                date_range=query_config.get("daterange_comparison"),
+                date_range=query_config.get("period_comparison"),
                 period=period,
                 comparison=True)
             )
 
         template = self.jinja_env.from_string(self.load_file(query_path))
         return template.render(dict_params)
```

