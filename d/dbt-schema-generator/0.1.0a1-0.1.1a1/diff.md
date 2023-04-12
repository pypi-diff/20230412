# Comparing `tmp/dbt_schema_generator-0.1.0a1.tar.gz` & `tmp/dbt_schema_generator-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_schema_generator-0.1.0a1.tar", last modified: Tue Apr 11 18:09:12 2023, max compression
+gzip compressed data, was "dbt_schema_generator-0.1.1a1.tar", last modified: Wed Apr 12 08:26:42 2023, max compression
```

## Comparing `dbt_schema_generator-0.1.0a1.tar` & `dbt_schema_generator-0.1.1a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-11 18:09:12.768461 dbt_schema_generator-0.1.0a1/
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1062 2023-04-11 15:56:50.000000 dbt_schema_generator-0.1.0a1/LICENSE
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-11 18:09:12.768461 dbt_schema_generator-0.1.0a1/PKG-INFO
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1195 2023-04-11 18:07:45.000000 dbt_schema_generator-0.1.0a1/README.md
-drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-11 18:09:12.764461 dbt_schema_generator-0.1.0a1/dbt_schema_generator/
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       28 2023-04-11 15:15:56.000000 dbt_schema_generator-0.1.0a1/dbt_schema_generator/__init__.py
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     6139 2023-04-11 16:05:40.000000 dbt_schema_generator-0.1.0a1/dbt_schema_generator/generator.py
-drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-11 18:09:12.768461 dbt_schema_generator-0.1.0a1/dbt_schema_generator.egg-info/
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-11 18:09:12.000000 dbt_schema_generator-0.1.0a1/dbt_schema_generator.egg-info/PKG-INFO
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)      316 2023-04-11 18:09:12.000000 dbt_schema_generator-0.1.0a1/dbt_schema_generator.egg-info/SOURCES.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)        1 2023-04-11 18:09:12.000000 dbt_schema_generator-0.1.0a1/dbt_schema_generator.egg-info/dependency_links.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       67 2023-04-11 18:09:12.000000 dbt_schema_generator-0.1.0a1/dbt_schema_generator.egg-info/entry_points.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       21 2023-04-11 18:09:12.000000 dbt_schema_generator-0.1.0a1/dbt_schema_generator.egg-info/top_level.txt
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       38 2023-04-11 18:09:12.768461 dbt_schema_generator-0.1.0a1/setup.cfg
--rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1028 2023-04-11 18:08:55.000000 dbt_schema_generator-0.1.0a1/setup.py
+drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 08:26:42.229226 dbt_schema_generator-0.1.1a1/
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1062 2023-04-11 15:56:50.000000 dbt_schema_generator-0.1.1a1/LICENSE
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-12 08:26:42.229226 dbt_schema_generator-0.1.1a1/PKG-INFO
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1195 2023-04-11 18:07:45.000000 dbt_schema_generator-0.1.1a1/README.md
+drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 08:26:42.217226 dbt_schema_generator-0.1.1a1/dbt_schema_generator/
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       28 2023-04-11 15:15:56.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator/__init__.py
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     6288 2023-04-12 08:19:21.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator/generator.py
+drwxrwxr-x   0 muizzlateef  (1001) muizzlateef  (1001)        0 2023-04-12 08:26:42.225226 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1757 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/PKG-INFO
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)      316 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/SOURCES.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)        1 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/dependency_links.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       67 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/entry_points.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       21 2023-04-12 08:26:41.000000 dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/top_level.txt
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)       38 2023-04-12 08:26:42.229226 dbt_schema_generator-0.1.1a1/setup.cfg
+-rw-rw-r--   0 muizzlateef  (1001) muizzlateef  (1001)     1006 2023-04-12 08:26:38.000000 dbt_schema_generator-0.1.1a1/setup.py
```

### Comparing `dbt_schema_generator-0.1.0a1/LICENSE` & `dbt_schema_generator-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_schema_generator-0.1.0a1/PKG-INFO` & `dbt_schema_generator-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_schema_generator
-Version: 0.1.0a1
+Version: 0.1.1a1
 Summary: A command-line tool to generate schema.yml files for specified dbt models
 Home-page: https://github.com/Muizzkolapo/dbt_schema_generator.git
 Author: Your Name
 Author-email: lateefmuizz@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt_schema_generator-0.1.0a1/README.md` & `dbt_schema_generator-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_schema_generator-0.1.0a1/dbt_schema_generator/generator.py` & `dbt_schema_generator-0.1.1a1/dbt_schema_generator/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     return schema
 
 def save_schema(schema: str, output_file: str) -> None:
     """Saves the schema YAML content to the output file."""
     with open(output_file, 'w') as f:
         f.write(schema)
 
+
 def main() -> None:
     parser = argparse.ArgumentParser(description='Generate schema.yml file for specified dbt models.')
     parser.add_argument('-m', '--models', type=str, required=False,
                         help='Comma-separated list of model names to include in the schema.yml file.')
     parser.add_argument('-p', '--path', type=str, required=False,
                         help='Path to include models in the schema.yml file.')
 
@@ -122,22 +123,24 @@
 
             if specified_models:
                 for model_name in specified_models:
                     model = {key: value for key, value in models.items() if value['name'] == model_name}
                     schema = create_schema(model)
                     model_directory = os.path.dirname(model[next(iter(model))]['original_file_path'])
                     output_file = os.path.join(project_path, model_directory, f"{model_name}.yml")
+                    print(f"Generating schema for model: {model_name}")
                     save_schema(schema, output_file)
             else:
                 for model in models.values():
                     single_model = {key: value for key, value in models.items() if value['name'] == model['name']}
                     schema = create_schema(single_model)
                     model_directory = os.path.dirname(model['original_file_path'])
                     output_file = os.path.join(project_path, model_directory, f"{model['name']}.yml")
+                    print(f"Generating schema for model: {model['name']}")
                     save_schema(schema, output_file)
         else:
             print("manifest.json file not found.")
     else:
         print(f"dbt project status: {status}")
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `dbt_schema_generator-0.1.0a1/dbt_schema_generator.egg-info/PKG-INFO` & `dbt_schema_generator-0.1.1a1/dbt_schema_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-schema-generator
-Version: 0.1.0a1
+Version: 0.1.1a1
 Summary: A command-line tool to generate schema.yml files for specified dbt models
 Home-page: https://github.com/Muizzkolapo/dbt_schema_generator.git
 Author: Your Name
 Author-email: lateefmuizz@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dbt_schema_generator-0.1.0a1/setup.py` & `dbt_schema_generator-0.1.1a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the README.md content
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='dbt_schema_generator',
-    version='0.1.0a1',  # First alpha release 
+    version='0.1.1a1',  
     author='Your Name',
     author_email='lateefmuizz@gmail.com',
     description='A command-line tool to generate schema.yml files for specified dbt models',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Muizzkolapo/dbt_schema_generator.git',
     license='MIT',
```

