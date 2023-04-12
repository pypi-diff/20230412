# Comparing `tmp/quickmpc-0.3.2.tar.gz` & `tmp/quickmpc-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-omv8n967/quickmpc-0.3.2.tar", last modified: Mon Apr 10 10:12:30 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-46fhb54f/quickmpc-0.3.3.tar", last modified: Wed Apr 12 08:18:21 2023, max compression
```

## Comparing `quickmpc-0.3.2.tar` & `quickmpc-0.3.3.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-10 10:12:15.000000 quickmpc-0.3.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 10:12:15.000000 quickmpc-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 10:12:15.000000 quickmpc-0.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 10:12:30.000000 quickmpc-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 10:12:15.000000 quickmpc-0.3.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-10 10:12:15.000000 quickmpc-0.3.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-10 10:12:15.000000 quickmpc-0.3.2/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-10 10:12:15.000000 quickmpc-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data-meshcode.csv
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data1-1.csv
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data1-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/data/data1-3.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/integration_demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/integration_demo/execute_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/integration_demo/progress_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/integration_demo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/demo/unit_demo/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/delete_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/demo_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/execute_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_computation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_elapsed_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/get_join_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-10 10:12:15.000000 quickmpc-0.3.2/demo/unit_demo/send_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-10 10:12:15.000000 quickmpc-0.3.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-10 10:12:15.000000 quickmpc-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/utils/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 10:12:15.000000 quickmpc-0.3.2/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-10 10:12:30.000000 quickmpc-0.3.2/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-10 10:12:30.000000 quickmpc-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 10:12:15.000000 quickmpc-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:12:30.000000 quickmpc-0.3.2/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-10 10:12:15.000000 quickmpc-0.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 08:17:59.000000 quickmpc-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 08:17:59.000000 quickmpc-0.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 08:18:21.000000 quickmpc-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 08:17:59.000000 quickmpc-0.3.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-12 08:17:59.000000 quickmpc-0.3.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 08:17:59.000000 quickmpc-0.3.3/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 08:17:59.000000 quickmpc-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data-meshcode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data1-1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data1-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data1-3.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/integration_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/integration_demo/execute_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/integration_demo/progress_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/integration_demo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/unit_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/delete_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/demo_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/execute_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_computation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_elapsed_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_join_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/send_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-12 08:17:59.000000 quickmpc-0.3.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 08:17:59.000000 quickmpc-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/qmpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-12 08:18:21.000000 quickmpc-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 08:17:59.000000 quickmpc-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/unit_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server1.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server2.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server2.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server3.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server3.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/unit_tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tox.ini
```

### Comparing `quickmpc-0.3.2/.vscode/settings.json` & `quickmpc-0.3.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/LICENSE` & `quickmpc-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/Pipfile.lock` & `quickmpc-0.3.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/README-ja.md` & `quickmpc-0.3.3/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/README.md` & `quickmpc-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/README-ja.md` & `quickmpc-0.3.3/demo/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/README.md` & `quickmpc-0.3.3/demo/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/integration_demo/execute_demo.py` & `quickmpc-0.3.3/demo/integration_demo/execute_demo.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/integration_demo/progress_demo.py` & `quickmpc-0.3.3/demo/integration_demo/progress_demo.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/unit_demo/delete_share.py` & `quickmpc-0.3.3/demo/unit_demo/delete_share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/unit_demo/demo_sharize.py` & `quickmpc-0.3.3/demo/unit_demo/demo_sharize.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/unit_demo/execute_computation.py` & `quickmpc-0.3.3/demo/unit_demo/execute_computation.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/unit_demo/get_computation_result.py` & `quickmpc-0.3.3/demo/unit_demo/get_computation_result.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/unit_demo/get_elapsed_time.py` & `quickmpc-0.3.3/demo/unit_demo/get_elapsed_time.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/unit_demo/get_join_table.py` & `quickmpc-0.3.3/demo/unit_demo/get_join_table.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/demo/unit_demo/send_share.py` & `quickmpc-0.3.3/demo/unit_demo/send_share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/mypy.ini` & `quickmpc-0.3.3/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/README.md` & `quickmpc-0.3.3/quickmpc/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/qmpc.py` & `quickmpc-0.3.3/quickmpc/qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/qmpc_server.py` & `quickmpc-0.3.3/quickmpc/qmpc_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,22 +41,24 @@
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class QMPCServer:
     endpoints: InitVar[List[str]]
     __client_stubs: Tuple[LibcToManageStub] = field(init=False)
