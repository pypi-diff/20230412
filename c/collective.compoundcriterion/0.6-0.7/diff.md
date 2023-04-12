# Comparing `tmp/collective.compoundcriterion-0.6.tar.gz` & `tmp/collective.compoundcriterion-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.compoundcriterion-0.6.tar", last modified: Mon Feb 13 11:06:15 2023, max compression
+gzip compressed data, was "dist/collective.compoundcriterion-0.7.tar", last modified: Wed Apr 12 09:00:59 2023, max compression
```

## Comparing `collective.compoundcriterion-0.6.tar` & `collective.compoundcriterion-0.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/
--rw-rw-r--   0 sge       (1000) sge       (1000)      140 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/.coveragerc
--rw-rw-r--   0 sge       (1000) sge       (1000)      131 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/.isort.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1477 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       81 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      478 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     5240 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     3098 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       48 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/buildout.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/buildout.d/
--rw-rw-r--   0 sge       (1000) sge       (1000)      599 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/buildout.d/base.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)       51 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/buildout.d/checkouts.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      649 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/buildout.d/development.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      522 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/buildout.d/sources.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      261 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/buildout.d/versions.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      197 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/ci.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/docs/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      732 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/docs/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/requirements.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1569 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/setup.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)      244 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/
--rw-rw-r--   0 sge       (1000) sge       (1000)      233 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1871 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/adapters.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2324 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)      447 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/interfaces.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/
--rw-rw-r--   0 sge       (1000) sge       (1000)      912 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/collective.compoundcriterion.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/es/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/es/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1197 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/es/LC_MESSAGES/collective.compoundcriterion.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)      845 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/fr/LC_MESSAGES/collective.compoundcriterion.po
--rwxrwxr-x   0 sge       (1000) sge       (1000)      152 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/update.sh
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      184 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/default/browserlayer.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/default/collectivecompoundcriterion_marker.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       67 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1228 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/default/registry.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/testing/
--rw-rw-r--   0 sge       (1000) sge       (1000)      232 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/testing/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1256 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2209 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/queryparser.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      253 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2516 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2132 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/testing.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1319 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/adapter.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/robot/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/robot/.gitkeep
--rw-rw-r--   0 sge       (1000) sge       (1000)    10545 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/test_criterion.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      633 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/test_robot.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1315 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/test_setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      987 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective/compoundcriterion/vocabularies.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-02-13 11:06:15.364507 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     5240 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     2191 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       53 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      126 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2023-02-13 11:06:15.000000 collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/top_level.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       53 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/entry_points.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/namespace_packages.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       11 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/top_level.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6776 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2191 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        1 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/not-zip-safe
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      126 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/requires.txt
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      253 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/setuphandlers.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2324 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/configure.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1887 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/adapters.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/es/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1197 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/es/LC_MESSAGES/collective.compoundcriterion.po
+-rwxrwxr-x   0 gbastien  (1000) gbastien  (1000)      152 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/update.sh
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      912 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/collective.compoundcriterion.pot
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/fr/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      845 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/fr/LC_MESSAGES/collective.compoundcriterion.po
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/testing/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      232 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/testing/metadata.xml
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/default/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      184 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/default/browserlayer.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       67 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/default/metadata.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1228 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/default/registry.xml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/default/collectivecompoundcriterion_marker.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2516 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/testing.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      447 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/interfaces.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2132 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/testing.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      987 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/vocabularies.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1319 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/adapter.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    11753 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/test_criterion.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/robot/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/robot/.gitkeep
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      633 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/test_robot.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1315 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/test_setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      233 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/__init__.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     2209 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/queryparser.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1256 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles.zcml
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      244 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/src/collective/__init__.py
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/docs/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      732 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/docs/LICENSE.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)    18092 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/docs/LICENSE.GPL
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       56 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/requirements.txt
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1684 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/setup.py
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     6776 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/PKG-INFO
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      478 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/MANIFEST.in
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     1653 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/CHANGES.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       81 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/CONTRIBUTORS.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)     3146 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/README.rst
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      140 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/.coveragerc
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      131 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/.isort.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       38 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/setup.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       48 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/buildout.cfg
+drwxrwxr-x   0 gbastien  (1000) gbastien  (1000)        0 2023-04-12 09:00:59.000000 collective.compoundcriterion-0.7/buildout.d/
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)       51 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/buildout.d/checkouts.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      261 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/buildout.d/versions.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      599 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/buildout.d/base.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      522 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/buildout.d/sources.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      649 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/buildout.d/development.cfg
+-rw-rw-r--   0 gbastien  (1000) gbastien  (1000)      197 2023-04-12 09:00:58.000000 collective.compoundcriterion-0.7/ci.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `collective.compoundcriterion-0.6/CHANGES.rst` & `collective.compoundcriterion-0.7/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+0.7 (2023-04-12)
+----------------
+
+- Do not break in `negative-previous-index` when some filters does not have
+  values (so the `'v'` is not there in the query).
+  [gbastien]
+
 0.6 (2023-02-13)
 ----------------
 
 - Added `negative-previous-index` and `negative-personal-labels` default adapters.
   Rely on `imio.helpers`. Removed dependency on `unittest2`.
   [gbastien]
```

### Comparing `collective.compoundcriterion-0.6/README.rst` & `collective.compoundcriterion-0.7/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ============================
 collective.compoundcriterion
 ============================
 
