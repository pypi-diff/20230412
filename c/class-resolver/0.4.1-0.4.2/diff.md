# Comparing `tmp/class_resolver-0.4.1.tar.gz` & `tmp/class_resolver-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_resolver-0.4.1.tar", last modified: Thu Apr  6 14:49:55 2023, max compression
+gzip compressed data, was "class_resolver-0.4.2.tar", last modified: Wed Apr 12 17:18:08 2023, max compression
```

## Comparing `class_resolver-0.4.1.tar` & `class_resolver-0.4.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.224177 class_resolver-0.4.1/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-03-13 12:44:09.000000 class_resolver-0.4.1/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      346 2022-03-13 12:44:09.000000 class_resolver-0.4.1/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)    12793 2023-04-06 14:49:55.224339 class_resolver-0.4.1/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)    11262 2022-03-13 12:44:09.000000 class_resolver-0.4.1/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.183683 class_resolver-0.4.1/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.189849 class_resolver-0.4.1/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.197236 class_resolver-0.4.1/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1110 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.BaseResolver.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     1690 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.ClassResolver.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     1174 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.FunctionResolver.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      118 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.KeywordArgumentError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.RegistrationError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.RegistrationNameConflict.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      139 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.RegistrationSynonymConflict.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     1570 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.Resolver.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.UnexpectedKeywordError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       78 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.get_cls.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       99 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.get_subclasses.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      105 2023-02-19 21:04:38.000000 class_resolver-0.4.1/docs/source/api/class_resolver.normalize_string.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7164 2023-04-06 14:49:54.000000 class_resolver-0.4.1/docs/source/conf.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.200292 class_resolver-0.4.1/docs/source/contrib/
--rw-r--r--   0 cthoyt     (501) staff       (20)      187 2023-02-21 22:29:06.000000 class_resolver-0.4.1/docs/source/contrib/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       71 2023-02-08 22:33:04.000000 class_resolver-0.4.1/docs/source/contrib/numpy.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       74 2022-03-13 12:44:09.000000 class_resolver-0.4.1/docs/source/contrib/optuna.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       87 2023-02-21 22:29:06.000000 class_resolver-0.4.1/docs/source/contrib/sklearn.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       75 2022-03-13 12:44:09.000000 class_resolver-0.4.1/docs/source/contrib/torch.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      331 2022-03-13 12:44:09.000000 class_resolver-0.4.1/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      539 2022-03-13 12:44:09.000000 class_resolver-0.4.1/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       67 2023-02-08 22:33:04.000000 class_resolver-0.4.1/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      358 2022-03-13 12:44:09.000000 class_resolver-0.4.1/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2692 2023-04-06 14:49:55.225375 class_resolver-0.4.1/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.184608 class_resolver-0.4.1/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.204177 class_resolver-0.4.1/src/class_resolver/
--rw-r--r--   0 cthoyt     (501) staff       (20)     2972 2023-02-08 22:33:04.000000 class_resolver-0.4.1/src/class_resolver/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13813 2023-02-19 20:43:34.000000 class_resolver-0.4.1/src/class_resolver/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    11254 2023-02-21 22:29:06.000000 class_resolver-0.4.1/src/class_resolver/base.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.210233 class_resolver-0.4.1/src/class_resolver/contrib/
--rw-r--r--   0 cthoyt     (501) staff       (20)      325 2023-02-19 20:53:52.000000 class_resolver-0.4.1/src/class_resolver/contrib/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1176 2023-02-08 22:33:04.000000 class_resolver-0.4.1/src/class_resolver/contrib/numpy.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2322 2022-03-13 12:44:09.000000 class_resolver-0.4.1/src/class_resolver/contrib/optuna.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2199 2023-02-21 22:29:06.000000 class_resolver-0.4.1/src/class_resolver/contrib/sklearn.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     7332 2023-04-06 14:49:37.000000 class_resolver-0.4.1/src/class_resolver/contrib/torch.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2258 2023-02-21 22:29:06.000000 class_resolver-0.4.1/src/class_resolver/contrib/torch_geometric.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1549 2023-02-19 20:43:34.000000 class_resolver-0.4.1/src/class_resolver/func.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        0 2022-03-13 12:44:09.000000 class_resolver-0.4.1/src/class_resolver/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     6070 2023-02-08 22:33:04.000000 class_resolver-0.4.1/src/class_resolver/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      127 2023-04-06 14:49:54.000000 class_resolver-0.4.1/src/class_resolver/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.207172 class_resolver-0.4.1/src/class_resolver.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)    12793 2023-04-06 14:49:55.000000 class_resolver-0.4.1/src/class_resolver.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     2464 2023-04-06 14:49:55.000000 class_resolver-0.4.1/src/class_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-04-06 14:49:55.000000 class_resolver-0.4.1/src/class_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)      129 2023-04-06 14:49:55.000000 class_resolver-0.4.1/src/class_resolver.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-03-13 12:44:53.000000 class_resolver-0.4.1/src/class_resolver.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      320 2023-04-06 14:49:55.000000 class_resolver-0.4.1/src/class_resolver.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       15 2023-04-06 14:49:55.000000 class_resolver-0.4.1/src/class_resolver.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.213497 class_resolver-0.4.1/tests/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.215560 class_resolver-0.4.1/tests/.pytest_cache/
--rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-02-07 21:00:24.000000 class_resolver-0.4.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-02-07 21:00:24.000000 class_resolver-0.4.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 cthoyt     (501) staff       (20)      302 2023-02-07 21:00:24.000000 class_resolver-0.4.1/tests/.pytest_cache/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.185402 class_resolver-0.4.1/tests/.pytest_cache/v/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.217396 class_resolver-0.4.1/tests/.pytest_cache/v/cache/
--rw-r--r--   0 cthoyt     (501) staff       (20)      111 2023-02-19 20:02:44.000000 class_resolver-0.4.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 cthoyt     (501) staff       (20)     3848 2023-02-21 22:57:19.000000 class_resolver-0.4.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-02-21 22:57:19.000000 class_resolver-0.4.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2022-03-13 12:44:09.000000 class_resolver-0.4.1/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2022-03-13 12:44:09.000000 class_resolver-0.4.1/tests/_private_extras.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    17352 2023-02-21 22:29:06.000000 class_resolver-0.4.1/tests/test_api.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.220164 class_resolver-0.4.1/tests/test_contrib/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.221867 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/
--rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-02-19 19:18:56.000000 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/.gitignore
--rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-02-19 19:18:56.000000 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 cthoyt     (501) staff       (20)      302 2023-02-19 19:18:56.000000 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.185998 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/v/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-06 14:49:55.223651 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/v/cache/
--rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-02-19 20:56:24.000000 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 cthoyt     (501) staff       (20)      173 2023-02-19 20:59:32.000000 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-02-19 20:59:32.000000 class_resolver-0.4.1/tests/test_contrib/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 cthoyt     (501) staff       (20)       58 2022-03-13 12:44:09.000000 class_resolver-0.4.1/tests/test_contrib/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      755 2023-02-08 22:33:04.000000 class_resolver-0.4.1/tests/test_contrib/test_numpy.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1212 2022-03-13 12:44:09.000000 class_resolver-0.4.1/tests/test_contrib/test_optuna.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1421 2023-02-21 22:29:06.000000 class_resolver-0.4.1/tests/test_contrib/test_sklearn.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2969 2022-03-13 12:44:09.000000 class_resolver-0.4.1/tests/test_contrib/test_torch.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1365 2023-02-21 22:29:06.000000 class_resolver-0.4.1/tests/test_contrib/test_torch_geometric.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3983 2023-02-19 20:43:34.000000 class_resolver-0.4.1/tests/test_function_resolver.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3725 2023-02-08 22:33:04.000000 class_resolver-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.248477 class_resolver-0.4.2/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-03-13 12:44:09.000000 class_resolver-0.4.2/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      346 2022-03-13 12:44:09.000000 class_resolver-0.4.2/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12793 2023-04-12 17:18:08.248713 class_resolver-0.4.2/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11262 2022-03-13 12:44:09.000000 class_resolver-0.4.2/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.210531 class_resolver-0.4.2/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.217150 class_resolver-0.4.2/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.223765 class_resolver-0.4.2/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1110 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.BaseResolver.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1690 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.ClassResolver.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1174 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.FunctionResolver.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      118 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.KeywordArgumentError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.RegistrationError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.RegistrationNameConflict.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      139 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.RegistrationSynonymConflict.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1570 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.Resolver.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.UnexpectedKeywordError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       78 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.get_cls.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       99 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.get_subclasses.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      105 2023-02-19 21:04:38.000000 class_resolver-0.4.2/docs/source/api/class_resolver.normalize_string.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7164 2023-04-12 17:18:07.000000 class_resolver-0.4.2/docs/source/conf.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.226351 class_resolver-0.4.2/docs/source/contrib/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      187 2023-02-21 22:29:06.000000 class_resolver-0.4.2/docs/source/contrib/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       71 2023-02-08 22:33:04.000000 class_resolver-0.4.2/docs/source/contrib/numpy.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       74 2022-03-13 12:44:09.000000 class_resolver-0.4.2/docs/source/contrib/optuna.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       87 2023-02-21 22:29:06.000000 class_resolver-0.4.2/docs/source/contrib/sklearn.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       75 2022-03-13 12:44:09.000000 class_resolver-0.4.2/docs/source/contrib/torch.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      331 2022-03-13 12:44:09.000000 class_resolver-0.4.2/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      539 2022-03-13 12:44:09.000000 class_resolver-0.4.2/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       67 2023-02-08 22:33:04.000000 class_resolver-0.4.2/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      358 2022-03-13 12:44:09.000000 class_resolver-0.4.2/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2761 2023-04-12 17:18:08.249928 class_resolver-0.4.2/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.211506 class_resolver-0.4.2/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.229115 class_resolver-0.4.2/src/class_resolver/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2972 2023-02-08 22:33:04.000000 class_resolver-0.4.2/src/class_resolver/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13836 2023-04-12 06:26:59.000000 class_resolver-0.4.2/src/class_resolver/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11380 2023-04-12 17:16:40.000000 class_resolver-0.4.2/src/class_resolver/base.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.234192 class_resolver-0.4.2/src/class_resolver/contrib/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      325 2023-02-19 20:53:52.000000 class_resolver-0.4.2/src/class_resolver/contrib/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1176 2023-02-08 22:33:04.000000 class_resolver-0.4.2/src/class_resolver/contrib/numpy.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2322 2022-03-13 12:44:09.000000 class_resolver-0.4.2/src/class_resolver/contrib/optuna.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2199 2023-02-21 22:29:06.000000 class_resolver-0.4.2/src/class_resolver/contrib/sklearn.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7401 2023-04-12 17:16:27.000000 class_resolver-0.4.2/src/class_resolver/contrib/torch.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2258 2023-02-21 22:29:06.000000 class_resolver-0.4.2/src/class_resolver/contrib/torch_geometric.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1549 2023-02-19 20:43:34.000000 class_resolver-0.4.2/src/class_resolver/func.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        0 2022-03-13 12:44:09.000000 class_resolver-0.4.2/src/class_resolver/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6070 2023-02-08 22:33:04.000000 class_resolver-0.4.2/src/class_resolver/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      127 2023-04-12 17:18:07.000000 class_resolver-0.4.2/src/class_resolver/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.231943 class_resolver-0.4.2/src/class_resolver.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12793 2023-04-12 17:18:08.000000 class_resolver-0.4.2/src/class_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2464 2023-04-12 17:18:08.000000 class_resolver-0.4.2/src/class_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-04-12 17:18:08.000000 class_resolver-0.4.2/src/class_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)      129 2023-04-12 17:18:08.000000 class_resolver-0.4.2/src/class_resolver.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-03-13 12:44:53.000000 class_resolver-0.4.2/src/class_resolver.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      371 2023-04-12 17:18:08.000000 class_resolver-0.4.2/src/class_resolver.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       15 2023-04-12 17:18:08.000000 class_resolver-0.4.2/src/class_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.237396 class_resolver-0.4.2/tests/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.239303 class_resolver-0.4.2/tests/.pytest_cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-02-07 21:00:24.000000 class_resolver-0.4.2/tests/.pytest_cache/.gitignore
+-rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-02-07 21:00:24.000000 class_resolver-0.4.2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 cthoyt     (501) staff       (20)      302 2023-02-07 21:00:24.000000 class_resolver-0.4.2/tests/.pytest_cache/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.212450 class_resolver-0.4.2/tests/.pytest_cache/v/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.241068 class_resolver-0.4.2/tests/.pytest_cache/v/cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      111 2023-04-12 06:52:17.000000 class_resolver-0.4.2/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3848 2023-04-12 07:23:04.000000 class_resolver-0.4.2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-04-12 07:23:04.000000 class_resolver-0.4.2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2022-03-13 12:44:09.000000 class_resolver-0.4.2/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2022-03-13 12:44:09.000000 class_resolver-0.4.2/tests/_private_extras.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    17352 2023-02-21 22:29:06.000000 class_resolver-0.4.2/tests/test_api.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.243946 class_resolver-0.4.2/tests/test_contrib/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.245813 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-02-19 19:18:56.000000 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/.gitignore
+-rw-r--r--   0 cthoyt     (501) staff       (20)      191 2023-02-19 19:18:56.000000 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 cthoyt     (501) staff       (20)      302 2023-02-19 19:18:56.000000 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.213165 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/v/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-04-12 17:18:08.247823 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/v/cache/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       37 2023-02-19 20:56:24.000000 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 cthoyt     (501) staff       (20)      173 2023-02-19 20:59:32.000000 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 cthoyt     (501) staff       (20)        2 2023-02-19 20:59:32.000000 class_resolver-0.4.2/tests/test_contrib/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 cthoyt     (501) staff       (20)       58 2022-03-13 12:44:09.000000 class_resolver-0.4.2/tests/test_contrib/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      755 2023-02-08 22:33:04.000000 class_resolver-0.4.2/tests/test_contrib/test_numpy.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1212 2022-03-13 12:44:09.000000 class_resolver-0.4.2/tests/test_contrib/test_optuna.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1421 2023-02-21 22:29:06.000000 class_resolver-0.4.2/tests/test_contrib/test_sklearn.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2969 2022-03-13 12:44:09.000000 class_resolver-0.4.2/tests/test_contrib/test_torch.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1365 2023-02-21 22:29:06.000000 class_resolver-0.4.2/tests/test_contrib/test_torch_geometric.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3983 2023-02-19 20:43:34.000000 class_resolver-0.4.2/tests/test_function_resolver.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3725 2023-02-08 22:33:04.000000 class_resolver-0.4.2/tests/test_utils.py
```

### Comparing `class_resolver-0.4.1/LICENSE` & `class_resolver-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/PKG-INFO` & `class_resolver-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: class_resolver
-Version: 0.4.1
+Version: 0.4.2
 Summary: Lookup and instantiate classes with style.
 Home-page: https://github.com/cthoyt/class-resolver
 Download-URL: https://github.com/cthoyt/class-resolver/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

