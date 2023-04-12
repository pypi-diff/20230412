# Comparing `tmp/kiara_plugin.network_analysis-0.4.8.tar.gz` & `tmp/kiara_plugin.network_analysis-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.network_analysis-0.4.8.tar", last modified: Sun Jan 15 17:41:05 2023, max compression
+gzip compressed data, was "kiara_plugin.network_analysis-0.4.9.tar", last modified: Tue Jan 24 20:29:08 2023, max compression
```

## Comparing `kiara_plugin.network_analysis-0.4.8.tar` & `kiara_plugin.network_analysis-0.4.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.448979 kiara_plugin.network_analysis-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.448979 kiara_plugin.network_analysis-0.4.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.448979 kiara_plugin.network_analysis-0.4.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/examples/pipelines/create_network_graph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/examples/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/examples/scripts/create_network_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.452980 kiara_plugin.network_analysis-0.4.8/examples/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/examples/streamlit/simple_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.448979 kiara_plugin.network_analysis-0.4.8/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-01-15 17:41:05.460980 kiara_plugin.network_analysis-0.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1402 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.448979 kiara_plugin.network_analysis-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.448979 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/pipelines/create.network_data.from.files.json
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/pipelines/import.network_data.from.local_file_paths.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-01-15 17:41:05.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-01-15 17:41:05.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 17:41:05.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-01-15 17:41:05.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 17:40:12.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-15 17:41:05.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-15 17:41:05.000000 kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 17:41:05.456980 kiara_plugin.network_analysis-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-01-15 17:40:02.000000 kiara_plugin.network_analysis-0.4.8/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.433916 kiara_plugin.network_analysis-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.433916 kiara_plugin.network_analysis-0.4.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.433916 kiara_plugin.network_analysis-0.4.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/examples/pipelines/create_network_graph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/examples/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/examples/scripts/create_network_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.437916 kiara_plugin.network_analysis-0.4.9/examples/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/examples/streamlit/simple_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.433916 kiara_plugin.network_analysis-0.4.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1402 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.433916 kiara_plugin.network_analysis-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.433916 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16952 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/pipelines/create.network_data.from.files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/pipelines/import.network_data.from.local_file_paths.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-01-24 20:29:08.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-01-24 20:29:08.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:29:08.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-24 20:29:08.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:28:21.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-24 20:29:08.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-24 20:29:08.000000 kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:29:08.441916 kiara_plugin.network_analysis-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-01-24 20:28:12.000000 kiara_plugin.network_analysis-0.4.9/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.network_analysis-0.4.8/.cruft.json` & `kiara_plugin.network_analysis-0.4.9/.cruft.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'b9f3af819a31735ed09c6b9cc605c12486bcfcd9'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "1d42cef85d7646d690df07481ac330b5d1a96d53",
+    "commit": "b9f3af819a31735ed09c6b9cc605c12486bcfcd9",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.network_analysis-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.network_analysis-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.network_analysis-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/.github/workflows/build-darwin.yaml` & `kiara_plugin.network_analysis-0.4.9/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/.github/workflows/build-linux.yaml` & `kiara_plugin.network_analysis-0.4.9/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/.github/workflows/build-windows.yaml` & `kiara_plugin.network_analysis-0.4.9/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/.gitignore` & `kiara_plugin.network_analysis-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/.pre-commit-config.yaml` & `kiara_plugin.network_analysis-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/LICENSE` & `kiara_plugin.network_analysis-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/Makefile` & `kiara_plugin.network_analysis-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/PKG-INFO` & `kiara_plugin.network_analysis-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.network_analysis
-Version: 0.4.8
+Version: 0.4.9
 Summary: kiara modules and datatypes for network analysis.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.network_analysis
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.network_analysis
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.network_analysis
 Keywords: kiara
```

### Comparing `kiara_plugin.network_analysis-0.4.8/README.md` & `kiara_plugin.network_analysis-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/docs/development.md` & `kiara_plugin.network_analysis-0.4.9/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/docs/index.md` & `kiara_plugin.network_analysis-0.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.network_analysis-0.4.9/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.network_analysis-0.4.9/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/examples/pipelines/create_network_graph.yaml` & `kiara_plugin.network_analysis-0.4.9/examples/pipelines/create_network_graph.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 pipeline_name: create_network_graph
 doc: Onboard network data
 steps:
