# Comparing `tmp/datajudge-1.5.0.tar.gz` & `tmp/datajudge-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajudge-1.5.0.tar", last modified: Tue Mar 14 12:45:53 2023, max compression
+gzip compressed data, was "datajudge-1.6.0.tar", last modified: Wed Apr 12 11:25:40 2023, max compression
```

## Comparing `datajudge-1.5.0.tar` & `datajudge-1.6.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      378 2023-03-14 12:44:21.876004 datajudge-1.5.0/.flake8
--rw-r--r--   0        0        0      154 2023-03-14 12:44:21.876004 datajudge-1.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1388 2023-03-14 12:44:21.876004 datajudge-1.5.0/.github/workflows/build_and_publish.yaml
--rw-r--r--   0        0        0    17607 2023-03-14 12:44:21.876004 datajudge-1.5.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2962 2023-03-14 12:44:21.876004 datajudge-1.5.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1437 2023-03-14 12:44:21.876004 datajudge-1.5.0/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0        0        0     1311 2023-03-14 12:44:21.876004 datajudge-1.5.0/.gitignore
--rw-r--r--   0        0        0      958 2023-03-14 12:44:21.876004 datajudge-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      268 2023-03-14 12:44:21.876004 datajudge-1.5.0/.readthedocs.yml
--rw-r--r--   0        0        0     2756 2023-03-14 12:44:21.876004 datajudge-1.5.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1515 2023-03-14 12:44:21.876004 datajudge-1.5.0/LICENSE
--rw-r--r--   0        0        0     1600 2023-03-14 12:44:21.876004 datajudge-1.5.0/README.md
--rw-r--r--   0        0        0       32 2023-03-14 12:44:21.876004 datajudge-1.5.0/_typos.toml
--rw-r--r--   0        0        0       84 2023-03-14 12:44:21.876004 datajudge-1.5.0/codecov.yml
--rw-r--r--   0        0        0     1241 2023-03-14 12:44:21.876004 datajudge-1.5.0/docker-compose.yaml
--rw-r--r--   0        0        0      638 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/Makefile
--rw-r--r--   0        0        0      764 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/make.bat
--rw-r--r--   0        0        0      905 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/conf.py
--rw-r--r--   0        0        0      983 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/development.rst
--rw-r--r--   0        0        0     5146 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/example.rst
--rw-r--r--   0        0        0     6419 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/example_dates.rst
--rw-r--r--   0        0        0     8642 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/example_exploration.rst
--rw-r--r--   0        0        0    12556 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/example_twitch.rst
--rw-r--r--   0        0        0      194 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/examples.rst
--rw-r--r--   0        0        0     1381 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/twitch_process.py
--rw-r--r--   0        0        0    17481 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/twitch_report.html
--rw-r--r--   0        0        0     2663 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/twitch_specification.py
--rw-r--r--   0        0        0      573 2023-03-14 12:44:21.876004 datajudge-1.5.0/docs/source/examples/twitch_upload.py
--rw-r--r--   0        0        0    70396 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/examples/twitch_version1.csv
--rw-r--r--   0        0        0    82951 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/examples/twitch_version2.csv
--rw-r--r--   0        0        0    78962 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/examples/twitchdata.csv
--rw-r--r--   0        0        0     8452 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/getting_started.rst
--rw-r--r--   0        0        0      543 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/index.rst
--rw-r--r--   0        0        0      155 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/installation.rst
--rw-r--r--   0        0        0     1527 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/motivation.rst
--rw-r--r--   0        0        0    51601 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/report_failing_query1.png
--rw-r--r--   0        0        0   163420 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/report_failing_query2.png
--rw-r--r--   0        0        0    11178 2023-03-14 12:44:21.880004 datajudge-1.5.0/docs/source/testing.rst
--rw-r--r--   0        0        0      445 2023-03-14 12:44:21.880004 datajudge-1.5.0/environment.yml
--rw-r--r--   0        0        0     1168 2023-03-14 12:44:21.880004 datajudge-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      510 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/__init__.py
--rw-r--r--   0        0        0     8560 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/base.py
--rw-r--r--   0        0        0     3437 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/column.py
--rw-r--r--   0        0        0    11708 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/date.py
--rw-r--r--   0        0        0     1788 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/groupby.py
--rw-r--r--   0        0        0     6427 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/miscs.py
--rw-r--r--   0        0        0     6075 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/nrows.py
--rw-r--r--   0        0        0     8260 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/numeric.py
--rw-r--r--   0        0        0     7220 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/row.py
--rw-r--r--   0        0        0     4532 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/stats.py
--rw-r--r--   0        0        0    11350 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/uniques.py
--rw-r--r--   0        0        0     7384 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/constraints/varchar.py
--rw-r--r--   0        0        0    42953 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/db_access.py
--rw-r--r--   0        0        0     1019 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/pytest_integration.py
--rw-r--r--   0        0        0    62220 2023-03-14 12:44:21.880004 datajudge-1.5.0/src/datajudge/requirements.py
--rwxr-xr-x   0        0        0      173 2023-03-14 12:44:21.880004 datajudge-1.5.0/start_db2.sh
--rwxr-xr-x   0        0        0      522 2023-03-14 12:44:21.884003 datajudge-1.5.0/start_mssql.sh
--rwxr-xr-x   0        0        0      140 2023-03-14 12:44:21.884003 datajudge-1.5.0/start_postgres.sh
--rw-r--r--   0        0        0        0 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/integration/__init__.py
--rw-r--r--   0        0        0    27446 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2848 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/integration/test_column_capitalization.py
--rw-r--r--   0        0        0     6805 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/integration/test_data_source.py
--rw-r--r--   0        0        0    71469 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/integration/test_integration.py
--rw-r--r--   0        0        0     2520 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/integration/test_stats.py
--rw-r--r--   0        0        0     2216 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/unit/test_condition.py
--rw-r--r--   0        0        0      726 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/unit/test_db_access.py
--rw-r--r--   0        0        0      856 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/unit/test_percentiles.py
--rw-r--r--   0        0        0     2208 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/unit/test_pytest.py
--rw-r--r--   0        0        0     1763 2023-03-14 12:44:21.884003 datajudge-1.5.0/tests/unit/test_set_functions.py
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 datajudge-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      378 2023-04-12 11:24:00.433271 datajudge-1.6.0/.flake8
+-rw-r--r--   0        0        0      154 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1388 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/build_and_publish.yaml
+-rw-r--r--   0        0        0    17607 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     2962 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1437 2023-04-12 11:24:00.433271 datajudge-1.6.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0        0        0     1311 2023-04-12 11:24:00.433271 datajudge-1.6.0/.gitignore
+-rw-r--r--   0        0        0      958 2023-04-12 11:24:00.437271 datajudge-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      268 2023-04-12 11:24:00.437271 datajudge-1.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     2866 2023-04-12 11:24:00.437271 datajudge-1.6.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1515 2023-04-12 11:24:00.437271 datajudge-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1600 2023-04-12 11:24:00.437271 datajudge-1.6.0/README.md
+-rw-r--r--   0        0        0       32 2023-04-12 11:24:00.437271 datajudge-1.6.0/_typos.toml
+-rw-r--r--   0        0        0       84 2023-04-12 11:24:00.437271 datajudge-1.6.0/codecov.yml
+-rw-r--r--   0        0        0     1241 2023-04-12 11:24:00.437271 datajudge-1.6.0/docker-compose.yaml
+-rw-r--r--   0        0        0      638 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/make.bat
+-rw-r--r--   0        0        0      905 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/conf.py
+-rw-r--r--   0        0        0      983 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/development.rst
+-rw-r--r--   0        0        0     5146 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example.rst
+-rw-r--r--   0        0        0     6419 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example_dates.rst
+-rw-r--r--   0        0        0     8642 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example_exploration.rst
+-rw-r--r--   0        0        0    12556 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/example_twitch.rst
+-rw-r--r--   0        0        0      194 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/examples.rst
+-rw-r--r--   0        0        0     1381 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_process.py
+-rw-r--r--   0        0        0    17481 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_report.html
+-rw-r--r--   0        0        0     2663 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_specification.py
+-rw-r--r--   0        0        0      573 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_upload.py
+-rw-r--r--   0        0        0    70396 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_version1.csv
+-rw-r--r--   0        0        0    82951 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitch_version2.csv
+-rw-r--r--   0        0        0    78962 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/examples/twitchdata.csv
+-rw-r--r--   0        0        0     8452 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      543 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/index.rst
+-rw-r--r--   0        0        0      155 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1527 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/motivation.rst
+-rw-r--r--   0        0        0    51601 2023-04-12 11:24:00.437271 datajudge-1.6.0/docs/source/report_failing_query1.png
+-rw-r--r--   0        0        0   163420 2023-04-12 11:24:00.441271 datajudge-1.6.0/docs/source/report_failing_query2.png
+-rw-r--r--   0        0        0    11178 2023-04-12 11:24:00.441271 datajudge-1.6.0/docs/source/testing.rst
+-rw-r--r--   0        0        0      445 2023-04-12 11:24:00.441271 datajudge-1.6.0/environment.yml
+-rw-r--r--   0        0        0     1168 2023-04-12 11:24:00.441271 datajudge-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/__init__.py
+-rw-r--r--   0        0        0     8560 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/base.py
+-rw-r--r--   0        0        0     3437 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/column.py
+-rw-r--r--   0        0        0    11708 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/date.py
+-rw-r--r--   0        0        0     1788 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/groupby.py
+-rw-r--r--   0        0        0     6427 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/miscs.py
+-rw-r--r--   0        0        0     6075 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/nrows.py
+-rw-r--r--   0        0        0     8260 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/numeric.py
+-rw-r--r--   0        0        0     7220 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/row.py
+-rw-r--r--   0        0        0     4532 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/stats.py
+-rw-r--r--   0        0        0    11350 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/uniques.py
+-rw-r--r--   0        0        0     7384 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/constraints/varchar.py
+-rw-r--r--   0        0        0    42690 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/db_access.py
+-rw-r--r--   0        0        0     1019 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/pytest_integration.py
+-rw-r--r--   0        0        0    62220 2023-04-12 11:24:00.441271 datajudge-1.6.0/src/datajudge/requirements.py
+-rwxr-xr-x   0        0        0      173 2023-04-12 11:24:00.441271 datajudge-1.6.0/start_db2.sh
+-rwxr-xr-x   0        0        0      522 2023-04-12 11:24:00.441271 datajudge-1.6.0/start_mssql.sh
+-rwxr-xr-x   0        0        0      140 2023-04-12 11:24:00.441271 datajudge-1.6.0/start_postgres.sh
+-rw-r--r--   0        0        0        0 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0    27552 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2848 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_column_capitalization.py
+-rw-r--r--   0        0        0     6795 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_data_source.py
+-rw-r--r--   0        0        0    71469 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_integration.py
+-rw-r--r--   0        0        0     2520 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     2216 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_condition.py
+-rw-r--r--   0        0        0      726 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_db_access.py
+-rw-r--r--   0        0        0      856 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_percentiles.py
+-rw-r--r--   0        0        0     2208 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_pytest.py
+-rw-r--r--   0        0        0     1763 2023-04-12 11:24:00.441271 datajudge-1.6.0/tests/unit/test_set_functions.py
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 datajudge-1.6.0/PKG-INFO
```

### Comparing `datajudge-1.5.0/.github/workflows/build_and_publish.yaml` & `datajudge-1.6.0/.github/workflows/build_and_publish.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -48,11 +48,11 @@
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.7.1
+      - uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `datajudge-1.5.0/.github/workflows/ci.yaml` & `datajudge-1.6.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/.github/workflows/codeql.yml` & `datajudge-1.6.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/.github/workflows/pre-commit-autoupdate.yml` & `datajudge-1.6.0/.github/workflows/pre-commit-autoupdate.yml`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       - name: Update pre-commit hooks and run
         id: versions
         env:
           PRE_COMMIT_USE_MAMBA: 1
         run: |
           pre-commit autoupdate
           pre-commit run -a || true
