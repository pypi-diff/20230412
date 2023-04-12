# Comparing `tmp/altinn3_test_lib-0.0.4.tar.gz` & `tmp/altinn3_test_lib-0.0.6.tar.gz`

## Comparing `altinn3_test_lib-0.0.4.tar` & `altinn3_test_lib-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/CODEOWNERS
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/azure-pipelines.yml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/hello_test.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/factories/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/factories/altinn_factory.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/factories/file_factory.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/factories/gcp_factories.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/mocking/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/mocking/environment_vars.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/mocking/mock_assist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/resources/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/resources/mocking.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/instance.json
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/instance_json_in.json
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/instance_json_out.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/simple_prefill.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/utils/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/src/altinn3_test_lib/utils/fileutils.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/README.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/CODEOWNERS
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/hello_test.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/factories/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/factories/altinn_factory.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/factories/file_factory.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/factories/gcp_factories.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/mocking/__init__.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/mocking/environment_vars.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/mocking/mock_assist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/resources/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/resources/mocking.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/instance.json
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/instance_json_in.json
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/instance_json_out.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/simple_prefill.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/utils/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/src/altinn3_test_lib/utils/fileutils.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.6/PKG-INFO
```

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/plugins.py` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/plugins.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/factories/altinn_factory.py` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/factories/altinn_factory.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/factories/file_factory.py` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/factories/file_factory.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/factories/gcp_factories.py` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/factories/gcp_factories.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/mocking/environment_vars.py` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/mocking/environment_vars.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/fixtures/mocking/mock_assist.py` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/fixtures/mocking/mock_assist.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/instance.json` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/instance.json`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/instance_json_in.json` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/instance_json_in.json`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/instance_json_out.json` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/instance_json_out.json`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/src/altinn3_test_lib/test_files/simple_prefill.txt` & `altinn3_test_lib-0.0.6/src/altinn3_test_lib/test_files/simple_prefill.txt`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/.gitignore` & `altinn3_test_lib-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/LICENSE` & `altinn3_test_lib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.4/PKG-INFO` & `altinn3_test_lib-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: altinn3-test-lib
-Version: 0.0.4
+Version: 0.0.6
 Summary: A POC project for modular test tools
 Author-email: Anders Hagen <nhk@ssb.no>, Rannveig Aasen <rsa@ssb.no>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: google-cloud-pubsub
+Requires-Dist: pytest-mock
+Requires-Dist: pytest~=7.2.1
+Requires-Dist: ssb-altinn3-util
 Description-Content-Type: text/markdown
 
 # Altinn3-test-lib
 Et Python bibliotek med felles test-funksjoner og mocke-objekt for bruk i altinn3-prosjektene
```

