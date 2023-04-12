# Comparing `tmp/cdktf-cdktf-provider-random-5.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-random-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-random-5.0.0.tar", last modified: Tue Jan 17 14:51:15 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-random-6.0.0.tar", last modified: Wed Apr 12 03:15:20 2023, max compression
```

## Comparing `cdktf-cdktf-provider-random-5.0.0.tar` & `cdktf-cdktf-provider-random-6.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.682936 cdktf-cdktf-provider-random-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-01-17 14:51:15.682936 cdktf-cdktf-provider-random-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:51:15.682936 cdktf-cdktf-provider-random-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45339 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/_jsii/provider-random@5.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/id/
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/id/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/integer/
--rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/integer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/password/
--rw-r--r--   0 runner    (1001) docker     (123)    46079 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/pet/
--rw-r--r--   0 runner    (1001) docker     (123)    22054 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/pet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/shuffle/
--rw-r--r--   0 runner    (1001) docker     (123)    23953 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/shuffle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/string_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    46090 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/string_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/uuid/
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-01-17 14:51:01.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/uuid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:51:15.678935 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-01-17 14:51:15.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-17 14:51:15.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:51:15.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:51:15.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-17 14:51:15.000000 cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.097818 cdktf-cdktf-provider-random-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153647 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/_jsii/provider-random@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/id/
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/id/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/integer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21435 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/integer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/password/
+-rw-r--r--   0 runner    (1001) docker     (123)    46079 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/pet/
+-rw-r--r--   0 runner    (1001) docker     (123)    22054 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/pet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (123)    23953 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/shuffle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/string_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    46090 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/string_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/uuid/
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-12 03:15:05.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/uuid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:20.101817 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-12 03:15:20.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-12 03:15:20.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:15:20.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 03:15:20.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 03:15:20.000000 cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-random-5.0.0/LICENSE` & `cdktf-cdktf-provider-random-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/PKG-INFO` & `cdktf-cdktf-provider-random-6.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-random
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt random Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-random.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-random.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +62,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-random-go`](https://github.com/cdktf/cdktf-provider-random-go) package.
 
 `go get github.com/cdktf/cdktf-provider-random-go/random`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-random).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform random Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-random-5.0.0/README.md` & `cdktf-cdktf-provider-random-6.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-random-go`](https://github.com/cdktf/cdktf-provider-random-go) package.
 
 `go get github.com/cdktf/cdktf-provider-random-go/random`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-random).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform random Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-random-5.0.0/setup.py` & `cdktf-cdktf-provider-random-6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-random",
-    "version": "5.0.0",
+    "version": "6.0.0",
     "description": "Prebuilt random Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-random.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -30,37 +30,38 @@
         "cdktf_cdktf_provider_random.provider",
         "cdktf_cdktf_provider_random.shuffle",
         "cdktf_cdktf_provider_random.string_resource",
         "cdktf_cdktf_provider_random.uuid"
     ],
     "package_data": {
         "cdktf_cdktf_provider_random._jsii": [
-            "provider-random@5.0.0.jsii.tgz"
+            "provider-random@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_random": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.15.0, <0.16.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.73.0, <2.0.0",
+        "jsii>=1.79.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-random-go`](https://github.com/cdktf/cdktf-provider-random-go) package.
 
 `go get github.com/cdktf/cdktf-provider-random-go/random`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-random).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform random Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/id/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/id/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/integer/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/integer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/password/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/password/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/pet/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/pet/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/provider/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/shuffle/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/string_resource/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/string_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random/uuid/__init__.py` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random/uuid/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-random
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt random Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-random.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-random.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,15 +62,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-random-go`](https://github.com/cdktf/cdktf-provider-random-go) package.
 
 `go get github.com/cdktf/cdktf-provider-random-go/random`
 
 ## Docs
 
-Find auto-generated docs for this provider here: [./API.md](./API.md)
+Find auto-generated docs for this provider here:
+
+* [Typescript](./docs/API.typescript.md)
+* [Python](./docs/API.python.md)
+* [Java](./docs/API.java.md)
+* [C#](./docs/API.csharp.md)
+* [Go](./docs/API.go.md)
+
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-random).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform random Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-random-5.0.0/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-random-6.0.0/src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_random/py.typed
 src/cdktf_cdktf_provider_random.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_random.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_random.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_random.egg-info/requires.txt
 src/cdktf_cdktf_provider_random.egg-info/top_level.txt
 src/cdktf_cdktf_provider_random/_jsii/__init__.py
-src/cdktf_cdktf_provider_random/_jsii/provider-random@5.0.0.jsii.tgz
+src/cdktf_cdktf_provider_random/_jsii/provider-random@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_random/id/__init__.py
 src/cdktf_cdktf_provider_random/integer/__init__.py
 src/cdktf_cdktf_provider_random/password/__init__.py
 src/cdktf_cdktf_provider_random/pet/__init__.py
 src/cdktf_cdktf_provider_random/provider/__init__.py
 src/cdktf_cdktf_provider_random/shuffle/__init__.py
 src/cdktf_cdktf_provider_random/string_resource/__init__.py
```

