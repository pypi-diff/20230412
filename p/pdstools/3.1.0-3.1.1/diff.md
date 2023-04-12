# Comparing `tmp/pdstools-3.1.0.tar.gz` & `tmp/pdstools-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.1.0.tar", last modified: Mon Apr 10 15:05:14 2023, max compression
+gzip compressed data, was "pdstools-3.1.1.tar", last modified: Wed Apr 12 15:49:37 2023, max compression
```

## Comparing `pdstools-3.1.0.tar` & `pdstools-3.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 15:05:04.000000 pdstools-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 15:05:14.071000 pdstools-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-10 15:05:04.000000 pdstools-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 15:05:14.000000 pdstools-3.1.0/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-10 15:05:04.000000 pdstools-3.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    57635 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40057 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.067000 pdstools-3.1.0/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    39142 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:14.071000 pdstools-3.1.0/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24211 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:05:04.000000 pdstools-3.1.0/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:05:14.071000 pdstools-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.140690 pdstools-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 15:49:26.000000 pdstools-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-12 15:49:37.140690 pdstools-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-12 15:49:26.000000 pdstools-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.132690 pdstools-3.1.1/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-12 15:49:37.000000 pdstools-3.1.1/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-12 15:49:37.000000 pdstools-3.1.1/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:49:37.000000 pdstools-3.1.1/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 15:49:37.000000 pdstools-3.1.1/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 15:49:37.000000 pdstools-3.1.1/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 15:49:37.000000 pdstools-3.1.1/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-12 15:49:26.000000 pdstools-3.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.128690 pdstools-3.1.1/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.132690 pdstools-3.1.1/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.132690 pdstools-3.1.1/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    57726 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40057 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.136690 pdstools-3.1.1/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.136690 pdstools-3.1.1/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.136690 pdstools-3.1.1/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.136690 pdstools-3.1.1/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.136690 pdstools-3.1.1/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.136690 pdstools-3.1.1/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    39142 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.140690 pdstools-3.1.1/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:37.140690 pdstools-3.1.1/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24211 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:49:26.000000 pdstools-3.1.1/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:49:37.140690 pdstools-3.1.1/setup.cfg
```

### Comparing `pdstools-3.1.0/LICENSE` & `pdstools-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/PKG-INFO` & `pdstools-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.0
+Version: 3.1.1
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
@@ -35,14 +35,16 @@
   <a href="https://github.com/pegasystems/pega-datascientist-tools/actions">
     <img src="https://github.com/pegasystems/pega-datascientist-tools/workflows/R%20tests/badge.svg" alt="R tests">
   </a>
   <!-- Code coverage -->
   <a href="https://codecov.io/gh/pegasystems/pega-datascientist-tools">
     <img src="https://codecov.io/gh/pegasystems/pega-datascientist-tools/branch/master/graph/badge.svg"/>
   </a>
+  <!-- PyPi package-->
+  <a href="https://badge.fury.io/py/pdstools"><img src="https://badge.fury.io/py/pdstools.svg" alt="PyPI version"></a>
   <!-- Wiki -->
   <a href="https://github.com/pegasystems/pega-datascientist-tools/wiki">
     <img src="https://img.shields.io/badge/wiki-up-success" alt="wiki">
   </a>
   <!-- Documentation -->
   <a href="https://pegasystems.github.io/pega-datascientist-tools/">
     <img src="https://img.shields.io/badge/Documentation-Up-brightgreen" alt="docs">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.0 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.1 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
@@ -10,16 +10,16 @@
 :: OSI Approved :: Apache Software License Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: docs Provides-Extra: app License-File: LICENSE
 ****** Pega Data Scientist Tools ******
                                   [Pega logo]
        [Python_tests] [R_tests]  [https://codecov.io/gh/pegasystems/pega-
-  datascientist-tools/branch/master/graph/badge.svg]  [wiki]  [docs]  [Apache
-                                 License_2.0]
+ datascientist-tools/branch/master/graph/badge.svg]  [PyPI_version]  [wiki]
+                         [docs]  [Apache_License_2.0]
 Open source tooling that helps data scientists working with Pega AI to analyze
 Pega decisioning and modeling performance. We release this under the Apache 2.0
 license and welcome contributing back, preferably through pull requests, but
 just submitting an Issue or sending a note to the authors is fine too. Pega
 does not make any representation or warranty with respect to this free
 software. The tools help to do analysis on Pega decisioning and predictive
 analytics as used in solutions such as Customer Decision Hub or Process AI,
```

### Comparing `pdstools-3.1.0/README.md` & `pdstools-3.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
   <a href="https://github.com/pegasystems/pega-datascientist-tools/actions">
     <img src="https://github.com/pegasystems/pega-datascientist-tools/workflows/R%20tests/badge.svg" alt="R tests">
   </a>
   <!-- Code coverage -->
   <a href="https://codecov.io/gh/pegasystems/pega-datascientist-tools">
     <img src="https://codecov.io/gh/pegasystems/pega-datascientist-tools/branch/master/graph/badge.svg"/>
   </a>
