# Comparing `tmp/dcqc-1.2.0.tar.gz` & `tmp/dcqc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcqc-1.2.0.tar", last modified: Mon Apr  3 22:37:45 2023, max compression
+gzip compressed data, was "dcqc-1.3.0.tar", last modified: Wed Apr 12 07:28:55 2023, max compression
```

## Comparing `dcqc-1.2.0.tar` & `dcqc-1.3.0.tar`

### file list

```diff
@@ -1,92 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.782023 dcqc-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-03 22:36:55.000000 dcqc-1.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.766023 dcqc-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.774023 dcqc-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-03 22:36:55.000000 dcqc-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-03 22:36:55.000000 dcqc-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-03 22:36:55.000000 dcqc-1.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-03 22:36:55.000000 dcqc-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-03 22:36:55.000000 dcqc-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-03 22:36:55.000000 dcqc-1.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-03 22:36:55.000000 dcqc-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-03 22:36:55.000000 dcqc-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 22:36:55.000000 dcqc-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-03 22:37:45.782023 dcqc-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-03 22:36:55.000000 dcqc-1.2.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-04-03 22:36:55.000000 dcqc-1.2.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-03 22:36:55.000000 dcqc-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.774023 dcqc-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.774023 dcqc-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-03 22:36:55.000000 dcqc-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-03 22:36:55.000000 dcqc-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-03 22:37:45.782023 dcqc-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-03 22:36:55.000000 dcqc-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.770023 dcqc-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.778023 dcqc-1.2.0/src/dcqc/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.778023 dcqc-1.2.0/src/dcqc/suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/suites/suite_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/suites/suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.778023 dcqc-1.2.0/src/dcqc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/tests/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/dcqc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.778023 dcqc-1.2.0/src/dcqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-03 22:37:45.000000 dcqc-1.2.0/src/dcqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-03 22:37:45.000000 dcqc-1.2.0/src/dcqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 22:37:45.000000 dcqc-1.2.0/src/dcqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-03 22:37:45.000000 dcqc-1.2.0/src/dcqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 22:37:45.000000 dcqc-1.2.0/src/dcqc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-03 22:37:45.000000 dcqc-1.2.0/src/dcqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 22:37:45.000000 dcqc-1.2.0/src/dcqc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.778023 dcqc-1.2.0/src/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-03 22:36:55.000000 dcqc-1.2.0/src/docker/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.778023 dcqc-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.778023 dcqc-1.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/circuit.tif
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/example.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/example.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/files.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/small.csv
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/suite.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/target.json
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/test.computed.json
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/test.external.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/test.internal.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 22:37:45.782023 dcqc-1.2.0/tests/data/tiffinfo/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/tiffinfo/exit_code.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/tiffinfo/std_err.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/data/tiffinfo/std_out.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-03 22:36:55.000000 dcqc-1.2.0/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-03 22:36:55.000000 dcqc-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.424489 dcqc-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-12 07:28:01.000000 dcqc-1.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.412489 dcqc-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-12 07:28:01.000000 dcqc-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 07:28:01.000000 dcqc-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 07:28:01.000000 dcqc-1.3.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-12 07:28:01.000000 dcqc-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 07:28:01.000000 dcqc-1.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 07:28:01.000000 dcqc-1.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 07:28:01.000000 dcqc-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-12 07:28:01.000000 dcqc-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 07:28:01.000000 dcqc-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 07:28:55.424489 dcqc-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 07:28:01.000000 dcqc-1.3.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-04-12 07:28:01.000000 dcqc-1.3.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-12 07:28:01.000000 dcqc-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 07:28:01.000000 dcqc-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-12 07:28:01.000000 dcqc-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-12 07:28:55.424489 dcqc-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 07:28:01.000000 dcqc-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.412489 dcqc-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.416489 dcqc-1.3.0/src/dcqc/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/dcqc/suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/suites/suite_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/suites/suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/dcqc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/tests/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/dcqc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/dcqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 07:28:55.000000 dcqc-1.3.0/src/dcqc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/src/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 07:28:01.000000 dcqc-1.3.0/src/docker/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.420489 dcqc-1.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/circuit.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/example.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/files.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/suite.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/target.json
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.computed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.external.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/test_contains_word_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:55.424489 dcqc-1.3.0/tests/data/tiffinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tiffinfo/exit_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tiffinfo/std_err.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/data/tiffinfo/std_out.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-12 07:28:01.000000 dcqc-1.3.0/tests/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-12 07:28:01.000000 dcqc-1.3.0/tox.ini
```

### Comparing `dcqc-1.2.0/.coveragerc` & `dcqc-1.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/.github/workflows/ci.yml` & `dcqc-1.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/.gitignore` & `dcqc-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/.pre-commit-config.yaml` & `dcqc-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/CONTRIBUTING.md` & `dcqc-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/LICENSE.txt` & `dcqc-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/PKG-INFO` & `dcqc-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.2.0/Pipfile.lock` & `dcqc-1.3.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/README.md` & `dcqc-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/docs/Makefile` & `dcqc-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/docs/conf.py` & `dcqc-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/docs/index.md` & `dcqc-1.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/pyproject.toml` & `dcqc-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/setup.cfg` & `dcqc-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/setup.py` & `dcqc-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/__init__.py` & `dcqc-1.3.0/src/dcqc/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/file.py` & `dcqc-1.3.0/src/dcqc/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 FileType("*", (), "format_1915")  # To represent all file types
 FileType("TXT", (".txt",), "format_1964")
 FileType("JSON", (".json",), "format_3464")
 FileType("JSON-LD", (".jsonld",), "format_3749")
 FileType("TIFF", (".tif", ".tiff"), "format_3591")
 FileType("OME-TIFF", (".ome.tif", ".ome.tiff"), "format_3727")
 FileType("TSV", (".tsv"), "format_3475")
