# Comparing `tmp/lupin-danquin-0.0.1.dev8.tar.gz` & `tmp/lupin-danquin-0.0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev8.tar", last modified: Wed Apr 12 10:49:45 2023, max compression
+gzip compressed data, was "lupin-danquin-0.0.1.dev9.tar", last modified: Wed Apr 12 14:56:49 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev8.tar` & `lupin-danquin-0.0.1.dev9.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.781654 lupin-danquin-0.0.1.dev8/
--rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev8/LICENCE
--rw-rw-rw-   0        0        0       67 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev8/MANIFEST.in
--rw-rw-rw-   0        0        0      573 2023-04-12 10:49:45.781654 lupin-danquin-0.0.1.dev8/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-04-12 10:45:59.000000 lupin-danquin-0.0.1.dev8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.755178 lupin-danquin-0.0.1.dev8/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-11 14:20:34.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.771301 lupin-danquin-0.0.1.dev8/lupin_danquin/assets/
--rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/assets/BeginingOfFile.md
--rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/assets/EndOfFile.md
--rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/check_coding_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.777300 lupin-danquin-0.0.1.dev8/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/application.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.778303 lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0     2206 2023-04-12 08:36:50.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.780656 lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     2948 2023-04-12 09:51:31.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     2509 2023-04-12 08:32:27.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/run.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.780656 lupin-danquin-0.0.1.dev8/lupin_danquin/templates/
--rw-rw-rw-   0        0        0     2801 2023-04-11 15:18:48.000000 lupin-danquin-0.0.1.dev8/lupin_danquin/templates/val3_documentation_md.j2
-drwxrwxrwx   0        0        0        0 2023-04-12 10:49:45.769301 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 10:49:45.000000 lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      906 2023-04-12 10:49:45.782655 lupin-danquin-0.0.1.dev8/setup.cfg
--rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.990008 lupin-danquin-0.0.1.dev9/
+-rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev9/LICENCE
+-rw-rw-rw-   0        0        0       67 2023-04-12 12:24:19.000000 lupin-danquin-0.0.1.dev9/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2023-04-12 14:56:49.990008 lupin-danquin-0.0.1.dev9/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-04-12 12:25:35.000000 lupin-danquin-0.0.1.dev9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.949904 lupin-danquin-0.0.1.dev9/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-12 12:24:19.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.969651 lupin-danquin-0.0.1.dev9/lupin_danquin/assets/
+-rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/assets/BeginingOfFile.md
+-rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/assets/EndOfFile.md
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.981118 lupin-danquin-0.0.1.dev9/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/application.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.984008 lupin-danquin-0.0.1.dev9/lupin_danquin/core/coding_rules_validator/
+-rw-rw-rw-   0        0        0        0 2023-04-12 13:03:44.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/coding_rules_validator/__init__.py
+-rw-rw-rw-   0        0        0     1339 2023-04-12 14:40:35.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.986007 lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     2008 2023-04-12 14:39:37.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.988007 lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     2657 2023-04-12 14:54:07.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     3078 2023-04-12 14:56:15.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.989009 lupin-danquin-0.0.1.dev9/lupin_danquin/templates/
+-rw-rw-rw-   0        0        0     2801 2023-04-12 12:24:19.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/templates/val3_documentation_md.j2
+drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.966976 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1069 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-04-12 14:56:49.992526 lupin-danquin-0.0.1.dev9/setup.cfg
+-rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev9/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev8/LICENCE` & `lupin-danquin-0.0.1.dev9/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/PKG-INFO` & `lupin-danquin-0.0.1.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev8/README.md` & `lupin-danquin-0.0.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/assets/BeginingOfFile.md` & `lupin-danquin-0.0.1.dev9/lupin_danquin/assets/BeginingOfFile.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/core/application.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/core/global_variable.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/core/local_variable.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/core/parameter.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/core/program.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/core/tools/utils.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,14 @@
 import codecs
 import logging
 import os
 import re
 import sys
 
 
