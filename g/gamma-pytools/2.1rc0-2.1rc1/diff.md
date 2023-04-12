# Comparing `tmp/gamma-pytools-2.1rc0.tar.gz` & `tmp/gamma-pytools-2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamma-pytools-2.1rc0.tar", last modified: Fri Sep 23 16:23:22 2022, max compression
+gzip compressed data, was "gamma-pytools-2.1rc1.tar", last modified: Wed Oct 26 17:51:52 2022, max compression
```

## Comparing `gamma-pytools-2.1rc0.tar` & `gamma-pytools-2.1rc1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0      666 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      689 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     4728 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/.gitignore
--rw-r--r--   0        0        0     1065 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/LICENSE
--rw-r--r--   0        0        0     4077 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/README.rst
--rw-r--r--   0        0        0    13509 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/RELEASE_NOTES.rst
--rw-r--r--   0        0        0    25508 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/azure-pipelines.yml
--rw-r--r--   0        0        0     1600 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/condabuild/meta.yaml
--rw-r--r--   0        0        0        0 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/config/spelling.dic
--rwxr-xr-x   0        0        0       95 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/dev-setup.sh
--rw-r--r--   0        0        0      770 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/environment.yml
--rwxr-xr-x   0        0        0    20668 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/make.py
--rw-r--r--   0        0        0      757 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/mypy.ini
--rw-r--r--   0        0        0     1749 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/pypi_description.rst
--rw-r--r--   0        0        0     2852 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/pyproject.toml
--rw-r--r--   0        0        0       60 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/sphinx/.gitignore
--rw-r--r--   0        0        0     1430 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/sphinx/base/_static/css/gamma.css
--rw-r--r--   0        0        0    28396 2022-09-23 16:22:08.092762 gamma-pytools-2.1rc0/sphinx/base/_static/gamma_logo.png
--rw-r--r--   0        0        0     1867 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/_static/js/gamma.js
--rw-r--r--   0        0        0      851 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1464 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/_templates/custom-module-template.rst
--rw-r--r--   0        0        0       64 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/_templates/getting-started-header.rst
--rw-r--r--   0        0        0     2783 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/bootstrap.py
--rw-r--r--   0        0        0     8061 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/conf_base.py
--rwxr-xr-x   0        0        0    17412 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/make_base.py
--rw-r--r--   0        0        0     1212 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/base/make_util.py
--rwxr-xr-x   0        0        0      285 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/make.py
--rw-r--r--   0        0        0    16224 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/source/_images/gamma_pytools_logo.png
--rw-r--r--   0        0        0       89 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/source/api_landing.rst
--rw-r--r--   0        0        0      449 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/source/conf.py
--rw-r--r--   0        0        0    16543 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/source/contribution_guide.rst
--rw-r--r--   0        0        0     1157 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/source/faqs.rst
--rw-r--r--   0        0        0      270 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/sphinx/source/index.rst
--rw-r--r--   0        0        0      118 2022-09-23 16:22:09.512740 gamma-pytools-2.1rc0/src/pytools/__init__.py
--rw-r--r--   0        0        0      209 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/api/__init__.py
--rw-r--r--   0        0        0    11874 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/api/_alltracker.py
--rw-r--r--   0        0        0    16056 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/api/_api.py
--rw-r--r--   0        0        0     4498 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/api/_decorators.py
--rw-r--r--   0        0        0     8591 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/api/_doc_validator.py
--rw-r--r--   0        0        0      104 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/api/doc/__init__.py
--rw-r--r--   0        0        0    10806 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/api/doc/_doc.py
--rw-r--r--   0        0        0      142 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/data/__init__.py
--rw-r--r--   0        0        0     9732 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/data/_linkage.py
--rw-r--r--   0        0        0    14286 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/data/_matrix.py
--rw-r--r--   0        0        0     8423 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/data/_simulation.py
--rw-r--r--   0        0        0       71 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/data/linkage/__init__.py
--rw-r--r--   0        0        0     4040 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/data/linkage/_linkage.py
--rw-r--r--   0        0        0     2941 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/__init__.py
--rw-r--r--   0        0        0    19468 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/_expression.py
--rw-r--r--   0        0        0      136 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/atomic/__init__.py
--rw-r--r--   0        0        0     3794 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/atomic/_atomic.py
--rw-r--r--   0        0        0      113 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/base/__init__.py
--rw-r--r--   0        0        0    11032 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/base/_base.py
--rw-r--r--   0        0        0      521 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/composite/__init__.py
--rw-r--r--   0        0        0     9060 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/composite/_composite.py
--rw-r--r--   0        0        0      143 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/composite/base/__init__.py
--rw-r--r--   0        0        0     3761 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/composite/base/_base.py
--rw-r--r--   0        0        0      125 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/formatter/__init__.py
--rw-r--r--   0        0        0    22319 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/formatter/_python.py
--rw-r--r--   0        0        0       64 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/operator/__init__.py
--rw-r--r--   0        0        0     7817 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/expression/operator/_operator.py
--rw-r--r--   0        0        0      107 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/fit/__init__.py
--rw-r--r--   0        0        0     4059 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/fit/_fit.py
--rw-r--r--   0        0        0       51 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/meta/__init__.py
--rw-r--r--   0        0        0     2162 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/meta/_meta.py
--rw-r--r--   0        0        0      101 2022-09-23 16:22:08.096762 gamma-pytools-2.1rc0/src/pytools/parallelization/__init__.py
--rw-r--r--   0        0        0    12349 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/parallelization/_parallelization.py
--rw-r--r--   0        0        0        0 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/py.typed
--rw-r--r--   0        0        0      111 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/sphinx/__init__.py
--rw-r--r--   0        0        0    12755 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/sphinx/_sphinx.py
--rw-r--r--   0        0        0      109 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/sphinx/util/__init__.py
--rw-r--r--   0        0        0    42554 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/sphinx/util/_util.py
--rw-r--r--   0        0        0      101 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/text/__init__.py
--rw-r--r--   0        0        0      823 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/text/_strings.py
--rw-r--r--   0        0        0     7466 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/text/_text.py
--rw-r--r--   0        0        0      198 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/__init__.py
--rw-r--r--   0        0        0    11047 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/_matplot.py
--rw-r--r--   0        0        0     2095 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/_text.py
--rw-r--r--   0        0        0    11284 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/_viz.py
--rw-r--r--   0        0        0       69 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/color/__init__.py
--rw-r--r--   0        0        0    12466 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/color/_color.py
--rw-r--r--   0        0        0     6424 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/color/_rgb.py
--rw-r--r--   0        0        0      119 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/__init__.py
--rw-r--r--   0        0        0     4948 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/_draw.py
--rw-r--r--   0        0        0    16230 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/_style.py
--rw-r--r--   0        0        0       76 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/base/__init__.py
--rw-r--r--   0        0        0     5042 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/base/_style.py
--rw-r--r--   0        0        0       97 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/distribution/__init__.py
--rw-r--r--   0        0        0     8266 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/distribution/_distribution.py
--rw-r--r--   0        0        0       68 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/distribution/base/__init__.py
--rw-r--r--   0        0        0     2392 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/distribution/base/_base.py
--rw-r--r--   0        0        0       86 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/matrix/__init__.py
--rw-r--r--   0        0        0    17783 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/matrix/_matrix.py
--rw-r--r--   0        0        0       62 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/matrix/base/__init__.py
--rw-r--r--   0        0        0     2255 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/matrix/base/_base.py
--rw-r--r--   0        0        0       79 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/util/__init__.py
--rw-r--r--   0        0        0     4912 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/src/pytools/viz/util/_matplot.py
--rw-r--r--   0        0        0       28 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/__init__.py
--rw-r--r--   0        0        0      696 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/conftest.py
--rw-r--r--   0        0        0      109 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/paths.py
--rw-r--r--   0        0        0       28 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/__init__.py
--rw-r--r--   0        0        0     7710 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/test_api.py
--rw-r--r--   0        0        0     6420 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/test_data.py
--rw-r--r--   0        0        0     7100 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/test_expression.py
--rw-r--r--   0        0        0     2590 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/test_jobs.py
--rw-r--r--   0        0        0     3052 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/test_sphinx.py
--rw-r--r--   0        0        0      861 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/test_text.py
--rw-r--r--   0        0        0        0 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/viz/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/viz/dendrogram/__init__.py
--rw-r--r--   0        0        0     3890 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/viz/dendrogram/test_dendrogram.py
--rw-r--r--   0        0        0     4837 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/viz/test_color.py
--rw-r--r--   0        0        0      504 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/pytools/viz/test_import.py
--rw-r--r--   0        0        0      175 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/test/test/test_docs.py
--rw-r--r--   0        0        0     2251 2022-09-23 16:22:08.100762 gamma-pytools-2.1rc0/tox.ini
--rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 gamma-pytools-2.1rc0/PKG-INFO
+-rw-r--r--   0        0        0      666 2022-10-26 17:50:42.603389 gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      689 2022-10-26 17:50:42.603389 gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     4728 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/.gitignore
+-rw-r--r--   0        0        0     1065 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/LICENSE
+-rw-r--r--   0        0        0     4077 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/README.rst
+-rw-r--r--   0        0        0    13743 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/RELEASE_NOTES.rst
+-rw-r--r--   0        0        0    25508 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/azure-pipelines.yml
+-rw-r--r--   0        0        0     1600 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/condabuild/meta.yaml
+-rw-r--r--   0        0        0        0 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/config/spelling.dic
+-rwxr-xr-x   0        0        0       95 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/dev-setup.sh
+-rw-r--r--   0        0        0      799 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/environment.yml
+-rwxr-xr-x   0        0        0    20668 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/make.py
+-rw-r--r--   0        0        0      757 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/mypy.ini
+-rw-r--r--   0        0        0     1749 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/pypi_description.rst
+-rw-r--r--   0        0        0     3001 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/pyproject.toml
+-rw-r--r--   0        0        0       60 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/.gitignore
+-rw-r--r--   0        0        0     1430 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_static/css/gamma.css
+-rw-r--r--   0        0        0    28396 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_static/gamma_logo.png
+-rw-r--r--   0        0        0     1867 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_static/js/gamma.js
+-rw-r--r--   0        0        0      851 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1464 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0       64 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/_templates/getting-started-header.rst
+-rw-r--r--   0        0        0     2783 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/bootstrap.py
+-rw-r--r--   0        0        0     8061 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/conf_base.py
+-rwxr-xr-x   0        0        0    17644 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/make_base.py
+-rw-r--r--   0        0        0     1212 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/base/make_util.py
+-rwxr-xr-x   0        0        0      285 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/make.py
+-rw-r--r--   0        0        0    16224 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/_images/gamma_pytools_logo.png
+-rw-r--r--   0        0        0       89 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/api_landing.rst
+-rw-r--r--   0        0        0      449 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/conf.py
+-rw-r--r--   0        0        0    16543 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/contribution_guide.rst
+-rw-r--r--   0        0        0     1157 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/faqs.rst
+-rw-r--r--   0        0        0      270 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/sphinx/source/index.rst
+-rw-r--r--   0        0        0      118 2022-10-26 17:50:43.675397 gamma-pytools-2.1rc1/src/pytools/__init__.py
+-rw-r--r--   0        0        0      209 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/__init__.py
+-rw-r--r--   0        0        0    12196 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_alltracker.py
+-rw-r--r--   0        0        0    16056 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_api.py
+-rw-r--r--   0        0        0     4872 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_decorators.py
+-rw-r--r--   0        0        0     8591 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/_doc_validator.py
+-rw-r--r--   0        0        0      104 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/doc/__init__.py
+-rw-r--r--   0        0        0    10806 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/api/doc/_doc.py
+-rw-r--r--   0        0        0      142 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/__init__.py
+-rw-r--r--   0        0        0     9732 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/_linkage.py
+-rw-r--r--   0        0        0    14286 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/_matrix.py
+-rw-r--r--   0        0        0     8423 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/_simulation.py
+-rw-r--r--   0        0        0       71 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/linkage/__init__.py
+-rw-r--r--   0        0        0     4040 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/data/linkage/_linkage.py
+-rw-r--r--   0        0        0     2941 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/__init__.py
+-rw-r--r--   0        0        0    19468 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/_expression.py
+-rw-r--r--   0        0        0      136 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/atomic/__init__.py
+-rw-r--r--   0        0        0     3794 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/atomic/_atomic.py
+-rw-r--r--   0        0        0      113 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/base/__init__.py
+-rw-r--r--   0        0        0    11032 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/base/_base.py
+-rw-r--r--   0        0        0      521 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/composite/__init__.py
+-rw-r--r--   0        0        0     9060 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/composite/_composite.py
+-rw-r--r--   0        0        0      143 2022-10-26 17:50:42.607389 gamma-pytools-2.1rc1/src/pytools/expression/composite/base/__init__.py
+-rw-r--r--   0        0        0     3761 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/composite/base/_base.py
+-rw-r--r--   0        0        0      125 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/formatter/__init__.py
+-rw-r--r--   0        0        0    22319 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/formatter/_python.py
+-rw-r--r--   0        0        0       64 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/operator/__init__.py
+-rw-r--r--   0        0        0     7817 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/expression/operator/_operator.py
+-rw-r--r--   0        0        0      107 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/fit/__init__.py
+-rw-r--r--   0        0        0     4059 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/fit/_fit.py
+-rw-r--r--   0        0        0       51 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/meta/__init__.py
+-rw-r--r--   0        0        0     2162 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/meta/_meta.py
+-rw-r--r--   0        0        0      101 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/parallelization/__init__.py
+-rw-r--r--   0        0        0    12349 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/parallelization/_parallelization.py
+-rw-r--r--   0        0        0        0 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/py.typed
+-rw-r--r--   0        0        0      111 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/__init__.py
+-rw-r--r--   0        0        0    12755 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/_sphinx.py
+-rw-r--r--   0        0        0      109 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/util/__init__.py
+-rw-r--r--   0        0        0    42554 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/sphinx/util/_util.py
+-rw-r--r--   0        0        0      101 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/text/__init__.py
+-rw-r--r--   0        0        0      823 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/text/_strings.py
+-rw-r--r--   0        0        0     7466 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/text/_text.py
+-rw-r--r--   0        0        0      198 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/__init__.py
+-rw-r--r--   0        0        0    11047 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/_matplot.py
+-rw-r--r--   0        0        0     2095 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/_text.py
+-rw-r--r--   0        0        0    11284 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/_viz.py
+-rw-r--r--   0        0        0       69 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/color/__init__.py
+-rw-r--r--   0        0        0    12466 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/color/_color.py
+-rw-r--r--   0        0        0     6475 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/color/_rgb.py
+-rw-r--r--   0        0        0      119 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/__init__.py
+-rw-r--r--   0        0        0     4948 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_draw.py
+-rw-r--r--   0        0        0    16230 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_style.py
+-rw-r--r--   0        0        0       76 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/base/__init__.py
+-rw-r--r--   0        0        0     5042 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/base/_style.py
+-rw-r--r--   0        0        0       97 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/__init__.py
+-rw-r--r--   0        0        0     8204 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/_distribution.py
+-rw-r--r--   0        0        0       68 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/base/__init__.py
+-rw-r--r--   0        0        0     2392 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/distribution/base/_base.py
+-rw-r--r--   0        0        0       86 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/__init__.py
+-rw-r--r--   0        0        0    17783 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/_matrix.py
+-rw-r--r--   0        0        0       62 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/base/__init__.py
+-rw-r--r--   0        0        0     2255 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/matrix/base/_base.py
+-rw-r--r--   0        0        0       79 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/util/__init__.py
+-rw-r--r--   0        0        0     4912 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/src/pytools/viz/util/_matplot.py
+-rw-r--r--   0        0        0       28 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/__init__.py
+-rw-r--r--   0        0        0      696 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/conftest.py
+-rw-r--r--   0        0        0      109 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/paths.py
+-rw-r--r--   0        0        0       28 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/__init__.py
+-rw-r--r--   0        0        0     7710 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_api.py
+-rw-r--r--   0        0        0     6420 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_data.py
+-rw-r--r--   0        0        0     7100 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_expression.py
+-rw-r--r--   0        0        0     2590 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_jobs.py
+-rw-r--r--   0        0        0     3052 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_sphinx.py
+-rw-r--r--   0        0        0      861 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/test_text.py
+-rw-r--r--   0        0        0        0 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/dendrogram/__init__.py
+-rw-r--r--   0        0        0     3890 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/dendrogram/test_dendrogram.py
+-rw-r--r--   0        0        0     4837 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/test_color.py
+-rw-r--r--   0        0        0      504 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/pytools/viz/test_import.py
+-rw-r--r--   0        0        0      175 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/test/test/test_docs.py
+-rw-r--r--   0        0        0     2251 2022-10-26 17:50:42.611389 gamma-pytools-2.1rc1/tox.ini
+-rw-r--r--   0        0        0     3909 1970-01-01 00:00:00.000000 gamma-pytools-2.1rc1/PKG-INFO
```

### Comparing `gamma-pytools-2.1rc0/.github/ISSUE_TEMPLATE/bug_report.md` & `gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/.github/ISSUE_TEMPLATE/feature_request.md` & `gamma-pytools-2.1rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/.gitignore` & `gamma-pytools-2.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/.pre-commit-config.yaml` & `gamma-pytools-2.1rc1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       - id: check-json
       - id: check-xml
       - id: check-yaml
         language: python_venv
         exclude: condabuild/meta.yaml
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.971
+    rev: v0.981
     hooks:
       - id: mypy
         files: src|sphinx|test
         language: python_venv
         language_version: python39
         additional_dependencies:
           - numpy~=1.22