+FileType("BAM", (".bam"), "format_2572")
+FileType("FASTQ", (".fastq", ".fastq.gz", ".fq", ".fq.gz"), "format_1930")
 
 
 # TODO: Leverage post-init function in dataclasses
 @dataclass
 class File(SerializableMixin):
     """Construct a File object.
```

### Comparing `dcqc-1.2.0/src/dcqc/main.py` & `dcqc-1.3.0/src/dcqc/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import json
 import sys
 from csv import DictWriter
 from pathlib import Path
 from typing import List
 
 from typer import Argument, Exit, Option, Typer
 
 from dcqc import __version__
-from dcqc.file import FileType
+from dcqc.file import File, FileType
 from dcqc.parsers import CsvParser, JsonParser
 from dcqc.reports import JsonReport
 from dcqc.suites.suite_abc import SuiteABC
 from dcqc.target import Target
 from dcqc.tests.test_abc import ExternalTestMixin, TestABC
 
 # Make commands optional to allow for `dcqc --version`
@@ -26,14 +27,16 @@
 output_path_arg = Argument(..., help="Path for output file")
 output_dir_path_arg = Argument(..., help="Directory path for output files")
 
 # Common options
 overwrite_opt = Option(False, "--overwrite", "-f", help="Ignore existing files")
 required_tests_opt = Option(None, "--required-tests", "-r", help="Required tests")
 skipped_tests_opt = Option(None, "--skipped-tests", "-s", help="Skipped tests")
+file_type_opt = Option(..., "--file-type", "-t", help="File type")
+metadata_opt = Option("{}", "--metadata", "-m", help="File metadata")
 
 
 @app.callback()
 def main(version: bool = False):
     """DCQC Python Package"""
     if version:
         print(f"DCQC Python Package Version: {__version__}")
@@ -167,7 +170,37 @@
             }
             rows.append(test_dict)
 
     fieldnames = list(rows[0])
     writer = DictWriter(sys.stdout, fieldnames)
     writer.writeheader()
     writer.writerows(rows)
+
+
+@app.command()
+def qc_file(
+    input_file: Path = input_path_arg,
+    file_type: str = file_type_opt,
+    metadata: str = metadata_opt,
+    required_tests: List[str] = required_tests_opt,
+    skipped_tests: List[str] = skipped_tests_opt,
+):
+    """Run QC tests on a single file (external tests are skipped)"""
+    # Interpret empty lists from CLI as None (to auto-generate values)
+    required_tests_maybe = required_tests if required_tests else None
+
+    # Prepare target
+    file_metadata = json.loads(metadata)
+    file_metadata["file_type"] = file_type
+    file = File(input_file.as_posix(), file_metadata)
+    target = Target(file)
+
+    # Prepare suite (skip all external tests)
+    suite = SuiteABC.from_target(target, required_tests_maybe, skipped_tests)
+    external_tests = [test.type for test in suite.tests if test.is_external_test]
+    skipped_tests += external_tests
+    suite = SuiteABC.from_target(target, required_tests_maybe, skipped_tests)
+
+    # Output QC report on stdout
+    report = JsonReport()
+    suite_json = report.generate(suite)
+    json.dump(suite_json, sys.stdout, indent=2)
```

### Comparing `dcqc-1.2.0/src/dcqc/mixins.py` & `dcqc-1.3.0/src/dcqc/mixins.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/parsers.py` & `dcqc-1.3.0/src/dcqc/parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/reports.py` & `dcqc-1.3.0/src/dcqc/reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/suites/suite_abc.py` & `dcqc-1.3.0/src/dcqc/suites/suite_abc.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/suites/suites.py` & `dcqc-1.3.0/src/dcqc/suites/suites.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,25 @@
 class JsonLdSuite(JsonSuite):
     file_type = FileType.get_file_type("JSON-LD")
     add_tests = (tests.JsonLdLoadTest,)
 
 
 class TiffSuite(FileSuite):
     file_type = FileType.get_file_type("TIFF")
-    add_tests = (tests.LibTiffInfoTest,)
+    add_tests = (tests.LibTiffInfoTest, tests.GrepDateTest)
 
 
 class OmeTiffSuite(TiffSuite):
     file_type = FileType.get_file_type("OME-TIFF")
     add_tests = (tests.OmeXmlSchemaTest, tests.BioFormatsInfoTest)
 
 
 class TSVSuite(FileSuite):
     file_type = FileType.get_file_type("TSV")
+
+
+class BAMSuite(FileSuite):
+    file_type = FileType.get_file_type("BAM")
+
+
+class FastqSuite(FileSuite):
+    file_type = FileType.get_file_type("FASTQ")
```

### Comparing `dcqc-1.2.0/src/dcqc/target.py` & `dcqc-1.3.0/src/dcqc/target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/tests/test_abc.py` & `dcqc-1.3.0/src/dcqc/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc/tests/tests.py` & `dcqc-1.3.0/src/dcqc/tests/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,7 +132,28 @@
             file.local_path.as_posix(),
         ]
         process = Process(
             container="quay.io/sagebionetworks/bftools:latest",
             command_args=command_args,
         )
         return process
+
+
+class GrepDateTest(ExternalTestMixin, TestABC):
+    tier = 4
+
+    def generate_process(self) -> Process:
+        file = self.get_file()
+        path = file.local_path.as_posix()
+        command_args = [
+            "grep",
+            "-E",
+            "-w",
+            "-i",
+            "'date|time'",
+            path,
+        ]
+        process = Process(
+            container="quay.io/biocontainers/coreutils:8.30--h14c3975_1000",
+            command_args=command_args,
+        )
+        return process
```

### Comparing `dcqc-1.2.0/src/dcqc/utils.py` & `dcqc-1.3.0/src/dcqc/utils.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/src/dcqc.egg-info/PKG-INFO` & `dcqc-1.3.0/src/dcqc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.2.0/src/dcqc.egg-info/SOURCES.txt` & `dcqc-1.3.0/src/dcqc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -55,23 +55,27 @@
 tests/test_main.py
 tests/test_parsers.py
 tests/test_reports.py
 tests/test_suites.py
 tests/test_target.py
 tests/test_tests.py
 tests/data/circuit.tif
+tests/data/example.bam
+tests/data/example.fastq
+tests/data/example.fastq.gz
 tests/data/example.jsonld
 tests/data/example.tsv
 tests/data/file.json
 tests/data/files.csv
 tests/data/generate.py
 tests/data/small.csv
 tests/data/suite.json
 tests/data/target.json
 tests/data/test.computed.json
 tests/data/test.external.json
 tests/data/test.internal.json
 tests/data/test.txt
+tests/data/test_contains_word_date.txt
 tests/data/tests.json
 tests/data/tiffinfo/exit_code.txt
 tests/data/tiffinfo/std_err.txt
 tests/data/tiffinfo/std_out.txt
```

### Comparing `dcqc-1.2.0/tests/conftest.py` & `dcqc-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/data/circuit.tif` & `dcqc-1.3.0/tests/data/circuit.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/data/example.jsonld` & `dcqc-1.3.0/tests/data/example.jsonld`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/data/generate.py` & `dcqc-1.3.0/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/data/suite.json` & `dcqc-1.3.0/tests/data/suite.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/data/tests.json` & `dcqc-1.3.0/tests/data/tests.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/test_acceptance.py` & `dcqc-1.3.0/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/test_file.py` & `dcqc-1.3.0/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/test_main.py` & `dcqc-1.3.0/tests/test_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -116,7 +116,21 @@
     assert output_path.exists()
 
 
 def test_list_tests():
     args = ["list-tests"]
     result = run_command(args)
     check_command_result(result)
+
+
+def test_qc_file(get_data):
+    tiff_path = get_data("circuit.tif")
+    args = [
+        "qc-file",
+        "-t",
+        "TIFF",
+        "-m",
+        '{"md5_checksum": "c7b08f6decb5e7572efbe6074926a843"}',
+        tiff_path,
+    ]
+    result = run_command(args)
+    check_command_result(result)
```

### Comparing `dcqc-1.2.0/tests/test_parsers.py` & `dcqc-1.3.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/test_reports.py` & `dcqc-1.3.0/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/test_suites.py` & `dcqc-1.3.0/tests/test_suites.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import pytest
 
 from dcqc.file import FileType
 from dcqc.suites.suite_abc import SuiteABC
 from dcqc.suites.suites import FileSuite, OmeTiffSuite, TiffSuite
 from dcqc.tests.test_abc import TestABC, TestStatus
-from dcqc.tests.tests import FileExtensionTest, LibTiffInfoTest
+from dcqc.tests.tests import FileExtensionTest, GrepDateTest, LibTiffInfoTest
 
 FileType("None", ())
 FileType("Unpaired", ())
 
 
 class RedundantFileSuite(TiffSuite):
     file_type = FileType.get_file_type("None")
-    del_tests = (LibTiffInfoTest,)
+    del_tests = (
+        LibTiffInfoTest,
+        GrepDateTest,
+    )
 
 
 class DummyTest(TestABC):
     def compute_status(self) -> TestStatus:
         return TestStatus.NONE
 
 
@@ -66,15 +69,15 @@
 
 def test_that_the_generic_file_suite_is_retrieved_for_an_unpaired_file_type():
     actual = SuiteABC.get_subclass_by_file_type("Unpaired")
     assert actual is FileSuite
 
 
 def test_that_the_default_required_tests_are_only_tiers_1_and_2(test_suites):
-    suite = test_suites["tiff"]
+    suite = test_suites["jsonld"]
     assert all(test.tier <= 2 for test in suite.tests)
 
 
 def test_that_skipped_tests_are_skipped_when_building_suite_from_tests(test_suites):
     suite = test_suites["tiff"]
     tests = suite.tests
     new_suite = SuiteABC.from_tests(tests, skipped_tests=["LibTiffInfoTest"])
@@ -93,24 +96,24 @@
     with pytest.raises(ValueError):
         SuiteABC.from_tests(tests)
 
 
 def test_that_a_suite_will_not_consider_unrequired_tests(test_targets):
     target = test_targets["bad"]
     required_tests = []
-    skipped_tests = ["LibTiffInfoTest"]
+    skipped_tests = ["LibTiffInfoTest", "GrepDateTest"]
     suite = SuiteABC.from_target(target, required_tests, skipped_tests)
     suite_status = suite.compute_status()
     assert suite_status == TestStatus.PASS
 
 
 def test_that_a_suite_will_consider_required_tests_when_failing(test_targets):
     target = test_targets["bad"]
     required_tests = ["FileExtensionTest"]
-    skipped_tests = ["LibTiffInfoTest"]
+    skipped_tests = ["LibTiffInfoTest", "GrepDateTest"]
     suite = SuiteABC.from_target(target, required_tests, skipped_tests)
     suite_status = suite.compute_status()
     assert suite_status == TestStatus.FAIL
 
 
 def test_that_a_suite_will_consider_required_tests_when_passing(test_targets):
     target = test_targets["good"]
```

### Comparing `dcqc-1.2.0/tests/test_target.py` & `dcqc-1.3.0/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.2.0/tests/test_tests.py` & `dcqc-1.3.0/tests/test_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -188,13 +188,44 @@
 def test_that_a_process_can_be_serialized_and_deserialized():
     process = Process("foo:bar", ["python"])
     process_dict = process.to_dict()
     process_from_dict = Process.from_dict(process_dict)
     assert process_dict == process_from_dict.to_dict()
 
 
+def test_that_the_grep_date_test_correctly_interprets_exit_code_0_and_1(
+    test_files, mocker
+):
+    tiff_file = test_files["tiff"]
+    target = Target(tiff_file)
+    with TemporaryDirectory() as tmp_dir:
+        path_0 = Path(tmp_dir, "code_0.txt")
+        path_1 = Path(tmp_dir, "code_1.txt")
+        path_0.write_text("0")
+        path_1.write_text("1")
+        good_outputs = {"std_out": path_1, "std_err": path_1, "exit_code": path_0}
+        bad_outputs = {"std_out": path_0, "std_err": path_0, "exit_code": path_1}
+
+        test = tests.GrepDateTest(target)
+        mocker.patch.object(test, "_find_process_outputs", return_value=good_outputs)
+        test_status = test.get_status()
+        assert test_status == TestStatus.PASS
+
+        test = tests.LibTiffInfoTest(target)
+        mocker.patch.object(test, "_find_process_outputs", return_value=bad_outputs)
+        test_status = test.get_status()
+        assert test_status == TestStatus.FAIL
+
+
+def test_that_the_grep_date_test_command_is_produced(test_targets):
+    target = test_targets["tiff"]
+    test = tests.GrepDateTest(target)
+    process = test.generate_process()
+    assert "grep" in process.command
+
+
 def test_for_an_error_when_getting_one_file_from_multi_file_target(test_files):
     file = test_files["good"]
     target = Target(file, file)
     test = tests.FileExtensionTest(target)
     with pytest.raises(ValueError):
         test.get_file()
```

### Comparing `dcqc-1.2.0/tox.ini` & `dcqc-1.3.0/tox.ini`

 * *Files identical despite different names*

