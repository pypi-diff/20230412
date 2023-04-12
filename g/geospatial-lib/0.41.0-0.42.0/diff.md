# Comparing `tmp/geospatial-lib-0.41.0.tar.gz` & `tmp/geospatial-lib-0.42.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospatial-lib-0.41.0.tar", max compression
+gzip compressed data, was "geospatial-lib-0.42.0.tar", max compression
```

## Comparing `geospatial-lib-0.41.0.tar` & `geospatial-lib-0.42.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35115 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/LICENSE
--rw-r--r--   0        0        0      380 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/README.md
--rw-r--r--   0        0        0       46 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/core/__init__.py
--rw-r--r--   0        0        0      374 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/core/core.py
--rw-r--r--   0        0        0     3378 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/core/logger.py
--rw-r--r--   0        0        0        0 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/db/__init__.py
--rw-r--r--   0        0        0    12368 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/db/pandas_handler.py
--rw-r--r--   0        0        0     4572 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/db/pg_core.py
--rw-r--r--   0        0        0     7270 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/db/pg_handler.py
--rw-r--r--   0        0        0      348 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/db/poetry.md
--rw-r--r--   0        0        0      519 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/main.py
--rw-r--r--   0        0        0        0 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/misc/__init__.py
--rw-r--r--   0        0        0      195 2023-02-23 23:34:33.324993 geospatial-lib-0.41.0/geospatial_lib/misc/extraction.py
--rw-r--r--   0        0        0     2512 2023-02-23 23:34:33.328993 geospatial-lib-0.41.0/geospatial_lib/misc/gridding.py
--rw-r--r--   0        0        0      835 2023-02-23 23:34:33.328993 geospatial-lib-0.41.0/geospatial_lib/misc/helpers.py
--rw-r--r--   0        0        0     1498 2023-02-23 23:34:33.328993 geospatial-lib-0.41.0/geospatial_lib/misc/processing.py
--rw-r--r--   0        0        0      534 2023-02-23 23:34:33.328993 geospatial-lib-0.41.0/pyproject.toml
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 geospatial-lib-0.41.0/setup.py
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 geospatial-lib-0.41.0/PKG-INFO
+-rw-r--r--   0        0        0    35115 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/LICENSE
+-rw-r--r--   0        0        0      380 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/README.md
+-rw-r--r--   0        0        0       46 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/core/__init__.py
+-rw-r--r--   0        0        0      374 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/core/core.py
+-rw-r--r--   0        0        0     3378 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/core/logger.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/db/__init__.py
+-rw-r--r--   0        0        0    12443 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/db/pandas_handler.py
+-rw-r--r--   0        0        0     4572 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/db/pg_core.py
+-rw-r--r--   0        0        0     7270 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/db/pg_handler.py
+-rw-r--r--   0        0        0      348 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/db/poetry.md
+-rw-r--r--   0        0        0      519 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/main.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/misc/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/misc/extraction.py
+-rw-r--r--   0        0        0     2512 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/misc/gridding.py
+-rw-r--r--   0        0        0      835 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/misc/helpers.py
+-rw-r--r--   0        0        0     1498 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/geospatial_lib/misc/processing.py
+-rw-r--r--   0        0        0      557 2023-04-12 20:52:44.982955 geospatial-lib-0.42.0/pyproject.toml
+-rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 geospatial-lib-0.42.0/setup.py
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 geospatial-lib-0.42.0/PKG-INFO
```

### Comparing `geospatial-lib-0.41.0/LICENSE` & `geospatial-lib-0.42.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/geospatial_lib/core/logger.py` & `geospatial-lib-0.42.0/geospatial_lib/core/logger.py`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/geospatial_lib/db/pandas_handler.py` & `geospatial-lib-0.42.0/geospatial_lib/db/pandas_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,50 +270,51 @@
         )
 
         lambda_functions_by_types = {
             # TODO simplify
             "DateTimeRange": lambda x:
                 f"{str(x)[0]}{str(x.lower) if x.lower is not None else _datetime_infinite_value},"
                 f"{str(x.upper) if x.upper is not None else _datetime_infinite_value}{str(x)[-1]}",
-            "datetime": lambda x: x.strftime("%Y-%m-%d %H:%M:%S.%f"),
+            "datetime": lambda x: f'{str(x.strftime("%Y-%m-%d %H:%M:%S"))}',
             "BaseGeometry": lambda x: self.__convert_shapely_to_ewkb(x, epsg),
             "dict": lambda x: dumps(x, ensure_ascii=False),
             "list": lambda x: "{}" if len(x) == 0 else '{' + ', '.join(f'"{feat}"' for feat in x) + '}',
             "default": lambda x: x.__str__(),
         }
 
         for column in data.columns:
             first_element = data[column].iat[0]
             if isinstance(first_element, DateTimeRange):
-                data.loc[:, column] = data[column].map(
+                data.loc[:, column] = data[column].apply(
                     lambda_functions_by_types["DateTimeRange"]
                 )
 
             elif isinstance(first_element, datetime):
-                data.loc[:, column] = data[column].map(
+                data.loc[:, column] = data[column].apply(
                     lambda_functions_by_types["datetime"]
                 )
+                data[column] = data[column].astype(str)
 
             elif isinstance(first_element, BaseGeometry):
-                data.loc[:, column] = data[column].map(
+                data.loc[:, column] = data[column].apply(
                     lambda_functions_by_types["BaseGeometry"]
                 )
 
             elif isinstance(first_element, dict):
-                data.loc[:, column] = data[column].map(
+                data.loc[:, column] = data[column].apply(
                     lambda_functions_by_types["dict"]
                 )
 
             elif isinstance(first_element, list):
-                data.loc[:, column] = data[column].map(
+                data.loc[:, column] = data[column].apply(
                     lambda_functions_by_types["list"]
                 )
 
             else:
-                data.loc[:, column] = data[column].map(
+                data.loc[:, column] = data[column].apply(
                     lambda_functions_by_types["default"]
                 )
 
         return data.to_dict("records")
 
     def df_explode_datetimerange_fields(self,
                                         data: Union[pd.DataFrame, gpd.GeoDataFrame]
```

