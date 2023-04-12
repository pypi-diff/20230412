# Comparing `tmp/runpod-0.9.1.tar.gz` & `tmp/runpod-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runpod-0.9.1.tar", last modified: Thu Mar 16 18:28:44 2023, max compression
+gzip compressed data, was "runpod-0.9.2.tar", last modified: Wed Apr 12 04:23:09 2023, max compression
```

## Comparing `runpod-0.9.1.tar` & `runpod-0.9.2.tar`

### file list

```diff
@@ -1,50 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-16 18:28:35.000000 runpod-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-03-16 18:28:44.845205 runpod-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-16 18:28:35.000000 runpod-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-16 18:28:35.000000 runpod-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.841205 runpod-0.9.1/runpod/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/runpod/api_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/api_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/runpod/api_wrapper/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/api_wrapper/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/api_wrapper/queries/cpu_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/runpod/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/endpoint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/runpod/serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/runpod/serverless/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/rp_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/rp_tips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/modules/worker_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/runpod/serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/utils/rp_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/utils/rp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/utils/rp_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/utils/rp_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-16 18:28:35.000000 runpod-0.9.1/runpod/serverless/work_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/runpod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-03-16 18:28:44.000000 runpod-0.9.1/runpod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-16 18:28:44.000000 runpod-0.9.1/runpod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 18:28:44.000000 runpod-0.9.1/runpod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-16 18:28:44.000000 runpod-0.9.1/runpod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-16 18:28:44.000000 runpod-0.9.1/runpod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-03-16 18:28:44.845205 runpod-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-16 18:28:35.000000 runpod-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-16 18:28:35.000000 runpod-0.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/tests/test_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-16 18:28:35.000000 runpod-0.9.1/tests/test_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-16 18:28:35.000000 runpod-0.9.1/tests/test_endpoint/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:28:44.845205 runpod-0.9.1/tests/test_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-16 18:28:35.000000 runpod-0.9.1/tests/test_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-16 18:28:35.000000 runpod-0.9.1/tests/test_serverless/test_module_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-16 18:28:35.000000 runpod-0.9.1/tests/test_serverless/test_pod_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.613602 runpod-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.589601 runpod-0.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.593601 runpod-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/CD_publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/CI_codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/CI_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 04:22:56.000000 runpod-0.9.2/.github/workflows/ci_pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-12 04:22:56.000000 runpod-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 04:22:56.000000 runpod-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-12 04:23:09.613602 runpod-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-12 04:22:56.000000 runpod-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.581601 runpod-0.9.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.593601 runpod-0.9.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28325 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/images/env_var_location.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.593601 runpod-0.9.2/docs/serverless/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.597601 runpod-0.9.2/docs/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_cleanup.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_download.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_upload.md
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/utils/rp_validator.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-12 04:22:56.000000 runpod-0.9.2/docs/serverless/worker.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.597601 runpod-0.9.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 04:22:56.000000 runpod-0.9.2/examples/call_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 04:22:56.000000 runpod-0.9.2/examples/call_endpoint_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-12 04:22:56.000000 runpod-0.9.2/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 04:22:56.000000 runpod-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 04:22:56.000000 runpod-0.9.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.597601 runpod-0.9.2/runpod/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/api_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/api_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/api_wrapper/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/api_wrapper/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/api_wrapper/queries/cpu_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod/endpoint/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/asyncio/asyncio_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/endpoint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.605601 runpod-0.9.2/runpod/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.605601 runpod-0.9.2/runpod/serverless/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/rp_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/rp_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/modules/worker_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.609602 runpod-0.9.2/runpod/serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/utils/rp_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-12 04:22:56.000000 runpod-0.9.2/runpod/serverless/work_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.601601 runpod-0.9.2/runpod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 04:23:09.000000 runpod-0.9.2/runpod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-12 04:23:09.613602 runpod-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 04:22:56.000000 runpod-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.609602 runpod-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.609602 runpod-0.9.2/tests/test_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_endpoint/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:23:09.613602 runpod-0.9.2/tests/test_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/test_module_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/test_pod_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_serverless/test_util_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/test_whatever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 04:22:56.000000 runpod-0.9.2/tests/whatever.py
```

### Comparing `runpod-0.9.1/LICENSE` & `runpod-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runpod-0.9.1/PKG-INFO` & `runpod-0.9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.1
+Version: 0.9.2
 Summary: Official Python library for RunPod API & SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 <div align="center">
 <h1>RunPod | Python Library </h1>
 
 [![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml)
 &nbsp;
@@ -55,69 +56,76 @@
 ### Quick Start
 
 Create an python script in your project that contains your model definition and the RunPod worker start code. Run this python code as your default container start command:
 
 ```python
 import runpod
 
-MODEL = 'YOUR_MODEL'
+def is_even(job):
 
-def run(job):
-    # Your inference code here
-    return MODEL.predict(job.input)
+    job_input = job["input"]
+    the_number = job_input["number"]
 
-runpod.serverless.start({"handler": run})
+    if not isinstance(the_number, int):
+        return {"error": "Silly human, you need to pass an integer."}
+
+    if the_number % 2 == 0:
+        return True
+
+    return False
+
+runpod.serverless.start({"handler": is_even})
 ```
 
 Make sure that this file is ran when your container starts. This can be accomplished by calling it in the docker command when you setup a template at [runpod.io/console/serverless/user/templates](https://www.runpod.io/console/serverless/user/templates) or by setting it as the default command in your Dockerfile.
 
 See our [blog post](https://www.runpod.io/blog/serverless-create-a-basic-api) for creating a basic Serverless API, or view the [details docs](https://docs.runpod.io/serverless-ai/custom-apis) for more information.
 
 ## API Language Library
 
 When interacting with the RunPod API you can use this library to make requests to the API.
 
 ```python
 import runpod
 
-runpod.api_key = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+runpod.api_key = "your_runpod_api_key_found_under_settings"
 ```
 
 ### Endpoints
 
 You can interact with RunPod endpoints via a `run` or `run_sync` method.
 
 ```python
 endpoint = runpod.Endpoint("ENDPOINT_ID")
 
 run_request = endpoint.run(
-    {"YOUR_MODEL_INPUT_JSON": "YOUR_MODEL_INPUT_VALUE"}
+    {"your_model_input_key": "your_model_input_value"}
 )
 
 # Check the status of the endpoint run request
 print(run_request.status())
 
 # Get the output of the endpoint run request, blocking until the endpoint run is complete.
 print(run_request.output())
 ```
 
 ```python
 endpoint = runpod.Endpoint("ENDPOINT_ID")
 
 run_request = endpoint.run_sync(
-    {"YOUR_MODEL_INPUT_JSON": "YOUR_MODEL_INPUT_VALUE"}
+    {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
 ## Directory
 
-```
+```BASH
 .
 ├── docs               # Documentation
 ├── runpod             # Package source code
 │   ├── endpoint       # Language library - Endpoints
 │   └── serverless     # SDK - Serverless Worker
 └── tests              # Package tests
 ```
```

### Comparing `runpod-0.9.1/README.md` & `runpod-0.9.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -33,69 +33,76 @@
 ### Quick Start
 
 Create an python script in your project that contains your model definition and the RunPod worker start code. Run this python code as your default container start command:
 
 ```python
 import runpod
 
-MODEL = 'YOUR_MODEL'
+def is_even(job):
 
-def run(job):
-    # Your inference code here
-    return MODEL.predict(job.input)
+    job_input = job["input"]
+    the_number = job_input["number"]
 
-runpod.serverless.start({"handler": run})
+    if not isinstance(the_number, int):
+        return {"error": "Silly human, you need to pass an integer."}
+
+    if the_number % 2 == 0:
+        return True
+
+    return False
+
+runpod.serverless.start({"handler": is_even})
 ```
 
 Make sure that this file is ran when your container starts. This can be accomplished by calling it in the docker command when you setup a template at [runpod.io/console/serverless/user/templates](https://www.runpod.io/console/serverless/user/templates) or by setting it as the default command in your Dockerfile.
 
 See our [blog post](https://www.runpod.io/blog/serverless-create-a-basic-api) for creating a basic Serverless API, or view the [details docs](https://docs.runpod.io/serverless-ai/custom-apis) for more information.
 
 ## API Language Library
 
 When interacting with the RunPod API you can use this library to make requests to the API.
 
 ```python
 import runpod
 
-runpod.api_key = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+runpod.api_key = "your_runpod_api_key_found_under_settings"
 ```
 
 ### Endpoints
 
 You can interact with RunPod endpoints via a `run` or `run_sync` method.
 
 ```python
 endpoint = runpod.Endpoint("ENDPOINT_ID")
 
 run_request = endpoint.run(
-    {"YOUR_MODEL_INPUT_JSON": "YOUR_MODEL_INPUT_VALUE"}
+    {"your_model_input_key": "your_model_input_value"}
 )
 
 # Check the status of the endpoint run request
 print(run_request.status())
 
 # Get the output of the endpoint run request, blocking until the endpoint run is complete.
 print(run_request.output())
 ```
 
 ```python
 endpoint = runpod.Endpoint("ENDPOINT_ID")
 
 run_request = endpoint.run_sync(
-    {"YOUR_MODEL_INPUT_JSON": "YOUR_MODEL_INPUT_VALUE"}
+    {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
 ## Directory
 
-```
+```BASH
 .
 ├── docs               # Documentation
 ├── runpod             # Package source code
 │   ├── endpoint       # Language library - Endpoints
 │   └── serverless     # SDK - Serverless Worker
 └── tests              # Package tests
 ```
```

### Comparing `runpod-0.9.1/runpod/endpoint/runner.py` & `runpod-0.9.2/runpod/endpoint/runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.1/runpod/serverless/modules/heartbeat.py` & `runpod-0.9.2/runpod/serverless/modules/heartbeat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-'''enables heartbeats'''
+"""Enables heartbeats."""
 
 import os
 import threading
 
 import requests
 
 import runpod.serverless.modules.logging as log
-from .worker_state import get_current_job_id, PING_URL, ping_interval
+from .worker_state import get_current_job_id, PING_URL, PING_INTERVAL
 
-session = requests.Session()
-session.headers.update({"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"})
+_session = requests.Session()
+_session.headers.update({"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"})
 
 
-def start_ping():
-    '''
-    Pings the heartbeat endpoint at the specified interval.
-    '''
-    ping_params = None
-
-    try:
-        job_id = get_current_job_id()
-
-        if job_id is not None:
-            ping_params = {
-                'job_id': job_id,
-            }
-
-        if PING_URL not in [None, 'PING_URL_NOT_SET']:
-            result = session.get(
+def _send_ping(ping_params=None):
+    if PING_URL not in [None, 'PING_URL_NOT_SET']:
+        try:
+            result = _session.get(
                 PING_URL,
                 params=ping_params,
-                timeout=int(ping_interval/1000)
+                timeout=int(PING_INTERVAL / 1000)
             )
 
             log.info(f"Heartbeat Sent  URL: {PING_URL}  Status: {result.status_code}")
-            log.info(f"Heartbeat Sent  Interval: {ping_interval}ms  Params: {ping_params}")
+            log.info(f"Heartbeat Sent  Interval: {PING_INTERVAL}ms  Params: {ping_params}")
+
+        except Exception as err:  # pylint: disable=broad-except
+            log.error(f"Heartbeat Failed  URL: {PING_URL}  Params: {ping_params}")
+            log.error(f"Heartbeat Fail  Error: {err}")
+
+
+def start_ping():
+    """
+    Pings the heartbeat endpoint at the specified interval.
+    """
+    job_id = get_current_job_id()
 
-    except Exception as err:  # pylint: disable=broad-except
-        log.error(f"Heartbeat Failed  URL: {PING_URL}  Params: {ping_params}")
-        log.error(f"Heartbeat Fail  Error: {err}")
-
-    finally:
-        heartbeat_thread = threading.Timer(int(ping_interval/1000), start_ping)
-        heartbeat_thread.daemon = True
-        heartbeat_thread.start()
+    ping_params = {
+        'job_id': job_id,
+    } if job_id is not None else None
+
+    _send_ping(ping_params)
+
+    log.debug(f"Scheduling next heartbeat in {PING_INTERVAL}ms")
+    heartbeat_thread = threading.Timer(int(PING_INTERVAL / 1000), start_ping)
+    heartbeat_thread.daemon = True
+    heartbeat_thread.start()
```

### Comparing `runpod-0.9.1/runpod/serverless/modules/job.py` & `runpod-0.9.2/runpod/serverless/modules/job.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,130 +1,135 @@
-'''
-job related helpers
-'''
+"""
+Job related helpers.
+"""
 
 import os
 import time
 import json
 import traceback
 
 import runpod.serverless.modules.logging as log
 from .worker_state import JOB_GET_URL, get_done_url
 from .retry import retry
 from .rp_tips import check_return_size
 
+_IS_LOCAL_TEST = os.environ.get("RUNPOD_WEBHOOK_GET_JOB", None) is None
+
+
+def _get_local():
+    """
+    Returns contents of test_input.json.
+    """
+    if not os.path.exists("test_input.json"):
+        log.warn("test_input.json not found, skipping local testing")
+        return None
+
+    with open("test_input.json", "r", encoding="UTF-8") as file:
+        test_inputs = json.loads(file.read())
+
+    if "id" not in test_inputs:
+        test_inputs["id"] = "local_test"
+
+    log.debug(f"Retrieved local job: {test_inputs}")
+    return test_inputs
+
 
 async def get_job(session):
-    '''
+    """
     Get the job from the queue.
-    '''
+    """
     next_job = None
 
     try:
-        if os.environ.get('RUNPOD_WEBHOOK_GET_JOB', None) is None:
-            log.warn('RUNPOD_WEBHOOK_GET_JOB not set, switching to get_local')
-            next_job = get_local()
+        if _IS_LOCAL_TEST:
+            log.warn("RUNPOD_WEBHOOK_GET_JOB not set, switching to get_local")
+            next_job = _get_local()
         else:
             async with session.get(JOB_GET_URL) as response:
                 next_job = await response.json()
+                log.debug(f"Retrieved remote job: {next_job}")
 
-        log.info(next_job)
+        if next_job is not None:
+            log.info(f"Received job: {next_job['id']}")
     except Exception as err:  # pylint: disable=broad-except
         log.error(f"Error while getting job: {err}")
 
     return next_job
 
 
 def run_job(handler, job):
-    '''
+    """
     Run the job using the handler.
     Returns the job output or error.
-    '''
-    log.info(f"Started working on {job['id']} at {time.time()} UTC")
+    """
+    start_time = time.time()
+    log.info(f'Started working on job {job["id"]} at {start_time} UTC')
 
     run_result = {"error": "Failed to return job output or capture error."}
 
     try:
         job_output = handler(job)
+        log.debug(f'Job {job["id"]} handler output: {job_output}')
 
         if isinstance(job_output, bool):
             run_result = {"output": job_output}
         elif "error" in job_output:
-            run_result = {"error": str(job_output['error'])}
+            run_result = {"error": str(job_output["error"])}
         elif "refresh_worker" in job_output:
             job_output.pop("refresh_worker")
             run_result = {
                 "stopPod": True,
                 "output": job_output
             }
         else:
             run_result = {"output": job_output}
 
         check_return_size(run_result)  # Checks the size of the return body.
     except Exception as err:    # pylint: disable=broad-except
-        log.error(f"Error while running job {job['id']}: {err}")
-
+        log.error(f'Error while running job {job["id"]}: {err}')
         run_result = {"error": f"handler: {str(err)} \ntraceback: {traceback.format_exc()}"}
-
     finally:
-        log.info(f"Finished working on {job['id']} at {time.time()} UTC")
-        log.info(f"Run result: {run_result}")
+        end_time = time.time()
+        log.info(f'Finished working on job {job["id"]} at {end_time} UTC')
+        log.info(f"Job {job['id']} took {end_time - start_time} seconds to complete")
+        log.debug(f"Run result: {run_result}")
 
         return run_result  # pylint: disable=lost-exception
 
 
 @retry(max_attempts=3, base_delay=1, max_delay=3)
 async def retry_send_result(session, job_data):
-    '''
-    wrapper for sending results
-    '''
+    """
+    Wrapper for sending results.
+    """
     headers = {
         "charset": "utf-8",
         "Content-Type": "application/x-www-form-urlencoded"
     }
 
-    log.info("result api call")
+    log.debug("Initiating result API call")
     async with session.post(get_done_url(),
                             data=job_data,
                             headers=headers,
                             raise_for_status=True) as resp:
         result = await resp.text()
-        log.debug(result)
+        log.debug(f"Result API response: {result}")
 
-    log.info("done with result api call")
+    log.info("Completed result API call")
 
 
 async def send_result(session, job_data, job):
     '''
     Return the job results.
     '''
     try:
         job_data = json.dumps(job_data, ensure_ascii=False)
-
-        if os.environ.get('RUNPOD_WEBHOOK_GET_JOB', None) is not None:
-            log.info(f"Sending job results: {job_data}")
+        if not _IS_LOCAL_TEST:
+            log.info(f"Sending job results for {job['id']}: {job_data}")
             await retry_send_result(session, job_data)
         else:
-            log.warn(f"Local test job results: {job_data}")
+            log.warn(f"Local test job results for {job['id']}: {job_data}")
 
     except Exception as err:  # pylint: disable=broad-except
         log.error(f"Error while returning job result {job['id']}: {err}")
     else:
         log.info(f"Successfully returned job result {job['id']}")
-
-
-# ------------------------------- Local Testing ------------------------------ #
-def get_local():
-    '''
-    Returns contents of test_input.json
-    '''
-    if not os.path.exists('test_input.json'):
-        log.warn('test_input.json not found, skipping local testing')
-        return None
-
-    with open('test_input.json', 'r', encoding="UTF-8") as file:
-        test_inputs = json.loads(file.read())
-
-    if 'id' not in test_inputs:
-        test_inputs['id'] = 'local_test'
-
-    return test_inputs
```

### Comparing `runpod-0.9.1/runpod/serverless/modules/logging.py` & `runpod-0.9.2/runpod/serverless/modules/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ''' PodWorker | modules | logging.py '''
 
 import os
 from dotenv import load_dotenv
 
-env_path = os.getcwd() + '/.env'
+env_path = os.path.join(os.getcwd(), '.env')
 load_dotenv(env_path)  # Load environment variables
 
 
 def log(message, level='INFO'):
     '''
     Log message to stdout if RUNPOD_DEBUG is true.
     '''
     set_level = os.environ.get('RUNPOD_DEBUG_LEVEL', 'DEBUG').upper()
     level = level.ljust(7)
 
-    if os.environ.get('RUNPOD_DEBUG', 'true') != 'true':
+    if os.environ.get('RUNPOD_DEBUG', 'true').lower() != 'true':
         return
 
     if set_level == 'ERROR' and level != 'ERROR':
         return
 
     if set_level == 'WARN' and level not in ['ERROR', 'WARN']:
         return
@@ -31,21 +31,22 @@
 
 
 def log_secret(secret_name, secret, level='INFO'):
     '''
     Censors secrets for logging.
     Replaces everything except the first and last characters with *
     '''
-    if secret is None and os.environ.get('RUNPOD_POD_ID', None) is not None:
-        secret = 'Could not read environment variable.'
-        log(f"{secret_name}: {secret}", 'ERROR')
-    elif os.environ.get('RUNPOD_POD_ID', None) is not None:
-        secret = str(secret)
-        redacted_secret = secret[0] + '*' * (len(secret)-2) + secret[-1]
-        log(f"{secret_name}: {redacted_secret}", level)
+    if os.environ.get('RUNPOD_POD_ID', None) is not None:
+        if secret is None:
+            secret = 'Could not read environment variable.'
+            log(f"{secret_name}: {secret}", 'ERROR')
+        else:
+            secret = str(secret)
+            redacted_secret = secret[0] + '*' * (len(secret)-2) + secret[-1]
+            log(f"{secret_name}: {redacted_secret}", level)
 
 
 def error(message):
     '''
     error log
     '''
     log(message, 'ERROR')
```

### Comparing `runpod-0.9.1/runpod/serverless/modules/retry.py` & `runpod-0.9.2/runpod/serverless/modules/retry.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 import random
 import asyncio
 from functools import wraps
 
 
 def retry(max_attempts, base_delay, max_delay):
     '''
-    decorator to retry async functions
+    A decorator to retry async functions in case of exceptions.
+
+    Args:
+        max_attempts: The maximum number of attempts to retry.
+        base_delay: The base delay in seconds between retries.
+        max_delay: The maximum delay in seconds between retries.
+
+    Returns:
+        A decorated async function with retry capabilities.
     '''
     def decorator(func):
         @wraps(func)
         async def wrapper(*args, **kwargs):
             attempt = 1
             while True:
                 try:
```

### Comparing `runpod-0.9.1/runpod/serverless/modules/worker_state.py` & `runpod-0.9.2/runpod/serverless/modules/worker_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 '''
-Handles getting stuff from env and updating global state like job id
+Handles getting stuff from environment variables and updating the global state like job id.
 '''
 
 import os
 import uuid
 
 CURRENT_JOB_ID = None
 
-worker_id = os.environ.get('RUNPOD_POD_ID', str(uuid.uuid4()))
+WORKER_ID = os.environ.get('RUNPOD_POD_ID', str(uuid.uuid4()))
 
-auth_header = {"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"}
-JOB_GET_URL = str(os.environ.get('RUNPOD_WEBHOOK_GET_JOB')).replace('$ID', worker_id)
-JOB_DONE_URL = str(os.environ.get('RUNPOD_WEBHOOK_POST_OUTPUT'))
-JOB_DONE_URL = JOB_DONE_URL.replace('$RUNPOD_POD_ID', worker_id)
-
-webhook_ping = os.environ.get('RUNPOD_WEBHOOK_PING', None)
-if webhook_ping is not None:
-    PING_URL = webhook_ping.replace('$RUNPOD_POD_ID', worker_id)
+
+def get_auth_header():
+    '''
+    Returns the authorization header with the API key.
+    '''
+    return {"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"}
+
+
+JOB_GET_URL = str(os.environ.get('RUNPOD_WEBHOOK_GET_JOB')).replace('$ID', WORKER_ID)
+JOB_DONE_URL_TEMPLATE = str(os.environ.get('RUNPOD_WEBHOOK_POST_OUTPUT'))
+JOB_DONE_URL_TEMPLATE = JOB_DONE_URL_TEMPLATE.replace('$RUNPOD_POD_ID', WORKER_ID)
+
+WEBHOOK_PING = os.environ.get('RUNPOD_WEBHOOK_PING', None)
+if WEBHOOK_PING is not None:
+    PING_URL = WEBHOOK_PING.replace('$RUNPOD_POD_ID', WORKER_ID)
 else:
     PING_URL = "PING_URL_NOT_SET"
 
-ping_interval = int(os.environ.get('RUNPOD_PING_INTERVAL', 10000))
+PING_INTERVAL = int(os.environ.get('RUNPOD_PING_INTERVAL', 10000))
 
 
 def get_current_job_id():
     '''
-    get current job id
+    Returns the current job id.
     '''
     return CURRENT_JOB_ID
 
 
 def get_done_url():
     '''
-    constructs done url using current job id
+    Constructs the done URL using the current job id.
     '''
-    return JOB_DONE_URL.replace('$ID', CURRENT_JOB_ID)
+    return JOB_DONE_URL_TEMPLATE.replace('$ID', CURRENT_JOB_ID)
 
 
 def set_job_id(new_job_id):
     '''
-    sets current job id
+    Sets the current job id.
     '''
     global CURRENT_JOB_ID  # pylint: disable=global-statement
     CURRENT_JOB_ID = new_job_id
```

### Comparing `runpod-0.9.1/runpod/serverless/utils/rp_cleanup.py` & `runpod-0.9.2/runpod/serverless/utils/rp_cleanup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Called to clean up the worker pod after a job is completed.
 '''
 
 import os
 import shutil
 
 
-def clean(folder_list=None):
+def clean(folder_list: list[str] = None):
     '''
     Removes the downloads folder.
     '''
     shutil.rmtree("input_objects", ignore_errors=True)
     shutil.rmtree("output_objects", ignore_errors=True)
 
     shutil.rmtree("job_files", ignore_errors=True)
```

### Comparing `runpod-0.9.1/runpod/serverless/utils/rp_upload.py` & `runpod-0.9.2/runpod/serverless/utils/rp_upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,126 @@
 ''' PodWorker | modules | upload.py '''
 
 import os
+import io
 import time
 import uuid
 import logging
 import threading
+import multiprocessing
 from io import BytesIO
+from typing import Optional, Tuple
 
+import boto3
 from PIL import Image
 from boto3 import session
 from boto3.s3.transfer import TransferConfig
 from botocore.config import Config
 from tqdm_loggable.auto import tqdm
 
 logger = logging.getLogger("runpod upload utility")
 FMT = "%(filename)-20s:%(lineno)-4d %(asctime)s %(message)s"
 logging.basicConfig(level=logging.INFO, format=FMT, handlers=[logging.StreamHandler()])
 
+
 # --------------------------- S3 Bucket Connection --------------------------- #
-bucket_session = session.Session()
+def get_boto_client(bucket_creds: Optional[dict] = None) -> Tuple[boto3.client, TransferConfig]:
+    '''
+    Returns a boto3 client and transfer config for the bucket.
+    '''
+    bucket_session = session.Session()
 
-boto_config = Config(
-    signature_version='s3v4',
-    retries={
-        'max_attempts': 3,
-        'mode': 'standard'
-    }
-)
+    boto_config = Config(
+        signature_version='s3v4',
+        retries={
+            'max_attempts': 3,
+            'mode': 'standard'
+        }
+    )
 
-if os.environ.get('BUCKET_ENDPOINT_URL', None) is not None:
-    boto_client = bucket_session.client(
-        's3',
-        endpoint_url=os.environ.get('BUCKET_ENDPOINT_URL', None),
-        aws_access_key_id=os.environ.get('BUCKET_ACCESS_KEY_ID', None),
-        aws_secret_access_key=os.environ.get('BUCKET_SECRET_ACCESS_KEY', None),
-        config=boto_config
+    transfer_config = TransferConfig(
+        multipart_threshold=1024 * 25,
+        max_concurrency=multiprocessing.cpu_count(),
+        multipart_chunksize=1024 * 25,
+        use_threads=True
     )
-else:
-    boto_client = None  # pylint: disable=invalid-name
+
+    if bucket_creds:
+        endpoint_url = bucket_creds['endpointUrl']
+        access_key_id = bucket_creds['accessId']
+        secret_access_key = bucket_creds['accessSecret']
+    else:
+        endpoint_url = os.environ.get('BUCKET_ENDPOINT_URL', None)
+        access_key_id = os.environ.get('BUCKET_ACCESS_KEY_ID', None)
+        secret_access_key = os.environ.get('BUCKET_SECRET_ACCESS_KEY', None)
+
+    if endpoint_url and access_key_id and secret_access_key:
+        boto_client = bucket_session.client(
+            's3',
+            endpoint_url=endpoint_url,
+            aws_access_key_id=access_key_id,
+            aws_secret_access_key=secret_access_key,
+            config=boto_config
+        )
+    else:
+        boto_client = None
+
+    return boto_client, transfer_config
 
 
 # ---------------------------------------------------------------------------- #
 #                                 Upload Image                                 #
 # ---------------------------------------------------------------------------- #
 def upload_image(job_id, image_location, result_index=0, results_list=None):
     '''
     Upload image to bucket storage.
     '''
     image_name = str(uuid.uuid4())[:8]
+    boto_client, _ = get_boto_client()
 
     if boto_client is None:
         # Save the output to a file
         print("No bucket endpoint set, saving to disk folder 'simulated_uploaded'")
         print("If this is a live endpoint, please reference the following:")
         print("https://github.com/runpod/runpod-python/blob/main/docs/serverless/worker-utils.md")
 
-        output = BytesIO()
-        img = Image.open(image_location)
-        img.save(output, format=img.format)
-
         os.makedirs("simulated_uploaded", exist_ok=True)
-        with open(f"simulated_uploaded/{image_name}.png", "wb") as file_output:
-            file_output.write(output.getvalue())
+        sim_upload_location = f"simulated_uploaded/{image_name}.png"
+        with Image.open(image_location) as img, open(sim_upload_location, "wb") as file_output:
+            img.save(file_output, format=img.format)
 
         if results_list is not None:
-            results_list[result_index] = f"simulated_uploaded/{image_name}.png"
+            results_list[result_index] = sim_upload_location
 
-        return f"simulated_uploaded/{image_name}.png"
+        return sim_upload_location
 
-    output = BytesIO()
-    img = Image.open(image_location)
-    img.save(output, format=img.format)
-
-    bucket = time.strftime('%m-%y')
-
-    # Upload to S3
-    boto_client.put_object(
-        Bucket=f'{bucket}',
-        Key=f'{job_id}/{image_name}.png',
-        Body=output.getvalue(),
-        ContentType="image/png"
-    )
+    with Image.open(image_location) as img:
+        output = BytesIO()
+        img.save(output, format=img.format)
+        output.seek(0)
 
-    output.close()
+        bucket = time.strftime('%m-%y')
+        boto_client.put_object(
+            Bucket=f'{bucket}',
+            Key=f'{job_id}/{image_name}.png',
+            Body=output.getvalue(),
+            ContentType="image/png"
+        )
 
-    presigned_url = boto_client.generate_presigned_url(
-        'get_object',
-        Params={
-            'Bucket': f'{bucket}',
-            'Key': f'{job_id}/{image_name}.png'
-        }, ExpiresIn=604800)
+        presigned_url = boto_client.generate_presigned_url(
+            'get_object',
+            Params={
+                'Bucket': f'{bucket}',
+                'Key': f'{job_id}/{image_name}.png'
+            }, ExpiresIn=604800)
 
-    if results_list is not None:
-        results_list[result_index] = presigned_url
+        if results_list is not None:
+            results_list[result_index] = presigned_url
 
-    return presigned_url
+        return presigned_url
 
 
 # ---------------------------------------------------------------------------- #
 #                                Files To Upload                               #
 # ---------------------------------------------------------------------------- #
 def files(job_id, file_list):
     '''
@@ -154,58 +176,78 @@
             temp_boto_client.put_object(
                 Bucket=str(bucket_creds['bucketName']),
                 Key=f'{job_id}/{selected_file}',
                 Body=file_data,
             )
 
         bucket_urls.append(
-            f"{bucket_creds['endpointUrl']}/{bucket_creds['bucketName']}/{job_id}/{file}")
+            f"{bucket_creds['endpointUrl']}/{bucket_creds['bucketName']}/{job_id}/{selected_file}")
 
     return bucket_urls
 
 
 # ------------------------- Single File Bucket Upload ------------------------ #
-def file(file_name, file_location, bucket_creds):
+def upload_file_to_bucket(
+        file_name: str, file_location: str,
+        bucket_creds: Optional[dict] = None,
+        bucket_name: Optional[str] = None,
+        prefix: Optional[str] = None) -> str:
     '''
-    Uploads a single file to bucket storage.
+    Uploads a single file to bucket storage and returns a presigned URL.
     '''
-    temp_bucket_session = session.Session()
+    boto_client, transfer_config = get_boto_client(bucket_creds)
 
-    temp_boto_config = Config(
-        signature_version='s3v4',
-        retries={
-            'max_attempts': 3,
-            'mode': 'standard'
-        }
-    )
+    if not bucket_name:
+        bucket_name = time.strftime('%m-%y')
 
-    temp_transfer_config = TransferConfig(
-        multipart_threshold=1024 * 25,
-        max_concurrency=10,
-        multipart_chunksize=1024 * 25,
-        use_threads=True
-    )
-
-    temp_boto_client = temp_bucket_session.client(
-        's3',
-        endpoint_url=bucket_creds['endpointUrl'],
-        aws_access_key_id=bucket_creds['accessId'],
-        aws_secret_access_key=bucket_creds['accessSecret'],
-        config=temp_boto_config
-    )
+    key = f"{prefix}/{file_name}" if prefix else file_name
 
     file_size = os.path.getsize(file_location)
     with tqdm(total=file_size, unit='B', unit_scale=True, desc=file_name) as progress_bar:
-        temp_boto_client.upload_file(
-            file_location, str(bucket_creds['bucketName']), f'{file_name}',
-            Config=temp_transfer_config,
+        boto_client.upload_file(
+            file_location, bucket_name, key,
+            Config=transfer_config,
             Callback=progress_bar.update
         )
 
-    presigned_url = temp_boto_client.generate_presigned_url(
+    presigned_url = boto_client.generate_presigned_url(
+        'get_object',
+        Params={
+            'Bucket': bucket_name,
+            'Key': key
+        }, ExpiresIn=604800)
+
+    return presigned_url
+
+
+# --------------------------- Upload Memory Object --------------------------- #
+def upload_in_memory_object(
+        file_name: str, file_data: bytes,
+        bucket_creds: Optional[dict] = None,
+        bucket_name: Optional[str] = None,
+        prefix: Optional[str] = None) -> str:
+    '''
+    Uploads an in-memory object (bytes) to bucket storage and returns a presigned URL.
+    '''
+    boto_client, transfer_config = get_boto_client(bucket_creds)
+
+    if not bucket_name:
+        bucket_name = time.strftime('%m-%y')
+
+    key = f"{prefix}/{file_name}" if prefix else file_name
+
+    file_size = len(file_data)
+    with tqdm(total=file_size, unit='B', unit_scale=True, desc=file_name) as progress_bar:
+        boto_client.upload_fileobj(
+            io.BytesIO(file_data), bucket_name, key,
+            Config=transfer_config,
+            Callback=progress_bar.update
+        )
+
+    presigned_url = boto_client.generate_presigned_url(
         'get_object',
         Params={
-            'Bucket': f"{bucket_creds['bucketName']}",
-            'Key': f"{file_name}"
+            'Bucket': bucket_name,
+            'Key': key
         }, ExpiresIn=604800)
 
     return presigned_url
```

### Comparing `runpod-0.9.1/runpod/serverless/utils/rp_validator.py` & `runpod-0.9.2/runpod/serverless/utils/rp_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 '''
 runpod | serverless | utils | validator.py
 Provides a function to validate the input to the model.
 '''
 # pylint: disable=too-many-branches
+from typing import Any, Dict, List, Union
 
 
-def validate(raw_input, schema):
+def _add_error(error_list: List[str], message: str) -> None:
+    error_list.append(message)
+
+
+def validate(raw_input: Dict[str, Any], schema: Dict[str, Any]
+             ) -> Dict[str, Union[Dict[str, Any], List[str]]]:
     '''
     Validates the input.
     Checks to see if the provided inputs match the expected types.
     Checks to see if the required inputs are included.
     Sets the default values for the inputs that are not provided.
     Validates the inputs using the lambda constraints.
 
@@ -19,41 +25,42 @@
     {"validated_input": {"input1": "value1", "input2": "value2"}
     '''
     error_list = []
 
     # Check for unexpected inputs.
     for key in raw_input:
         if key not in schema:
-            error_list.append(f"Unexpected input. {key} is not a valid input option.")
+            _add_error(error_list, f"Unexpected input. {key} is not a valid input option.")
 
     # Checks for missing required inputs or sets the default values.
     for key, rules in schema.items():
         if 'required' not in rules:
-            error_list.append(f"Schema error, missing 'required' for {key}.")
+            _add_error(error_list, f"Schema error, missing 'required' for {key}.")
         elif rules['required'] and key not in raw_input:
-            error_list.append(f"{key} is a required input.")
+            _add_error(error_list, f"{key} is a required input.")
         elif rules['required'] and key not in raw_input and "default" not in rules:
-            error_list.append(f"Schema error, missing default value for {key}.")
+            _add_error(error_list, f"Schema error, missing default value for {key}.")
         elif not rules['required'] and key not in raw_input and "default" not in rules:
-            error_list.append(f"Schema error, missing default value for {key}.")
+            _add_error(error_list, f"Schema error, missing default value for {key}.")
         elif not rules['required'] and key not in raw_input:
             raw_input[key] = raw_input.get(key, rules['default'])
 
     for key, rules in schema.items():
         # Enforce floats to be floats.
         if rules['type'] is float and type(raw_input[key]) in [int, float]:
             raw_input[key] = float(raw_input[key])
 
         # Check for the correct type.
         if not isinstance(raw_input[key], rules['type']) and raw_input[key] is not None:
-            error_list.append(f"{key} should be {rules['type']} type, not {type(raw_input[key])}.")
+            _add_error(
+                error_list, f"{key} should be {rules['type']} type, not {type(raw_input[key])}.")
 
         # Check lambda constraints.
         if "constraints" in rules:
             if not rules['constraints'](raw_input[key]):
-                error_list.append(f"{key} does not meet the constraints.")
+                _add_error(error_list, f"{key} does not meet the constraints.")
 
     validation_return = {"validated_input": raw_input}
     if error_list:
         validation_return = {"errors": error_list}
 
     return validation_return
```

### Comparing `runpod-0.9.1/runpod/serverless/work_loop.py` & `runpod-0.9.2/runpod/serverless/work_loop.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,63 @@
-'''
+"""
 runpod | serverless | worker_loop.py
 Called to convert a container into a worker pod for the runpod serverless platform.
-'''
+"""
 
 import os
 
 import aiohttp
 
 import runpod.serverless.modules.logging as log
 from .modules.heartbeat import start_ping
 from .modules.job import get_job, run_job, send_result
 from .modules.worker_state import set_job_id
 
+_TIMEOUT = aiohttp.ClientTimeout(total=300, connect=2, sock_connect=2)
 
-timeout = aiohttp.ClientTimeout(total=300, connect=2, sock_connect=2)
+
+def _get_auth_header() -> dict:
+    return {"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"}
+
+
+def _is_local_testing() -> bool:
+    return os.environ.get("RUNPOD_WEBHOOK_GET_JOB", None) is None
 
 
 async def start_worker(config):
-    '''
-    starts the worker loop
-    '''
-    auth_header = {"Authorization": f"{os.environ.get('RUNPOD_AI_API_KEY')}"}
+    """
+    Starts the worker loop.
+    """
+    auth_header = _get_auth_header()
 
-    async with aiohttp.ClientSession(headers=auth_header) as session:
+    async with aiohttp.ClientSession(headers=auth_header, timeout=_TIMEOUT) as session:
 
         start_ping()
 
         while True:
             job = await get_job(session)
 
             if job is None:
-                log.info("No job available before idle timeout.")
+                log.info("No job available, waiting for the next one.")
                 continue
 
             if job["input"] is None:
-                log.error("No input parameter provided. Erroring out request.")
+                log.error(f"Job {job['id']} has no input parameter provided. Skipping this job.")
                 continue
 
             set_job_id(job["id"])
 
+            log.info(f"Processing job {job['id']}")
             job_result = run_job(config["handler"], job)
 
+            # If refresh_worker is set, pod will be reset after job is complete.
+            if config.get("refresh_worker", False):
+                log.info(f"Refresh worker flag set, stopping pod after job {job['id']}.")
+                job_result["stopPod"] = True
+
             await send_result(session, job_result, job)
 
             set_job_id(None)
 
-            if os.environ.get('RUNPOD_WEBHOOK_GET_JOB', None) is None:
+            if _is_local_testing():
                 log.info("Local testing complete, exiting.")
                 break
```

### Comparing `runpod-0.9.1/runpod.egg-info/PKG-INFO` & `runpod-0.9.2/runpod.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runpod
-Version: 0.9.1
+Version: 0.9.2
 Summary: Official Python library for RunPod API & SDK.
 Home-page: https://github.com/runpod/runpod-python
 Author: RunPod
 Author-email: support@runpod.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/runpod/runpod-python/issues
 Keywords: runpod,ai,gpu,serverless,SDK,API,python,library
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 <div align="center">
 <h1>RunPod | Python Library </h1>
 
 [![CI | Code Quality](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml/badge.svg)](https://github.com/runpod/runpod-python/actions/workflows/ci_pylint.yml)
 &nbsp;
@@ -55,69 +56,76 @@
 ### Quick Start
 
 Create an python script in your project that contains your model definition and the RunPod worker start code. Run this python code as your default container start command:
 
 ```python
 import runpod
 
-MODEL = 'YOUR_MODEL'
+def is_even(job):
 
-def run(job):
-    # Your inference code here
-    return MODEL.predict(job.input)
+    job_input = job["input"]
+    the_number = job_input["number"]
 
-runpod.serverless.start({"handler": run})
+    if not isinstance(the_number, int):
+        return {"error": "Silly human, you need to pass an integer."}
+
+    if the_number % 2 == 0:
+        return True
+
+    return False
+
+runpod.serverless.start({"handler": is_even})
 ```
 
 Make sure that this file is ran when your container starts. This can be accomplished by calling it in the docker command when you setup a template at [runpod.io/console/serverless/user/templates](https://www.runpod.io/console/serverless/user/templates) or by setting it as the default command in your Dockerfile.
 
 See our [blog post](https://www.runpod.io/blog/serverless-create-a-basic-api) for creating a basic Serverless API, or view the [details docs](https://docs.runpod.io/serverless-ai/custom-apis) for more information.
 
 ## API Language Library
 
 When interacting with the RunPod API you can use this library to make requests to the API.
 
 ```python
 import runpod
 
-runpod.api_key = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+runpod.api_key = "your_runpod_api_key_found_under_settings"
 ```
 
 ### Endpoints
 
 You can interact with RunPod endpoints via a `run` or `run_sync` method.
 
 ```python
 endpoint = runpod.Endpoint("ENDPOINT_ID")
 
 run_request = endpoint.run(
-    {"YOUR_MODEL_INPUT_JSON": "YOUR_MODEL_INPUT_VALUE"}
+    {"your_model_input_key": "your_model_input_value"}
 )
 
 # Check the status of the endpoint run request
 print(run_request.status())
 
 # Get the output of the endpoint run request, blocking until the endpoint run is complete.
 print(run_request.output())
 ```
 
 ```python
 endpoint = runpod.Endpoint("ENDPOINT_ID")
 
 run_request = endpoint.run_sync(
-    {"YOUR_MODEL_INPUT_JSON": "YOUR_MODEL_INPUT_VALUE"}
+    {"your_model_input_key": "your_model_input_value"}
 )
 
 # Returns the job results if completed within 90 seconds, otherwise, returns the job status.
 print(run_request )
 ```
 
 ## Directory
 
-```
+```BASH
 .
 ├── docs               # Documentation
 ├── runpod             # Package source code
 │   ├── endpoint       # Language library - Endpoints
 │   └── serverless     # SDK - Serverless Worker
 └── tests              # Package tests
 ```
```

### Comparing `runpod-0.9.1/setup.cfg` & `runpod-0.9.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = runpod
-version = 0.9.1
+version = 0.0.0  # Placeholder value, will be overridden by setuptools_scm
 description = Official Python library for RunPod API & SDK.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = runpod, ai, gpu, serverless, SDK, API, python, library
 url = https://github.com/runpod/runpod-python
 project_urls = 
 	Bug Tracker = https://github.com/runpod/runpod-python/issues
@@ -22,19 +22,28 @@
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >= 3.6
 install_requires = 
+	backoff == 2.2.1
 	pillow >= 9.3.0
 	python-dotenv >= 0.21.0
 	requests >= 2.28.1
 	tqdm-loggable >= 0.1.3
 	boto3 >= 1.26.15
 	aiohttp >= 3.8.3
 	fastapi[all] >= 0.89.0
 
+[options.extras_require]
+test = 
+	pytest
+	pytest-asyncio
+
+[setuptools_scm]
+write_to = runpod/_version.py
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `runpod-0.9.1/tests/test_endpoint/test_runner.py` & `runpod-0.9.2/tests/test_endpoint/test_runner.py`

 * *Files identical despite different names*

### Comparing `runpod-0.9.1/tests/test_serverless/test_module_download.py` & `runpod-0.9.2/tests/test_serverless/test_module_download.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,96 @@
 ''' Tests for runpod | serverless | modules | download.py '''
 # pylint: disable=R0903,W0613
 
+import os
 import unittest
 from unittest.mock import patch, mock_open
 
-from runpod.serverless.utils.rp_download import download_input_objects
+import requests
+
+from runpod.serverless.utils.rp_download import download_files_from_urls
 
 URL_LIST = ['https://example.com/picture.jpg',
             'https://example.com/picture.jpg?X-Amz-Signature=123']
 
+JOB_ID = "job_123"
+
 
 def mock_requests_get(*args, **kwargs):
     '''
     Mocks requests.get
     '''
+    headers = {
+        'Content-Disposition': 'attachment; filename="picture.jpg"'
+    }
+
     class MockResponse:
         ''' Mocks requests.get response '''
 
-        def __init__(self, content, status_code):
+        def __init__(self, content, status_code, headers=None):
             '''
             Mocks requests.get response
             '''
             self.content = content
             self.status_code = status_code
+            self.headers = headers or {}
+
+        def raise_for_status(self):
+            ''' Mocks raise_for_status function '''
+            if 400 <= self.status_code < 600:
+                raise requests.exceptions.RequestException(f"Status code: {self.status_code}")
+
+        def __enter__(self):
+            return self
+
+        def __exit__(self, *args):
+            pass
 
     if args[0] in URL_LIST:
-        return MockResponse(b'nothing', 200)
+        return MockResponse(b'nothing', 200, headers)
 
     return MockResponse(None, 404)
 
 
-class TestDownloadInputObjects(unittest.TestCase):
-    ''' Tests for download_input_objects '''
+class TestDownloadFilesFromUrls(unittest.TestCase):
+    ''' Tests for download_files_from_urls '''
 
     @patch('os.makedirs', return_value=None)
     @patch('requests.get', side_effect=mock_requests_get)
     @patch('builtins.open', new_callable=mock_open)
-    def test_download_input_objects(self, mock_open_file, mock_get, mock_makedirs):
+    def test_download_files_from_urls(self, mock_open_file, mock_get, mock_makedirs):
         '''
-        Tests download_input_objects
+        Tests download_files_from_urls
         '''
-        objects = download_input_objects(
-            ['https://example.com/picture.jpg', ]
+        downloaded_files = download_files_from_urls(
+            JOB_ID, ['https://example.com/picture.jpg', ]
         )
 
-        self.assertEqual(len(objects), 1)
+        self.assertEqual(len(downloaded_files), 1)
 
         # Check that the url was called with requests.get
         self.assertIn('https://example.com/picture.jpg', mock_get.call_args_list[0][0])
 
-        mock_open_file.assert_called_once_with(objects[0], 'wb')
-        mock_makedirs.assert_called_once_with('input_objects', exist_ok=True)
+        mock_open_file.assert_called_once_with(downloaded_files[0], 'wb')
+        mock_makedirs.assert_called_once_with(os.path.abspath(
+            f'jobs/{JOB_ID}/downloaded_files'), exist_ok=True)
 
     @patch('os.makedirs', return_value=None)
     @patch('requests.get', side_effect=mock_requests_get)
     @patch('builtins.open', new_callable=mock_open)
-    def test_download_input_objects_signed(self, mock_open_file, mock_get, mock_makedirs):
+    def test_download_files_from_urls_signed(self, mock_open_file, mock_get, mock_makedirs):
         '''
-        Tests download_input_objects with signed urls
+        Tests download_files_from_urls with signed urls
         '''
-        objects = download_input_objects(
-            ['https://example.com/picture.jpg?X-Amz-Signature=123', ]
+        downloaded_files = download_files_from_urls(
+            JOB_ID, ['https://example.com/picture.jpg?X-Amz-Signature=123', ]
         )
 
-        # Confirms that the same number of objects were downloaded as urls provided
-        self.assertEqual(len(objects), 1)
+        # Confirms that the same number of files were downloaded as urls provided
+        self.assertEqual(len(downloaded_files), 1)
 
         # Check that the url was called with requests.get
         self.assertIn(URL_LIST[1], mock_get.call_args_list[0][0])
 
-        mock_open_file.assert_called_once_with(objects[0], 'wb')
-        mock_makedirs.assert_called_once_with('input_objects', exist_ok=True)
+        mock_open_file.assert_called_once_with(downloaded_files[0], 'wb')
+        mock_makedirs.assert_called_once_with(os.path.abspath(
+            f'jobs/{JOB_ID}/downloaded_files'), exist_ok=True)
```

### Comparing `runpod-0.9.1/tests/test_serverless/test_pod_worker.py` & `runpod-0.9.2/tests/test_serverless/test_pod_worker.py`

 * *Files identical despite different names*

