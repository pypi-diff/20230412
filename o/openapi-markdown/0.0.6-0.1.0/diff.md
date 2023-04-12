# Comparing `tmp/openapi_markdown-0.0.6.tar.gz` & `tmp/openapi_markdown-0.1.0.tar.gz`

## Comparing `openapi_markdown-0.0.6.tar` & `openapi_markdown-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/pypi.sh
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/src/openapi_markdown/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/src/openapi_markdown/generator.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/src/openapi_markdown/templates/api_doc_template.md.j2
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/src/openapi_markdown/templates/example.md.j2
--rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/tests/openapi.json
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/tests/test.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/LICENSE
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 openapi_markdown-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/pypi.sh
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/src/openapi_markdown/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/src/openapi_markdown/generator.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/src/openapi_markdown/templates/api_doc_template.md.j2
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/src/openapi_markdown/templates/example.md.j2
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/src/openapi_markdown/templates/security_scheme.md.j2
+-rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/tests/openapi.json
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/tests/test.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/LICENSE
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 openapi_markdown-0.1.0/PKG-INFO
```

### Comparing `openapi_markdown-0.0.6/src/openapi_markdown/generator.py` & `openapi_markdown-0.1.0/src/openapi_markdown/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
             return f"[{schema_name}](#{schema_name.lower()})"
         elif key == 'type':
             return f"{ref[key]}"
         else:
             return 'Not implemented type}'
 
 
-
 def to_markdown(api_file, output_file):
     # Load the OpenAPI 3.0 specification file in either JSON or YAML format
     with open(api_file) as f:
         spec_data = json.load(f) if api_file.endswith(".json") else yaml.safe_load(f)
     spec = Spec.from_dict(spec_data)
     # Load the Jinja2 template file
     if os.path.exists('templates'):
```

### Comparing `openapi_markdown-0.0.6/src/openapi_markdown/templates/api_doc_template.md.j2` & `openapi_markdown-0.1.0/src/openapi_markdown/templates/api_doc_template.md.j2`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 {% for server in spec.servers
 %}| {{ server.url }} | {{ server.description }} |
 {% endfor %}
 
 
 ## Authentication
 
-{{ spec.components.security_schemes }}
+{% with root = spec.components %}
+{% include './security_scheme.md.j2' %}
+{% endwith %}
 
 ## APIs
 
 {% for path, methods in spec.paths.items() %}
 
 {% for method, operation in methods.items() %}
 ### {{ method.upper() }} {{ path }}
@@ -59,15 +61,17 @@
 
 {% if response.description %}
 {{ response.description }}
 {% endif %}
 
 {% if 'application/json' in response.content %}
 {{ response.content['application/json'].schema | ref_to_link  }}
+{% with root = response.content['application/json'] %}
 {% include './example.md.j2' %}
+{% endwith %}
 {% endif %}
 {% if '*/*' in response.content %}
 {{ response.content['*/*'].schema | ref_to_link  }}
 {% with root = response.content['*/*'] %}
 {% include "./example.md.j2" %}
 {% endwith %}
 {% endif %}
```

### Comparing `openapi_markdown-0.0.6/tests/openapi.json` & `openapi_markdown-0.1.0/tests/openapi.json`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.6/LICENSE` & `openapi_markdown-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.6/README.md` & `openapi_markdown-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.6/pyproject.toml` & `openapi_markdown-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openapi-markdown"
-version = "0.0.6"
+version = "0.1.0"
 authors = [
     { name="soonoh", email="soonoh.jung@vrerv.com" },
 ]
 description = "Generates API documentation from an OpenAPI specification file"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `openapi_markdown-0.0.6/PKG-INFO` & `openapi_markdown-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-markdown
-Version: 0.0.6
+Version: 0.1.0
 Summary: Generates API documentation from an OpenAPI specification file
 Project-URL: Homepage, https://github.com/vrerv/openapi-markdown
 Project-URL: Bug Tracker, https://github.com/vrerv/openapi-markdown/issues
 Author-email: soonoh <soonoh.jung@vrerv.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