+    __client_channels: Tuple[grpc.Channel] = field(init=False)
     __party_size: int = field(init=False)
     token: str
     retry_num: int = 10
     retry_wait_time: int = 5
 
     def __post_init__(self, endpoints: List[str]) -> None:
-        stubs = [LibcToManageStub(QMPCServer.__create_grpc_channel(ep))
-                 for ep in endpoints]
+        chs = [QMPCServer.__create_grpc_channel(ep) for ep in endpoints]
+        stubs = [LibcToManageStub(ch) for ch in chs]
+        object.__setattr__(self, "_QMPCServer__client_channels", chs)
         object.__setattr__(self, "_QMPCServer__client_stubs", stubs)
         object.__setattr__(self, "_QMPCServer__party_size", len(endpoints))
 
     @staticmethod
     def __create_grpc_channel(endpoint: str) -> grpc.Channel:
         channel: grpc.Channel = None
         o = urlparse(endpoint)
@@ -88,14 +90,23 @@
         if not all([0 <= join <= 2 for join in join_order[1]]):
             logger.error('join value must be in the range of 0 to 2')
             return False
         return True
 
     def __retry(self, f: Callable, *request: Any) -> Any:
         for _ in range(self.retry_num):
+            # channelの接続チェック
+            try:
+                for ch in self.__client_channels:
+                    grpc.channel_ready_future(ch).result(timeout=5)
+            except grpc.FutureTimeoutError as e:
+                logger.error(e)
+                continue
+
+            # requestを送る
             try:
                 return f(*request)
             except grpc.RpcError as e:
                 logger.error(f'{e.details()} ({e.code()})')
 
                 # エラーが詳細な情報を持っているか確認
                 status = rpc_status.from_call(e)
```

### Comparing `quickmpc-0.3.2/quickmpc/share.py` & `quickmpc-0.3.3/quickmpc/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/utils/make_pieces.py` & `quickmpc-0.3.3/quickmpc/utils/make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/utils/overload_tools.py` & `quickmpc-0.3.3/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/utils/parse_csv.py` & `quickmpc-0.3.3/quickmpc/utils/parse_csv.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/utils/random.py` & `quickmpc-0.3.3/quickmpc/utils/random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc/utils/restore.py` & `quickmpc-0.3.3/quickmpc/utils/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/quickmpc.egg-info/SOURCES.txt` & `quickmpc-0.3.3/quickmpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/certificates/server1.key` & `quickmpc-0.3.3/tests/unit_tests/certificates/server1.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/certificates/server1.pem` & `quickmpc-0.3.3/tests/unit_tests/certificates/server1.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/certificates/server2.key` & `quickmpc-0.3.3/tests/unit_tests/certificates/server2.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/certificates/server2.pem` & `quickmpc-0.3.3/tests/unit_tests/certificates/server2.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/certificates/server3.key` & `quickmpc-0.3.3/tests/unit_tests/certificates/server3.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/certificates/server3.pem` & `quickmpc-0.3.3/tests/unit_tests/certificates/server3.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/conftest.py` & `quickmpc-0.3.3/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/local_server.py` & `quickmpc-0.3.3/tests/unit_tests/local_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_files/edge_data.csv` & `quickmpc-0.3.3/tests/unit_tests/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_files/string_data.csv` & `quickmpc-0.3.3/tests/unit_tests/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.3.3/tests/unit_tests/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_over_load.py` & `quickmpc-0.3.3/tests/unit_tests/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_parse.py` & `quickmpc-0.3.3/tests/unit_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_qmpc.py` & `quickmpc-0.3.3/tests/unit_tests/test_qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_random.py` & `quickmpc-0.3.3/tests/unit_tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_restore.py` & `quickmpc-0.3.3/tests/unit_tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_share_recons.py` & `quickmpc-0.3.3/tests/unit_tests/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.2/tests/unit_tests/test_share_sharize.py` & `quickmpc-0.3.3/tests/unit_tests/test_share_sharize.py`

 * *Files identical despite different names*