### Comparing `geospatial-lib-0.41.0/geospatial_lib/db/pg_core.py` & `geospatial-lib-0.42.0/geospatial_lib/db/pg_core.py`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/geospatial_lib/db/pg_handler.py` & `geospatial-lib-0.42.0/geospatial_lib/db/pg_handler.py`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/geospatial_lib/main.py` & `geospatial-lib-0.42.0/geospatial_lib/main.py`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/geospatial_lib/misc/gridding.py` & `geospatial-lib-0.42.0/geospatial_lib/misc/gridding.py`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/geospatial_lib/misc/helpers.py` & `geospatial-lib-0.42.0/geospatial_lib/misc/helpers.py`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/geospatial_lib/misc/processing.py` & `geospatial-lib-0.42.0/geospatial_lib/misc/processing.py`

 * *Files identical despite different names*

### Comparing `geospatial-lib-0.41.0/pyproject.toml` & `geospatial-lib-0.42.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "geospatial-lib"
-version = "0.41.0"
+version = "0.42.0"
 description = "A library with some geo functions"
 authors = ["amauryval <amauryval@gmail.com>"]
 license = "GPL3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.0"
 geopandas = "^0.12.2"
 xlrd = "^2.0.1"
 SQLAlchemy = "^2.0.4"
 GeoAlchemy2 = "^0.13.1"
 SQLAlchemy-Utils = "^0.40.0"
-psycopg2-binary = "^2.9.5"
+psycopg2-binary = "^2.9.6"
+setuptools = "^67.6.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
+pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `geospatial-lib-0.41.0/setup.py` & `geospatial-lib-0.42.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 {'': ['*']}
 
 install_requires = \
 ['GeoAlchemy2>=0.13.1,<0.14.0',
  'SQLAlchemy-Utils>=0.40.0,<0.41.0',
  'SQLAlchemy>=2.0.4,<3.0.0',
  'geopandas>=0.12.2,<0.13.0',
- 'psycopg2-binary>=2.9.5,<3.0.0',
+ 'psycopg2-binary>=2.9.6,<3.0.0',
+ 'setuptools>=67.6.1,<68.0.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'geospatial-lib',
-    'version': '0.41.0',
+    'version': '0.42.0',
     'description': 'A library with some geo functions',
     'long_description': 'GeoLib\n=====\n[![RunTest](https://github.com/amauryval/geolib/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/amauryval/geolib/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/amauryval/geolib/branch/master/graph/badge.svg)](https://codecov.io/gh/amauryval/geolib)\n\n\n# install\n```bash\npyenv local 3.11.0\npoetry env use 3.11.0\npoetry install\n```',
     'author': 'amauryval',
     'author_email': 'amauryval@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `geospatial-lib-0.41.0/PKG-INFO` & `geospatial-lib-0.42.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: geospatial-lib
-Version: 0.41.0
+Version: 0.42.0
 Summary: A library with some geo functions
 License: GPL3
 Author: amauryval
 Author-email: amauryval@gmail.com
 Requires-Python: ==3.11.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: GeoAlchemy2 (>=0.13.1,<0.14.0)
 Requires-Dist: SQLAlchemy (>=2.0.4,<3.0.0)
 Requires-Dist: SQLAlchemy-Utils (>=0.40.0,<0.41.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
-Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
+Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 GeoLib
 =====
 [![RunTest](https://github.com/amauryval/geolib/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/amauryval/geolib/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/amauryval/geolib/branch/master/graph/badge.svg)](https://codecov.io/gh/amauryval/geolib)
```

