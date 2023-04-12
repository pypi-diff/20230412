# Comparing `tmp/openapi_markdown-0.0.3.tar.gz` & `tmp/openapi_markdown-0.0.4.tar.gz`

## Comparing `openapi_markdown-0.0.3.tar` & `openapi_markdown-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/pypi.sh
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/requirement.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/src/openapi_markdown/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/src/openapi_markdown/generator.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/src/openapi_markdown/templates/api_doc_template.md.j2
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/src/openapi_markdown/templates/example.md.j2
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/tests/openapi.json
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/tests/test.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/LICENSE
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 openapi_markdown-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/pypi.sh
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/requirement.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/__init__.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/generator.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/templates/api_doc_template.md.j2
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/src/openapi_markdown/templates/example.md.j2
+-rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/tests/openapi.json
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/tests/test.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/LICENSE
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 openapi_markdown-0.0.4/PKG-INFO
```

### Comparing `openapi_markdown-0.0.3/src/openapi_markdown/generator.py` & `openapi_markdown-0.0.4/src/openapi_markdown/generator.py`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.3/src/openapi_markdown/templates/api_doc_template.md.j2` & `openapi_markdown-0.0.4/src/openapi_markdown/templates/api_doc_template.md.j2`

 * *Files 1% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 | Name | Type | Required | Description |
 |------|------|----------|-------------|
 {% for param in operation.parameters
 %}| {{ param.name }} | {{ param.schema.type }} | {{ param.required }} | {{ param.description }} |
 {% endfor %}
 {% endif %}
 
-{% if operation.request_body %}
+{% if operation.requestBody %}
 #### Request Body
 
-{% if 'application/json' in operation.request_body.content %}
-{{ operation.request_body.content['application/json'].schema | ref_to_link }}
+{% if 'application/json' in operation.requestBody.content %}
+{{ operation.requestBody.content['application/json'].schema | ref_to_link }}
 {% endif %}
-{% if '*/*' in operation.request_body.content %}
-{{ operation.request_body.content['*/*'].schema | ref_to_link  }}
+{% if '*/*' in operation.requestBody.content %}
+{{ operation.requestBody.content['*/*'].schema | ref_to_link  }}
 {% endif %}
 
 
 {% endif %}
 
 #### Responses
```

### Comparing `openapi_markdown-0.0.3/LICENSE` & `openapi_markdown-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.3/README.md` & `openapi_markdown-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `openapi_markdown-0.0.3/pyproject.toml` & `openapi_markdown-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openapi-markdown"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="soonoh", email="soonoh.jung@vrerv.com" },
 ]
 description = "Generates API documentation from an OpenAPI specification file"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `openapi_markdown-0.0.3/PKG-INFO` & `openapi_markdown-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-markdown
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generates API documentation from an OpenAPI specification file
 Project-URL: Homepage, https://github.com/vrerv/openapi-markdown
 Project-URL: Bug Tracker, https://github.com/vrerv/openapi-markdown/issues
 Author-email: soonoh <soonoh.jung@vrerv.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

