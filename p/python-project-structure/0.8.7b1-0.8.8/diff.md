# Comparing `tmp/python-project-structure-0.8.7b1.tar.gz` & `tmp/python-project-structure-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.7b1.tar", last modified: Tue Apr 11 20:57:10 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.8.tar", last modified: Tue Apr 11 22:51:09 2023, max compression
```

## Comparing `python-project-structure-0.8.7b1.tar` & `python-project-structure-0.8.8.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.656696 python-project-structure-0.8.7b1/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    58038 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4776 2023-04-11 20:56:55.000000 python-project-structure-0.8.7b1/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5044 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/gitlab-runner/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       46 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/gitlab-runner/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/gitlab-runner/config/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1323 2023-04-11 20:39:14.000000 python-project-structure-0.8.7b1/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.664696 python-project-structure-0.8.7b1/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 20:56:57.000000 python-project-structure-0.8.7b1/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.660696 python-project-structure-0.8.7b1/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1829 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 20:57:10.668696 python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-11 20:57:10.000000 python-project-structure-0.8.7b1/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.7b1/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.955779 python-project-structure-0.8.8/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.959779 python-project-structure-0.8.8/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    58045 2023-04-11 21:22:27.000000 python-project-structure-0.8.8/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5159 2023-04-11 22:50:54.000000 python-project-structure-0.8.8/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13218 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.959779 python-project-structure-0.8.8/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5044 2023-04-11 20:39:14.000000 python-project-structure-0.8.8/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/gitlab-runner/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       46 2023-04-11 20:39:14.000000 python-project-structure-0.8.8/gitlab-runner/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/gitlab-runner/config/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1323 2023-04-11 20:39:14.000000 python-project-structure-0.8.8/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2627 2023-04-11 22:50:56.000000 python-project-structure-0.8.8/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.955779 python-project-structure-0.8.8/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13218 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1829 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      160 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/tox.ini
```

### Comparing `python-project-structure-0.8.7b1/.dir-locals.el.in` & `python-project-structure-0.8.8/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/.dockerignore` & `python-project-structure-0.8.8/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/.env.in` & `python-project-structure-0.8.8/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/.github/workflows/build-test.yml` & `python-project-structure-0.8.8/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/.gitignore` & `python-project-structure-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/.gitlab-ci.yml` & `python-project-structure-0.8.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/.pre-commit-config.yaml` & `python-project-structure-0.8.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/.prospector.yaml` & `python-project-structure-0.8.8/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/CONTRIBUTING.rst` & `python-project-structure-0.8.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/Dockerfile` & `python-project-structure-0.8.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/Dockerfile.devel` & `python-project-structure-0.8.8/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/LICENSE` & `python-project-structure-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/Makefile` & `python-project-structure-0.8.8/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -650,18 +650,18 @@
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
 ifeq ($(VCS_BRANCH),master)
 # Merge the bumped version back into `develop`:
 	bump_rev="$$(git rev-parse HEAD)"
-	git checkout --track "$(VCS_UPSTREAM_REMOTE)/develop" --
+	git checkout --track "$(VCS_COMPARE_REMOTE)/develop" --
 	git merge --ff --gpg-sign \
 	    -m "Merge branch 'master' release back into develop" "$${bump_rev}"
-	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:develop"
+	git push --no-verify --tags "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
 	git checkout "$${bump_rev}" --
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
 # Ensure the tag is available for creating the GitHub release below but push *before* to
 # GitLab to avoid a race with repository mirrorying:
 	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
```

### Comparing `python-project-structure-0.8.7b1/NEWS.rst` & `python-project-structure-0.8.8/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+python-project-structure 0.8.8 (2023-04-11)
+===========================================
+
+No significant changes.
+
+
+python-project-structure 0.8.8b0 (2023-04-11)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+python-project-structure 0.8.7 (2023-04-11)
+===========================================
+
+No significant changes.
+
+
 python-project-structure 0.8.7b1 (2023-04-11)
 =============================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Tue Apr 11 08:15:25 PM UTC 2023. (upgrade-requirements)
```

### Comparing `python-project-structure-0.8.7b1/PKG-INFO` & `python-project-structure-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.7b1
+Version: 0.8.8
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.7b1/README.rst` & `python-project-structure-0.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/TODO.rst` & `python-project-structure-0.8.8/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/bin/cz-check-bump` & `python-project-structure-0.8.8/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/bin/entrypoint` & `python-project-structure-0.8.8/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/bin/get-base-version` & `python-project-structure-0.8.8/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/Dockerfile` & `python-project-structure-0.8.8/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/Makefile` & `python-project-structure-0.8.8/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/README.rst` & `python-project-structure-0.8.8/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/bin/entrypoint` & `python-project-structure-0.8.8/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/requirements-py310.txt` & `python-project-structure-0.8.8/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/requirements-py311.txt` & `python-project-structure-0.8.8/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/requirements-py37.txt` & `python-project-structure-0.8.8/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/requirements-py38.txt` & `python-project-structure-0.8.8/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/build-host/requirements-py39.txt` & `python-project-structure-0.8.8/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/docker-compose.override.yml` & `python-project-structure-0.8.8/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/docker-compose.yml` & `python-project-structure-0.8.8/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/gitlab-runner/config/config.toml.in` & `python-project-structure-0.8.8/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/pyproject.toml` & `python-project-structure-0.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.7b1"
+version = "0.8.8"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
 """
```

### Comparing `python-project-structure-0.8.7b1/requirements/build.txt.in` & `python-project-structure-0.8.8/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py310/build.txt` & `python-project-structure-0.8.8/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py310/devel.txt` & `python-project-structure-0.8.8/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py311/build.txt` & `python-project-structure-0.8.8/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py311/devel.txt` & `python-project-structure-0.8.8/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py37/build.txt` & `python-project-structure-0.8.8/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py37/devel.txt` & `python-project-structure-0.8.8/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py38/build.txt` & `python-project-structure-0.8.8/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py38/devel.txt` & `python-project-structure-0.8.8/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py39/build.txt` & `python-project-structure-0.8.8/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/requirements/py39/devel.txt` & `python-project-structure-0.8.8/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/setup.cfg` & `python-project-structure-0.8.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.8/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.7b1
+Version: 0.8.8
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.7b1/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.8/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.8/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.8/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.7b1/tox.ini` & `python-project-structure-0.8.8/tox.ini`

 * *Files identical despite different names*