+  <!-- PyPi package-->
+  <a href="https://badge.fury.io/py/pdstools"><img src="https://badge.fury.io/py/pdstools.svg" alt="PyPI version"></a>
   <!-- Wiki -->
   <a href="https://github.com/pegasystems/pega-datascientist-tools/wiki">
     <img src="https://img.shields.io/badge/wiki-up-success" alt="wiki">
   </a>
   <!-- Documentation -->
   <a href="https://pegasystems.github.io/pega-datascientist-tools/">
     <img src="https://img.shields.io/badge/Documentation-Up-brightgreen" alt="docs">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ****** Pega Data Scientist Tools ******
                                   [Pega logo]
        [Python_tests] [R_tests]  [https://codecov.io/gh/pegasystems/pega-
-  datascientist-tools/branch/master/graph/badge.svg]  [wiki]  [docs]  [Apache
-                                 License_2.0]
+ datascientist-tools/branch/master/graph/badge.svg]  [PyPI_version]  [wiki]
+                         [docs]  [Apache_License_2.0]
 Open source tooling that helps data scientists working with Pega AI to analyze
 Pega decisioning and modeling performance. We release this under the Apache 2.0
 license and welcome contributing back, preferably through pull requests, but
 just submitting an Issue or sending a note to the authors is fine too. Pega
 does not make any representation or warranty with respect to this free
 software. The tools help to do analysis on Pega decisioning and predictive
 analytics as used in solutions such as Customer Decision Hub or Process AI,
```

### Comparing `pdstools-3.1.0/pdstools.egg-info/PKG-INFO` & `pdstools-3.1.1/pdstools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.0
+Version: 3.1.1
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
@@ -35,14 +35,16 @@
   <a href="https://github.com/pegasystems/pega-datascientist-tools/actions">
     <img src="https://github.com/pegasystems/pega-datascientist-tools/workflows/R%20tests/badge.svg" alt="R tests">
   </a>
   <!-- Code coverage -->
   <a href="https://codecov.io/gh/pegasystems/pega-datascientist-tools">
     <img src="https://codecov.io/gh/pegasystems/pega-datascientist-tools/branch/master/graph/badge.svg"/>
   </a>
+  <!-- PyPi package-->
+  <a href="https://badge.fury.io/py/pdstools"><img src="https://badge.fury.io/py/pdstools.svg" alt="PyPI version"></a>
   <!-- Wiki -->
   <a href="https://github.com/pegasystems/pega-datascientist-tools/wiki">
     <img src="https://img.shields.io/badge/wiki-up-success" alt="wiki">
   </a>
   <!-- Documentation -->
   <a href="https://pegasystems.github.io/pega-datascientist-tools/">
     <img src="https://img.shields.io/badge/Documentation-Up-brightgreen" alt="docs">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.0 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.1 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
@@ -10,16 +10,16 @@
 :: OSI Approved :: Apache Software License Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: docs Provides-Extra: app License-File: LICENSE
 ****** Pega Data Scientist Tools ******
                                   [Pega logo]
        [Python_tests] [R_tests]  [https://codecov.io/gh/pegasystems/pega-
-  datascientist-tools/branch/master/graph/badge.svg]  [wiki]  [docs]  [Apache
-                                 License_2.0]
+ datascientist-tools/branch/master/graph/badge.svg]  [PyPI_version]  [wiki]
+                         [docs]  [Apache_License_2.0]
 Open source tooling that helps data scientists working with Pega AI to analyze
 Pega decisioning and modeling performance. We release this under the Apache 2.0
 license and welcome contributing back, preferably through pull requests, but
 just submitting an Issue or sending a note to the authors is fine too. Pega
 does not make any representation or warranty with respect to this free
 software. The tools help to do analysis on Pega decisioning and predictive
 analytics as used in solutions such as Customer Decision Hub or Process AI,
```

### Comparing `pdstools-3.1.0/pdstools.egg-info/SOURCES.txt` & `pdstools-3.1.1/pdstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/pyproject.toml` & `pdstools-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/__init__.py` & `pdstools-3.1.1/python/pdstools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python pdstools"""
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 
 from polars import enable_string_cache
 
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
```

### Comparing `pdstools-3.1.0/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.1.1/python/pdstools/adm/ADMDatamart.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,16 @@
             Raises an error if timestamp conversion to given/default date format(timestamp_fmt) fails
             See 'https://strftime.org/' for timestamp formats
         Returns
         -------
         Union[pl.DataFrame, pl.LazyFrame]
             The input dataframe, but the proper typing applied
         """