### Comparing `class_resolver-0.4.1/README.md` & `class_resolver-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/docs/source/api/class_resolver.BaseResolver.rst` & `class_resolver-0.4.2/docs/source/api/class_resolver.BaseResolver.rst`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/docs/source/api/class_resolver.ClassResolver.rst` & `class_resolver-0.4.2/docs/source/api/class_resolver.ClassResolver.rst`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/docs/source/api/class_resolver.FunctionResolver.rst` & `class_resolver-0.4.2/docs/source/api/class_resolver.FunctionResolver.rst`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/docs/source/api/class_resolver.Resolver.rst` & `class_resolver-0.4.2/docs/source/api/class_resolver.Resolver.rst`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/docs/source/conf.py` & `class_resolver-0.4.2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'class_resolver'
 copyright = f'{date.today().year}, Charles Tapley Hoyt'
 author = 'Charles Tapley Hoyt'
 
 # The full version, including alpha/beta/rc tags.
-release = '0.4.1'
+release = '0.4.2'
 
 # The short X.Y version.
 parsed_version = re.match(
     '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?',
     release,
 )
 version = parsed_version.expand('\g<major>.\g<minor>.\g<patch>')
```

### Comparing `class_resolver-0.4.1/docs/source/installation.rst` & `class_resolver-0.4.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/setup.cfg` & `class_resolver-0.4.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = class_resolver
-version = 0.4.1
+version = 0.4.2
 description = Lookup and instantiate classes with style.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/class-resolver
 download_url = https://github.com/cthoyt/class-resolver/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/class-resolver/issues
