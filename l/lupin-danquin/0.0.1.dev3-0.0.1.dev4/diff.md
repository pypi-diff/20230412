# Comparing `tmp/lupin-danquin-0.0.1.dev3.tar.gz` & `tmp/lupin-danquin-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev3.tar", last modified: Tue Apr 11 08:33:32 2023, max compression
+gzip compressed data, was "lupin-danquin-0.0.1.dev4.tar", last modified: Wed Apr 12 09:43:14 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev3.tar` & `lupin-danquin-0.0.1.dev4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.927216 lupin-danquin-0.0.1.dev3/
--rw-rw-rw-   0        0        0     1093 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev3/LICENCE
--rw-rw-rw-   0        0        0       67 2023-04-11 08:12:17.000000 lupin-danquin-0.0.1.dev3/MANIFEST.in
--rw-rw-rw-   0        0        0      573 2023-04-11 08:33:32.927216 lupin-danquin-0.0.1.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     1010 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.895696 lupin-danquin-0.0.1.dev3/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-09 16:33:06.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.914700 lupin-danquin-0.0.1.dev3/lupin_danquin/assets/
--rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/assets/BeginingOfFile.md
--rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/assets/EndOfFile.md
--rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/check_coding_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.923216 lupin-danquin-0.0.1.dev3/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/application.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-09 15:14:46.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.924219 lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0     1917 2023-04-09 21:52:28.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.926214 lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     3261 2023-04-11 08:28:18.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     1438 2023-04-11 08:14:47.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/run.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.927216 lupin-danquin-0.0.1.dev3/lupin_danquin/templates/
--rw-rw-rw-   0        0        0     2728 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/templates/val3_documentation_md.j2
-drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.912699 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 16:34:59.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      906 2023-04-11 08:33:32.928214 lupin-danquin-0.0.1.dev3/setup.cfg
--rw-rw-rw-   0        0        0      172 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.775613 lupin-danquin-0.0.1.dev4/
+-rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev4/LICENCE
+-rw-rw-rw-   0        0        0       67 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev4/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2023-04-12 09:43:14.775613 lupin-danquin-0.0.1.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     1010 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.749589 lupin-danquin-0.0.1.dev4/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-12 09:43:14.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.765103 lupin-danquin-0.0.1.dev4/lupin_danquin/assets/
+-rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/assets/BeginingOfFile.md
+-rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/assets/EndOfFile.md
+-rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/check_coding_rules.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.771616 lupin-danquin-0.0.1.dev4/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/application.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.773616 lupin-danquin-0.0.1.dev4/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     2206 2023-04-12 08:36:50.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.774613 lupin-danquin-0.0.1.dev4/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     2952 2023-04-12 08:23:58.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     2509 2023-04-12 08:32:27.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.775613 lupin-danquin-0.0.1.dev4/lupin_danquin/templates/
+-rw-rw-rw-   0        0        0     2801 2023-04-11 15:18:48.000000 lupin-danquin-0.0.1.dev4/lupin_danquin/templates/val3_documentation_md.j2
+drwxrwxrwx   0        0        0        0 2023-04-12 09:43:14.764103 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-12 09:43:14.000000 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-12 09:43:14.000000 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:43:14.000000 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-12 09:43:14.000000 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-12 09:43:14.000000 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 09:43:14.000000 lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-04-12 09:43:14.776614 lupin-danquin-0.0.1.dev4/setup.cfg
+-rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev4/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev3/LICENCE` & `lupin-danquin-0.0.1.dev4/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/PKG-INFO` & `lupin-danquin-0.0.1.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev3/README.md` & `lupin-danquin-0.0.1.dev4/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/assets/BeginingOfFile.md` & `lupin-danquin-0.0.1.dev4/lupin_danquin/assets/BeginingOfFile.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/check_coding_rules.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/check_coding_rules.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/core/application.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/core/global_variable.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/core/local_variable.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/core/parameter.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/core/program.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/utils.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/core/tools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+import codecs
 import logging
 import os
 import re
 import sys
 
 
 def must_get_string_value_from_env_var(var_name: str):
@@ -32,21 +33,20 @@
     sys.exit(1)
 
 
 def info(msg: str) -> None:
     logging.info(msg)
 
 
-def get_version():
+def update_version():
     """get version from setup.cfg file and
     update __version__ in lupin_danquin.__init__.py
     """
     with open("setup.cfg", "r", encoding="utf-8") as f:
         setup_cfg = f.read()
