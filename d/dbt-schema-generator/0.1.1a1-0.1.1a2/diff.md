# Comparing `tmp/dbt_schema_generator-0.1.1a1.tar.gz` & `tmp/dbt_schema_generator-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_schema_generator-0.1.1a1.tar", last modified: Wed Apr 12 08:26:42 2023, max compression
+gzip compressed data, was "dbt_schema_generator-0.1.1a2.tar", last modified: Wed Apr 12 15:39:30 2023, max compression
```

## Comparing `dbt_schema_generator-0.1.1a1.tar` & `dbt_schema_generator-0.1.1a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 08:26:42.229226 dbt_schema_generator-0.1.1a1/
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1062 2023-04-11 15:56:50.000000 dbt_schema_generator-0.1.1a1/LICENSE
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-12 08:26:42.229226 dbt_schema_generator-0.1.1a1/PKG-INFO
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1195 2023-04-11 18:07:45.000000 dbt_schema_generator-0.1.1a1/README.md
-drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 08:26:42.217226 dbt_schema_generator-0.1.1a1/dbt_schema_generator/
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       28 2023-04-11 15:15:56.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator/__init__.py
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     6288 2023-04-12 08:19:21.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator/generator.py
-drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 08:26:42.225226 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/PKG-INFO
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)      316 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/SOURCES.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)        1 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/dependency_links.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       67 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/entry_points.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       21 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/top_level.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       38 2023-04-12 08:26:42.229226 dbt_schema_generator-0.1.1a1/setup.cfg
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1006 2023-04-12 08:26:38.000000 dbt_schema_generator-0.1.1a1/setup.py
+drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 15:39:30.063027 dbt_schema_generator-0.1.1a2/
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1062 2023-04-12 15:25:52.000000 dbt_schema_generator-0.1.1a2/LICENSE
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-12 15:39:30.063027 dbt_schema_generator-0.1.1a2/PKG-INFO
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1195 2023-04-12 15:25:52.000000 dbt_schema_generator-0.1.1a2/README.md
+drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 15:39:30.059026 dbt_schema_generator-0.1.1a2/dbt_schema_generator/
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       28 2023-04-12 15:25:52.000000 dbt_schema_generator-0.1.1a2/dbt_schema_generator/__init__.py
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     6294 2023-04-12 15:28:44.000000 dbt_schema_generator-0.1.1a2/dbt_schema_generator/generator.py
+drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 15:39:30.063027 dbt_schema_generator-0.1.1a2/dbt_schema_generator.egg-info/
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-12 15:39:29.000000 dbt_schema_generator-0.1.1a2/dbt_schema_generator.egg-info/PKG-INFO
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)      316 2023-04-12 15:39:29.000000 dbt_schema_generator-0.1.1a2/dbt_schema_generator.egg-info/SOURCES.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)        1 2023-04-12 15:39:29.000000 dbt_schema_generator-0.1.1a2/dbt_schema_generator.egg-info/dependency_links.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       67 2023-04-12 15:39:29.000000 dbt_schema_generator-0.1.1a2/dbt_schema_generator.egg-info/entry_points.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       21 2023-04-12 15:39:29.000000 dbt_schema_generator-0.1.1a2/dbt_schema_generator.egg-info/top_level.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       38 2023-04-12 15:39:30.063027 dbt_schema_generator-0.1.1a2/setup.cfg
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1006 2023-04-12 15:35:35.000000 dbt_schema_generator-0.1.1a2/setup.py
```

### Comparing `dbt_schema_generator-0.1.1a1/LICENSE` & `dbt_schema_generator-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_schema_generator-0.1.1a1/PKG-INFO` & `dbt_schema_generator-0.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_schema_generator
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A command-line tool to generate schema.yml files for specified dbt models
 Home-page: https://github.com/Muizzkolapo/dbt_schema_generator.git
 Author: Your Name
 Author-email: lateefmuizz@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt_schema_generator-0.1.1a1/README.md` & `dbt_schema_generator-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_schema_generator-0.1.1a1/dbt_schema_generator/generator.py` & `dbt_schema_generator-0.1.1a2/dbt_schema_generator/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,29 +64,29 @@
         if original_file_path.startswith(path_name) and node_value['resource_type'] == 'model':
             models[node_key] = node_value
     return models
 
 
 def create_schema(models: Dict) -> str:
     """Creates the schema YAML content from the models."""
-    schema = "version: 2\nmodels:\n"
+    schema = "version: 2\n\nmodels:\n\n"
     for model in models.values():
         model_dict = {
             'name': model['name'],
             'description': '',
             'columns': []
         }
         for column_name, column_value in model['columns'].items():
             column_dict = {
                 'name': column_name,
                 'description': '',
             }
             model_dict['columns'].append(column_dict)
 
-        model_lines = f"  - name: {model_dict['name']}\n    description: '{model_dict['description']}'\n    columns:\n"
+        model_lines = f"  - name: {model_dict['name']}\n    description: '{model_dict['description']}'\n    columns:\n\n"
         column_lines = "\n".join([f"      - name: {col['name']}\n        description: '{col['description']}'\n" for col in model_dict['columns']])
         schema += f"{model_lines}{column_lines}\n"
     return schema
 
 def save_schema(schema: str, output_file: str) -> None:
     """Saves the schema YAML content to the output file."""
     with open(output_file, 'w') as f:
```

### Comparing `dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/PKG-INFO` & `dbt_schema_generator-0.1.1a2/dbt_schema_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-generator
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A command-line tool to generate schema.yml files for specified dbt models
 Home-page: https://github.com/Muizzkolapo/dbt_schema_generator.git
 Author: Your Name
 Author-email: lateefmuizz@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt_schema_generator-0.1.1a1/setup.py` & `dbt_schema_generator-0.1.1a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the README.md content
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='dbt_schema_generator',
-    version='0.1.1a1',  
+    version='0.1.1a2',  
     author='Your Name',
     author_email='lateefmuizz@gmail.com',
     description='A command-line tool to generate schema.yml files for specified dbt models',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Muizzkolapo/dbt_schema_generator.git',
     license='MIT',
```

