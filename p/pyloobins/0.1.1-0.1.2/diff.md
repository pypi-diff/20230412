# Comparing `tmp/pyloobins-0.1.1.tar.gz` & `tmp/pyloobins-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.1.tar", max compression
+gzip compressed data, was "pyloobins-0.1.2.tar", max compression
```

## Comparing `pyloobins-0.1.1.tar` & `pyloobins-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-11 00:56:15.923700 pyloobins-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.451802 pyloobins-0.1.1/LOOBins/.gitkeep
--rw-r--r--   0        0        0      331 2023-04-11 00:56:15.923980 pyloobins-0.1.1/README.md
--rw-r--r--   0        0        0      844 2023-04-11 00:56:33.886265 pyloobins-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.1/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-11 00:56:15.925235 pyloobins-0.1.1/src/pyloobins/cli.py
--rw-r--r--   0        0        0     3582 2023-04-11 00:56:15.925856 pyloobins-0.1.1/src/pyloobins/models.py
--rw-r--r--   0        0        0     1056 2023-04-11 00:56:15.926235 pyloobins-0.1.1/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     1965 2023-04-11 00:56:15.926520 pyloobins-0.1.1/src/pyloobins/util.py
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 pyloobins-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1295 2023-04-12 01:43:08.133020 pyloobins-0.1.2/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0      331 2023-04-11 23:56:04.085703 pyloobins-0.1.2/README.md
+-rw-r--r--   0        0        0      877 2023-04-12 01:51:41.595228 pyloobins-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.2/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-11 23:56:04.085870 pyloobins-0.1.2/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     3582 2023-04-11 23:56:04.086003 pyloobins-0.1.2/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1177 2023-04-12 00:48:36.484104 pyloobins-0.1.2/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2610 2023-04-11 23:58:27.122687 pyloobins-0.1.2/src/pyloobins/util.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 pyloobins-0.1.2/PKG-INFO
```

### Comparing `pyloobins-0.1.1/LICENSE` & `pyloobins-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.1/pyproject.toml` & `pyloobins-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
 readme = "README.md"
 packages = [{include = "pyloobins", from = "src"}]
-include = ["LOOBins/*"]
+include = ["LOOBins/*.yml"]
 homepage = "https://loobins.io/"
 repository = "https://github.com/infosecB/LOOBins"
 keywords = ["cybersecurity", "cli", "lol"]
+license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.5"
 pyyaml = "^6.0"
 click = "^8.1.3"
 jinja2 = "^3.1.2"
```

### Comparing `pyloobins-0.1.1/src/pyloobins/cli.py` & `pyloobins-0.1.2/src/pyloobins/cli.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.1/src/pyloobins/models.py` & `pyloobins-0.1.2/src/pyloobins/models.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.1/src/pyloobins/templates/loobin.md.j2` & `pyloobins-0.1.2/src/pyloobins/templates/loobin.md.j2`

 * *Files 20% similar despite different names*

```diff
@@ -14,36 +14,40 @@
 tags: {{ tags }}
 ---
 
 # {{ loobin.name }}
 {{ loobin.full_description }}
 | Created | Tactics | Tags |
 |---|---|---|
-| {{ loobin.created }} | {% for t in tags %}<span class="badge text-bg-secondary">{{ t }}</span>{% endfor %} | <span class="badge text-bg-danger">TACTIC8</span>  |
+| {{ loobin.created }} | {% for t in tactics %}<span class="badge text-bg-danger">{{ t }}</span> {% endfor %}  | {% for t in tags %}<span class="badge text-bg-secondary">{{ t }}</span> {% endfor %} | 
 
 ## Paths
 {% for path in loobin.paths %}
-- {{ path }}
+- `{{ path }}`
 {% endfor %}
 
-## Example Usage
+## Use Cases
 {% for example in loobin.example_use_cases %}
-### {{ example.name }}
+#### {{ example.name }}
 {{ example.description }}
 
 `{{ example.code }}`
 {% endfor %}
 
 ## Detections
 {% for detection in loobin.detections %}
 - [{{ detection.name }}]({{ detection.url }})
 {% endfor %}
 
-# Resources
+{% if loobin.resources %}
+## Resources
 {% for resource in loobin.resources %}
 - [{{ resource.name }}]({{ resource.url }})
 {% endfor %}
+{% endif %}
 
-# Acknowledgements
+{% if loobin.acknowledgements %}
+## Acknowledgements
 {% for acknowledgement in loobin.acknowledgements %}
 - {{ acknowledgement }}
 {% endfor %}
+{% endif %}
```

### Comparing `pyloobins-0.1.1/src/pyloobins/util.py` & `pyloobins-0.1.2/src/pyloobins/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,35 @@
 """Utility functions that support the CLI and library"""
+import pathlib
+import site
 from datetime import date
 
 import yaml
 
 from .models import Detection, ExampleUseCase, LOOBin, Resource
 
 
+def get_loobins() -> list:
+    """Returns a list of LOOBin objects"""
+    loobins = []
+    yml_files = (pathlib.Path(site.getsitepackages()[0]) / "LOOBins").glob("**/*.yml")
+    for yml_file in yml_files:
+        with open(yml_file, "r", encoding="utf-8") as stream:
+            try:
+                yml_content = yaml.safe_load(stream)
+            except yaml.YAMLError as exc:
+                print(exc)
+        try:
+            loobins.append(LOOBin(**yml_content))  # type: ignore
+        except Exception as exc:
+            # TODO add more specific Exception handling
+            print(exc)
+    return loobins
+
+
 def validate_loobin(yml_path: str) -> bool:
     """Validates LOOBin YAML file"""
     with open(yml_path, "r", encoding="utf-8") as stream:
         try:
             yml_content = yaml.safe_load(stream)
         except yaml.YAMLError as exc:
             print(exc)
```

### Comparing `pyloobins-0.1.1/PKG-INFO` & `pyloobins-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pyloobins
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for managing the LOOBins model and schema.
 Home-page: https://loobins.io/
+License: GPL-3.0-or-later
 Keywords: cybersecurity,cli,lol
 Author: infosecB
 Author-email: brendan@infosecb.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
```

