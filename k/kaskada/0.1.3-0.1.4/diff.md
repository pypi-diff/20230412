# Comparing `tmp/kaskada-0.1.3.tar.gz` & `tmp/kaskada-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.1.3.tar", max compression
+gzip compressed data, was "kaskada-0.1.4.tar", max compression
```

## Comparing `kaskada-0.1.3.tar` & `kaskada-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,83 @@
--rw-r--r--   0        0        0     1098 2023-04-11 22:38:35.487057 kaskada-0.1.3/README.md
--rw-r--r--   0        0        0     3387 2023-04-11 22:38:35.487057 kaskada-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7084 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/fenlmagic/utils.py
--rw-r--r--   0        0        0     1179 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0     6381 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/api/release.py
--rw-r--r--   0        0        0     8961 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/api/session.py
--rw-r--r--   0        0        0     5688 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-04-11 22:38:35.487057 kaskada-0.1.3/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7318 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0     9805 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0     8594 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9232 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10098 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/table.py
--rw-r--r--   0        0        0     6690 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/utils.py
--rw-r--r--   0        0        0     4515 2023-04-11 22:38:35.491057 kaskada-0.1.3/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-11 22:38:35.491057 kaskada-0.1.3/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     2266 1970-01-01 00:00:00.000000 kaskada-0.1.3/setup.py
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 kaskada-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-04-11 22:38:35.487057 kaskada-0.1.4/README.md
+-rw-r--r--   0        0        0     3223 2023-04-11 23:54:13.671660 kaskada-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7084 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0     1546 2023-04-11 23:46:04.727618 kaskada-0.1.4/src/kaskada/api/__pycache__/api_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     5350 2023-04-11 23:46:04.731618 kaskada-0.1.4/src/kaskada/api/__pycache__/release.cpython-310.pyc
+-rw-r--r--   0        0        0     8797 2023-04-11 23:46:04.727618 kaskada-0.1.4/src/kaskada/api/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0     1179 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0     6381 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     8961 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/api/session.py
+-rw-r--r--   0        0        0     5688 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-04-11 22:38:35.487057 kaskada-0.1.4/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7318 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0     9805 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0     6457 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/common_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     3499 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/destinations_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2491 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/fenl_diagnostics_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     7685 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4932 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/materialization_service_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0     1570 2023-04-11 23:46:03.995632 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/options_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2461 2023-04-11 23:46:04.647619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/pulsar_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     8772 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     3917 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/query_service_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0     3255 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/schema_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2169 2023-04-11 23:46:04.651619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/sources_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     7592 2023-04-11 23:46:04.647619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4952 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/table_service_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0     3806 2023-04-11 23:46:03.991632 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      425 2023-04-11 23:46:03.999632 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/test_cases_pb2_grpc.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     5783 2023-04-11 23:46:04.655619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4330 2023-04-11 23:46:04.659619 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/__pycache__/view_service_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0    13053 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    16901 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0     6628 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5994 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6043 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     3526 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     6348 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0    15562 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1846 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    21703 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     4981 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3561 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    16795 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4886 2023-04-11 23:44:52.285139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     3258 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2882 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    15322 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6835 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0    11387 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    26185 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-04-11 23:44:52.289139 kaskada-0.1.4/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8594 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9232 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10098 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/table.py
+-rw-r--r--   0        0        0     6690 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4515 2023-04-11 22:38:35.491057 kaskada-0.1.4/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-11 22:38:35.491057 kaskada-0.1.4/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     2325 1970-01-01 00:00:00.000000 kaskada-0.1.4/setup.py
+-rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 kaskada-0.1.4/PKG-INFO
```

### Comparing `kaskada-0.1.3/README.md` & `kaskada-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/pyproject.toml` & `kaskada-0.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.1.3"
+version = "0.1.4"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
     { include = "fenlmagic", from = "src" },
 ]
-include = [ "**/src/kaskada/kaskada/**/*.py"]
+include = ["**/src/kaskada/kaskada/**/*.py"]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 certifi = "^2022.12.7"
 domonic = "^0.9.11"
 googleapis-common-protos = "^1.58.0"
 html5lib = "^1.1"
@@ -41,77 +41,77 @@
 types-six = "^1.16.21.4"
 types-typed-ast = "^1.5.8.3"
 autoflake = "^2.0.0"
 autopep8 = "^2.0.1"
 types-protobuf = "^4.21.0.5"
 
 [tool.poe.tasks]