-  - module_type: import.file
+  - module_type: import.local.file
     step_id: import_edges_file
   - module_type: create.table.from.file
     step_id: create_edges_table
     input_links:
       file: import_edges_file.file
-  - module_type: import.file
+  - module_type: import.local.file
     step_id: import_nodes_file
   - module_type: create.table.from.file
     step_id: create_nodes_table
     input_links:
       file: import_nodes_file.file
   - module_type: create.network_data.from.tables
     step_id: assemble_network_data
```

### Comparing `kiara_plugin.network_analysis-0.4.8/examples/scripts/create_network_data.py` & `kiara_plugin.network_analysis-0.4.9/examples/scripts/create_network_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 from kiara.interfaces.python_api.workflow import Workflow
 from kiara.utils.cli import terminal_print_model
 
 workflow = Workflow.create("network_analysis")
 
-workflow.add_step(operation="import.file", step_id="import_edges")
+workflow.add_step(operation="import.local.file", step_id="import_edges")
 workflow.add_step(operation="create.table.from.file", step_id="create_edges_table")
-workflow.add_step(operation="import.file", step_id="import_nodes")
+workflow.add_step(operation="import.local.file", step_id="import_nodes")
 workflow.add_step(operation="create.table.from.file", step_id="create_nodes_table")
 workflow.add_step(
     operation="create.network_data.from.tables", step_id="assemble_network_data"
 )
 
 workflow.connect_steps("import_edges", "file", "create_edges_table", "file")
 workflow.connect_steps("import_nodes", "file", "create_nodes_table", "file")
```

### Comparing `kiara_plugin.network_analysis-0.4.8/examples/streamlit/simple_graph.py` & `kiara_plugin.network_analysis-0.4.9/examples/streamlit/simple_graph.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,254 +1,252 @@
 # -*- coding: utf-8 -*-
 
 # run with:
 #
 # streamlit run examples/streamlit/network_analysis/create_graphs.py
 