-      - uses: peter-evans/create-pull-request@2b011faafdcbc9ceb11414d64d0573f37c774b04
+      - uses: peter-evans/create-pull-request@5b4a9f6a9e2af26e5f02351490b90d01eb8ec1e5
         with:
           commit-message: "Auto-update pre-commit hooks"
           title: "Auto-update pre-commit hooks"
           body: |
             New versions of the used pre-commit hooks were detected.
             This PR updates them to the latest and already ran `pre-commit run -a` for you to fix any changes in formatting.
           branch: pre-commit-autoupdate
```

### Comparing `datajudge-1.5.0/.gitignore` & `datajudge-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/.pre-commit-config.yaml` & `datajudge-1.6.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/Quantco/pre-commit-mirrors-black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-conda
         args:
           - --safe
           - --target-version=py38
   - repo: https://github.com/Quantco/pre-commit-mirrors-flake8
     rev: 6.0.0
@@ -12,22 +12,22 @@
       - id: flake8-conda
   - repo: https://github.com/Quantco/pre-commit-mirrors-isort
     rev: 5.12.0
     hooks:
       - id: isort-conda
         additional_dependencies: [-c, conda-forge, toml=0.10.2]
   - repo: https://github.com/Quantco/pre-commit-mirrors-mypy
-    rev: "1.0.1"
+    rev: "1.1.1"
     hooks:
       - id: mypy-conda
         additional_dependencies: [-c, conda-forge, types-setuptools]
   - repo: https://github.com/Quantco/pre-commit-mirrors-pyupgrade
     rev: 3.3.1
     hooks:
       - id: pyupgrade-conda
         args:
           - --py38-plus
   - repo: https://github.com/Quantco/pre-commit-mirrors-typos