```

### Comparing `gamma-pytools-2.1rc0/LICENSE` & `gamma-pytools-2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/README.rst` & `gamma-pytools-2.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/RELEASE_NOTES.rst` & `gamma-pytools-2.1rc1/RELEASE_NOTES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,22 @@
 
 *pytools* 2.0
 -------------
 
 *pytools* 2.0 features enhanced visualisations together with additional API improvements,
 and is now subject to static type checking with |mypy|.
 
+2.0.5
+~~~~~
+
+- API: de-dent docstrings before processing them with the :obj:``.subsdoc`` decorator
+- FIX: in method :meth:`.AllTracker.resolve_forward_references`, unwrap functions before
+  accessing their ``__globals__`` attribute
+
+
 2.0.4
 ~~~~~
 
 - FIX: make :meth:`.MatplotStyle.get_renderer()` compatible with
   :mod:`matplotlib` |nbsp| 3.6
```

### Comparing `gamma-pytools-2.1rc0/azure-pipelines.yml` & `gamma-pytools-2.1rc1/azure-pipelines.yml`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         displayName: 'mypy'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install mypy~=0.971 numpy~=1.22
+              python -m pip install mypy~=0.981 numpy~=1.22
               python -m mypy src
             displayName: 'Run mypy'
 
   # detect whether the build config (pyproject.toml) was changed -> then we must run a build test
   - stage: detect_build_config_changes
     displayName: 'Pyproject.toml build config'
```