-    [tool.poe.tasks.clean]
-    help = "Remove generated files"
-    cmd  = """
+[tool.poe.tasks.clean]
+help = "Remove generated files"
+cmd = """
         # multiline commands including comments work too!
         rm -rf .coverage
             .mypy_cache
             .pytest_cache
             ./**/__pycache__
             dist
             htmlcov
             ./tests/fixtures/simple_project/venv
             ./tests/fixtures/venv_project/myvenv
             ./tests/fixtures/poetry_plugin_project/**/.venv
             ./tests/temp
     """
 
-    [tool.poe.tasks.format-isort]
-    help = "Run import sort (isort) on the code base"
-    cmd = "isort src tests"
-
-    [tool.poe.tasks.format-black]
-    help = "Run black on the code base"
-    cmd = "black src tests"
-
-    [tool.poe.tasks.format]
-    help = "Run formating tools on the code base"
-    sequence  = ["format-isort", "format-black"]
-
-    [tool.poe.tasks.test]
-    help = "Run unit and feature tests"
-    cmd = "pytest --cov=src"
-
-    [tool.poe.tasks.types-fenlmagic]
-    help = "Run the type checker for fenlmagic"
-    cmd  = "mypy --ignore-missing-imports src/fenlmagic"
-
-    [tool.poe.tasks.types-python]
-    help = "Run the type checker for python client"
-    cmd  = "mypy --ignore-missing-imports src/kaskada"
-
-    [tool.poe.tasks.types]
-    help = "Run the type checker"
-    sequence = ["types-fenlmagic", "types-python"]
-
-    [tool.poe.tasks.lint]
-    help = "Run the linter"
-    cmd  = "pylint src --ignore-paths=src/kaskada/kaskada"
-
-    [tool.poe.tasks.style-black]
-    help = "Validate black code style"
-    cmd  = "black src --check --diff --target-version=py310"
-
-    [tool.poe.tasks.style-isort]
-    help = "Validate isort code style"
-    cmd  = "isort src --check --diff"
-
-    [tool.poe.tasks.style]
-    help = "Validate code style"
-    sequence = ["style-isort", "style-black"]
-
-    [tool.poe.tasks.remove-imports-vars]
-    help = "Run to remove unused imports and variables"
-    cmd = "autoflake -r --in-place --remove-unused-variables src/"
+[tool.poe.tasks.format-isort]
+help = "Run import sort (isort) on the code base"
+cmd = "isort src tests"
+
+[tool.poe.tasks.format-black]
+help = "Run black on the code base"
+cmd = "black src tests"
+
+[tool.poe.tasks.format]
+help = "Run formating tools on the code base"
+sequence = ["format-isort", "format-black"]
+
+[tool.poe.tasks.test]
+help = "Run unit and feature tests"
+cmd = "pytest --cov=src"
+
+[tool.poe.tasks.types-fenlmagic]
+help = "Run the type checker for fenlmagic"
+cmd = "mypy --ignore-missing-imports src/fenlmagic"
+
+[tool.poe.tasks.types-python]
+help = "Run the type checker for python client"
+cmd = "mypy --ignore-missing-imports src/kaskada"
+
+[tool.poe.tasks.types]
+help = "Run the type checker"
+sequence = ["types-fenlmagic", "types-python"]
+
+[tool.poe.tasks.lint]
+help = "Run the linter"
+cmd = "pylint src --ignore-paths=src/kaskada/kaskada"
+
+[tool.poe.tasks.style-black]
+help = "Validate black code style"
+cmd = "black src --check --diff --target-version=py310"
+
+[tool.poe.tasks.style-isort]
+help = "Validate isort code style"
+cmd = "isort src --check --diff"
+
+[tool.poe.tasks.style]
+help = "Validate code style"
+sequence = ["style-isort", "style-black"]
+
+[tool.poe.tasks.remove-imports-vars]
+help = "Run to remove unused imports and variables"
+cmd = "autoflake -r --in-place --remove-unused-variables src/"
 
 [tool.isort]
 profile = "black"
 skip = ["src/kaskada/kaskada"]
 
 [tool.mypy]
 exclude = ["src/kaskada/kaskada"]
```

### Comparing `kaskada-0.1.3/src/fenlmagic/__init__.py` & `kaskada-0.1.4/src/fenlmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/api/api_utils.py` & `kaskada-0.1.4/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/api/release.py` & `kaskada-0.1.4/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/api/session.py` & `kaskada-0.1.4/src/kaskada/api/session.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/client.py` & `kaskada-0.1.4/src/kaskada/client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/formatters.css` & `kaskada-0.1.4/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/formatters.js` & `kaskada-0.1.4/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/formatters.py` & `kaskada-0.1.4/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/formatters_helpers.py` & `kaskada-0.1.4/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/formatters_shared.py` & `kaskada-0.1.4/src/kaskada/formatters_shared.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/materialization.py` & `kaskada-0.1.4/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/query.py` & `kaskada-0.1.4/src/kaskada/query.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/slice_filters.py` & `kaskada-0.1.4/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/table.py` & `kaskada-0.1.4/src/kaskada/table.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/utils.py` & `kaskada-0.1.4/src/kaskada/utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/src/kaskada/view.py` & `kaskada-0.1.4/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/vendor/validate/validate.proto` & `kaskada-0.1.4/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/vendor/validate/validate_pb2.py` & `kaskada-0.1.4/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/vendor/validate/validate_pb2.pyi` & `kaskada-0.1.4/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.3/setup.py` & `kaskada-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src', 'fenlmagic': 'src/fenlmagic', 'validate': 'vendor/validate'}
 
 packages = \
-['fenlmagic', 'kaskada', 'kaskada.api', 'validate']
+['fenlmagic',
+ 'kaskada',
+ 'kaskada.api',
+ 'kaskada.kaskada.v1alpha',
+ 'kaskada.kaskada.v2alpha',
+ 'validate']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['certifi>=2022.12.7,<2023.0.0',
  'domonic>=0.9.11,<0.10.0',
@@ -22,15 +27,15 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kaskada-0.1.3/PKG-INFO` & `kaskada-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.1.3
+Version: 0.1.4
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