-    rev: 1.13.16
+    rev: 1.13.20
     hooks:
       - id: typos-conda
         exclude: "\\.csv$"
```

### Comparing `datajudge-1.5.0/CHANGELOG.rst` & `datajudge-1.6.0/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,22 @@
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Changelog
 =========
 
 
+1.6.0 - 2022.04.12
+------------------
+
+**Other changes**
+
+- Ensure compatibility with ``sqlalchemy`` >= 2.0.
+
+
 1.5.0 - 2022.03.14
 ------------------
 
 **New features**
 
 - Implement :meth:`datajudge.BetweenRequirement.add_max_null_fraction_constraint` and
   :meth:`datajudge.WithinRequirement.add_max_null_fraction_constraint`.
@@ -47,15 +55,15 @@
 
 **New features**
 
 - Implemented specification of number of counterexamples in :meth:`~datajudge.WithinRequirement.add_varchar_regex_constraint`.
 - Implemented in-database regex matching for some dialects via ``computation_in_db`` parameter in :meth:`~datajudge.WithinRequirement.add_varchar_regex_constraint`.
 - Added support for BigQuery backends.
 
-**Bug fix:**
+**Bug fix**
 
 - Snowflake-sqlalchemy version 1.4.0 introduced an unexpected change in behaviour. This problem is resolved by pinning it to the previous version, 1.3.4.
 
 
 1.1.1 - 2022.06.30
 ------------------