@@ -35,14 +35,16 @@
 	development tool
 	configurability
 
 [options]
 zip_safe = false
 include_package_data = True
 python_requires = >=3.7
+install_requires = 
+	importlib-metadata > 3.6; python_version<"3.10"
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
```

### Comparing `class_resolver-0.4.1/src/class_resolver/__init__.py` & `class_resolver-0.4.2/src/class_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/src/class_resolver/api.py` & `class_resolver-0.4.2/src/class_resolver/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,14 @@
         if key in lookup_dict:
             return lookup_dict[key]
         elif lookup_dict_synonyms is not None and key in lookup_dict_synonyms:
             return lookup_dict_synonyms[key]
         else:
             valid_choices = sorted(set(lookup_dict.keys()).union(lookup_dict_synonyms or []))
             raise KeyError(
-                f"Invalid {base.__name__} name: {query}. Valid choices are: {valid_choices}"
+                f"Invalid {base.__name__} name: {query} (normalized to: {key}). Valid choices are: {valid_choices}"
             )
     elif isinstance(query, base):
         return query.__class__
     elif isinstance(query, type) and issubclass(query, base):
         return query
     raise TypeError(f"Not subclass of {base.__name__}: {query}")
```

### Comparing `class_resolver-0.4.1/src/class_resolver/base.py` & `class_resolver-0.4.2/src/class_resolver/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
 
 """A base resolver."""
 
 import logging
