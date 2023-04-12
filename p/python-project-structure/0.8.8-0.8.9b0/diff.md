# Comparing `tmp/python-project-structure-0.8.8.tar.gz` & `tmp/python-project-structure-0.8.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-structure-0.8.8.tar", last modified: Tue Apr 11 22:51:09 2023, max compression
+gzip compressed data, was "python-project-structure-0.8.9b0.tar", last modified: Wed Apr 12 16:22:09 2023, max compression
```

## Comparing `python-project-structure-0.8.8.tar` & `python-project-structure-0.8.9b0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.dir-locals.el.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.dockerignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.env.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.955779 python-project-structure-0.8.8/.github/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.959779 python-project-structure-0.8.8/.github/workflows/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.github/workflows/build-test.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4182 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.gitlab-ci.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.pre-commit-config.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/.prospector.yaml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/CONTRIBUTING.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/Dockerfile.devel
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/LICENSE
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    58045 2023-04-11 21:22:27.000000 python-project-structure-0.8.8/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5159 2023-04-11 22:50:54.000000 python-project-structure-0.8.8/NEWS.rst
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13218 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/PKG-INFO
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/README.rst
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/TODO.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.959779 python-project-structure-0.8.8/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/cz-check-bump
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/entrypoint
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/get-base-version
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/bin/hadolint
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/build-host/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/Dockerfile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/Makefile
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/README.rst
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/build-host/bin/
--rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/bin/entrypoint
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py310.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py311.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py37.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py38.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/build-host/requirements-py39.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/build-host/requirements.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/dist/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/dist/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5044 2023-04-11 20:39:14.000000 python-project-structure-0.8.8/docker-compose.override.yml
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/docker-compose.yml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/gitlab-runner/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       46 2023-04-11 20:39:14.000000 python-project-structure-0.8.8/gitlab-runner/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/gitlab-runner/config/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1323 2023-04-11 20:39:14.000000 python-project-structure-0.8.8/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/home/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/home/.gitignore
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/home/.pypirc.in
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2627 2023-04-11 22:50:56.000000 python-project-structure-0.8.8/pyproject.toml
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/build.txt.in
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py310/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py310/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py310/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py310/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py311/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py311/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py311/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py311/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py37/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py37/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py37/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py37/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.963779 python-project-structure-0.8.8/requirements/py38/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py38/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py38/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py38/user.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/requirements/py39/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/requirements/py39/build.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py39/devel.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-11 22:50:57.000000 python-project-structure-0.8.8/requirements/py39/user.txt
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/setup.cfg
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.955779 python-project-structure-0.8.8/src/
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/python_project_structure.egg-info/
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13218 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/PKG-INFO
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1829 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/entry_points.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/requires.txt
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/python_project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/pythonprojectstructure/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/__main__.py
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/pythonprojectstructure/newsfragments/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/newsfragments/.gitignore
-drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-11 22:51:09.967779 python-project-structure-0.8.8/src/pythonprojectstructure/tests/
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/tests/__init__.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/tests/test_cli.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/src/pythonprojectstructure/utils.py
--rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      160 2023-04-11 22:51:09.000000 python-project-structure-0.8.8/src/pythonprojectstructure/version.py
--rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 11:32:46.000000 python-project-structure-0.8.8/tox.ini
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      543 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.dir-locals.el.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.dockerignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      687 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.env.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/.github/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/.github/workflows/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4593 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1479 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4519 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/.gitlab-ci.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      779 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2377 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/.prospector.yaml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3931 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2519 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2859 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/Dockerfile.devel
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1081 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/LICENSE
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    58045 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5312 2023-04-12 16:21:49.000000 python-project-structure-0.8.9b0/NEWS.rst
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/PKG-INFO
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)    12157 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/README.rst
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2744 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/TODO.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2792 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/cz-check-bump
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      977 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/entrypoint
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     1101 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/get-base-version
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)      321 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/bin/hadolint
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/build-host/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2092 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/Dockerfile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1438 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/Makefile
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      746 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/README.rst
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/build-host/bin/
+-rwxrwxrwx   0 python-project-structure  (1001) python-project-structure  (1001)     2058 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      731 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      674 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      948 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      729 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)        4 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/build-host/requirements.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/dist/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      122 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/dist/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5044 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/docker-compose.override.yml
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      651 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/docker-compose.yml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/gitlab-runner/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       46 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/gitlab-runner/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/gitlab-runner/config/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1323 2023-04-12 16:04:03.000000 python-project-structure-0.8.9b0/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/home/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       64 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/home/.gitignore
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      327 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/home/.pypirc.in
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2629 2023-04-12 16:21:50.000000 python-project-structure-0.8.9b0/pyproject.toml
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      578 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/build.txt.in
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py310/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py310/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4945 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py310/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py311/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2414 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py311/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4696 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      264 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py311/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py37/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2645 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py37/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     5416 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      406 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py37/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py38/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2515 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py38/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4985 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py38/user.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/requirements/py39/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     2412 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/requirements/py39/build.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4972 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      262 2023-04-12 16:21:51.000000 python-project-structure-0.8.9b0/requirements/py39/user.txt
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     1701 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/setup.cfg
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/src/
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.256429 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)    13220 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)     1829 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)        1 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       73 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      146 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/requires.txt
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)       23 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/python_project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/src/pythonprojectstructure/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4262 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      201 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/__main__.py
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       91 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/newsfragments/.gitignore
+drwxr-xr-x   0 python-project-structure  (1001) python-project-structure  (1001)        0 2023-04-12 16:22:09.260429 python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)       72 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/__init__.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     4438 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/test_cli.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)      395 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/utils.py
+-rw-r--r--   0 python-project-structure  (1001) python-project-structure  (1001)      162 2023-04-12 16:22:09.000000 python-project-structure-0.8.9b0/src/pythonprojectstructure/version.py
+-rw-rw-rw-   0 python-project-structure  (1001) python-project-structure  (1001)     3443 2023-04-11 13:41:59.000000 python-project-structure-0.8.9b0/tox.ini
```

### Comparing `python-project-structure-0.8.8/.dir-locals.el.in` & `python-project-structure-0.8.9b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/.dockerignore` & `python-project-structure-0.8.9b0/.dockerignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/.env.in` & `python-project-structure-0.8.9b0/.env.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/.github/workflows/build-test.yml` & `python-project-structure-0.8.9b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/.gitignore` & `python-project-structure-0.8.9b0/.gitignore`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/.gitlab-ci.yml` & `python-project-structure-0.8.9b0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
   GH_TOKEN: "$PROJECT_GITHUB_PAT"
   # Uncomment to get more debugging output:
   # DEBUG: "true"
 
 stages:
   - "build-test"
   - "release"
+  - "release-tag"
   - "scheduled"
 
 build-test:
   stage: "build-test"
   rules:
     - if: >-
         ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
@@ -100,25 +101,41 @@
   variables:
     DOCKER_BUILD_PULL: "true"
   rules:
     - if: >-
         ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
         && $CI_PROJECT_NAMESPACE == "rpatterson"
         && $CI_COMMIT_BRANCH != null
-        && $CI_COMMIT_BRANCH =~ "^(develop|master)$"
+        && $CI_COMMIT_BRANCH =~ /^(develop|master)$/
         && $CI_PIPELINE_SOURCE != "schedule"
         && $CI_COMMIT_MESSAGE !~ /(?ims).*\[actions skip\].*/
   script:
     - >-
       entrypoint make -e release-python test-clean
   artifacts:
     paths:
       - "./NEWS-release.rst"
       - "./dist/python?project?structure-*"
 
+
+release-tag:
+  stage: "release-tag"
+  needs: []
+  dependencies: []
+  rules:
+    - if: >-
+        $CI_COMMIT_TAG != null && $CI_COMMIT_TAG =~ /^v*\.*\.*$/
+  inherit:
+    default: false
+  # Version tags are only created and pushed if the pipeline that generated the
+  # release succeeded:
+  script:
+    - >-
+      true
+
 # TEMPLATE: Optionally add a scheduled pipeline with the following variables to
 # periodically upgrade all requirements and run CI:
 # - `DOCKER_BUILD_PULL=true`
 # - `SCHEDULED_TARGETS=devel-upgrade-branch`
 # - `TEMPLATE_IGNORE_EXISTING=true`
 # WARNING: Running this even just daily can easily exhaust the gitlab.org free quotas.
```