-def must_get_string_value_from_env_var(var_name: str):
-    """Get a string value from an environment variable.
-    Args:
-        var_name (str): The name of the environment variable.
-    Returns:
-        str: The value of the environment variable.
-    Logs:
-        Error: If the environment {var_name} variable is not set.
-        sys.exit(1)
-    """
-    if not os.getenv(var_name):
-        logging.error(f"Environment variable {var_name} is not set.")
-        sys.exit(1)
-    return os.getenv(var_name)
-
-
 def configure_logging():
     logging.basicConfig(
         format="%(asctime)s %(levelname)s: %(message)s", level=logging.INFO
     )
 
 
 def die(msg: str) -> None:
@@ -33,14 +17,18 @@
     sys.exit(1)
 
 
 def info(msg: str) -> None:
     logging.info(msg)
 
 
+def warn(msg: str) -> None:
+    logging.warning(msg)
+
+
 def update_version():
     """get version from setup.cfg file and
     update __version__ in lupin_danquin.__init__.py
     """
     with open("setup.cfg", "r", encoding="utf-8") as f:
         setup_cfg = f.read()
     _version = re.search(
@@ -72,7 +60,15 @@
 def read_file(file_path: str) -> str:
     if not os.path.exists(file_path):
         die(msg=f"File '{file_path}' does not exist.")
     info(msg=f"Get informations from {file_path}")
     with codecs.open(file_path, encoding="utf-8") as f:
         result = f.read()
     return result
+
+
+def find_usrapp_dir() -> str:
+    """Find the usrapp directory"""
+    for dirpath, dirnames, filenames in os.walk(os.getcwd()):
+        if "usrapp" in dirnames:
+            return os.path.join(dirpath, "usrapp")
+    die(msg="'usrapp' directory not found")
```

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,34 +9,28 @@
     Template,
     TemplateNotFound,
     TemplateError,
     TemplateRuntimeError,
 )
 
 from lupin_danquin.core.application import Application
-from lupin_danquin.core.tools.utils import die, info
+from lupin_danquin.core.tools.utils import die, find_usrapp_dir, info
 
 
 class Val3Documentation:
-    USR_APP_DIR = "usrapp"
-
-    def _find_usrapp_dir(self) -> str:
-        """Find the usrapp directory"""
-        for dirpath, dirnames, filenames in os.walk(os.getcwd()):
-            if self.USR_APP_DIR in dirnames:
-                return os.path.join(dirpath, self.USR_APP_DIR)
-        die(msg=f"'{self.USR_APP_DIR}' directory not found")
+    def __init__(self):
+        self.user_app_dir = find_usrapp_dir()
 
     def _get_informations_from_applications(
         self, application_names: List
     ) -> List[Dict[str, Any]]:
         """Get all informations from applications"""
 
         apps_information = []
-        base_program_path = self._find_usrapp_dir() + os.sep
+        base_program_path = self.user_app_dir + os.sep
         for application_name in application_names:
             program_path = base_program_path + application_name
             if not os.path.isdir(program_path):
                 die(msg=f"Application '{application_name}' not found")
             info(msg=f"Get informations from '{application_name}'")
             apps_information.append(
                 Application(
@@ -74,12 +68,10 @@
 
         template = self._get_local_template()
         try:
             content = template.render(context)
         except (TemplateError, TemplateRuntimeError) as e:
             die(msg=f"Error rendering Jinja2 template: {e}")
 
-        with codecs.open(
-            "./val3_documentation.md", "w", encoding="utf-8"
-        ) as f:
+        with codecs.open("./val3_documentation.md", "w", encoding="utf-8") as f:
             f.write(content)
         info(msg="val3_documentation.md generated")
```

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/run.py` & `lupin-danquin-0.0.1.dev9/lupin_danquin/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 import typer
 
 from lupin_danquin.core.tools.utils import (
     configure_logging,
     convert_application_name_to_list,
     read_file,
 )
+
+from lupin_danquin.core.coding_rules_validator.coging_rules_validator import (
+    CodingRulesValidator,
+)
 from lupin_danquin.core.val3_doc_generator.val3_doc_generator import Val3Documentation
-from lupin_danquin.__init__ import __version__
+from lupin_danquin import __version__
 
 
 load_dotenv()
 
 
 cli = typer.Typer()
 
@@ -21,15 +25,15 @@
 @cli.command(help="Print version")
 def version():
     print(f"Version: {__version__}")
 
 
 @cli.command()
 def valdocs(
-    application_names: Optional[str] = typer.Argument(
+    application_names: str = typer.Argument(
         ...,
         help="Name of applications to be documented. Ex: 'app1,app2,app3'",
         envvar="VAL3_APPLICATIONS",
     ),
     beginning_file_path: Optional[str] = typer.Option(
         None,
         "--beginning-file-path",
@@ -56,20 +60,40 @@
     :param end_file_path: Path to the file containing the end content of the documentation
     :type end_file_path: str
     :example: danq valdocs "App1,App2" --beginning-file-path "beginning.txt" --end-file-path "end.txt"
     or danq valdocs "App1,App2" -b "beginning.txt" -e "end.txt"
     """
     configure_logging()
 
+    applications_list = convert_application_name_to_list(application_names)
+
     if not beginning_file_path:
         begining_of_file = ""
     else:
         begining_of_file = read_file(beginning_file_path)
     if not end_file_path:
         end_of_file = ""
     else:
         end_of_file = read_file(end_file_path)
 
-    applications_list = convert_application_name_to_list(application_names)
     Val3Documentation().generate_markdown(
         applications_list, begining_of_file, end_of_file
     )
+
+
+@cli.command()
+def check_coding_rules(
+    application_names: str = typer.Argument(
+        ...,
+        help="Name of applications to be check. Ex: 'app1,app2,app3'",
+        envvar="VAL3_APPLICATIONS",
+    )
+):
+    """
+    Check coding rules
+    """
+    configure_logging()
+
+    applications_list = convert_application_name_to_list(application_names)
+
+    check_coding_rules = CodingRulesValidator(applications_list)
+    check_coding_rules.validate()
```

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin/templates/val3_documentation_md.j2` & `lupin-danquin-0.0.1.dev9/lupin_danquin/templates/val3_documentation_md.j2`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev8
+Version: 0.0.1.dev9
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev8/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENCE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 lupin_danquin/__init__.py
 lupin_danquin/__main__.py
-lupin_danquin/check_coding_rules.py
 lupin_danquin/run.py
 lupin_danquin.egg-info/PKG-INFO
 lupin_danquin.egg-info/SOURCES.txt
 lupin_danquin.egg-info/dependency_links.txt
 lupin_danquin.egg-info/entry_points.txt
 lupin_danquin.egg-info/not-zip-safe
 lupin_danquin.egg-info/requires.txt
@@ -20,12 +19,14 @@
 lupin_danquin/core/application.py
 lupin_danquin/core/global_variable.py
 lupin_danquin/core/line_ended.py
 lupin_danquin/core/local_variable.py
 lupin_danquin/core/parameter.py
 lupin_danquin/core/program.py
 lupin_danquin/core/rules.py
+lupin_danquin/core/coding_rules_validator/__init__.py
+lupin_danquin/core/coding_rules_validator/coging_rules_validator.py
 lupin_danquin/core/tools/__init__.py
 lupin_danquin/core/tools/utils.py
 lupin_danquin/core/val3_doc_generator/__init__.py
 lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
 lupin_danquin/templates/val3_documentation_md.j2
```

### Comparing `lupin-danquin-0.0.1.dev8/setup.cfg` & `lupin-danquin-0.0.1.dev9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 312e 6465 7638 0d0a 6465 7363 7269 7074  1.dev8..descript
+00000030: 312e 6465 7639 0d0a 6465 7363 7269 7074  1.dev9..descript
 00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
 00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
 00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
 00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
 00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
 000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords =
```