### Comparing `gamma-pytools-2.1rc0/condabuild/meta.yaml` & `gamma-pytools-2.1rc1/condabuild/meta.yaml`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/environment.yml` & `gamma-pytools-2.1rc1/environment.yml`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   # run
   - joblib ~= 1.1
   - matplotlib ~= 3.5
   - numpy ~= 1.22
   - pandas ~= 1.4
   - python ~= 3.9
   - scipy ~= 1.8
+  - typing_extensions ~= 4.3
   - typing_inspect ~= 0.7
   # build/test
   - conda-build ~= 3.21
   - conda-verify ~= 3.1
   - docutils ~= 0.17
   - flit ~= 3.0
   - jinja2 ~= 2.11
```

### Comparing `gamma-pytools-2.1rc0/make.py` & `gamma-pytools-2.1rc1/make.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/mypy.ini` & `gamma-pytools-2.1rc1/mypy.ini`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/pypi_description.rst` & `gamma-pytools-2.1rc1/pypi_description.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/pyproject.toml` & `gamma-pytools-2.1rc1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 author = "Boston Consulting Group (BCG)"
 home-page = "https://github.com/BCG-Gamma/pytools"
 description-file = "pypi_description.rst"
 dist-name = "gamma-pytools"
 license = "Apache Software License v2.0"
 
 requires = [
-    "joblib         >=0.14,<2a",
-    "matplotlib     ~=3.0",
-    "numpy          >=1.21,<2a",
-    "pandas         >=0.24,<2a",
-    "scipy          ~=1.2",
-    "typing_inspect ~=0.4",
+    "joblib            >=0.14,<2a",
+    "matplotlib        ~=3.0",
+    "numpy             >=1.21,<2a",
+    "pandas            >=0.24,<2a",
+    "scipy             ~=1.2",
+    "typing_inspect    ~=0.4",
+    "typing_extensions ~=4.0",
 ]
 
 requires-python = ">=3.7,<4a"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
@@ -66,31 +67,33 @@
 
 [build]
 # comma-separated list of packages to be built from source in pip min builds
 no-binary.min = ["matplotlib"]
 
 [build.matrix.min]
 # minimum requirements of gamma-pytools
-joblib         = "~=0.14.0"
-matplotlib     = "~=3.0.3"
-numpy          = "==1.21.6"  # cannot use ~= due to conda bug
-pandas         = "~=0.24.2"
-python         = "==3.7.12"  # cannot use ~= due to conda bug
-scipy          = "~=1.2.1"
-typing_inspect = "~=0.4.0"
+joblib            = "~=0.14.0"
+matplotlib        = "~=3.0.3"
+numpy             = "==1.21.6"  # cannot use ~= due to conda bug
+pandas            = "~=0.24.2"
+python            = "==3.7.12"  # cannot use ~= due to conda bug
+scipy             = "~=1.2.1"
+typing_inspect    = "~=0.4.0"
+typing_extensions = "~=4.0.0"
 
 [build.matrix.max]
 # maximum requirements of gamma-pytools
-joblib         = "~=1.1"
-matplotlib     = "~=3.5"
-numpy          = ">=1.23,<2a"  # cannot use ~= due to conda bug
-pandas         = "~=1.4"
-python         = ">=3.9,<4a"   # cannot use ~= due to conda bug
-scipy          = "~=1.8"
-typing_inspect = "~=0.7"
+joblib            = "~=1.1"
+matplotlib        = "~=3.5"
+numpy             = ">=1.23,<2a"  # cannot use ~= due to conda bug
+pandas            = "~=1.4"
+python            = ">=3.9,<4a"   # cannot use ~= due to conda bug
+scipy             = "~=1.8"
+typing_inspect    = "~=0.7"
+typing_extensions = "~=4.3"
 
 [tool.black]
 # quiet = "True"
 line-length = 88
 target_version = ['py37']
 include = '\.pyi?$'
 exclude = '''
```