```

### Comparing `datajudge-1.5.0/LICENSE` & `datajudge-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/README.md` & `datajudge-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docker-compose.yaml` & `datajudge-1.6.0/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/Makefile` & `datajudge-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/make.bat` & `datajudge-1.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/conf.py` & `datajudge-1.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/development.rst` & `datajudge-1.6.0/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/example.rst` & `datajudge-1.6.0/docs/source/examples/example.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/example_dates.rst` & `datajudge-1.6.0/docs/source/examples/example_dates.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/example_exploration.rst` & `datajudge-1.6.0/docs/source/examples/example_exploration.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/example_twitch.rst` & `datajudge-1.6.0/docs/source/examples/example_twitch.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/twitch_process.py` & `datajudge-1.6.0/docs/source/examples/twitch_process.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/twitch_report.html` & `datajudge-1.6.0/docs/source/examples/twitch_report.html`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/twitch_specification.py` & `datajudge-1.6.0/docs/source/examples/twitch_specification.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/twitch_upload.py` & `datajudge-1.6.0/docs/source/examples/twitch_upload.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/twitch_version1.csv` & `datajudge-1.6.0/docs/source/examples/twitch_version1.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/twitch_version2.csv` & `datajudge-1.6.0/docs/source/examples/twitch_version2.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/examples/twitchdata.csv` & `datajudge-1.6.0/docs/source/examples/twitchdata.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/getting_started.rst` & `datajudge-1.6.0/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/index.rst` & `datajudge-1.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/motivation.rst` & `datajudge-1.6.0/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/report_failing_query1.png` & `datajudge-1.6.0/docs/source/report_failing_query1.png`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/report_failing_query2.png` & `datajudge-1.6.0/docs/source/report_failing_query2.png`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/docs/source/testing.rst` & `datajudge-1.6.0/docs/source/testing.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/pyproject.toml` & `datajudge-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/base.py` & `datajudge-1.6.0/src/datajudge/constraints/base.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/column.py` & `datajudge-1.6.0/src/datajudge/constraints/column.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/date.py` & `datajudge-1.6.0/src/datajudge/constraints/date.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/groupby.py` & `datajudge-1.6.0/src/datajudge/constraints/groupby.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/miscs.py` & `datajudge-1.6.0/src/datajudge/constraints/miscs.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/nrows.py` & `datajudge-1.6.0/src/datajudge/constraints/nrows.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/numeric.py` & `datajudge-1.6.0/src/datajudge/constraints/numeric.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/row.py` & `datajudge-1.6.0/src/datajudge/constraints/row.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/stats.py` & `datajudge-1.6.0/src/datajudge/constraints/stats.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/uniques.py` & `datajudge-1.6.0/src/datajudge/constraints/uniques.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/constraints/varchar.py` & `datajudge-1.6.0/src/datajudge/constraints/varchar.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/db_access.py` & `datajudge-1.6.0/src/datajudge/db_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
                 sa.text(query_string)
                 .columns(*[sa.column(column_name) for column_name in columns])
                 .subquery()
             )
             self.clause = subquery
         else:
             wrapped_query = f"({query_string}) as t"
-            self.clause = sa.select(["*"]).select_from(sa.text(wrapped_query)).alias()
+            self.clause = sa.select("*").select_from(sa.text(wrapped_query)).alias()
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(query_string={self.query_string}, name={self.name}, columns={self.columns})"
 
@@ -304,18 +304,18 @@
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(data_source={self.data_source!r}, columns={self.columns!r}, condition={self.condition!r})"
 
     def get_selection(self, engine: sa.engine.Engine):
         clause = self.data_source.get_clause(engine)
         if self.columns:
             selection = sa.select(
-                [clause.c[column_name] for column_name in self.get_columns(engine)]
+                *[clause.c[column_name] for column_name in self.get_columns(engine)]
             )
         else:
-            selection = sa.select([clause])
+            selection = sa.select(clause)
         if self.condition is not None:
             text = str(self.condition)
             if is_snowflake(engine):
                 text = self.condition.snowflake_str()
             selection = selection.where(sa.text(text))
         if is_mssql(engine) and isinstance(self.data_source, TableDataSource):
             # Allow dirty reads when using MSSQL.
@@ -382,56 +382,56 @@
 def get_date_span(engine, ref, date_column_name):
     if is_snowflake(engine):
         date_column_name = lowercase_column_names(date_column_name)
     subquery = ref.get_selection(engine).alias()
     column = subquery.c[date_column_name]
     if is_postgresql(engine):
         selection = sa.select(
-            [
+            *[
                 sa.sql.extract(
                     "day",
                     (
                         sa.func.date_trunc(sa.literal("day"), sa.func.max(column))
                         - sa.func.date_trunc(sa.literal("day"), sa.func.min(column))
                     ),
                 )
             ]
         )
     elif is_mssql(engine) or is_snowflake(engine):
         selection = sa.select(
-            [
+            *[
                 sa.func.datediff(
                     sa.text("day"),
                     sa.func.min(column),
                     sa.func.max(column),
                 )
             ]
         )
     elif is_bigquery(engine):
         selection = sa.select(
-            [
+            *[
                 sa.func.date_diff(
                     sa.func.max(column),
                     sa.func.min(column),
                     sa.literal_column("DAY"),
                 )
             ]
         )
     elif is_impala(engine):
         selection = sa.select(
-            [
+            *[
                 sa.func.datediff(
                     sa.func.to_date(sa.func.max(column)),
                     sa.func.to_date(sa.func.min(column)),
                 )
             ]
         )
     elif is_db2(engine):
         selection = sa.select(
-            [
+            *[
                 sa.func.days_between(
                     sa.func.max(column),
                     sa.func.min(column),
                 )
             ]
         )
     else:
@@ -500,25 +500,25 @@
             )
             for dimension in range(dimensionality)
         ]
     )
 
     join_condition = sa.and_(*key_conditions, violation_condition)
     violation_selection = sa.select(
-        table_key_columns
-        + [
+        *table_key_columns,
+        *[
             table.c[start_column]
             for table in [table1, table2]
             for start_column in start_columns
-        ]
-        + [
+        ],
+        *[
             table.c[end_column]
             for table in [table1, table2]
             for end_column in end_columns
-        ]
+        ],
     ).select_from(table1.join(table2, join_condition))
 
     # Note, Kevin, 21/12/09
     # The following approach would likely be preferable to the approach used
     # subsequently. Sadly, it seems to not work for mssql. As of now, it is
     # unclear to me why.
 
@@ -535,15 +535,15 @@
     violation_subquery = violation_selection.subquery()
 
     keys = (
         get_table_columns(violation_subquery, key_columns)
         if key_columns
         else violation_subquery.columns
     )
-    violation_subquery = sa.select(keys, group_by=keys).subquery()
+    violation_subquery = sa.select(*keys).group_by(*keys).subquery()
 
     n_violations_selection = sa.select(sa.func.count()).select_from(violation_subquery)
 
     return violation_selection, n_violations_selection
 
 
 def _not_in_interval_condition(
@@ -620,21 +620,21 @@
     end_rank_column = (
         sa.func.row_number()
         .over(order_by=[raw_end_table.c[col] for col in [end_column] + key_columns])
         .label("end_rank")
     )
 
     start_table = (
-        sa.select([*raw_start_table.columns, start_rank_column])
+        sa.select(*raw_start_table.columns, start_rank_column)
         .where(start_not_in_other_interval_condition)
         .subquery()
     )
 
     end_table = (
-        sa.select([*raw_end_table.columns, end_rank_column])
+        sa.select(*raw_end_table.columns, end_rank_column)
         .where(end_not_in_other_interval_condition)
         .subquery()
     )
 
     legitimate_gap_size = 1 if end_included else 0
 
     if is_mssql(engine) or is_snowflake(engine):
@@ -693,28 +693,26 @@
             for key_column in key_columns
         ],
         start_table.c["start_rank"] == end_table.c["end_rank"] + 1,
         gap_condition,
     )
 
     violation_selection = sa.select(
-        [
-            *get_table_columns(start_table, key_columns),
-            start_table.c[start_column],
-            end_table.c[end_column],
-        ]
+        *get_table_columns(start_table, key_columns),
+        start_table.c[start_column],
+        end_table.c[end_column],
     ).select_from(start_table.join(end_table, join_condition))
 
     violation_subquery = violation_selection.subquery()
 
     keys = get_table_columns(violation_subquery, key_columns)
 
-    grouped_violation_subquery = sa.select(keys, group_by=keys).subquery()
+    grouped_violation_subquery = sa.select(*keys).group_by(*keys).subquery()
 
-    n_violations_selection = sa.select([sa.func.count()]).select_from(
+    n_violations_selection = sa.select(sa.func.count()).select_from(
         grouped_violation_subquery
     )
 
     return violation_selection, n_violations_selection
 
 
 def get_row_count(engine, ref, row_limit: int = None):
@@ -722,17 +720,15 @@
 
     If `row_limit` is given, the number of rows is capped at the limit.
     """
     subquery = ref.get_selection(engine)
     if row_limit:
         subquery = subquery.limit(row_limit)
     subquery = subquery.alias()
-    selection = sa.select([sa.cast(sa.func.count(), sa.BigInteger)]).select_from(
-        subquery
-    )
+    selection = sa.select(sa.cast(sa.func.count(), sa.BigInteger)).select_from(subquery)
     result = engine.connect().execute(selection).scalar()
     return result, [selection]
 
 
 def get_column(
     engine: sa.engine.Engine,
     ref: DataReference,
@@ -744,19 +740,19 @@
     If an aggregation operation is passed, the results are aggregated accordingly
     and a single scalar value is returned.
     """
     subquery = ref.get_selection(engine).alias()
     column = subquery.c[ref.get_column(engine)]
 
     if not aggregate_operator:
-        selection = sa.select([column])
+        selection = sa.select(column)
         result = engine.connect().execute(selection).scalars().all()
 
     else:
-        selection = sa.select([aggregate_operator(column)])
+        selection = sa.select(aggregate_operator(column))
         result = engine.connect().execute(selection).scalar()
 
     return result, [selection]
 
 
 def get_min(engine, ref):
     column_operator = sa.func.min
@@ -780,26 +776,24 @@
 def get_percentile(engine, ref, percentage):
     row_count = "dj_row_count"
     row_num = "dj_row_num"
     column_name = ref.get_column(engine)
     column = ref.get_selection(engine).subquery().c[column_name]
     subquery = (
         sa.select(
-            [
-                column,
-                sa.func.row_number().over(order_by=column).label(row_num),
-                sa.func.count().over(partition_by=None).label(row_count),
-            ]
+            column,
+            sa.func.row_number().over(order_by=column).label(row_num),
+            sa.func.count().over(partition_by=None).label(row_count),
         )
         .where(column.is_not(None))
         .subquery()
     )
 
     constrained_selection = (
-        sa.select(subquery.columns)
+        sa.select(*subquery.columns)
         .where(subquery.c[row_num] * 100.0 / subquery.c[row_count] <= percentage)
         .subquery()
     )
 
     max_selection = sa.select(
         sa.func.max(constrained_selection.c[row_num])
     ).scalar_subquery()
@@ -846,15 +840,15 @@
 def get_uniques(
     engine: sa.engine.Engine, ref: DataReference
 ) -> tuple[Counter, list[sa.select]]:
     if not ref.get_columns(engine):
         return Counter({}), []
     selection = ref.get_selection(engine).alias()
     columns = [selection.c[column_name] for column_name in ref.get_columns(engine)]
-    selection = sa.select([*columns, sa.func.count()], group_by=columns)
+    selection = sa.select(*columns, sa.func.count()).group_by(*columns)
 
     def _scalar_accessor(row):
         return row[0]
 
     def _tuple_accessor(row):
         return row[0 : len(columns)]
 
@@ -871,33 +865,33 @@
     )
     return result, [selection]
 
 
 def get_unique_count(engine, ref):
     selection = ref.get_selection(engine)
     subquery = selection.distinct().alias()
-    selection = sa.select([sa.func.count()]).select_from(subquery)
+    selection = sa.select(sa.func.count()).select_from(subquery)
     result = engine.connect().execute(selection).scalar()
     return result, [selection]
 
 
 def get_unique_count_union(engine, ref, ref2):
     selection1 = ref.get_selection(engine)
     selection2 = ref2.get_selection(engine)
     subquery = sa.sql.union(selection1, selection2).alias().select().distinct().alias()
-    selection = sa.select([sa.func.count()]).select_from(subquery)
+    selection = sa.select(sa.func.count()).select_from(subquery)
     result = engine.connect().execute(selection).scalar()
     return result, [selection]
 
 
 def get_missing_fraction(engine, ref):
     selection = ref.get_selection(engine).subquery()
-    n_rows_total_selection = sa.select([sa.func.count()]).select_from(selection)
+    n_rows_total_selection = sa.select(sa.func.count()).select_from(selection)
     n_rows_missing_selection = (
-        sa.select([sa.func.count()])
+        sa.select(sa.func.count())
         .select_from(selection)
         .where(selection.c[ref.get_column(engine)].is_(None))
     )
     with engine.connect() as connection:
         n_rows_total = connection.execute(n_rows_total_selection).scalar()
         n_rows_missing = connection.execute(n_rows_missing_selection).scalar()
 
@@ -943,15 +937,15 @@
 
 def get_row_difference_count(engine, ref, ref2):
     selection1 = ref.get_selection(engine)
     selection2 = ref2.get_selection(engine)
     subquery = (
         sa.sql.except_(selection1, selection2).alias().select().distinct().alias()
     )
-    selection = sa.select([sa.func.count()]).select_from(subquery)
+    selection = sa.select(sa.func.count()).select_from(subquery)
     result = engine.connect().execute(selection).scalar()
     return result, [selection]
 
 
 def get_row_mismatch(engine, ref, ref2, match_and_compare):
     subselection1 = ref.get_selection(engine).alias()
     subselection2 = ref2.get_selection(engine).alias()
@@ -978,38 +972,38 @@
     compare = sa.and_(
         *[
             sa.or_(column1 == column2, sa.and_(column1.is_(None), column2.is_(None)))
             for column1, column2 in zip(comparing_columns1, comparing_columns2)
         ]
     )
 
-    avg_match_column = sa.func.avg(sa.case([(compare, 0.0)], else_=1.0))
+    avg_match_column = sa.func.avg(sa.case((compare, 0.0), else_=1.0))
 
-    selection_difference = sa.select([avg_match_column]).select_from(
+    selection_difference = sa.select(avg_match_column).select_from(
         subselection1.join(subselection2, match)
     )
     selection_n_rows = sa.select(sa.func.count()).select_from(
         subselection1.join(subselection2, match)
     )
     result_mismatch = engine.connect().execute(selection_difference).scalar()
     result_n_rows = engine.connect().execute(selection_n_rows).scalar()
     return result_mismatch, result_n_rows, [selection_difference, selection_n_rows]
 
 
 def get_duplicate_sample(engine, ref):
     initial_selection = ref.get_selection(engine).alias()
     aggregate_subquery = (
-        sa.select([initial_selection, sa.func.count().label("n_copies")])
+        sa.select(initial_selection, sa.func.count().label("n_copies"))
         .select_from(initial_selection)
         .group_by(*initial_selection.columns)
         .alias()
     )
     duplicate_selection = (
         sa.select(
-            [
+            *[
                 column
                 for column in aggregate_subquery.columns
                 if column.key != "n_copies"
             ]
         )
         .select_from(aggregate_subquery)
         .where(aggregate_subquery.c.n_copies > 1)
@@ -1023,16 +1017,16 @@
 ):
     clause = ref.data_source.get_clause(engine)
     # NOTE: This was needed to appease mypy.
     if not ref.get_columns(engine):
         raise ValueError("There must be a column to group by")
     group_columns = [clause.c[column] for column in ref.get_columns(engine)]
     agg_column = clause.c[aggregation_column]
-    selection = sa.select(
-        [*group_columns, sa.func.array_agg(agg_column)], group_by=[*group_columns]
+    selection = sa.select(*group_columns, sa.func.array_agg(agg_column)).group_by(
+        *group_columns
     )
     return [selection]
 
 
 def snowflake_parse_variant_column(value: str):
     # Snowflake returns non-primitive columns such as arrays as JSON string,
     # but we want them in their deserialized form.
@@ -1060,27 +1054,23 @@
     ``cdf_label``.
     """
     col = ref.get_column(engine)
     selection = ref.get_selection(engine).subquery()
 
     # Step 1: Calculate the CDF over the value column.
     cdf_selection = sa.select(
-        [
-            selection.c[col].label(value_label),
-            sa.func.cume_dist().over(order_by=col).label(cdf_label),
-        ]
+        selection.c[col].label(value_label),
+        sa.func.cume_dist().over(order_by=col).label(cdf_label),
     ).subquery()
 
     # Step 2: Aggregate rows s.t. every value occurs only once.
     grouped_cdf_selection = (
         sa.select(
-            [
-                cdf_selection.c[value_label],
-                sa.func.max(cdf_selection.c[cdf_label]).label(cdf_label),
-            ]
+            cdf_selection.c[value_label],
+            sa.func.max(cdf_selection.c[cdf_label]).label(cdf_label),
         )
         .group_by(cdf_selection.c[value_label])
         .subquery()
     )
     return grouped_cdf_selection
 
 
@@ -1132,21 +1122,19 @@
             .label(group_label)
         )
 
     # Step 4: Create a grouper id based on the value count; this is just a helper for forward-filling.
     # In other words, we point rows to their most recent present value - per sample. This is necessary
     # Due to the nature of the full outer join.
     indexed_cross_cdf = sa.select(
-        [
-            cross_cdf.c[value_label],
-            _cdf_index_column(cross_cdf, value_label, cdf_label1, group_label1),
-            cross_cdf.c[cdf_label1],
-            _cdf_index_column(cross_cdf, value_label, cdf_label2, group_label2),
-            cross_cdf.c[cdf_label2],
-        ]
+        cross_cdf.c[value_label],
+        _cdf_index_column(cross_cdf, value_label, cdf_label1, group_label1),
+        cross_cdf.c[cdf_label1],
+        _cdf_index_column(cross_cdf, value_label, cdf_label2, group_label2),
+        cross_cdf.c[cdf_label2],
     ).subquery()
 
     def _forward_filled_cdf_column(table, cdf_label, value_label, group_label):
         return (
             # Step 6: Replace NULL values at the beginning with 0 to enable computation of difference.
             sa.func.coalesce(
                 (
@@ -1156,23 +1144,21 @@
                     )
                 ),
                 0,
             ).label(cdf_label)
         )
 
     filled_cross_cdf = sa.select(
-        [
-            indexed_cross_cdf.c[value_label],
-            _forward_filled_cdf_column(
-                indexed_cross_cdf, cdf_label1, value_label, group_label1
-            ),
-            _forward_filled_cdf_column(
-                indexed_cross_cdf, cdf_label2, value_label, group_label2
-            ),
-        ]
+        indexed_cross_cdf.c[value_label],
+        _forward_filled_cdf_column(
+            indexed_cross_cdf, cdf_label1, value_label, group_label1
+        ),
+        _forward_filled_cdf_column(
+            indexed_cross_cdf, cdf_label2, value_label, group_label2
+        ),
     )
     return filled_cross_cdf, cdf_label1, cdf_label2
 
 
 def get_ks_2sample(
     engine: sa.engine.Engine,
     ref1: DataReference,
@@ -1215,15 +1201,15 @@
         violation_selection = sa.select(subquery.c[column]).where(
             sa.not_(sa.func.regexp_like(subquery.c[column], regex))
         )
     else:
         violation_selection = sa.select(subquery.c[column]).where(
             sa.not_(subquery.c[column].regexp_match(regex))
         )
-    n_violations_selection = sa.select([sa.func.count()]).select_from(
+    n_violations_selection = sa.select(sa.func.count()).select_from(
         violation_selection.subquery()
     )
 
     selections = [n_violations_selection]
 
     if n_counterexamples == -1:
         counterexamples_selection = violation_selection
```

