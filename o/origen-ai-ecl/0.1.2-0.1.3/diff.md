# Comparing `tmp/origen_ai_ecl-0.1.2.tar.gz` & `tmp/origen_ai_ecl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "origen_ai_ecl-0.1.2.tar", max compression
+gzip compressed data, was "origen_ai_ecl-0.1.3.tar", max compression
```

## Comparing `origen_ai_ecl-0.1.2.tar` & `origen_ai_ecl-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      838 2023-04-11 17:02:03.162509 origen_ai_ecl-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-12 09:13:45.683953 origen_ai_ecl-0.1.2/origen/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:13:45.683953 origen_ai_ecl-0.1.2/origen/ai/__init__.py
--rw-r--r--   0        0        0      146 2023-04-12 09:14:10.540759 origen_ai_ecl-0.1.2/origen/ai/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   733080 2023-04-12 09:13:45.637953 origen_ai_ecl-0.1.2/origen/ai/ecl.cpython-311-x86_64-linux-gnu.so
--rw-r--r--   0        0        0     2128 2023-04-12 09:50:58.274202 origen_ai_ecl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1393 1970-01-01 00:00:00.000000 origen_ai_ecl-0.1.2/setup.py
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 origen_ai_ecl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      838 2023-04-11 17:02:03.162509 origen_ai_ecl-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 09:51:45.402868 origen_ai_ecl-0.1.3/origen/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 09:51:45.402868 origen_ai_ecl-0.1.3/origen/ai/__init__.py
+-rwxr-xr-x   0        0        0   733080 2023-04-12 09:51:45.364868 origen_ai_ecl-0.1.3/origen/ai/ecl.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0     2128 2023-04-12 09:52:04.830730 origen_ai_ecl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1393 1970-01-01 00:00:00.000000 origen_ai_ecl-0.1.3/setup.py
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 origen_ai_ecl-0.1.3/PKG-INFO
```

### Comparing `origen_ai_ecl-0.1.2/README.md` & `origen_ai_ecl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `origen_ai_ecl-0.1.2/origen/ai/ecl.cpython-311-x86_64-linux-gnu.so` & `origen_ai_ecl-0.1.3/origen/ai/ecl.cpython-311-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `origen_ai_ecl-0.1.2/pyproject.toml` & `origen_ai_ecl-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "origen-ai-ecl"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Luis Arce <luis@origen.ai>"]
 readme = "README.md"
 packages = [{include = "origen/**/*"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `origen_ai_ecl-0.1.2/setup.py` & `origen_ai_ecl-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['origen', 'origen.ai']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'origen-ai-ecl',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '',
     'long_description': '# opm-origen\n\n## Prerequisites\n\n- Install make, cmake and g++\n- Build/Install Opm-Common\n- Build/Install Opm-Grid\n\n## Install opm packages\n\n```bash\nsudo apt-add-repository ppa:opm/ppa\nsudo apt-get update\n\nsudo apt-get install libopm-common-dev\nsudo apt-get install libopm-grid-dev\n```\n\n## How to build\n\n```bash\ngit clone git@github.com:OriGenAI/opm-origen.git\ncd opm-origen\nmkdir build\ncd build\ncmake ..\nmake\n```\n\n## How to use\n\n- Copy the binary under `build/lib` folder\n- Import the binary from your Python code\n- Call the library functions\n\n## Example\n\n```python\nfrom origen.ai.ecl import read_transmissibility\n\ntrans = read_transmissibility("path-to-data.DATA")\nprint(trans)\n```\n\n## Develop\n\nYou can use the main.cpp file to debug. Just call your function from there and compile the code. You will find the binary in `build/bin/main`\n',
     'author': 'Luis Arce',
     'author_email': 'luis@origen.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `origen_ai_ecl-0.1.2/PKG-INFO` & `origen_ai_ecl-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: origen-ai-ecl
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Luis Arce
 Author-email: luis@origen.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