### Comparing `gamma-pytools-2.1rc0/sphinx/base/_static/css/gamma.css` & `gamma-pytools-2.1rc1/sphinx/base/_static/css/gamma.css`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/base/_static/gamma_logo.png` & `gamma-pytools-2.1rc1/sphinx/base/_static/gamma_logo.png`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/base/_static/js/gamma.js` & `gamma-pytools-2.1rc1/sphinx/base/_static/js/gamma.js`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/base/_templates/custom-class-template.rst` & `gamma-pytools-2.1rc1/sphinx/base/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/base/_templates/custom-module-template.rst` & `gamma-pytools-2.1rc1/sphinx/base/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/base/bootstrap.py` & `gamma-pytools-2.1rc1/sphinx/base/bootstrap.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/base/conf_base.py` & `gamma-pytools-2.1rc1/sphinx/base/conf_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/base/make_base.py` & `gamma-pytools-2.1rc1/sphinx/base/make_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,23 @@
 CMD_SPHINX_BUILD = "sphinx-build"
 CMD_SPHINX_AUTOGEN = "sphinx-autogen"
 
 # File paths
 DIR_SPHINX_BASE = os.path.dirname(os.path.realpath(__file__))
 DIR_REPO_ROOT = os.path.dirname(DIR_SPHINX_ROOT)
 DIR_REPO_PARENT = os.path.dirname(DIR_REPO_ROOT)
