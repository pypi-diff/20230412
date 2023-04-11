# Comparing `tmp/spark_quality_rules_tools-0.2.4.tar.gz` & `tmp/spark_quality_rules_tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.2.4.tar", last modified: Tue Apr 11 12:29:06 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.2.5.tar", last modified: Tue Apr 11 23:54:56 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.2.4.tar` & `spark_quality_rules_tools-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      155 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3846 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3088 2023-04-08 05:49:00.000000 spark_quality_rules_tools-0.2.4/README.md
--rw-rw-rw-   0        0        0       86 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-04-11 12:19:40.000000 spark_quality_rules_tools-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.966518 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     1728 2023-04-10 14:18:27.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    19489 2023-04-08 05:39:17.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      216 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2472 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/dataframe.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/external/
--rw-rw-rw-   0        0        0    71803 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/external/folder_process.png
--rw-rw-rw-   0        0        0     1056 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/memory.py
--rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    16245 2023-04-10 23:11:39.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     2475 2023-04-11 12:15:42.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.982144 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/table.html
-drwxrwxrwx   0        0        0        0 2023-04-11 12:29:06.966518 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     3846 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-11 12:29:06.000000 spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/
+-rw-rw-rw-   0        0        0     1092 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      155 2023-04-11 23:35:17.000000 spark_quality_rules_tools-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3887 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3088 2023-04-11 14:27:34.000000 spark_quality_rules_tools-0.2.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-04-11 23:54:48.000000 spark_quality_rules_tools-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.469640 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     1728 2023-04-11 14:27:34.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.485270 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    19489 2023-04-11 14:27:34.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.507427 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-11 22:08:20.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2472 2022-07-12 20:46:27.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/dataframe.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.507427 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/external/
+-rw-rw-rw-   0        0        0    71803 2022-10-17 12:27:14.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/external/folder_process.png
+-rw-rw-rw-   0        0        0     1056 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/memory.py
+-rw-rw-rw-   0        0        0     2113 2022-07-28 23:32:51.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.507427 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      716 2022-07-28 16:09:02.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-11 17:19:50.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3344 2023-04-11 22:30:11.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.523053 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-07-12 20:31:55.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/templates/table.html
+drwxrwxrwx   0        0        0        0 2023-04-11 23:54:56.485270 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     3887 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      243 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-11 23:54:56.000000 spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.2.4/LICENSE` & `spark_quality_rules_tools-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/PKG-INFO` & `spark_quality_rules_tools-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
-Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
@@ -110,7 +112,9 @@
 
 - choco install visualcpp-build-tools
 
 ## Reference
 
 - Jonathan Quiza [github](https://github.com/jonaqp).
 - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
+
+
```

### Comparing `spark_quality_rules_tools-0.2.4/README.md` & `spark_quality_rules_tools-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/setup.py` & `spark_quality_rules_tools-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.2.4',
+    version='0.2.5',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/dataframe.py` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/external/folder_process.png` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/external/folder_process.png`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/memory.py` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/memory.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/rules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-import warnings
-
-warnings.filterwarnings('always')
-warnings.filterwarnings('ignore')
-
-
 def get_validate_rules(hocons_dir=None):
     import os
     import sys
     import json
     from spark_quality_rules_tools.utils import BASE_DIR
+    from spark_quality_rules_tools.utils.color import get_color, get_color_b, get_color_r, get_color_g
     from pyhocon.converter import HOCONConverter
     from pyhocon import ConfigFactory
     from prettytable import PrettyTable
 
     is_windows = sys.platform.startswith('win')
     dir_default_rules = os.path.join(BASE_DIR, "utils", "resource", "rules.json")
     file_conf = hocons_dir
@@ -39,26 +34,42 @@
         haas_columns = haas_rule["config"]
         haas_rules_type = str(haas_class).split(".")[4]
         haas_rules_class = str(haas_class).split(".")[5]
 
         rules_version = default_rules["rules_config"][haas_rules_type][haas_rules_class][0]["rules_version"]
         rules_columns = default_rules["rules_config"][haas_rules_type][haas_rules_class][0]["rules_columns"][0]
         rules_columns_all = {**rules_columns, **rules_default_properties}
-
-        print("type=>", haas_rules_type, "class=>", haas_rules_class, "version=>", rules_version)
+        rules_columns_required = [key for key, val in rules_columns_all.items() if val[1] == "true"]
 
         t = PrettyTable()
-        t.field_names = [f"Variable", "Value", "Dtype Actual", "Dtype Esperado", "Es Obligatorio"]
+        print(f"type   => {get_color_g(haas_rules_type)}")
+        print(f"class  => {get_color_g(haas_rules_class)}")
+        print(f"version=> {get_color_g(rules_version)}")
 
-        if 'id' not in haas_columns.keys():
-            print("variable id: no existe")
-        else:
-            print("variable id:", haas_columns["id"])
+        t.field_names = [f"Variable", "Value", "Dtype Actual", "Dtype Esperado", "Es Obligatorio"]
+        for col in rules_columns_required:
+            if str(col) not in haas_columns.keys():
+                t.add_row([get_color_r(col),
+                           get_color_r("variable requerida"),
+                           get_color_r("variable requerida"),
+                           get_color_r(rules_columns_all[col][0]),
+                           get_color_r(rules_columns_all[col][1])
+                           ])
 
         for col, value in haas_columns.items():
             if not str(col) in rules_columns_all.keys():
-                t.add_row([col, value, str(type(col)), "Deprecado", "false"])
+                t.add_row([get_color_b(col),
+                           get_color_b(value),
+                           get_color_b("Deprecado"),
+                           get_color_b("Deprecado"),
+                           get_color_b("Deprecado")
+                           ])
 
         for col, value in haas_columns.items():
             if str(col) in rules_columns_all.keys():
-                t.add_row([col, value, str(type(value)), rules_columns_all[col][0], rules_columns_all[col][1]])
+                t.add_row([get_color(col),
+                           get_color(value),
+                           get_color(str(type(value))),
+                           get_color(rules_columns_all[col][0]),
+                           get_color(rules_columns_all[col][1])
+                           ])
         print(t)
```

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools/utils/templates/table.html` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
-Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
@@ -110,7 +112,9 @@
 
 - choco install visualcpp-build-tools
 
 ## Reference
 
 - Jonathan Quiza [github](https://github.com/jonaqp).
 - Jonathan Quiza [RumiMLSpark](http://rumi-ml.herokuapp.com/).
+
+
```

### Comparing `spark_quality_rules_tools-0.2.4/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.2.5/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