-import os
-import tempfile
-from typing import Iterable, List, Tuple
-
-import networkx as nx
-import streamlit as st
-import streamlit.components.v1 as components
-from kiara import Kiara
-from kiara.interfaces.python_api.operation import KiaraOperation
-from kiara.models.values.value import Value
-from kiara_plugin.tabular.models.table import KiaraTableMetadata
-from pyvis.network import Network
-from streamlit.uploaded_file_manager import UploadedFile
-
-from kiara_plugin.network_analysis.models import NetworkData
-
-st.title("Kiara/streamlit experiment - create a network graph")
-
-kiara_obj = Kiara.instance()
-
-
-def import_bytes(kiara: Kiara, uploaded_file: UploadedFile):
-
-    with tempfile.TemporaryDirectory() as tmpdirname:
-        path = os.path.join(tmpdirname, uploaded_file.name)
-        with open(path, "wb") as f:
-            f.write(uploaded_file.getbuffer())
-
-        op = KiaraOperation(kiara=kiara, operation_name="create.table.from.file")
-        inputs = {"file": path}
-        job_id = op.queue_job(**inputs)
-
-        op.save_result(
-            job_id=job_id, aliases={"table": uploaded_file.name.replace(".", "__")}
-        )
-
-        # imported: ValueSet = kiara.run(  # type: ignore
-        #     "file.import_from.local.file_path",
-        #     inputs={"source": path},
-        # )
-        # file_item = imported.get_value_obj("value_item")
-        # assert file_item is not None
-        # file_item.save(aliases=[uploaded_file.name.replace(".", "__")])
-
-
-def onboard_file(kiara: Kiara, uploaded_file):
-
-    if uploaded_file:
-        if isinstance(uploaded_file, UploadedFile):
-            import_bytes(kiara=kiara, uploaded_file=uploaded_file)
-        else:
-            for x in uploaded_file:
-                import_bytes(kiara=kiara, uploaded_file=x)
-
-
-def find_all_aliases_of_type(kiara: Kiara, value_type: str) -> List[str]:
-
-    result = []
-    for alias, alias_item in kiara.alias_registry.aliases.items():
-        value = kiara.data_registry.get_value(alias_item.value_id)
-        if value.data_type_name == value_type:
-            result.append(alias)
-
-    return result
-
-
-def table_mgmt(kiara: Kiara):
-
-    fp = st.sidebar.file_uploader(
-        "Import table(s) from csv file(s)", type=["csv"], accept_multiple_files=True
-    )
-    if fp:
-        onboard_file(kiara=kiara, uploaded_file=fp)
-
-    st.sidebar.write("## All your tables:")
-    all_table_aliases = find_all_aliases_of_type(kiara, value_type="table")
-    if not all_table_aliases:
-        st.sidebar.write(" -- no tables --")
-    else:
-        for a in all_table_aliases:
-            st.sidebar.write(a)
-
-
-def graphs_list(kiara: Kiara):
-
-    st.sidebar.write("## All your graphs:")
-    all_graph_aliases = find_all_aliases_of_type(kiara, value_type="network_data")
-    if not all_graph_aliases:
-        st.sidebar.write(" -- no graphs --")
-    else:
-        for a in all_graph_aliases:
-            st.sidebar.write(a)
-
-
-def create_graph(kiara: Kiara):
-    def create_graph(
-        alias, edges, nodes, source_column, target_column, weight_column, node_index
-    ) -> Tuple[str, Value]:
-
-        st.write("GRAPH")
-        if not alias:
-            return ("No alias specified, doing nothing...", None)
-
-        all_graph_aliases = find_all_aliases_of_type(kiara, value_type="network_data")
-        if alias in all_graph_aliases:
-            return (f"Alias '{alias}' already registered.", None)
-
-        if not edges:
-            return ("No edges table specified, doing nothing...", None)
-
-        inputs = {
-            "edges": f"alias:{edges}",
-            "nodes": f"alias:{nodes}",
-            "source_column_name": source_column,
-            "target_column_name": target_column,
-            "id_column_name": node_index,
-        }
-
-        try:
-            op = KiaraOperation(
-                kiara=kiara, operation_name="create.network_data.from.tables"
-            )
-
-            job_id = op.queue_job(**inputs)
-            result = op.retrieve_result(job_id=job_id)
-
-            op.save_result(job_id=job_id, aliases={"network_data": alias})
-
-            network_data = result.get_value_obj("network_data")
-
-            return (f"Saved network graph as: {alias}.", network_data)
-        except Exception as e:
-            return (f"Error creating graph: {e}", None)
-
-        return ("CREATED GRAPH", None)
-
-    def get_table_column_names(alias):
-
-        if not alias:
-            return []
-        value = kiara.data_registry.get_value(f"alias:{alias}")
-        if not value:
-            return []
-
-        md: KiaraTableMetadata = value.get_property_data("metadata.table")
-        return md.table.column_names
-
-    def find_likely_index(options: Iterable, keyword: str):
-
-        for idx, alias in enumerate(options):
-            if keyword.lower() in alias.lower():
-                return idx
-
-        return 0
-
-    graph = None
-
-    st.write("Create a new graph")
-
-    graph_alias = st.text_input("The alias for the graph")
-    all_table_aliases = find_all_aliases_of_type(kiara, value_type="table")
-
-    default_edge_table = find_likely_index(all_table_aliases, "edge")
-    default_node_table = find_likely_index(all_table_aliases, "node")
-
-    select_edges = st.selectbox("Edges", all_table_aliases, index=default_edge_table)
-    select_nodes = st.selectbox("Nodes", all_table_aliases, index=default_node_table)
-
-    edge_column_names = get_table_column_names(select_edges)
-    nodes_column_names = get_table_column_names(select_nodes)
-
-    default_source_name = find_likely_index(edge_column_names, "source")
-    default_target_name = find_likely_index(edge_column_names, "target")
-    default_weight_name = find_likely_index(edge_column_names, "weight")
-    default_id_name = find_likely_index(nodes_column_names, "Id")
-
-    source_column_name = st.selectbox(
-        "Source column name", edge_column_names, index=default_source_name
-    )
-    target_column_name = st.selectbox(
-        "Target column name", edge_column_names, index=default_target_name
-    )
-    weight_column_name = st.selectbox(
-        "Weight column name", edge_column_names, index=default_weight_name
-    )
-    nodes_index_name = st.selectbox(
-        "Nodes table_index", nodes_column_names, index=default_id_name
-    )
-
-    create_button = st.button(label="Create graph")
-    if create_button:
-        result, graph = create_graph(
-            alias=graph_alias,
-            edges=select_edges,
-            nodes=select_nodes,
-            source_column=source_column_name,
-            target_column=target_column_name,
-            weight_column=weight_column_name,
-            node_index=nodes_index_name,
-        )
-        st.info(result)
-
-    if graph is None:
-        return
-
-    st.write("Graph properties")
-    for prop in graph.property_names:
-        with st.expander(prop):
-            data = graph.get_property_data(prop)
-            st.write(data.dict())
-
-    network_data: NetworkData = graph.data
-    vis_graph = Network(
-        height="465px", bgcolor="#222222", font_color="white", directed=True
-    )
-    # add or remove "directed=True" above for displaying a directed graph with directed edges (with arrows)
-    vis_graph.from_nx(network_data.as_networkx_graph(graph_type=nx.DiGraph))
-    # change networkX graph type above to "Graph", "DiGraph", "MultiGraph", "MultiDiGraph" according to graph type
-    # add this line "vis_graph.set_edge_smooth('dynamic')" to display parallel edges, otherwise they will be stacked upon each other and thus be invisible
-
-    # Generate network with specific layout settings
-    vis_graph.repulsion(
-        node_distance=420,
-        central_gravity=0.33,
-        spring_length=110,
-        spring_strength=0.10,
-        damping=0.95,
-    )
-
-    # Save and read graph as HTML file (on Streamlit Sharing)
-    try:
-        path = "/tmp"
-        vis_graph.save_graph(f"{path}/pyvis_graph.html")
-        HtmlFile = open(f"{path}/pyvis_graph.html", "r", encoding="utf-8")
-
-    # Save and read graph as HTML file (locally)
-    except Exception:
-        path = "/html_files"
-        vis_graph.save_graph(f"{path}/pyvis_graph.html")
-        HtmlFile = open(f"{path}/pyvis_graph.html", "r", encoding="utf-8")
-
-    # Load HTML file in HTML component for display on Streamlit page
-    components.html(HtmlFile.read(), height=800, width=800)
-
-
-table_mgmt(kiara=kiara_obj)
-create_graph(kiara=kiara_obj)
-graphs_list(kiara=kiara_obj)
+# import os
+# import tempfile
+# from typing import Iterable, List, Tuple
+#
+# import networkx as nx
+# import streamlit as st
+# import streamlit.components.v1 as components
+# from kiara import Kiara
+# from kiara.models.values.value import Value
+# from kiara_plugin.tabular.models.table import KiaraTableMetadata
+# from pyvis.network import Network
+#
+# from kiara_plugin.network_analysis.models import NetworkData
+#
+# st.title("Kiara/streamlit experiment - create a network graph")
+#
+# kiara_obj = Kiara.instance()
+#
+#
+# def import_bytes(kiara: Kiara, uploaded_file: UploadedFile):
+#
+#     with tempfile.TemporaryDirectory() as tmpdirname:
+#         path = os.path.join(tmpdirname, uploaded_file.name)
+#         with open(path, "wb") as f:
+#             f.write(uploaded_file.getbuffer())
+#
+#         op = KiaraOperation(kiara=kiara, operation_name="create.table.from.file")
+#         inputs = {"file": path}
+#         job_id = op.queue_job(**inputs)
+#
+#         op.save_result(
+#             job_id=job_id, aliases={"table": uploaded_file.name.replace(".", "__")}
+#         )
+#
+#         # imported: ValueSet = kiara.run(  # type: ignore
+#         #     "file.import_from.local.file_path",
+#         #     inputs={"source": path},
+#         # )
+#         # file_item = imported.get_value_obj("value_item")
+#         # assert file_item is not None
+#         # file_item.save(aliases=[uploaded_file.name.replace(".", "__")])
+#
+#
+# def onboard_file(kiara: Kiara, uploaded_file):
+#
+#     if uploaded_file:
+#         if isinstance(uploaded_file, UploadedFile):
+#             import_bytes(kiara=kiara, uploaded_file=uploaded_file)
+#         else:
+#             for x in uploaded_file:
+#                 import_bytes(kiara=kiara, uploaded_file=x)
+#
+#
+# def find_all_aliases_of_type(kiara: Kiara, value_type: str) -> List[str]:
+#
+#     result = []
+#     for alias, alias_item in kiara.alias_registry.aliases.items():
+#         value = kiara.data_registry.get_value(alias_item.value_id)
+#         if value.data_type_name == value_type:
+#             result.append(alias)
+#
+#     return result
+#
+#
+# def table_mgmt(kiara: Kiara):
+#
+#     fp = st.sidebar.file_uploader(
+#         "Import table(s) from csv file(s)", type=["csv"], accept_multiple_files=True
+#     )
+#     if fp:
+#         onboard_file(kiara=kiara, uploaded_file=fp)
+#
+#     st.sidebar.write("## All your tables:")
+#     all_table_aliases = find_all_aliases_of_type(kiara, value_type="table")
+#     if not all_table_aliases:
+#         st.sidebar.write(" -- no tables --")
+#     else:
+#         for a in all_table_aliases:
+#             st.sidebar.write(a)
+#
+#
+# def graphs_list(kiara: Kiara):
+#
+#     st.sidebar.write("## All your graphs:")
+#     all_graph_aliases = find_all_aliases_of_type(kiara, value_type="network_data")
+#     if not all_graph_aliases:
+#         st.sidebar.write(" -- no graphs --")
+#     else:
+#         for a in all_graph_aliases:
+#             st.sidebar.write(a)
+#
+#
+# def create_graph(kiara: Kiara):
+#     def create_graph(
+#         alias, edges, nodes, source_column, target_column, weight_column, node_index
+#     ) -> Tuple[str, Value]:
+#
+#         st.write("GRAPH")
+#         if not alias:
+#             return ("No alias specified, doing nothing...", None)
+#
+#         all_graph_aliases = find_all_aliases_of_type(kiara, value_type="network_data")
+#         if alias in all_graph_aliases:
+#             return (f"Alias '{alias}' already registered.", None)
+#
+#         if not edges:
+#             return ("No edges table specified, doing nothing...", None)
+#
+#         inputs = {
+#             "edges": f"alias:{edges}",
+#             "nodes": f"alias:{nodes}",
+#             "source_column_name": source_column,
+#             "target_column_name": target_column,
+#             "id_column_name": node_index,
+#         }
+#
+#         try:
+#             op = KiaraOperation(
+#                 kiara=kiara, operation_name="create.network_data.from.tables"
+#             )
+#
+#             job_id = op.queue_job(**inputs)
+#             result = op.retrieve_result(job_id=job_id)
+#
+#             op.save_result(job_id=job_id, aliases={"network_data": alias})
+#
+#             network_data = result.get_value_obj("network_data")
+#
+#             return (f"Saved network graph as: {alias}.", network_data)
+#         except Exception as e:
+#             return (f"Error creating graph: {e}", None)
+#
+#         return ("CREATED GRAPH", None)
+#
+#     def get_table_column_names(alias):
+#
+#         if not alias:
+#             return []
+#         value = kiara.data_registry.get_value(f"alias:{alias}")
+#         if not value:
+#             return []
+#
+#         md: KiaraTableMetadata = value.get_property_data("metadata.table")
+#         return md.table.column_names
+#
+#     def find_likely_index(options: Iterable, keyword: str):
+#
+#         for idx, alias in enumerate(options):
+#             if keyword.lower() in alias.lower():
+#                 return idx
+#
+#         return 0
+#
+#     graph = None
+#
+#     st.write("Create a new graph")
+#
+#     graph_alias = st.text_input("The alias for the graph")
+#     all_table_aliases = find_all_aliases_of_type(kiara, value_type="table")
+#
+#     default_edge_table = find_likely_index(all_table_aliases, "edge")
+#     default_node_table = find_likely_index(all_table_aliases, "node")
+#
+#     select_edges = st.selectbox("Edges", all_table_aliases, index=default_edge_table)
+#     select_nodes = st.selectbox("Nodes", all_table_aliases, index=default_node_table)
+#
+#     edge_column_names = get_table_column_names(select_edges)
+#     nodes_column_names = get_table_column_names(select_nodes)
+#
+#     default_source_name = find_likely_index(edge_column_names, "source")
+#     default_target_name = find_likely_index(edge_column_names, "target")
+#     default_weight_name = find_likely_index(edge_column_names, "weight")
+#     default_id_name = find_likely_index(nodes_column_names, "Id")
+#
+#     source_column_name = st.selectbox(
+#         "Source column name", edge_column_names, index=default_source_name
+#     )
+#     target_column_name = st.selectbox(
+#         "Target column name", edge_column_names, index=default_target_name
+#     )
+#     weight_column_name = st.selectbox(
+#         "Weight column name", edge_column_names, index=default_weight_name
+#     )
+#     nodes_index_name = st.selectbox(
+#         "Nodes table_index", nodes_column_names, index=default_id_name
+#     )
+#
+#     create_button = st.button(label="Create graph")
+#     if create_button:
+#         result, graph = create_graph(
+#             alias=graph_alias,
+#             edges=select_edges,
+#             nodes=select_nodes,
+#             source_column=source_column_name,
+#             target_column=target_column_name,
+#             weight_column=weight_column_name,
+#             node_index=nodes_index_name,
+#         )
+#         st.info(result)
+#
+#     if graph is None:
+#         return
+#
+#     st.write("Graph properties")
+#     for prop in graph.property_names:
+#         with st.expander(prop):
+#             data = graph.get_property_data(prop)
+#             st.write(data.dict())
+#
+#     network_data: NetworkData = graph.data
+#     vis_graph = Network(
+#         height="465px", bgcolor="#222222", font_color="white", directed=True
+#     )
+#     # add or remove "directed=True" above for displaying a directed graph with directed edges (with arrows)
+#     vis_graph.from_nx(network_data.as_networkx_graph(graph_type=nx.DiGraph))
+#     # change networkX graph type above to "Graph", "DiGraph", "MultiGraph", "MultiDiGraph" according to graph type
+#     # add this line "vis_graph.set_edge_smooth('dynamic')" to display parallel edges, otherwise they will be stacked upon each other and thus be invisible
+#
+#     # Generate network with specific layout settings
+#     vis_graph.repulsion(
+#         node_distance=420,
+#         central_gravity=0.33,
+#         spring_length=110,
+#         spring_strength=0.10,
+#         damping=0.95,
+#     )
+#
+#     # Save and read graph as HTML file (on Streamlit Sharing)
+#     try:
+#         path = "/tmp"
+#         vis_graph.save_graph(f"{path}/pyvis_graph.html")
+#         HtmlFile = open(f"{path}/pyvis_graph.html", "r", encoding="utf-8")
+#
+#     # Save and read graph as HTML file (locally)
+#     except Exception:
+#         path = "/html_files"
+#         vis_graph.save_graph(f"{path}/pyvis_graph.html")
+#         HtmlFile = open(f"{path}/pyvis_graph.html", "r", encoding="utf-8")
+#
+#     # Load HTML file in HTML component for display on Streamlit page
+#     components.html(HtmlFile.read(), height=800, width=800)
+#
+#
+# table_mgmt(kiara=kiara_obj)
+# create_graph(kiara=kiara_obj)
+# graphs_list(kiara=kiara_obj)
```

### Comparing `kiara_plugin.network_analysis-0.4.8/mkdocs.yml` & `kiara_plugin.network_analysis-0.4.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/pyproject.toml` & `kiara_plugin.network_analysis-0.4.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara>=0.4.26",
-    "kiara-plugin.tabular>=0.4.19"
+    "kiara>=0.4.29",
+    "kiara-plugin.tabular>=0.4.20"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
@@ -47,14 +47,30 @@
 dev_utils = [
     "kiara[dev_utils]"
 ]
 dev_all = [
     "kiara[dev_all]"
 ]
 