-PROJECT_NAME = os.path.split(os.path.realpath(DIR_REPO_ROOT))[1]
 DIR_PACKAGE_SRC = os.path.join(DIR_REPO_ROOT, "src")
+# get all subdirectories of DIR_PACKAGE_SRC
+PACKAGE_NAMES = [
+    package
+    for package in os.listdir(DIR_PACKAGE_SRC)
+    if os.path.isdir(os.path.join(DIR_PACKAGE_SRC, package))
+]
+assert len(PACKAGE_NAMES) == 1, "only one package per Sphinx build is supported"
+PROJECT_NAME = PACKAGE_NAMES[0]
 DIR_DOCS = os.path.join(DIR_REPO_ROOT, "docs")
 DIR_DOCS_VERSION = os.path.join(DIR_DOCS, "docs-version")
 DIR_SPHINX_SOURCE = os.path.join(DIR_SPHINX_ROOT, "source")
 DIR_SPHINX_AUX = os.path.join(DIR_SPHINX_ROOT, "auxiliary")
 DIR_SPHINX_API_GENERATED = os.path.join(DIR_SPHINX_SOURCE, "apidoc")
 DIR_SPHINX_GENERATED = os.path.join(DIR_SPHINX_SOURCE, "_generated")
 DIR_SPHINX_BUILD = os.path.join(DIR_SPHINX_ROOT, "build")