### Comparing `datajudge-1.5.0/src/datajudge/pytest_integration.py` & `datajudge-1.6.0/src/datajudge/pytest_integration.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/src/datajudge/requirements.py` & `datajudge-1.6.0/src/datajudge/requirements.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/start_mssql.sh` & `datajudge-1.6.0/start_mssql.sh`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/integration/conftest.py` & `datajudge-1.6.0/tests/integration/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,27 +63,27 @@
         return sa.String(40)
     return sa.String()
 
 
 @pytest.fixture(scope="module")
 def engine(backend):
     engine = get_engine(backend)
-    with engine.connect() as conn:
+    with engine.begin() as conn:
         if engine.name in ("postgresql", "bigquery", "impala"):
-            conn.execute(f"CREATE SCHEMA IF NOT EXISTS {SCHEMA}")
+            conn.execute(sa.text(f"CREATE SCHEMA IF NOT EXISTS {SCHEMA}"))
     return engine
 
 
 @pytest.fixture(scope="module")
 def metadata():
     return sa.MetaData()
 
 
 def _handle_table(engine, metadata, table_name, columns, data):
-    with engine.connect() as conn:
+    with engine.begin() as conn:
         if sa.inspect(conn).has_table(table_name, schema=SCHEMA):
             return
         table = sa.Table(table_name, metadata, *columns, schema=SCHEMA)
         table.create(conn)
         conn.execute(table.insert().values(), data)
 
 