+        from polars.datatypes import Datetime, Date
+
         retype = {
             pl.Categorical: ["Issue", "Group", "Channel", "Direction", "Configuration"],
             # pl.Int64: ["Positives", "Negatives", "ResponseCount"],
             pl.Float64: ["Performance"],
         }
         to_retype = []
         for type, cols in retype.items():
@@ -508,15 +510,16 @@
                 if col in set(df.columns):
                     to_retype.append(pl.col(col).cast(type))
         df = df.with_columns(to_retype)
 
         timestampCol = "SnapshotTime"
         if timestampCol not in df.columns:
             df = df.with_columns(SnapshotTime=None)
-        elif df.schema[timestampCol] not in pl.DATETIME_DTYPES:
+        elif df.schema[timestampCol].base_type() not in {Datetime, Date}:
+            print(df.schema[timestampCol])
             df = df.with_columns(
                 cdh_utils.parsePegaDateTimeFormats(
                     timestampCol, timestamp_fmt, strict_conversion
                 )
             )
 
         return df
@@ -794,18 +797,18 @@
                 .unnest("tempName")
                 .lazy()
                 .collect()
             )
         )
 
     def discover_modelTypes(
-        self, df: pl.LazyFrame, by:str="Configuration"
+        self, df: pl.LazyFrame, by: str = "Configuration"
     ) -> Dict:  # pragma: no cover
         """Discovers the type of model embedded in the pyModelData column.
-        
+
         By default, we do a groupby Configuration, because a model rule can only
         contain one type of model. Then, for each configuration, we look into the
         pyModelData blob and find the _serialClass, returning it in a dict.
 
         Parameters
         ----------
         df: pl.LazyFrame
@@ -1332,15 +1335,15 @@
         predictor files to disk, which Quarto then picks up to generate.
 
         By running this method directly, you have control over the exact
         filters you want to use. Simply use the top-level :attr:`.query`
         argument to filter the ADMDatamart class to the desired level.
 
         This method also propagates the predictorCategorization used by the ADMDatamart
-        class into the Health Check. Simply set the `predictorCategorization` to a 
+        class into the Health Check. Simply set the `predictorCategorization` to a
         supported function and this will be reflected in the Health Check:
         see :meth:`pdstools.utils.cdh_utils.defaultPredictorCategorization`.
 
         Parameters
         ----------
         name : Optional[str]
             The name of the Health Check file
@@ -1361,15 +1364,15 @@
             An override for the `lazy` memory_strategy. If set to True, still allows
             for collecting of data. Naturally, we need to collect the data in order
             to cache it to disk for the health check, so if set to False
             with a `lazy` memory_strategy, you won't be able to generate.
         Keyword arguments
         -----------------
         modelData_only: bool, default = False
-            If set to True, calls model-based Health Check files. Can be used if 
+            If set to True, calls model-based Health Check files. Can be used if
             predictor binning data is missing
 
         Returns
         -------
         str:
             The full path to the generated Health Check file.
         """
@@ -1464,15 +1467,15 @@
         if delete_temp_files:
             delete_temp_files(working_dir, files)
 
         return filename
 
     def exportTables(self, file: Path = "Tables.xlsx"):
         """Exports all tables from `pdstools.adm.Tables` into one Excel file.
-        
+
         Parameters
         ----------
         file: Path, default = 'Tables.xlsx'
             The file name of the exported Excel file
 
         """
         from xlsxwriter import Workbook
```

### Comparing `pdstools-3.1.0/python/pdstools/adm/ADMTrees.py` & `pdstools-3.1.1/python/pdstools/adm/ADMTrees.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/adm/Tables.py` & `pdstools-3.1.1/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/app/cli.py` & `pdstools-3.1.1/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/app/pages/Health Check.py` & `pdstools-3.1.1/python/pdstools/app/pages/Health Check.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.1.1/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/ih/legacy_IH.py` & `pdstools-3.1.1/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/pega_io/API.py` & `pdstools-3.1.1/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/pega_io/File.py` & `pdstools-3.1.1/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/pega_io/S3.py` & `pdstools-3.1.1/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/plots/plot_base.py` & `pdstools-3.1.1/python/pdstools/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/plots/plots_plotly.py` & `pdstools-3.1.1/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.1.1/python/pdstools/reports/HealthCheck.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/reports/HealthCheckModel.qmd` & `pdstools-3.1.1/python/pdstools/reports/HealthCheckModel.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/utils/cdh_utils.py` & `pdstools-3.1.1/python/pdstools/utils/cdh_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/utils/datasets.py` & `pdstools-3.1.1/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/utils/hds_utils.py` & `pdstools-3.1.1/python/pdstools/utils/hds_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/utils/pega_template.py` & `pdstools-3.1.1/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/utils/polars_ext.py` & `pdstools-3.1.1/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/utils/show_versions.py` & `pdstools-3.1.1/python/pdstools/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.1.1/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.0/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.1.1/python/pdstools/valuefinder/ValueFinder.py`

 * *Files identical despite different names*