```

### Comparing `gamma-pytools-2.1rc0/sphinx/base/make_util.py` & `gamma-pytools-2.1rc1/sphinx/base/make_util.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/source/_images/gamma_pytools_logo.png` & `gamma-pytools-2.1rc1/sphinx/source/_images/gamma_pytools_logo.png`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/source/contribution_guide.rst` & `gamma-pytools-2.1rc1/sphinx/source/contribution_guide.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/sphinx/source/faqs.rst` & `gamma-pytools-2.1rc1/sphinx/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/api/_alltracker.py` & `gamma-pytools-2.1rc1/src/pytools/api/_alltracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,27 +299,37 @@
     except AttributeError:
         # the object cannot be a type or function; no action required
         return
 
     # keep track of classes we already visited to prevent infinite recursion
     visited: Set[type] = set()
 
-    def _update(_obj: Any, local_ns: Optional[Dict[str, Any]] = None) -> None:
+    def _update(
+        _obj: Union[type, FunctionType], local_ns: Optional[Dict[str, Any]] = None
+    ) -> None:
         if isinstance(_obj, type) and _obj.__module__ == my_module:
             if _obj not in visited:
                 visited.add(_obj)
                 local_ns = dict(_obj.__dict__)
                 for member in vars(_obj).values():
                     _update(member, local_ns=local_ns)
                 _update_annotations(_obj, local_ns)
 
         elif isinstance(_obj, FunctionType) and _obj.__module__ == my_module:
             _update_annotations(_obj, local_ns)
 
-    def _update_annotations(_obj: Any, local_ns: Optional[Dict[str, Any]]) -> None:
+    def _update_annotations(
+        _obj: Union[type, FunctionType], local_ns: Optional[Dict[str, Any]]
+    ) -> None:
+        # unwrap the object to get the underlying function, if applicable
+        while isinstance(_obj, FunctionType):
+            try:
+                _obj = _obj.__wrapped__  # type: ignore
+            except AttributeError:
+                break
         annotations = get_type_hints(
             _obj, globalns=getattr(_obj, "__globals__", globals_), localns=local_ns
         )
         if annotations:
             _obj.__annotations__ = annotations
 
     _update(obj)
```

### Comparing `gamma-pytools-2.1rc0/src/pytools/api/_api.py` & `gamma-pytools-2.1rc1/src/pytools/api/_api.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/api/_decorators.py` & `gamma-pytools-2.1rc1/src/pytools/api/_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Core implementation of decorators in :mod:`pytools.api`.
 """
 
 import logging
 import re
+import textwrap
 from typing import Any, Callable, Optional, Type, TypeVar
 
 from pytools.api._alltracker import AllTracker
 
 log = logging.getLogger(__name__)
 
 
@@ -37,30 +38,30 @@
     .. code-block:: python
 
       class A:
           def my_function(self) -> None:
           \"""Some documentation\"""
           # …
 
-      @inheritdoc(match="[see superclass]")
+      @inheritdoc(match=\"""[see superclass]\""")
       class B(A):
           def my_function(self) -> None:
           \"""[see superclass]\"""
           # …
 
           def my_other_function(self) -> None:
           \"""This docstring will not be replaced\"""
           # …
 
     In this example, the docstring of ``my_function`` will be replaced with the
     docstring of the overridden function of the same name, or with ``None`` if no
     overridden function exists, or if that function has no docstring.
 
-    :param match: the parent docstring will be inherited if the current docstring
-        is equal to match
+    :param match: the exact text a docstring has to match in order to be replaced
+        by the parent's docstring
     :return: the parameterized decorator
     """
 
     def _inheritdoc_inner(_cls: T_Type) -> T_Type:
         if not type(_cls):
             raise TypeError(
                 f"@{inheritdoc.__name__} can only decorate classes, "
@@ -95,33 +96,39 @@
 ) -> Callable[[T], T]:
     """
     Decorator for substituting parts of an object's docstring.
 
     Matches the given pattern in the docstring, and substitutes it with the given
     replacement string (analogous to :func:`re.sub`).
 
+    Prior to matching, the docstring is *de-dented*, i.e. the indentation of the
+    first line is removed from all lines. This ensures that docstrings that are
+    indented to align with the opening triple quotes are matched correctly, regardless
+    of the indentation level.
+
     :param pattern: a regular expression for the pattern to match
     :param replacement: the replacement for substrings matching the pattern
     :param using: get the docstring from the given object as the basis for the
         substitution
     :return: the parameterized decorator
     """
 
     def _decorate(_obj: T) -> T:
         origin = _obj if using is None else using
         docstring_original = _get_docstring(origin)
         if not isinstance(docstring_original, str):
             raise ValueError(
                 f"docstring of {origin!r} is not a string: {docstring_original!r}"
             )