### Comparing `python-project-structure-0.8.8/.pre-commit-config.yaml` & `python-project-structure-0.8.9b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/.prospector.yaml` & `python-project-structure-0.8.9b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/CONTRIBUTING.rst` & `python-project-structure-0.8.9b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/Dockerfile` & `python-project-structure-0.8.9b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/Dockerfile.devel` & `python-project-structure-0.8.9b0/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/LICENSE` & `python-project-structure-0.8.9b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/Makefile` & `python-project-structure-0.8.9b0/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/NEWS.rst` & `python-project-structure-0.8.9b0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+python-project-structure 0.8.9b0 (2023-04-12)
+=============================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
 python-project-structure 0.8.8 (2023-04-11)
 ===========================================
 
 No significant changes.
 
 
 python-project-structure 0.8.8b0 (2023-04-11)
```

### Comparing `python-project-structure-0.8.8/PKG-INFO` & `python-project-structure-0.8.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.8
+Version: 0.8.9b0
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.8/README.rst` & `python-project-structure-0.8.9b0/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/TODO.rst` & `python-project-structure-0.8.9b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/bin/cz-check-bump` & `python-project-structure-0.8.9b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/bin/entrypoint` & `python-project-structure-0.8.9b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/bin/get-base-version` & `python-project-structure-0.8.9b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/Dockerfile` & `python-project-structure-0.8.9b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/Makefile` & `python-project-structure-0.8.9b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/README.rst` & `python-project-structure-0.8.9b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/bin/entrypoint` & `python-project-structure-0.8.9b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/requirements-py310.txt` & `python-project-structure-0.8.9b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/requirements-py311.txt` & `python-project-structure-0.8.9b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/requirements-py37.txt` & `python-project-structure-0.8.9b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/requirements-py38.txt` & `python-project-structure-0.8.9b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/build-host/requirements-py39.txt` & `python-project-structure-0.8.9b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/docker-compose.override.yml` & `python-project-structure-0.8.9b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/docker-compose.yml` & `python-project-structure-0.8.9b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/gitlab-runner/config/config.toml.in` & `python-project-structure-0.8.9b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/pyproject.toml` & `python-project-structure-0.8.9b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.8"
+version = "0.8.9b0"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
 """
```

### Comparing `python-project-structure-0.8.8/requirements/build.txt.in` & `python-project-structure-0.8.9b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py310/build.txt` & `python-project-structure-0.8.9b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py310/devel.txt` & `python-project-structure-0.8.9b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py311/build.txt` & `python-project-structure-0.8.9b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py311/devel.txt` & `python-project-structure-0.8.9b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py37/build.txt` & `python-project-structure-0.8.9b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py37/devel.txt` & `python-project-structure-0.8.9b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py38/build.txt` & `python-project-structure-0.8.9b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py38/devel.txt` & `python-project-structure-0.8.9b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py39/build.txt` & `python-project-structure-0.8.9b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/requirements/py39/devel.txt` & `python-project-structure-0.8.9b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/setup.cfg` & `python-project-structure-0.8.9b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/src/python_project_structure.egg-info/PKG-INFO` & `python-project-structure-0.8.9b0/src/python_project_structure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-project-structure
-Version: 0.8.8
+Version: 0.8.9b0
 Summary: Python project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/python-project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-project-structure-0.8.8/src/python_project_structure.egg-info/SOURCES.txt` & `python-project-structure-0.8.9b0/src/python_project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/src/pythonprojectstructure/__init__.py` & `python-project-structure-0.8.9b0/src/pythonprojectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/src/pythonprojectstructure/tests/test_cli.py` & `python-project-structure-0.8.9b0/src/pythonprojectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-project-structure-0.8.8/tox.ini` & `python-project-structure-0.8.9b0/tox.ini`

 * *Files identical despite different names*