-    print(setup_cfg)
     _version = re.search(
         r"(^version = )(\d{1,2}\.\d{1,2}\.\d{1,2})(\.[a-z]{1,})?(\d{1,2})?",
         setup_cfg,
         re.MULTILINE,
     )
     version = ""
     for group in _version.group(2, 3, 4):
@@ -63,7 +63,16 @@
     """Convert application name to list.
     Args:
         application_name (str): The name of the application.
     Returns:
         list: The list of the application name.
     """
     return [app.strip() for app in application_name.split(",") if app.strip()]
+
+
+def read_file(file_path: str) -> str:
+    if not os.path.exists(file_path):
+        die(msg=f"File '{file_path}' does not exist.")
+    info(msg=f"Get informations from {file_path}")
+    with codecs.open(file_path, encoding="utf-8") as f:
+        result = f.read()
+    return result
```

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-0.0.1.dev4/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,36 +29,26 @@
     def _get_informations_from_applications(
         self, application_names: List
     ) -> List[Dict[str, Any]]:
         """Get all informations from applications"""
 
         apps_information = []
         base_program_path = self._find_usrapp_dir() + os.sep
-        print(f"base_program_path: {base_program_path}")
         for application_name in application_names:
             program_path = base_program_path + application_name
+            if not os.path.isdir(program_path):
+                die(msg=f"Application '{application_name}' not found")
+            info(msg=f"Get informations from '{application_name}'")
             apps_information.append(
                 Application(
                     program_path, application_name
                 ).get_all_information_from_app()
             )
         return apps_information
 
-    def _read_begining_of_file(self) -> str:
-        with codecs.open(
-            "lupin_danquin/assets/BeginingOfFile.md", encoding="utf-8"
-        ) as f:
-            result = f.read()
-        return result
-
-    def _read_end_of_file(self) -> str:
-        with codecs.open("lupin_danquin/assets/EndOfFile.md", encoding="utf-8") as f:
-            result = f.read()
-        return result
-
     def _get_local_template(self) -> Template:
         try:
             # Create jinja2 environment
             env = Environment(
                 loader=PackageLoader("lupin_danquin", "templates"),
                 autoescape=select_autoescape(),
                 trim_blocks=True,
@@ -68,20 +58,21 @@
             template = env.get_template("val3_documentation_md.j2")
             return template
         except TemplateNotFound:
             die(
                 msg="Template 'lupin_danquin/templates/val3_documentation_md.j2 not found"
             )
 
-    def generate_markdown(self, applications_list: List) -> None:
+    def generate_markdown(
+        self, applications_list: List, begining_of_file, end_of_file
+    ) -> None:
         """Generate the documentation"""
-        info(msg="Get informations from VAL3 applications")
         context = {
-            "begining_of_file": self._read_begining_of_file(),
-            "end_of_file": self._read_end_of_file(),
+            "beginning_of_file": begining_of_file,
+            "end_of_file": end_of_file,
             "applications": self._get_informations_from_applications(applications_list),
         }
 
         template = self._get_local_template()
         try:
             content = template.render(context)
         except (TemplateError, TemplateRuntimeError) as e:
```

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin/templates/val3_documentation_md.j2` & `lupin-danquin-0.0.1.dev4/lupin_danquin/templates/val3_documentation_md.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-{{ begining_of_file }}
-
+{% if beginning_of_file %}
+{{ beginning_of_file }}
+{% endif %}
 {% for app in applications %}
 {% set name = app.name %}
 {% set description = app.description %}
 {% set dependencies = app.dependencies %}
 {% set type_dependencies = app.type_dependencies %}
 {% set global_variables = app.global_variables %}
 {% set private_program_list = app.private_program_list %}
@@ -89,9 +90,10 @@
 {% endfor %}
 {% endif %}
 {{ public_program.description }}
 {% endfor %}
 {% endif %}
 
 {% endfor %}
-
-{{ end_of_file }}
+{% if end_of_file %}
+{{ end_of_file }}
+{% endif %}
```

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-0.0.1.dev4/lupin_danquin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev3/setup.cfg` & `lupin-danquin-0.0.1.dev4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 312e 6465 7633 0d0a 6465 7363 7269 7074  1.dev3..descript
+00000030: 312e 6465 7634 0d0a 6465 7363 7269 7074  1.dev4..descript
 00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
 00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
 00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
 00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
 00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
 000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords =
```