+import sys
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Collection,
     Dict,
     Generic,
     Iterable,
     Iterator,
     Mapping,
     Optional,
     Set,
 )
 
-from pkg_resources import iter_entry_points
+if sys.version_info[:2] >= (3, 10):
+    from importlib.metadata import entry_points
+else:
+    from importlib_metadata import entry_points
 
 from .utils import Hint, OptionalKwargs, X, Y, make_callback, normalize_string
 
 if TYPE_CHECKING:
     import optuna
 
 __all__ = [
@@ -255,19 +259,19 @@
     def register_entrypoint(self, group: str) -> None:
         """Register additional entries from an entrypoint."""
         for element in self._from_entrypoint(group).difference(self.lookup_dict.values()):
             self.register(element)
 
     @staticmethod
     def _from_entrypoint(group: str) -> Set[X]:
-        elements = set()
-        for entry in iter_entry_points(group=group):
+        elements: Set[X] = set()
+        for entry in entry_points(group=group):
             try:
                 element = entry.load()
-            except ImportError:
+            except (ImportError, AttributeError):
                 logger.warning("could not load %s", entry.name)
             else:
                 elements.add(element)
         return elements
 
     @classmethod
     def from_entrypoint(cls, group: str, **kwargs) -> "BaseResolver":
```

### Comparing `class_resolver-0.4.1/src/class_resolver/contrib/numpy.py` & `class_resolver-0.4.2/src/class_resolver/contrib/numpy.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/src/class_resolver/contrib/optuna.py` & `class_resolver-0.4.2/src/class_resolver/contrib/optuna.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/src/class_resolver/contrib/sklearn.py` & `class_resolver-0.4.2/src/class_resolver/contrib/sklearn.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/src/class_resolver/contrib/torch.py` & `class_resolver-0.4.2/src/class_resolver/contrib/torch.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,37 @@
 )
 """A resolver for :class:`torch.optim.Optimizer` classes.
 
 .. code-block:: python
 
     from class_resolver import Hint, OptionalKwargs
     from class_resolver.contrib.torch import optimizer_resolver
-    from torch import Parameter
+    from torch import Parameter, nn
     from torch.optim import Optimizer
 
-    def train(optimizer: Hint[Optimizer] = "adam", optimizer_kwargs: OptionalKwargs = None):
-        model = [Parameter(torch.randn(2, 2, requires_grad=True))]
-        optimizer = optimizer_resolver.make(optimizer, optimizer_kwargs, model=model)
+    dataset = ...
+
+    def train(
+        model: nn.Module,
+        optimizer: Hint[Optimizer] = "adam",
+        optimizer_kwargs: OptionalKwargs = None,
+    ):
+        optimizer = optimizer_resolver.make(
+            optimizer, optimizer_kwargs, params=model.parameters(),
+        )
 
         for epoch in range(20):
             for input, target in dataset:
                 optimizer.zero_grad()
                 output = model(input)
                 loss = loss_fn(output, target)
                 loss.backward()
                 optimizer.step()
 
         return model
-
 """
 
 ACTIVATION_SKIP = {
     activation.MultiheadAttention,
     activation.Softmax2d,
 }
 