-        docstring_substituted, n = re.subn(pattern, replacement, docstring_original)
+        docstring_dedented = textwrap.dedent(docstring_original)
+        docstring_substituted, n = re.subn(pattern, replacement, docstring_dedented)
         if not n:
             raise ValueError(
                 f"subsdoc: pattern {pattern!r} "
-                f"not found in docstring {docstring_original!r}"
+                f"not found in docstring {docstring_dedented!r}"
             )
         _set_docstring(_obj, docstring_substituted)
         return _obj
 
     if not (isinstance(pattern, str)):
         raise ValueError("arg pattern must be a string")
     if not (isinstance(replacement, str)):
```

### Comparing `gamma-pytools-2.1rc0/src/pytools/api/_doc_validator.py` & `gamma-pytools-2.1rc1/src/pytools/api/_doc_validator.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/api/doc/_doc.py` & `gamma-pytools-2.1rc1/src/pytools/api/doc/_doc.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/data/_linkage.py` & `gamma-pytools-2.1rc1/src/pytools/data/_linkage.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/data/_matrix.py` & `gamma-pytools-2.1rc1/src/pytools/data/_matrix.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/data/_simulation.py` & `gamma-pytools-2.1rc1/src/pytools/data/_simulation.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/data/linkage/_linkage.py` & `gamma-pytools-2.1rc1/src/pytools/data/linkage/_linkage.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/__init__.py` & `gamma-pytools-2.1rc1/src/pytools/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/_expression.py` & `gamma-pytools-2.1rc1/src/pytools/expression/_expression.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/atomic/_atomic.py` & `gamma-pytools-2.1rc1/src/pytools/expression/atomic/_atomic.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/base/_base.py` & `gamma-pytools-2.1rc1/src/pytools/expression/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/composite/__init__.py` & `gamma-pytools-2.1rc1/src/pytools/expression/composite/__init__.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/composite/_composite.py` & `gamma-pytools-2.1rc1/src/pytools/expression/composite/_composite.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/composite/base/_base.py` & `gamma-pytools-2.1rc1/src/pytools/expression/composite/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/formatter/_python.py` & `gamma-pytools-2.1rc1/src/pytools/expression/formatter/_python.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/expression/operator/_operator.py` & `gamma-pytools-2.1rc1/src/pytools/expression/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/fit/_fit.py` & `gamma-pytools-2.1rc1/src/pytools/fit/_fit.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/meta/_meta.py` & `gamma-pytools-2.1rc1/src/pytools/meta/_meta.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/parallelization/_parallelization.py` & `gamma-pytools-2.1rc1/src/pytools/parallelization/_parallelization.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/sphinx/_sphinx.py` & `gamma-pytools-2.1rc1/src/pytools/sphinx/_sphinx.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/sphinx/util/_util.py` & `gamma-pytools-2.1rc1/src/pytools/sphinx/util/_util.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/text/_strings.py` & `gamma-pytools-2.1rc1/src/pytools/text/_strings.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/text/_text.py` & `gamma-pytools-2.1rc1/src/pytools/text/_text.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/_matplot.py` & `gamma-pytools-2.1rc1/src/pytools/viz/_matplot.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/_text.py` & `gamma-pytools-2.1rc1/src/pytools/viz/_text.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/_viz.py` & `gamma-pytools-2.1rc1/src/pytools/viz/_viz.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/color/_color.py` & `gamma-pytools-2.1rc1/src/pytools/viz/color/_color.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/color/_rgb.py` & `gamma-pytools-2.1rc1/src/pytools/viz/color/_rgb.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, Optional, Tuple, cast, overload
 
 from matplotlib.colors import to_rgb
+from typing_extensions import TypeAlias
 
 from pytools.api import AllTracker
 
 log = logging.getLogger(__name__)
 
 
 #
@@ -29,15 +30,15 @@
     "RgbaColor",
 ]
 
 
 #
 # Type Aliases
 #
-TupleRgb = Tuple[float, float, float]
+TupleRgb: TypeAlias = Tuple[float, float, float]
 
 #
 # Ensure all symbols introduced below are included in __all__
 #
 
 __tracker = AllTracker(globals())