@@ -764,24 +764,28 @@
         primary_key = ""
     elif is_db2(engine):
         str_datatype = "VARCHAR(20)"
         # Primary key needs to be non-nullable.
         primary_key = ""
     else:
         str_datatype = "TEXT"
-    with engine.connect() as connection:
-        connection.execute(f"DROP TABLE IF EXISTS {SCHEMA}.{table_name}")
+    with engine.begin() as connection:
+        connection.execute(sa.text(f"DROP TABLE IF EXISTS {SCHEMA}.{table_name}"))
         connection.execute(
-            f"CREATE TABLE {SCHEMA}.{table_name} "
-            f"(id INTEGER {primary_key}, "
-            f"{uppercase_column} {str_datatype}, {lowercase_column} INTEGER)"
+            sa.text(
+                f"CREATE TABLE {SCHEMA}.{table_name} "
+                f"(id INTEGER {primary_key}, "
+                f"{uppercase_column} {str_datatype}, {lowercase_column} INTEGER)"
+            )
         )
         connection.execute(
-            f"INSERT INTO {SCHEMA}.{table_name} "
-            f"(id, {uppercase_column}, {lowercase_column}) VALUES (1, 'QuantCo', 100)"
+            sa.text(
+                f"INSERT INTO {SCHEMA}.{table_name} "
+                f"(id, {uppercase_column}, {lowercase_column}) VALUES (1, 'QuantCo', 100)"
+            )
         )
     return TEST_DB_NAME, SCHEMA, table_name, uppercase_column, lowercase_column
 
 
 @pytest.fixture(scope="module")
 def cross_cdf_table1(engine, metadata):
     table_name = "cross_cdf_table1"