@@ -174,21 +180,26 @@
 the following example shows how a training loop can be first turned into a funciton
 then parametrized to accept a LRScheduler hint.
 
 .. code-block:: python
 
     from class_resolver import Hint, OptionalKwargs
     from class_resolver.contrib.torch import lr_scheduler_resolver
-    from torch import Parameter
+    from torch import Parameter, nn
     from torch.optim import SGD
     from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 
-    def train(scheduler: Hint[LRScheduler] = "exponential", scheduler_kwargs: OptionalKwargs = None):
-        model = [Parameter(torch.randn(2, 2, requires_grad=True))]
-        optimizer = SGD(model, 0.1)
+    dataset = ...
+
+    def train(
+        model: nn.Module,
+        scheduler: Hint[LRScheduler] = "exponential",
+        scheduler_kwargs: OptionalKwargs = None,
+    ):
+        optimizer = SGD(params=model.parameters(), lr=0.1)
         scheduler = lr_scheduler_resolver.make(scheduler, scheduler_kwargs, optimizer=optimizer)
 
         for epoch in range(20):
             for input, target in dataset:
                 optimizer.zero_grad()
                 output = model(input)
                 loss = loss_fn(output, target)
```

### Comparing `class_resolver-0.4.1/src/class_resolver/contrib/torch_geometric.py` & `class_resolver-0.4.2/src/class_resolver/contrib/torch_geometric.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/src/class_resolver/func.py` & `class_resolver-0.4.2/src/class_resolver/func.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/src/class_resolver/utils.py` & `class_resolver-0.4.2/src/class_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/src/class_resolver.egg-info/PKG-INFO` & `class_resolver-0.4.2/src/class_resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: class-resolver
-Version: 0.4.1
+Version: 0.4.2
 Summary: Lookup and instantiate classes with style.
 Home-page: https://github.com/cthoyt/class-resolver
 Download-URL: https://github.com/cthoyt/class-resolver/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

### Comparing `class_resolver-0.4.1/src/class_resolver.egg-info/SOURCES.txt` & `class_resolver-0.4.2/src/class_resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/.pytest_cache/v/cache/nodeids` & `class_resolver-0.4.2/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_api.py` & `class_resolver-0.4.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_contrib/test_numpy.py` & `class_resolver-0.4.2/tests/test_contrib/test_numpy.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_contrib/test_optuna.py` & `class_resolver-0.4.2/tests/test_contrib/test_optuna.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_contrib/test_sklearn.py` & `class_resolver-0.4.2/tests/test_contrib/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_contrib/test_torch.py` & `class_resolver-0.4.2/tests/test_contrib/test_torch.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_contrib/test_torch_geometric.py` & `class_resolver-0.4.2/tests/test_contrib/test_torch_geometric.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_function_resolver.py` & `class_resolver-0.4.2/tests/test_function_resolver.py`

 * *Files identical despite different names*

### Comparing `class_resolver-0.4.1/tests/test_utils.py` & `class_resolver-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