-.. image:: https://secure.travis-ci.org/collective/collective.compoundcriterion.png
-   :target: http://travis-ci.org/collective/collective.compoundcriterion
+.. image:: https://github.com/collective/collective.compoundcriterion/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/collective/collective.compoundcriterion/actions/workflows/main.yml
 
 .. image:: https://coveralls.io/repos/collective/collective.compoundcriterion/badge.svg?branch=master&service=github
   :target: https://coveralls.io/github/collective/collective.compoundcriterion?branch=master
 
 
 This package add a new kind of criterion available for plone.app.collection.
```

### Comparing `collective.compoundcriterion-0.6/buildout.d/base.cfg` & `collective.compoundcriterion-0.7/buildout.d/base.cfg`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/buildout.d/development.cfg` & `collective.compoundcriterion-0.7/buildout.d/development.cfg`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/buildout.d/sources.cfg` & `collective.compoundcriterion-0.7/buildout.d/sources.cfg`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/docs/LICENSE.GPL` & `collective.compoundcriterion-0.7/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/docs/LICENSE.rst` & `collective.compoundcriterion-0.7/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/setup.py` & `collective.compoundcriterion-0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 long_description = (
     open('README.rst').read() + '\n' +
     'Contributors\n============\n' + '\n' + open('CONTRIBUTORS.rst').read() +
     '\n' + open('CHANGES.rst').read() + '\n')
 
 setup(
     name='collective.compoundcriterion',
-    version='0.6',
+    version='0.7',
     description="Compound criterion for plone.app.collection managing complex query",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
+        "Development Status :: 6 - Mature",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
+        "License :: OSI Approved :: GNU General Public License (GPL)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
     ],
     keywords='Plone collection criterion',
     author='IMIO',
     author_email='support@imio.be',
     url='http://pypi.python.org/pypi/collective.compoundcriterion',
```

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/adapters.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,21 @@
            negativize values.  So for example, if previous index is portal_type,
            values are negativized, elements with none of the defined portal_type
            will be found.'''
         # get previous index
         previous = None
         for value in self.context.query:
             if value[u'i'] == u'CompoundCriterion' and \
-               self._adapter_name in value[u'v']:
+               self._adapter_name in value.get(u'v', []):
                 break
             previous = value
 
         query = {}
         if previous:
-            query[previous[u'i']] = {'not': previous[u'v']}
+            query[previous[u'i']] = {'not': previous.get(u'v', [])}
         return query
 
 
 class NegativePersonalLabelsAdapter(object):
 
     def __init__(self, context):
         self.context = context
```

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/configure.zcml` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/collective.compoundcriterion.pot` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/collective.compoundcriterion.pot`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/es/LC_MESSAGES/collective.compoundcriterion.po` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/es/LC_MESSAGES/collective.compoundcriterion.po`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/locales/fr/LC_MESSAGES/collective.compoundcriterion.po` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/locales/fr/LC_MESSAGES/collective.compoundcriterion.po`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles/default/registry.xml` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/profiles.zcml` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/queryparser.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/queryparser.py`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/testing.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/testing.py`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/testing.zcml` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/testing.zcml`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/adapter.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/adapter.py`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/test_criterion.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/test_criterion.py`

 * *Files 7% similar despite different names*

```diff
@@ -229,14 +229,41 @@
             query=query,
             sort_on='getId')
         collection = self.portal['collection']
         # the portal_type was negativized
         self.assertEqual(
             parseFormquery(collection, collection.query),
             {'portal_type': {'not': ['Document']}})
+        # does not break with query without 'v'
+        query[0].pop('v')
+        collection.setQuery(query)
+        self.assertEqual(
+            parseFormquery(collection, collection.query),
+            {'portal_type': {'not': []}})
+        # when several filters and one is empty
+        query = [
+            {
+                'i': 'CompoundCriterion',
+                'o': 'plone.app.querystring.operation.compound.is',
+            },
+            {
+                'i': 'portal_type',
+                'o': 'plone.app.querystring.operation.compound.is',
+                'v': ['Document'],
+            },
+            {
+                'i': 'CompoundCriterion',
+                'o': 'plone.app.querystring.operation.compound.is',
+                'v': ['negative-previous-index'],
+            },
+        ]
+        collection.setQuery(query)
+        self.assertEqual(
+            parseFormquery(collection, collection.query),
+            {'portal_type': {'not': ['Document']}})
 
     def test_negative_personal_labels_adapter(self):
         """The negative-personal-labels will result in a query with previous index
            "labels" having negativized and memberized values."""
         login(self.portal, TEST_USER_NAME)
         query = [
             {
@@ -258,7 +285,13 @@
             query=query,
             sort_on='getId')
         collection = self.portal['collection']
         # the portal_type was negativized
         self.assertEqual(
             parseFormquery(collection, collection.query),
             {'labels': {'not': ['test_user_1_:follow', 'test_user_1_:read']}})
+        # does not break with query without 'v'
+        query[0].pop('v')
+        collection.setQuery(query)
+        self.assertEqual(
+            parseFormquery(collection, collection.query),
+            {'labels': {'not': []}})
```

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/test_robot.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/tests/test_setup.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective/compoundcriterion/vocabularies.py` & `collective.compoundcriterion-0.7/src/collective/compoundcriterion/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.compoundcriterion-0.6/src/collective.compoundcriterion.egg-info/SOURCES.txt` & `collective.compoundcriterion-0.7/src/collective.compoundcriterion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