```

### Comparing `datajudge-1.5.0/tests/integration/test_column_capitalization.py` & `datajudge-1.6.0/tests/integration/test_column_capitalization.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/integration/test_data_source.py` & `datajudge-1.6.0/tests/integration/test_data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,33 +30,33 @@
 
     query = (
         f"SELECT * FROM {schema_name1}.{table_name1} {union} "
         f"SELECT * FROM {schema_name2}.{table_name2}"
     )
     data_source = RawQueryDataSource(query, "string query")
     derived_clause = data_source.get_clause(engine)
-    derived_selection = sa.select([derived_clause])
+    derived_selection = sa.select(derived_clause)
     with engine.connect() as connection:
         rows = connection.execute(derived_selection).scalars().fetchall()
     assert set(rows) == set(range(1, 20))
 
 
 def test_custom_data_source_from_expression(engine, metadata, int_table1, int_table2):
     _, schema_name1, table_name1 = int_table1
     _, schema_name2, table_name2 = int_table2
     table1 = sa.Table(table_name1, metadata, schema=schema_name1, autoload_with=engine)
     table2 = sa.Table(table_name2, metadata, schema=schema_name2, autoload_with=engine)
     subquery = sa.union(
-        sa.select([table1]).where(table1.c["col_int"] < 10),
-        sa.select([table2]).where(table2.c["col_int"] > 10),
+        sa.select(table1).where(table1.c["col_int"] < 10),
+        sa.select(table2).where(table2.c["col_int"] > 10),
     ).subquery()