```

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/_draw.py` & `gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_draw.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/_style.py` & `gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/_style.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/dendrogram/base/_style.py` & `gamma-pytools-2.1rc1/src/pytools/viz/dendrogram/base/_style.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/distribution/_distribution.py` & `gamma-pytools-2.1rc1/src/pytools/viz/distribution/_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         # add axis labels and legend
         ax.set_xlabel(x_label, color=colors.foreground)
         ax.set_ylabel("count", color=colors.foreground)
         ax.legend()
 
 
 @inheritdoc(match="[see superclass]")
-class ECDFDrawer(Drawer[Union[Sequence[float], ArrayLike], ECDFStyle]):
+class ECDFDrawer(Drawer[ArrayLike, ECDFStyle]):
     """
     Drawer for empirical cumulative density functions (ECDFs), highlighting
     outliers using Tukey's outlier test.
 
     The drawer highlights samples as `outliers` or `far outliers`.
 
     A sample is considered an outlier if it is outside the range
@@ -155,17 +155,15 @@
 
         self.iqr_multiple = iqr_multiple
         self.iqr_multiple_far = iqr_multiple_far
         self.hide_far_outliers = hide_far_outliers
 
     __init__.__doc__ = cast(str, Drawer.__init__.__doc__) + cast(str, __init__.__doc__)
 
-    def draw(
-        self, data: Union[Sequence[float], ArrayLike], *, title: Optional[str] = None
-    ) -> None:
+    def draw(self, data: ArrayLike, *, title: Optional[str] = None) -> None:
         """
         Draw the ECDF.
 
         :param data: the data to draw
         :param title: the title of the chart (optional; defaults to ``"ECDF"``; if arg
             `data` is a :class:`~.Series` or any other class with a `name`
             attribute, then the default title will include the name)
```

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/distribution/base/_base.py` & `gamma-pytools-2.1rc1/src/pytools/viz/distribution/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/matrix/_matrix.py` & `gamma-pytools-2.1rc1/src/pytools/viz/matrix/_matrix.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/matrix/base/_base.py` & `gamma-pytools-2.1rc1/src/pytools/viz/matrix/base/_base.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/src/pytools/viz/util/_matplot.py` & `gamma-pytools-2.1rc1/src/pytools/viz/util/_matplot.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/conftest.py` & `gamma-pytools-2.1rc1/test/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/test_api.py` & `gamma-pytools-2.1rc1/test/test/pytools/test_api.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/test_data.py` & `gamma-pytools-2.1rc1/test/test/pytools/test_data.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/test_expression.py` & `gamma-pytools-2.1rc1/test/test/pytools/test_expression.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/test_jobs.py` & `gamma-pytools-2.1rc1/test/test/pytools/test_jobs.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/test_sphinx.py` & `gamma-pytools-2.1rc1/test/test/pytools/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/test_text.py` & `gamma-pytools-2.1rc1/test/test/pytools/test_text.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/viz/dendrogram/test_dendrogram.py` & `gamma-pytools-2.1rc1/test/test/pytools/viz/dendrogram/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/test/test/pytools/viz/test_color.py` & `gamma-pytools-2.1rc1/test/test/pytools/viz/test_color.py`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/tox.ini` & `gamma-pytools-2.1rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `gamma-pytools-2.1rc0/PKG-INFO` & `gamma-pytools-2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamma-pytools
-Version: 2.1rc0
+Version: 2.1rc1
 Summary: A collection of Python extensions and tools used in BCG GAMMA's open-source libraries.
 Home-page: https://github.com/BCG-Gamma/pytools
 License: Apache Software License v2.0
 Author: Boston Consulting Group (BCG)
 Requires-Python: >=3.7,<4a
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,20 +16,21 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: joblib         >=0.14,<2a
-Requires-Dist: matplotlib     ~=3.0
-Requires-Dist: numpy          >=1.21,<2a
-Requires-Dist: pandas         >=0.24,<2a
-Requires-Dist: scipy          ~=1.2
-Requires-Dist: typing_inspect ~=0.4
+Requires-Dist: joblib            >=0.14,<2a
+Requires-Dist: matplotlib        ~=3.0
+Requires-Dist: numpy             >=1.21,<2a
+Requires-Dist: pandas            >=0.24,<2a
+Requires-Dist: scipy             ~=1.2
+Requires-Dist: typing_inspect    ~=0.4
+Requires-Dist: typing_extensions ~=4.0
 Requires-Dist: sphinx ~= 4.5 ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ~= 1.19 ; extra == "docs"
 Requires-Dist: pydata-sphinx-theme ~= 0.8.1 ; extra == "docs"
 Requires-Dist: jinja2 ~= 2.11 ; extra == "docs"
 Requires-Dist: nbsphinx ~= 0.8.9 ; extra == "docs"
 Requires-Dist: jupyter == 1 ; extra == "docs"
 Requires-Dist: docutils ~= 0.17 ; extra == "docs"
```