+[project.entry-points."kiara.plugin"]
+network_analysis = "kiara_plugin.network_analysis"
+
+[project.entry-points."kiara.data_types"]
+network_analysis = "kiara_plugin.network_analysis:find_data_types"
+
+[project.entry-points."kiara.model_classes"]
+network_analysis = "kiara_plugin.network_analysis:find_model_classes"
+
+[project.entry-points."kiara.modules"]
+network_analysis = "kiara_plugin.network_analysis:find_modules"
+
+[project.entry-points."kiara.pipelines"]
+network_analysis = "kiara_plugin.network_analysis:find_pipelines"
+
+
 [project.urls]
 homepage = "https://github.com/DHARPA-Project/kiara_plugin.network_analysis"
 documentation = "https://DHARPA-Project.github.io/kiara_plugin.network_analysis"
 repository = "https://github.com/DHARPA-Project/kiara_plugin.network_analysis"
 
 [tool.black]
 include = '\.pyi?$'
```

### Comparing `kiara_plugin.network_analysis-0.4.8/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.network_analysis-0.4.9/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/scripts/documentation/gen_info_pages.py` & `kiara_plugin.network_analysis-0.4.9/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/scripts/documentation/gen_module_doc.py` & `kiara_plugin.network_analysis-0.4.9/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/setup.cfg` & `kiara_plugin.network_analysis-0.4.9/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 [options]
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
-[options.entry_points]
-kiara.data_types = 
-	network_analysis = kiara_plugin.network_analysis:find_data_types
-kiara.model_classes = 
-	network_analysis = kiara_plugin.network_analysis:find_model_classes
-kiara.modules = 
-	network_analysis = kiara_plugin.network_analysis:find_modules
-kiara.pipelines = 
-	network_analysis = kiara_plugin.network_analysis:find_pipelines
-
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [aliases]
 build = bdist_wheel