-    selection = sa.select([subquery])
+    selection = sa.select(subquery)
     data_source = ExpressionDataSource(selection, "expression")
     derived_clause = data_source.get_clause(engine)
-    derived_selection = sa.select([derived_clause])
+    derived_selection = sa.select(derived_clause)
     with engine.connect() as connection:
         rows = connection.execute(derived_selection).scalars().fetchall()
 
     assert set(rows) == (set(range(1, 10)) | set(range(11, 20)))
 
 
 @pytest.mark.parametrize(
```

### Comparing `datajudge-1.5.0/tests/integration/test_integration.py` & `datajudge-1.6.0/tests/integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/integration/test_stats.py` & `datajudge-1.6.0/tests/integration/test_stats.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/unit/test_condition.py` & `datajudge-1.6.0/tests/unit/test_condition.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/unit/test_db_access.py` & `datajudge-1.6.0/tests/unit/test_db_access.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/unit/test_percentiles.py` & `datajudge-1.6.0/tests/unit/test_percentiles.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/unit/test_pytest.py` & `datajudge-1.6.0/tests/unit/test_pytest.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/tests/unit/test_set_functions.py` & `datajudge-1.6.0/tests/unit/test_set_functions.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.5.0/PKG-INFO` & `datajudge-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datajudge
-Version: 1.5.0
+Version: 1.6.0
 Summary: datajudge allows to assess  whether data from database complies with reference
 Keywords: test,databases,validation
 Author-email: "QuantCo, Inc." <noreply@quantco.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