```

### Comparing `kiara_plugin.network_analysis-0.4.8/setup.py` & `kiara_plugin.network_analysis-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/__init__.py` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/data_types.py` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/data_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/models.py` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/modules/__init__.py` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/pipelines/create.network_data.from.files.json` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/pipelines/create.network_data.from.files.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/pipelines/import.network_data.from.local_file_paths.json` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/pipelines/import.network_data.from.local_file_paths.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'steps'": "{0: {'module_type': 'import.local.file'}, 2: {'module_type': 'import.local.file'}}"}*

```diff
@@ -12,26 +12,26 @@
     },
     "output_aliases": {
         "assemble_network_data.network_data": "network_data"
     },
     "pipeline_name": "import.network_data.from.local_file_paths",
     "steps": [
         {
-            "module_type": "import.file",
+            "module_type": "import.local.file",
             "step_id": "import_edges_file"
         },
         {
             "input_links": {
                 "file": "import_edges_file.file"
             },
             "module_type": "create.table.from.file",
             "step_id": "create_edges_table"
         },
         {
-            "module_type": "import.file",
+            "module_type": "import.local.file",
             "step_id": "import_nodes_file"
         },
         {
             "input_links": {
                 "file": "import_nodes_file.file"
             },
             "module_type": "create.table.from.file",
```

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin/network_analysis/utils.py` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin/network_analysis/utils.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/PKG-INFO` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.network-analysis
-Version: 0.4.8
+Version: 0.4.9
 Summary: kiara modules and datatypes for network analysis.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.network_analysis
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.network_analysis
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.network_analysis
 Keywords: kiara
```

### Comparing `kiara_plugin.network_analysis-0.4.8/src/kiara_plugin.network_analysis.egg-info/SOURCES.txt` & `kiara_plugin.network_analysis-0.4.9/src/kiara_plugin.network_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

