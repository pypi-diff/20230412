# Comparing `tmp/pdfstitcher-0.8.5.tar.gz` & `tmp/pdfstitcher-0.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfstitcher-0.8.5.tar", last modified: Wed Apr 12 19:04:50 2023, max compression
+gzip compressed data, was "pdfstitcher-0.8b1.tar", last modified: Thu Feb 16 23:39:23 2023, max compression
```

## Comparing `pdfstitcher-0.8.5.tar` & `pdfstitcher-0.8b1.tar`

### file list

```diff
@@ -1,91 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.507093 pdfstitcher-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-04-12 19:04:50.507093 pdfstitcher-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.495092 pdfstitcher-0.8.5/pdfstitcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/bug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/layerfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.487092 pdfstitcher-0.8.5/pdfstitcher/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.487092 pdfstitcher-0.8.5/pdfstitcher/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    18724 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.487092 pdfstitcher-0.8.5/pdfstitcher/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.487092 pdfstitcher-0.8.5/pdfstitcher/locale/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    21711 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.487092 pdfstitcher-0.8.5/pdfstitcher/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.487092 pdfstitcher-0.8.5/pdfstitcher/locale/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19252 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/nb_NO/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.499092 pdfstitcher-0.8.5/pdfstitcher/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.503093 pdfstitcher-0.8.5/pdfstitcher/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.503093 pdfstitcher-0.8.5/pdfstitcher/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.503093 pdfstitcher-0.8.5/pdfstitcher/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.503093 pdfstitcher-0.8.5/pdfstitcher/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.491093 pdfstitcher-0.8.5/pdfstitcher/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.503093 pdfstitcher-0.8.5/pdfstitcher/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 19:04:37.000000 pdfstitcher-0.8.5/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.mo
--rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.po
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/pagefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/pdf_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.503093 pdfstitcher-0.8.5/pdfstitcher/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   342175 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/resources/stitcher-icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/tile_pages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.503093 pdfstitcher-0.8.5/pdfstitcher/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16454 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/ui/io_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/ui/layers_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/ui/main_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/ui/tile_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/update_loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pdfstitcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.495092 pdfstitcher-0.8.5/pdfstitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23072 2023-04-12 19:04:50.000000 pdfstitcher-0.8.5/pdfstitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-12 19:04:50.000000 pdfstitcher-0.8.5/pdfstitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:04:50.000000 pdfstitcher-0.8.5/pdfstitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 19:04:50.000000 pdfstitcher-0.8.5/pdfstitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 19:04:50.000000 pdfstitcher-0.8.5/pdfstitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 19:04:50.000000 pdfstitcher-0.8.5/pdfstitcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:04:50.507093 pdfstitcher-0.8.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:04:50.507093 pdfstitcher-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 19:03:15.000000 pdfstitcher-0.8.5/tests/test_tile_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/bug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/layerfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/cs_CZ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/nb_NO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/pdfstitcher/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/pdfstitcher/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.412699 pdfstitcher-0.8b1/pdfstitcher/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/pdfstitcher/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-16 23:39:12.000000 pdfstitcher-0.8b1/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/pagefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/pdf_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/pdfstitcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/pdfstitcher/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   342175 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/resources/stitcher-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/tile_pages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/pdfstitcher/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15558 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/ui/io_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/ui/layers_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18459 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/ui/main_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/ui/tile_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/update_loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pdfstitcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 23:39:23.416699 pdfstitcher-0.8b1/pdfstitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-02-16 23:39:23.000000 pdfstitcher-0.8b1/pdfstitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-16 23:39:23.000000 pdfstitcher-0.8b1/pdfstitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 23:39:23.000000 pdfstitcher-0.8b1/pdfstitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-16 23:39:23.000000 pdfstitcher-0.8b1/pdfstitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-16 23:39:23.000000 pdfstitcher-0.8b1/pdfstitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-16 23:39:23.000000 pdfstitcher-0.8b1/pdfstitcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 23:39:23.420699 pdfstitcher-0.8b1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-02-16 23:38:27.000000 pdfstitcher-0.8b1/setup.py
```

### Comparing `pdfstitcher-0.8.5/LICENSE` & `pdfstitcher-0.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/PKG-INFO` & `pdfstitcher-0.8b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfstitcher
-Version: 0.8.5
+Version: 0.8b1
 Summary: The open source PDF stitching software for sewists, by sewists.
 Author: Charlotte Curtis
 Author-email: c.f.curtis@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
@@ -394,18 +394,17 @@
 
 Since version 0.4, it is also possible to select layers for inclusion/exclusion in the final output. Additionally, line properties can be modified for each layer if the input PDF is compatible.
 
 For up-to-date information, also check out https://www.pdfstitcher.org.
 
 ## Download the latest release
 * [Windows (7 or 10, 64-bit)](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/pdfstitcher.exe)
-* [macOS - Intel Processor](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-InstallerX64.dmg)
-* [macOS - M1/M2 Processor](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-InstallerARM64.dmg)
+* [macOS (High Sierra or higher)](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-Installer.dmg)
 * <a href='https://flathub.org/apps/details/com.github.cfcurtis.pdfstitcher'><img width='120' alt='Download on Flathub' src='https://flathub.org/assets/badges/flathub-badge-en.svg'/></a>
-* Using pip: `pip install pdfstitcher` **Note: Requires Python <= 3.11**. As of November 2022, there is no wheel available for wxPython for 3.11+.
+* Using pip: `pip install pdfstitcher` **Note: Requires Python <= 3.9.13**. As of February 2022, there is no wheel available for wxPython for 3.10.
 
 ## Translations:
 
 <a href="https://hosted.weblate.org/engage/pdfstitcher/">
 <img src="https://hosted.weblate.org/widgets/pdfstitcher/-/287x66-grey.png" alt="Translation status" /></a>
 
 PDFStitcher will detect system language settings and change localisation if supported. 
@@ -424,12 +423,12 @@
 * Exclude layers (either deactivate or remove)
 * Modify line properties (colour, thickness, style (solid, dashed, dotted))
 
 ## Development Installation
 Most people probably want to just use the executable links above. However, to edit the code, clone this repo and install in editable mode using the command:
 
 ```console
-$ pip install -e ".[dev]"
+$ pip install -e .
 ```
 
 ## Help!
 Found a bug, or have an idea for a great new feature? Check out the [Issues](https://github.com/cfcurtis/pdfstitcher/issues) tab to see if it's an open issue, or submit a new one if it's not on the list.
```

### Comparing `pdfstitcher-0.8.5/README.md` & `pdfstitcher-0.8b1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 Since version 0.4, it is also possible to select layers for inclusion/exclusion in the final output. Additionally, line properties can be modified for each layer if the input PDF is compatible.
 
 For up-to-date information, also check out https://www.pdfstitcher.org.
 
 ## Download the latest release
 * [Windows (7 or 10, 64-bit)](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/pdfstitcher.exe)
-* [macOS - Intel Processor](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-InstallerX64.dmg)
-* [macOS - M1/M2 Processor](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-InstallerARM64.dmg)
+* [macOS (High Sierra or higher)](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-Installer.dmg)
 * <a href='https://flathub.org/apps/details/com.github.cfcurtis.pdfstitcher'><img width='120' alt='Download on Flathub' src='https://flathub.org/assets/badges/flathub-badge-en.svg'/></a>
-* Using pip: `pip install pdfstitcher` **Note: Requires Python <= 3.11**. As of November 2022, there is no wheel available for wxPython for 3.11+.
+* Using pip: `pip install pdfstitcher` **Note: Requires Python <= 3.9.13**. As of February 2022, there is no wheel available for wxPython for 3.10.
 
 ## Translations:
 
 <a href="https://hosted.weblate.org/engage/pdfstitcher/">
 <img src="https://hosted.weblate.org/widgets/pdfstitcher/-/287x66-grey.png" alt="Translation status" /></a>
 
 PDFStitcher will detect system language settings and change localisation if supported. 
@@ -33,12 +32,12 @@
 * Exclude layers (either deactivate or remove)
 * Modify line properties (colour, thickness, style (solid, dashed, dotted))
 
 ## Development Installation
 Most people probably want to just use the executable links above. However, to edit the code, clone this repo and install in editable mode using the command:
 
 ```console
-$ pip install -e ".[dev]"
+$ pip install -e .
 ```
 
 ## Help!
 Found a bug, or have an idea for a great new feature? Check out the [Issues](https://github.com/cfcurtis/pdfstitcher/issues) tab to see if it's an open issue, or submit a new one if it's not on the list.
```

#### html2text {}

```diff
@@ -3,30 +3,28 @@
 imposition. This program was created in order to convert sewing patterns into a
 convenient format for projecting, though it could be used to stitch together
 any PDF. Since version 0.4, it is also possible to select layers for inclusion/
 exclusion in the final output. Additionally, line properties can be modified
 for each layer if the input PDF is compatible. For up-to-date information, also
 check out https://www.pdfstitcher.org. ## Download the latest release *
 [Windows (7 or 10, 64-bit)](https://github.com/cfcurtis/pdfstitcher/releases/
-latest/download/pdfstitcher.exe) * [macOS - Intel Processor](https://
+latest/download/pdfstitcher.exe) * [macOS (High Sierra or higher)](https://
 github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-
-InstallerX64.dmg) * [macOS - M1/M2 Processor](https://github.com/cfcurtis/
-pdfstitcher/releases/latest/download/PDFStitcher-InstallerARM64.dmg) *
-[Download_on_Flathub] * Using pip: `pip install pdfstitcher` **Note: Requires
-Python <= 3.11**. As of November 2022, there is no wheel available for wxPython
-for 3.11+. ## Translations: [Translation_status] PDFStitcher will detect system
-language settings and change localisation if supported. Previous versions can
-be found by clicking on the "releases" link to the right. Want to contribute a
-translation? PDFStitcher is now on [weblate!](https://hosted.weblate.org/
-engage/pdfstitcher/). ## Features * Stitch together pages in any order with
-specified number of rows/columns * Rotate pages for stitching * Add a margin
-around the final output * Trim or overlap the edges of each page by a specified
-amount * Add blank pages by including zeros in the page list (e.g. 1-5,0,6-10)
-* Layers are automatically preserved if present in the source document *
-Exclude layers (either deactivate or remove) * Modify line properties (colour,
-thickness, style (solid, dashed, dotted)) ## Development Installation Most
-people probably want to just use the executable links above. However, to edit
-the code, clone this repo and install in editable mode using the command:
-```console $ pip install -e ".[dev]" ``` ## Help! Found a bug, or have an idea
-for a great new feature? Check out the [Issues](https://github.com/cfcurtis/
-pdfstitcher/issues) tab to see if it's an open issue, or submit a new one if
-it's not on the list.
+Installer.dmg) * [Download_on_Flathub] * Using pip: `pip install pdfstitcher`
+**Note: Requires Python <= 3.9.13**. As of February 2022, there is no wheel
+available for wxPython for 3.10. ## Translations: [Translation_status]
+PDFStitcher will detect system language settings and change localisation if
+supported. Previous versions can be found by clicking on the "releases" link to
+the right. Want to contribute a translation? PDFStitcher is now on [weblate!]
+(https://hosted.weblate.org/engage/pdfstitcher/). ## Features * Stitch together
+pages in any order with specified number of rows/columns * Rotate pages for
+stitching * Add a margin around the final output * Trim or overlap the edges of
+each page by a specified amount * Add blank pages by including zeros in the
+page list (e.g. 1-5,0,6-10) * Layers are automatically preserved if present in
+the source document * Exclude layers (either deactivate or remove) * Modify
+line properties (colour, thickness, style (solid, dashed, dotted)) ##
+Development Installation Most people probably want to just use the executable
+links above. However, to edit the code, clone this repo and install in editable
+mode using the command: ```console $ pip install -e . ``` ## Help! Found a bug,
+or have an idea for a great new feature? Check out the [Issues](https://
+github.com/cfcurtis/pdfstitcher/issues) tab to see if it's an open issue, or
+submit a new one if it's not on the list.
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/app.py` & `pdfstitcher-0.8b1/pdfstitcher/pdfstitcher.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/pdfstitcher/layerfilter.py` & `pdfstitcher-0.8b1/pdfstitcher/layerfilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     "RG": [0, 0, 0],
     "rg": [0, 0, 0],
     "K": pdf_ops.rgb_to_cmyk([0, 0, 0]),
     "k": pdf_ops.rgb_to_cmyk([0, 0, 0]),
     "d": pdf_ops.line_style_arr[0],
 }
 
-
 # helper functions to dump page to file for debugging
 def write_page(fname, page):
     with open(fname, "w") as f:
         commands = pikepdf.parse_content_stream(page)
         f.write(pikepdf.unparse_content_stream(commands).decode("pdfdoc"))
 
 
@@ -40,14 +39,15 @@
         pdf=None,
         keep_ocs="all",
         keep_non_oc=True,
         delete_ocgs=True,
         page_range=[],
         line_props={},
     ):
+
         self.pdf = pdf
         self.keep_ocs = keep_ocs
         self.keep_non_oc = keep_non_oc
         self.delete_ocgs = delete_ocgs
         self.objs_to_delete = []
         self.page_range = page_range
 
@@ -305,18 +305,18 @@
             if oc_names is None:
                 other_obs[key] = xobj
             elif any(name in self.keep_ocs for name in oc_names):
                 oc_obs[key] = xobj
 
         return oc_obs, other_obs
 
-    def run(self, progress_win=None):
+    def run(self, set_progress_range=None, update_progress=None, progress_was_cancelled=None):
         """
         The primary method to run the filter.
-        If called from PDFStitcher gui, the progress window will be updated.
+        If called from pdfstitcher.py, the progress window will be updated.
         Returns:
             pikepdf.Pdf: the filtered PDF
         """
         self.processed_objects = set()
 
         if "/OCProperties" not in self.pdf.Root.keys():
             return self.pdf
@@ -330,15 +330,15 @@
 
         # open a new copy of the input
         self.out_pdf = pikepdf.Pdf.open(self.pdf.filename)
         page_range = self.process_page_range()
         n_page = len(page_range)
 
         # initialize the progress window
-        progress_win and progress_win.SetRange(n_page)  # don't run if the callback is None
+        set_progress_range and set_progress_range(n_page)  # don't run if the callback is None
 
         # update the OC dictionaries
         parse_streams = self.delete_ocgs and self.keep_ocs != "all"
         # update_ocs modifies the keep_ocs list if it was previously 'all'!
         self.update_ocs()
 
         if self.line_props != {}:
@@ -348,20 +348,20 @@
         # Either deleting content or modifying line properties requires parsing streams
         if parse_streams:
             for p in page_range:
                 # reset the state before each page
                 self.initialize_state()
                 self.filter_content(self.out_pdf.pages[p - 1])
                 # update the progress bar for each page, then check if user cancelled
-                progress_win and progress_win.Update(page_range.index(p))
-                if progress_win and progress_win.WasCancelled():
+                update_progress and update_progress(page_range.index(p))
+                if progress_was_cancelled and progress_was_cancelled():
                     return None
 
         # done, update progress and strip out unused stuff
-        progress_win and progress_win.Update(n_page)
+        update_progress and update_progress(n_page)
         self.out_pdf.remove_unreferenced_resources()
         return self.out_pdf
 
     def filter_stream(self, ob, current_layer_name=""):
         """
         Filters the stream itself (page or form)
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/cs_CZ/LC_MESSAGES/pdfstitcher.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-05-27 15:19+0000\n"
 "Last-Translator: Charlotte Curtis <c.f.curtis@gmail.com>\n"
 "Language: cs_CZ\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/pdfstitcher/user-"
 "interface/cs/>\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
@@ -31,14 +31,17 @@
 
 msgid "Bottom to top"
 msgstr "Zdola nahoru"
 
 msgid "Cannot open file"
 msgstr "Nemůže otevřít soubor"
 
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr "Nelze přepsat vstupní PDF, prosím vyberte jiný soubor pro výstupní PDF"
+
 msgid "Centimetres"
 msgstr "Centimetry"
 
 msgid "Clockwise"
 msgstr "O 90° doprava"
 
 msgid "Columns then rows"
@@ -58,14 +61,17 @@
 
 msgid "Deselected layers:"
 msgstr "Neoznačené vrstvy:"
 
 msgid "Dotted"
 msgstr "Tečkovaná"
 
+msgid "Exception"
+msgstr "Výjimka"
+
 msgid "Generate PDF"
 msgstr "Vytvořit PDF"
 
 msgid "Hide"
 msgstr "Skrýt"
 
 msgid "Inches"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/da/LC_MESSAGES/pdfstitcher.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-02-25 12:58+0000\n"
 "Last-Translator: Anne Lindholt <anneloppe@gmail.com>\n"
 "Language: da\n"
 "Language-Team: Danish <https://hosted.weblate.org/projects/pdfstitcher/user-"
 "interface/da/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -34,14 +34,18 @@
 
 msgid "Bottom to top"
 msgstr "Nedefra og op"
 
 msgid "Cannot open file"
 msgstr "Kan ikke åbne fil"
 
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr ""
+"Kan ikke overskrive input-PDF, vælg venligst en anden fil til output-PDF"
+
 msgid "Centimetres"
 msgstr "Centimeter"
 
 msgid "Clockwise"
 msgstr "Med uret"
 
 msgid "Columns then rows"
@@ -61,14 +65,17 @@
 
 msgid "Deselected layers:"
 msgstr "Fravalgte lag:"
 
 msgid "Dotted"
 msgstr "Prikket"
 
+msgid "Exception"
+msgstr "Undtagelse"
+
 msgid "Generate PDF"
 msgstr "Generér PDF"
 
 msgid "Hide"
 msgstr "Skjul"
 
 msgid "Horizontal alignment"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/de_DE/LC_MESSAGES/pdfstitcher.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-02-16 22:57+0000\n"
 "Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
 "Language: de_DE\n"
 "Language-Team: German <https://hosted.weblate.org/projects/pdfstitcher/user-"
 "interface/de/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -31,14 +31,19 @@
 
 msgid "Bottom to top"
 msgstr "Unten nach oben"
 
 msgid "Cannot open file"
 msgstr "Datei kann nicht geöffnet werden"
 
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr ""
+"Die Quelldatei kann nicht überschrieben werden, bitte einen andern Pfad für "
+"die Ausgabe wählen"
+
 msgid "Centimetres"
 msgstr "Zentimeter"
 
 msgid "Clockwise"
 msgstr "Rechts"
 
 msgid "Columns then rows"
@@ -58,14 +63,17 @@
 
 msgid "Deselected layers:"
 msgstr "Abgewählte Ebenen:"
 
 msgid "Dotted"
 msgstr "Gepunktet"
 
+msgid "Exception"
+msgstr "Fehler"
+
 msgid "Generate PDF"
 msgstr "PDF erstellen"
 
 msgid "Hide"
 msgstr "Verstecken"
 
 msgid "Horizontal alignment"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/fr_FR/LC_MESSAGES/pdfstitcher.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-02-16 22:57+0000\n"
 "Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
 "Language: fr_FR\n"
 "Language-Team: French <https://hosted.weblate.org/projects/pdfstitcher/user-"
 "interface/fr/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
@@ -34,14 +34,19 @@
 
 msgid "Bottom to top"
 msgstr "De bas en haut"
 
 msgid "Cannot open file"
 msgstr "Impossible d'ouvrir le fichier"
 
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr ""
+"Impossible d'écrire sur le fichier source, choississez un autre nom de "
+"fichier pour la destination"
+
 msgid "Centimetres"
 msgstr "Centimètres"
 
 msgid "Clockwise"
 msgstr "Horaire"
 
 msgid "Columns then rows"
@@ -61,14 +66,17 @@
 
 msgid "Deselected layers:"
 msgstr "Tout désélectionner :"
 
 msgid "Dotted"
 msgstr "Pointillés"
 
+msgid "Exception"
+msgstr "Erreur"
+
 msgid "Generate PDF"
 msgstr "Générer un PDF"
 
 msgid "Hide"
 msgstr "Masquer"
 
 msgid "Horizontal alignment"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-02-22 21:29+0100\n"
 "Last-Translator: \n"
 "Language: hu_HU\n"
 "Language-Team: hu_HU <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -33,14 +33,17 @@
 
 msgid "Bottom to top"
 msgstr "Lentről felfelé"
 
 msgid "Cannot open file"
 msgstr "A kiválasztott fájlt nem lehet megnyitni"
 
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr "A bemeneti fájl nem írható fölül, válasszon másik fájlt a kimenethez"
+
 msgid "Centimetres"
 msgstr "Centiméter"
 
 msgid "Clockwise"
 msgstr "Óramutató járásával megegyezően"
 
 msgid "Columns then rows"
@@ -60,14 +63,17 @@
 
 msgid "Deselected layers:"
 msgstr "Ki nem jelölt rétegek:"
 
 msgid "Dotted"
 msgstr "Pontozott"
 
+msgid "Exception"
+msgstr "Kivéve"
+
 msgid "Generate PDF"
 msgstr "PDF létrehozása"
 
 msgid "Hide"
 msgstr "Elrejtése"
 
 msgid "Horizontal alignment"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-03-01 18:59+0000\n"
 "Last-Translator: Enrica <enui.mail@gmail.com>\n"
 "Language: it\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/pdfstitcher/user-"
 "interface/it/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -34,14 +34,19 @@
 
 msgid "Bottom to top"
 msgstr "Dal basso all'alto"
 
 msgid "Cannot open file"
 msgstr "Impossibile aprire il file"
 
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr ""
+"Impossibile sovrascrivere il file origine, per favore scegliere un nome file "
+"differente"
+
 msgid "Centimetres"
 msgstr "Centimetri"
 
 msgid "Clockwise"
 msgstr "In senso orario"
 
 msgid "Columns then rows"
@@ -61,14 +66,17 @@
 
 msgid "Deselected layers:"
 msgstr "Livelli deselezionati:"
 
 msgid "Dotted"
 msgstr "Punteggiato"
 
+msgid "Exception"
+msgstr "Eccezione"
+
 msgid "Generate PDF"
 msgstr "Generare PDF"
 
 msgid "Hide"
 msgstr "Nascondi"
 
 msgid "Horizontal alignment"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-02-16 22:57+0000\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language: nb_NO\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
 "pdfstitcher/user-interface/nb_NO/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -49,14 +49,17 @@
 
 msgid "Deselect all"
 msgstr "Fravelg alt"
 
 msgid "Deselected layers:"
 msgstr "Fravalgte lag:"
 
+msgid "Exception"
+msgstr "Unntak"
+
 msgid "Generate PDF"
 msgstr "Generer PDF"
 
 msgid "Hide"
 msgstr "Skjul"
 
 msgid "Horizontal alignment"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,25 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
-"PO-Revision-Date: 2023-02-26 08:35+0000\n"
-"Last-Translator: ssantos <ssantos@web.de>\n"
-"Language: pt\n"
-"Language-Team: Portuguese <https://hosted.weblate.org/projects/pdfstitcher/"
-"user-interface/pt/>\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
+"PO-Revision-Date: 2022-02-25 12:58+0000\n"
+"Last-Translator: Adriano de Souza Xavier <adrianosoxav@gmail.com>\n"
+"Language: pt_BR\n"
+"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
+"pdfstitcher/user-interface/pt_BR/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.8.0\n"
 
 msgid "Amount to trim from each page"
-msgstr "Quantidade para cortar de cada página"
+msgstr "Quantidade pra cortar de cada página"
 
 msgid "Amount to trim from edges"
 msgstr "Quantidade para aparar das bordas"
 
 msgid "Apply"
 msgstr "Aplicar"
 
@@ -32,64 +32,51 @@
 msgid "Bottom"
 msgstr "Baixo"
 
 msgid "Bottom to top"
 msgstr "De baixo para cima"
 
 msgid "Cannot open file"
-msgstr "Não foi possível abrir o ficheiro"
+msgstr "Não foi possível abrir o arquivo"
+
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr ""
+"Não posso sobrescrever o arquivo de entrada, por favor selecione um arquivo "
+"diferente como saída"
 
 msgid "Centimetres"
 msgstr "Centímetros"
 
-msgid "Check for updates"
-msgstr "Verificar se há atualizações"
-
-msgid "Check for updates on startup"
-msgstr "Verificar se há atualizações na inicialização"
-
-msgid "Checking for updates"
-msgstr "A verificar se há atualizações"
-
-msgid "Choose a directory"
-msgstr "Escolha um diretório"
-
 msgid "Clockwise"
 msgstr "Sentido horário"
 
 msgid "Columns then rows"
 msgstr "Colunas e depois linhas"
 
-msgid "Could not copy to clipboard"
-msgstr "Não foi possível copiar para a área de transferência"
-
 msgid "Counterclockwise"
 msgstr "Sentido anti-horário"
 
 msgid "Dashed"
 msgstr "Tracejadas"
 
-msgid "Default open directory"
-msgstr "Diretório padrão para abrir"
-
-msgid "Default save directory"
-msgstr "Diretório padrão para gravar"
-
 msgid "Delete"
 msgstr "Deletar"
 
 msgid "Deselect all"
 msgstr "Desmarcar tudo"
 
 msgid "Deselected layers:"
 msgstr "Camadas não selecionadas:"
 
 msgid "Dotted"
 msgstr "Pontilhada"
 
+msgid "Exception"
+msgstr "Exceção"
+
 msgid "Generate PDF"
 msgstr "Gerar PDF"
 
 msgid "Hide"
 msgstr "Esconder"
 
 msgid "Horizontal alignment"
@@ -101,15 +88,15 @@
 msgid "Include non-optional content"
 msgstr "Incluir conteúdo não opcional"
 
 msgid "Input document not loaded"
 msgstr "O documento de entrada não foi carregado"
 
 msgid "Input filename (pdf)"
-msgstr "Nome do ficheiro de entrada (PDF)"
+msgstr "Nome do arquivo de entrada (PDF)"
 
 msgid "Invalid input"
 msgstr "Entrada inválida"
 
 msgid "Invalid rotation value"
 msgstr "Valor de rotação inválido"
 
@@ -179,44 +166,43 @@
 "Nota: If ambas linhas e colunas forem especificadas, as linhas serão "
 "ignoradas."
 
 msgid "Number of Columns"
 msgstr "Número de colunas"
 
 msgid "Number of columns in tiled grid."
-msgstr "Quantidade de colunas na grade lado a lado."
+msgstr "Número de colunas na grade lado a lado."
 
 msgid "Number of rows in tiled grid."
-msgstr "Quantidade de linhas na grade lado a lado."
+msgstr "Número de linhas na grade lado a lado."
 
 msgid "OR Number of Rows"
 msgstr "OU número de linhas"
 
 msgid "Only {} pages in document, skipping {}"
 msgstr "Apenas {} páginas no documento, pulando {}"
 
 msgid "Open the PDF and save selected page range without modifying"
 msgstr ""
-"Abre o PDF e salva o intervalo de páginas selecionado SEM modificar o "
-"ficheiro"
+"Abre o PDF e salva o intervalo de páginas selecionado SEM modificar o arquivo"
 
 msgid "Opening"
 msgstr "Abrindo"
 
 msgid "Optional Parameters"
 msgstr "Parâmetros opcionais"
 
 msgid "Options"
 msgstr "Opções"
 
 msgid "Output Options"
 msgstr "Opções de saída"
 
 msgid "Output filename (pdf)"
-msgstr "Nome do ficheiro de saída (PDF)"
+msgstr "Nome do arquivo de saída (PDF)"
 
 msgid "Output size:"
 msgstr "Tamanho da saída:"
 
 msgid "Overlap"
 msgstr "Sobreposição"
 
@@ -233,28 +219,28 @@
 msgstr ""
 "As páginas são montadas na ordem especificada. 0 insere uma página em branco."
 
 msgid ""
 "Pages to tile. May be range or list (e.g. 1-5 or 1,3,5-7, etc). Default: "
 "entire document."
 msgstr ""
-"Páginas para pôr lado a lado. Pode ser um intervalo ou uma lista (ex: 1-5 ou "
-"1,3,5-7, etc.). Padrão: Usar o documento inteiro."
+"Páginas pra colocar lado a lado. Pode ser um intervalo ou uma lista (ex: 1-5 "
+"ou 1,3,5-7, etc.). Padrão: Usar o documento inteiro."
 
 msgid "Please specify a page range"
 msgstr "Por favor especifique um intervalo de páginas"
 
 msgid "Process Layers"
 msgstr "Processar camadas"
 
 msgid "Process layers and save without tiling pages"
-msgstr "Processar as camadas e gravar SEM pôr as páginas lado a lado"
+msgstr "Processar as camadas e salvar SEM colocar as páginas lado a lado"
 
 msgid "Process layers then tile pages and save"
-msgstr "Processar as camadas, pôr as páginas lado a lado e gravar"
+msgstr "Processar as camadas, colocar as páginas lado a lado e salvar"
 
 msgid "Required Parameters"
 msgstr "Parâmetros obrigatórios"
 
 msgid "Reset"
 msgstr "Redefinir"
 
@@ -273,54 +259,54 @@
 msgid "Rotation"
 msgstr "Rotação"
 
 msgid "Rows then columns"
 msgstr "Linhas e depois colunas"
 
 msgid "Save output as"
-msgstr "Gravar a saída como"
+msgstr "Salvar a saída como"
 
 msgid "Select all"
 msgstr "Selecionar tudo"
 
 msgid "Select input PDF"
 msgstr "Selecione o PDF de entrada"
 
 msgid "Select layers to include in output document."
-msgstr "Selecionar as camadas para incluir no documento de saída."
+msgstr "Selecionar as camadas pra incluir no documento de saída."
 
 msgid "Select line properties to modify"
-msgstr "Selecione as propriedades da linha para modificar"
+msgstr "Selecione as propriedades da linha pra modificar"
 
 msgid "Set TrimBox to MediaBox"
 msgstr "Definir TrimBox para o MediaBox"
 
 msgid "Solid"
 msgstr "Sólido"
 
 msgid "Something went wrong"
 msgstr "Alguma coisa deu errado"
 
 msgid "Successfully written to"
 msgstr "Gravado com sucesso em"
 
 msgid "Tile PDF pages into one document."
-msgstr "Páginas lado a lado num só documento."
+msgstr "Páginas lado a lado em um só documento."
 
 msgid "Tile Pages"
-msgstr "Pôr páginas lado a lado"
+msgstr "Colocar páginas lado a lado"
 
 msgid "Tile pages"
-msgstr "Pôr páginas lado a lado"
+msgstr "Colocar páginas lado a lado"
 
 msgid "Tile pages and save without processing layers"
-msgstr "Pôr as páginas lado a lado e gravar SEM processar as camadas"
+msgstr "Colocar as páginas lado a lado e salvar SEM processar as camadas"
 
 msgid "Tiling successful"
-msgstr "As páginas foram postas lado a lado"
+msgstr "As páginas foram colocadas lado a lado"
 
 msgid "Tiling with {} rows and {} columns"
 msgstr "Páginas lado a lado com {} linhas e {} colunas"
 
 msgid "To insert a blank page, include a zero in the page list."
 msgstr "Para inserir uma página em branco, inclua um zero na lista de páginas."
 
@@ -349,16 +335,16 @@
 msgstr "Aviso! A saída é maior do que {} {}, talvez não abra corretamente."
 
 msgid ""
 "Warning: Some pages have been scaled because a target size was set. You "
 "should not see this warning if using the PDFStitcher GUI."
 msgstr ""
 "Aviso: Algumas páginas foram esticadas porque um tamanho alvo foi "
-"configurado. Não deveria ver esse aviso se estiver usando o PDFStitcher com "
-"interface gráfica."
+"configurado. Você não deveria ver esse aviso se estiver usando o PDFStitcher "
+"com interface gráfica."
 
 msgid "Warning: The pages {} have a different size than the page before"
 msgstr "Aviso: As páginas {} têm um tamanho diferente da página anterior"
 
 msgid "Warning: requested {} columns, but there are only {} pages"
 msgstr "Aviso: Foram requisitadas {} colunas, mas só têm {} páginas"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/es_ES/LC_MESSAGES/pdfstitcher.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,366 +1,377 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
-"PO-Revision-Date: 2022-02-25 12:58+0000\n"
-"Last-Translator: Adriano de Souza Xavier <adrianosoxav@gmail.com>\n"
-"Language: pt_BR\n"
-"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
-"pdfstitcher/user-interface/pt_BR/>\n"
-"Plural-Forms: nplurals=2; plural=n > 1\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
+"PO-Revision-Date: 2023-01-20 14:35+0000\n"
+"Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
+"Language: es_ES\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/pdfstitcher/user-"
+"interface/es/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.8.0\n"
 
 msgid "Amount to trim from each page"
-msgstr "Quantidade pra cortar de cada página"
+msgstr "Margen a recortar de cada página"
 
 msgid "Amount to trim from edges"
-msgstr "Quantidade para aparar das bordas"
+msgstr "La cantidad a recortar de los bordes"
 
 msgid "Apply"
 msgstr "Aplicar"
 
 msgid "Apply to"
-msgstr "Aplicar à"
+msgstr "Aplicar a"
 
 msgid "Apply to checked"
-msgstr "Aplicar aos que estão marcados"
+msgstr "Aplicar a selección"
 
 msgid "Bottom"
-msgstr "Baixo"
+msgstr "Abajo"
 
 msgid "Bottom to top"
-msgstr "De baixo para cima"
+msgstr "De Abajo hacia arriba"
 
 msgid "Cannot open file"
-msgstr "Não foi possível abrir o arquivo"
+msgstr "No se puede abrir el archivo"
+
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr ""
+"No se puede sobreescribir el archivo original, por favor selecciona un ombre "
+"diferente"
 
 msgid "Centimetres"
 msgstr "Centímetros"
 
 msgid "Clockwise"
-msgstr "Sentido horário"
+msgstr "Sentido horario"
 
 msgid "Columns then rows"
-msgstr "Colunas e depois linhas"
+msgstr "Columnas luego Filas"
 
 msgid "Counterclockwise"
-msgstr "Sentido anti-horário"
+msgstr "Sentido anti-horario"
 
 msgid "Dashed"
-msgstr "Tracejadas"
+msgstr "Guiones"
 
 msgid "Delete"
-msgstr "Deletar"
+msgstr "Borrar"
 
 msgid "Deselect all"
-msgstr "Desmarcar tudo"
+msgstr "Deseleccionar todo"
 
 msgid "Deselected layers:"
-msgstr "Camadas não selecionadas:"
+msgstr "Capas no seleccionadas:"
 
 msgid "Dotted"
-msgstr "Pontilhada"
+msgstr "Punteada"
+
+msgid "Exception"
+msgstr "Excepción"
 
 msgid "Generate PDF"
-msgstr "Gerar PDF"
+msgstr "Generar PDF"
 
 msgid "Hide"
-msgstr "Esconder"
+msgstr "Ocultar"
 
 msgid "Horizontal alignment"
-msgstr "Alinhamento horizontal"
+msgstr "Alineación horizontal"
 
 msgid "Inches"
-msgstr "Polegadas"
+msgstr "Pulgadas"
 
 msgid "Include non-optional content"
-msgstr "Incluir conteúdo não opcional"
+msgstr "Incluir contenido no opcional"
 
 msgid "Input document not loaded"
-msgstr "O documento de entrada não foi carregado"
+msgstr "Documento a combinar no cargado"
 
 msgid "Input filename (pdf)"
-msgstr "Nome do arquivo de entrada (PDF)"
+msgstr "Nombre del archivo de entrada (pdf)"
 
 msgid "Invalid input"
-msgstr "Entrada inválida"
+msgstr "Selección invalida"
 
 msgid "Invalid rotation value"
-msgstr "Valor de rotação inválido"
+msgstr "Valor de rotación no válido"
 
 msgid "Invalid trim value specified, ignoring"
-msgstr "O valor especificado para os aparos é inválido, ignorando"
+msgstr "Valor de recorte especificado no válido, ignorando"
 
 msgid "Layer Name"
-msgstr "Nome da Camada"
+msgstr "Nombre de la capa"
 
 msgid "Layers"
-msgstr "Camadas"
+msgstr "Capas"
 
 msgid "Left"
-msgstr "Esquerda"
+msgstr "Izquierda"
 
 msgid "Left to right"
-msgstr "Da esquerda para a direita"
+msgstr "Izquierda a Derecha"
 
 msgid "Line Colour"
-msgstr "Cor da linha"
+msgstr "Color de línea"
 
 msgid "Line Properties"
-msgstr "Propriedades da linha"
+msgstr "Propiedades de la línea"
 
 msgid "Line Style"
-msgstr "Estilo da linha"
+msgstr "Estilo de línea"
 
 msgid "Line Thickness"
-msgstr "Espessura da linha"
+msgstr "Grueso de línea"
 
 msgid "Load PDF to view layers."
-msgstr "Carregar o PDF para ver as camadas."
+msgstr "Cargar PDF para ver las capas."
 
 msgid "Make sure  isn't open in another program"
-msgstr "Garanta que  não está aberto em outro programa"
+msgstr "Asegúrese de que no está abierto en otro programa"
 
 msgid "Margin size in inches."
-msgstr "Tamanho da margem em polegadas."
+msgstr "Tamaño del margen en pulgadas."
 
 msgid "Margin to add to final output"
-msgstr "Margem para adicionar à saída final"
+msgstr "Margen para agregar alrededor del patron final"
 
 msgid "Margins"
-msgstr "Margens"
+msgstr "Margenes"
 
 msgid "May help fix things when output is not as expected"
-msgstr "Pode ajudar a corrigir as coisas quando a saída não é a esperada"
+msgstr ""
+"Puede arreglar algunas cosas cuando el archivo final no es como se esperaba"
 
 msgid "Middle"
-msgstr "Meio"
+msgstr "Medio"
 
 msgid "No layers found in input document."
-msgstr "Nenhuma camada encontrada no documento de entrada."
+msgstr "No se encontraron capas en el documento ingresado."
 
 msgid "No layers selected, generated PDF would be blank."
-msgstr "Nenhuma camada selecionada, será gerado um PDF em branco."
+msgstr "No hay capas seleccionadas, el PDF generado estara en blanco."
 
 msgid "No page range specified, defaulting to all"
-msgstr ""
-"Nenhum intervalo de páginas especificado, usaremos o valor padrão: todas"
+msgstr "No se especifico un rango de paginas, se usaran todas"
 
 msgid "None"
-msgstr "Nenhum"
+msgstr "Nada"
 
 msgid "Note: If both rows and columns are specified, rows are ignored."
 msgstr ""
-"Nota: If ambas linhas e colunas forem especificadas, as linhas serão "
-"ignoradas."
+"Nota: Si se especifican tanto filas como columnas, se ignoran las filas."
 
 msgid "Number of Columns"
-msgstr "Número de colunas"
+msgstr "Numero de Columnas"
 
 msgid "Number of columns in tiled grid."
-msgstr "Número de colunas na grade lado a lado."
+msgstr "Número de columnas en la cuadrícula de mosaicos."
 
 msgid "Number of rows in tiled grid."
-msgstr "Número de linhas na grade lado a lado."
+msgstr "Número de filas de la cuadrícula en mosaico."
 
 msgid "OR Number of Rows"
-msgstr "OU número de linhas"
+msgstr "O Número de filas"
 
 msgid "Only {} pages in document, skipping {}"
-msgstr "Apenas {} páginas no documento, pulando {}"
+msgstr "Solo hay {} páginas en el documento, omitiendo {}"
 
 msgid "Open the PDF and save selected page range without modifying"
-msgstr ""
-"Abre o PDF e salva o intervalo de páginas selecionado SEM modificar o arquivo"
+msgstr "Abrir el PDF y guardar las paginas seleccionadas sin modificar"
 
 msgid "Opening"
-msgstr "Abrindo"
+msgstr "Abriendo"
 
 msgid "Optional Parameters"
-msgstr "Parâmetros opcionais"
+msgstr "Párametros Opcionales"
 
 msgid "Options"
-msgstr "Opções"
+msgstr "Opciones"
 
 msgid "Output Options"
-msgstr "Opções de saída"
+msgstr "Opciones de salida"
 
 msgid "Output filename (pdf)"
-msgstr "Nome do arquivo de saída (PDF)"
+msgstr "Fichero de salida (pdf)"
 
 msgid "Output size:"
-msgstr "Tamanho da saída:"
+msgstr "Tamaño de salida:"
 
 msgid "Overlap"
-msgstr "Sobreposição"
+msgstr "Traslapar"
 
 msgid "Page Range"
-msgstr "Intervalo de Páginas"
+msgstr "Rango de páginas"
 
 msgid "Page Rotation"
-msgstr "Rotação da página"
+msgstr "Rotación de página"
 
 msgid "Page order"
-msgstr "Ordem das páginas"
+msgstr "Orden de las páginas"
 
 msgid "Pages assemble in specified order. 0 inserts a blank page."
 msgstr ""
-"As páginas são montadas na ordem especificada. 0 insere uma página em branco."
+"Las páginas se ensamblan en el orden especificado. Use 0 para insertar una "
+"página en blanco."
 
 msgid ""
 "Pages to tile. May be range or list (e.g. 1-5 or 1,3,5-7, etc). Default: "
 "entire document."
 msgstr ""
-"Páginas pra colocar lado a lado. Pode ser um intervalo ou uma lista (ex: 1-5 "
-"ou 1,3,5-7, etc.). Padrão: Usar o documento inteiro."
+"Páginas a embaldosar. Puede ser un rango o una lista (por ejemplo, 1-5 o "
+"1,3,5-7, etc). Por defecto: todo el documento."
 
 msgid "Please specify a page range"
-msgstr "Por favor especifique um intervalo de páginas"
+msgstr "Por favor especifique un rango de paginas"
 
 msgid "Process Layers"
-msgstr "Processar camadas"
+msgstr "Procesar capas"
 
 msgid "Process layers and save without tiling pages"
-msgstr "Processar as camadas e salvar SEM colocar as páginas lado a lado"
+msgstr "Edite y guarde capas sin fusionar páginas"
 
 msgid "Process layers then tile pages and save"
-msgstr "Processar as camadas, colocar as páginas lado a lado e salvar"
+msgstr "Procesar capas, juntar paginas y guardar"
 
 msgid "Required Parameters"
-msgstr "Parâmetros obrigatórios"
+msgstr "Parámetros Requeridos"
 
 msgid "Reset"
-msgstr "Redefinir"
+msgstr "Reiniciar"
 
 msgid "Reset checked"
-msgstr "Redefinir os que estão marcados"
+msgstr "Reiniciar selección"
 
 msgid "Right"
-msgstr "Direita"
+msgstr "Derecha"
 
 msgid "Right to left"
-msgstr "Da direta para a esquerda"
+msgstr "Derecha a Izquierda"
 
 msgid "Rotate pages (90, 180, or 270 degrees)"
-msgstr "Girar páginas (90, 180 ou 270 graus)"
+msgstr "Girar páginas (90, 180 o 270 grados)"
 
 msgid "Rotation"
-msgstr "Rotação"
+msgstr "Rotación"
 
 msgid "Rows then columns"
-msgstr "Linhas e depois colunas"
+msgstr "Filas luego Columnas"
 
 msgid "Save output as"
-msgstr "Salvar a saída como"
+msgstr "Guardar el nuevo PDF como"
 
 msgid "Select all"
-msgstr "Selecionar tudo"
+msgstr "Seleccionar todo"
 
 msgid "Select input PDF"
-msgstr "Selecione o PDF de entrada"
+msgstr "Selecciona PDF a combinar"
 
 msgid "Select layers to include in output document."
-msgstr "Selecionar as camadas pra incluir no documento de saída."
+msgstr "Seleccione capas a incluir en el documento de salida."
 
 msgid "Select line properties to modify"
-msgstr "Selecione as propriedades da linha pra modificar"
+msgstr "Seleccione las propiedades de la línea a modificar"
 
 msgid "Set TrimBox to MediaBox"
-msgstr "Definir TrimBox para o MediaBox"
+msgstr "Cambiar TrimBox a MediaBox"
 
 msgid "Solid"
-msgstr "Sólido"
+msgstr "Solida"
 
 msgid "Something went wrong"
-msgstr "Alguma coisa deu errado"
+msgstr "Algo salió mal"
 
 msgid "Successfully written to"
-msgstr "Gravado com sucesso em"
+msgstr "Guardado exitosamente en"
 
 msgid "Tile PDF pages into one document."
-msgstr "Páginas lado a lado em um só documento."
+msgstr "Agrupa las páginas PDF en un documento."
 
 msgid "Tile Pages"
-msgstr "Colocar páginas lado a lado"
+msgstr "Juntar paginas"
 
 msgid "Tile pages"
-msgstr "Colocar páginas lado a lado"
+msgstr "Juntar paginas"
 
 msgid "Tile pages and save without processing layers"
-msgstr "Colocar as páginas lado a lado e salvar SEM processar as camadas"
+msgstr "Juntar paginas y guardar sin procesar capas"
 
 msgid "Tiling successful"
-msgstr "As páginas foram colocadas lado a lado"
+msgstr "Combinación exitosa"
 
 msgid "Tiling with {} rows and {} columns"
-msgstr "Páginas lado a lado com {} linhas e {} colunas"
+msgstr "Combinando con {} filas y {} columnas"
 
 msgid "To insert a blank page, include a zero in the page list."
-msgstr "Para inserir uma página em branco, inclua um zero na lista de páginas."
+msgstr ""
+"Para insertar una página en blanco, incluya un cero en la lista de páginas."
 
 msgid "Top"
-msgstr "Cima"
+msgstr "Arriba"
 
 msgid "Top to bottom"
-msgstr "De cima para baixo"
+msgstr "De Arriba hacia abajo"
 
 msgid "Trim"
-msgstr "Aparar"
+msgstr "Recortar"
 
 msgid "Turn Around"
-msgstr "Virar"
+msgstr "Dar la vuelta"
 
 msgid "Unable to open"
-msgstr "Não consegui abrir"
+msgstr "No es posible abrir el archivo"
 
 msgid "Units"
 msgstr "Unidades"
 
 msgid "Vertical alignment"
-msgstr "Alinhamento vertical"
+msgstr "Alineación vertical"
 
 msgid "Warning! Output is larger than {} {}, may not open correctly."
-msgstr "Aviso! A saída é maior do que {} {}, talvez não abra corretamente."
+msgstr ""
+"¡Advertencia! La salida es mayor que {} {}, es posible que no se abra "
+"correctamente."
 
 msgid ""
 "Warning: Some pages have been scaled because a target size was set. You "
 "should not see this warning if using the PDFStitcher GUI."
 msgstr ""
-"Aviso: Algumas páginas foram esticadas porque um tamanho alvo foi "
-"configurado. Você não deveria ver esse aviso se estiver usando o PDFStitcher "
-"com interface gráfica."
+"Advertencia: Algunas páginas se han escalado porque se ha establecido un "
+"tamaño objetivo. No debería ver esta advertencia si utiliza la interfaz "
+"gráfica de PDFStitcher."
 
 msgid "Warning: The pages {} have a different size than the page before"
-msgstr "Aviso: As páginas {} têm um tamanho diferente da página anterior"
+msgstr ""
+"Atención: Las páginas {} tienen un tamaño diferente al de la página anterior"
 
 msgid "Warning: requested {} columns, but there are only {} pages"
-msgstr "Aviso: Foram requisitadas {} colunas, mas só têm {} páginas"
+msgstr "Advertencia: se han solicitado {} columnas, pero sólo hay {} páginas"
 
 msgid "Warning: requested {} rows, but there are only {} pages"
-msgstr "Aviso: Foram requisitadas {} linhas, mas só têm {} páginas"
+msgstr "Advertencia: se han solicitado {} filas, pero sólo hay {} páginas"
 
 msgid "cm"
 msgstr "cm"
 
 msgid ""
 "given as left,right,top,bottom (e.g. 0.5,0,0.5,0 would trim half an inch "
 "from left and top)"
 msgstr ""
-"dado como esquerda,direita,superior,inferior (ex: 0.5,0,0.5,0 apararia meia "
-"polegada da esquerda e da parte superior)"
+"indicados como izquierda,derecha,arriba,abajo (por ejemplo, 0,5,0,0,5,0 "
+"recortaría media pulgada de la izquierda y la parte superior)"
 
 msgid "in"
-msgstr "pol"
+msgstr "pulg"
 
 msgid "only numeric values allowed"
-msgstr "Apenas valores numéricos são permitidos"
+msgstr "Solo se permiten valores numéricos"
 
 msgid "pt"
 msgstr "pt"
 
 msgid "unable to write to"
-msgstr "Incapaz de gravar em"
+msgstr "Imposible guardar en"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo` & `pdfstitcher-0.8b1/pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: pdfstitcher VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-02-24 10:30-0700\n"
+"POT-Creation-Date: 2021-10-04 11:04-0600\n"
 "PO-Revision-Date: 2022-02-20 18:57+0000\n"
 "Last-Translator: Oğuz Ersen <oguzersen@protonmail.com>\n"
 "Language: tr\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/pdfstitcher/user-"
 "interface/tr/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
@@ -34,14 +34,19 @@
 
 msgid "Bottom to top"
 msgstr "Aşağıdan yukarıya"
 
 msgid "Cannot open file"
 msgstr "Dosya açılamıyor"
 
+msgid "Cant overwrite input file, please select a different file for output"
+msgstr ""
+"Girdi dosyasının üzerine yazılamıyor, lütfen çıktı için farklı bir dosya "
+"seçin"
+
 msgid "Centimetres"
 msgstr "Santimetre"
 
 msgid "Clockwise"
 msgstr "Saat yönünde"
 
 msgid "Columns then rows"
@@ -61,14 +66,17 @@
 
 msgid "Deselected layers:"
 msgstr "Seçimi kaldırılan katmanlar:"
 
 msgid "Dotted"
 msgstr "Noktalı"
 
+msgid "Exception"
+msgstr "İstisna"
+
 msgid "Generate PDF"
 msgstr "PDF oluştur"
 
 msgid "Hide"
 msgstr "Gizle"
 
 msgid "Horizontal alignment"
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/pagefilter.py` & `pdfstitcher-0.8b1/pdfstitcher/pagefilter.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/pdfstitcher/pdf_operators.py` & `pdfstitcher-0.8b1/pdfstitcher/pdf_operators.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/pdfstitcher/resources/stitcher-icon.ico` & `pdfstitcher-0.8b1/pdfstitcher/resources/stitcher-icon.ico`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/pdfstitcher/tile_pages.py` & `pdfstitcher-0.8b1/pdfstitcher/tile_pages.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,24 +51,25 @@
         rows=None,
         cols=None,
         target_width=None,
         target_height=None,
         vertical_align=SW_ALIGN_V.BOTTOM,
         horizontal_align=SW_ALIGN_H.LEFT,
     ):
+
         self.in_doc = in_doc
 
         if isinstance(page_range, str):
             self.page_range = utils.parse_page_range(page_range)
         elif isinstance(page_range, (list, tuple)):
             self.page_range = page_range
         else:
             self.page_range = []
 
-        self.trim = trim
+        self.set_trim(trim)
         self.margin = margin
         self.rotation = rotation
         self.actually_trim = actually_trim
         self.override_trim = override_trim
 
         self.col_major = col_major
         self.right_to_left = right_to_left
@@ -86,29 +87,27 @@
         if self.target_width:
             self.target_width = Config.general["units"].units_to_px(self.target_width)
 
         # Optional vertical and horizontal alignment in case pages are non-uniform in size
         self.vertical_align = vertical_align
         self.horizontal_align = horizontal_align
 
-    @property
-    def trim(self):
-        return self._trim
-
-    @trim.setter
-    def trim(self, trim):
+    def set_trim(self, trim):
         if len(trim) == 1:
-            self._trim = [trim[0], trim[0], trim[0], trim[0]]
-        elif len(trim) == 2:
-            self._trim = [trim[0], trim[0], trim[1], trim[1]]
-        elif len(trim) == 4:
-            self._trim = trim
+            self.trim = [trim, trim, trim, trim]
+
+        if len(trim) == 2:
+            self.trim = [trim[0], trim[0], trim[1], trim[1]]
+
+        if len(trim) == 4:
+            self.trim = trim
+
         else:
             print(_("Invalid trim value specified, ignoring"))
-            self._trim = [0, 0, 0, 0]
+            self.trim = [0, 0, 0, 0]
 
     def show_options(self):
         # convert the margin and trim options into pixels
         # translation_note: in = "inches", cm = "centimetres"
         rotstr = _("None")
 
         if self.rotation == SW_ROTATION.CLOCKWISE:
@@ -150,41 +149,80 @@
         print("    " + _("Margins") + ": {} {}".format(self.margin, Config.general["units"]))
         print("    " + _("Trim") + ": {} {}".format(self.trim, Config.general["units"]))
         print("    " + _("Rotation") + ": {}".format(rotstr))
         print("    " + _("Page order") + ": {}, {}, {}".format(orderstr, lrstr, btstr))
         print("    " + _("Vertical alignment") + ": {}".format(alvstr))
         print("    " + _("Horizontal alignment") + ": {}".format(alhstr))
 
-    def build_pagelist(self, new_doc: pikepdf.Pdf, trim: list) -> tuple:
+    def run(
+        self,
+        rows=None,
+        cols=None,
+        target_width=None,
+        target_height=None,
+        vertical_align=None,
+        horizontal_align=None,
+    ):
         """
-        Loops through the pages and constructs the list of pages, their length/width, and XObjects.
-        Returns a tuple containing content_dict, pw, ph, page_names.
-        Still too much going on in this function!
+        The main function for tiling pages.
         """
-        # define the dictionary to store xobjects and the corresponding names (e.g. MC0, MC1, etc.)
+
+        # First, go through the pages and normalize the various boxes
+        for page in self.in_doc.pages:
+            utils.normalize_boxes(page)
+
+        if rows or cols:
+            self.rows = rows
+            self.cols = cols
+
+        if target_width is not None:
+            self.target_width = Config.general["units"].units_to_px(target_width)
+        if target_height is not None:
+            self.target_height = Config.general["units"].units_to_px(target_height)
+
+        if vertical_align is not None:
+            self.vertical_align = vertical_align
+        if horizontal_align is not None:
+            self.horizontal_align = horizontal_align
+
+        if self.in_doc is None:
+            print(_("Input document not loaded"))
+            return
+
+        # initialize a new document
+        new_doc = utils.init_new_doc(self.in_doc)
+
+        # define the dictionary to store xobjects
         content_dict = pikepdf.Dictionary({})
+
         page_names = []
         pw = []
         ph = []
 
         page_count = len(self.in_doc.pages)
+        trim = [Config.general["units"].units_to_px(t) for t in self.trim]
+
         # initialize the width/height indices based on page rotation
         page_rot = 0
 
         if "/Rotate" in self.in_doc.Root.Pages.keys():
             page_rot = self.in_doc.Root.Pages.Rotate % 360
 
         for p in self.page_range:
             if p > 0:
                 break
 
         # get a pointer to the reference page and parse out the width and height
         ref_page = self.in_doc.pages[p - 1]
         ref_width, ref_height = utils.get_page_dims(ref_page, page_rot)
 
+        user_unit = 1
+        if "/UserUnit" in ref_page.keys():
+            user_unit = float(ref_page.UserUnit)
+
         different_size = set()
 
         for p in self.page_range:
             if p > page_count:
                 print(_("Only {} pages in document, skipping {}").format(page_count, p))
                 continue
 
@@ -233,15 +271,14 @@
                 if abs(p_width - ref_width) > 1 or abs(p_height - ref_height) > 1:
                     different_size.add(p)
 
                 # update the reference handles to be the current page
                 ref_width = p_width
                 ref_height = p_height
 
-                # magic sauce to copy the info to the new document as an XOBject
                 content_dict[pagekey] = new_doc.copy_foreign(new_page.as_form_xobject())
 
             else:
                 # blank page, use the reference for sizes and such
                 page_names.append(None)
                 pw.append(ref_width)
                 ph.append(ref_height)
@@ -249,71 +286,17 @@
         if len(different_size) > 0:
             print(
                 _("Warning: The pages {} have a different size than the page before").format(
                     different_size
                 )
             )
 
-        return content_dict, pw, ph, page_names
-
-    def adjust_trim_order(self, px_trim: list) -> None:
-        """
-        Rearranges the trim order based on page rotation.
-        """
-        # swap the trim order
-        # default: left,right,top,bottom
-        order = [0, 1, 2, 3]
-
-        if self.rotation == SW_ROTATION.CLOCKWISE:
-            order = [3, 2, 0, 1]
-        if self.rotation == SW_ROTATION.COUNTERCLOCKWISE:
-            order = [2, 3, 1, 0]
-        if self.rotation == SW_ROTATION.TURNAROUND:
-            order = [1, 0, 3, 2]
-
-        px_trim = [px_trim[o] for o in order]
-
-    def compute_target_size(self, n_tiles: int, pw: list, ph: list, trim: list) -> tuple:
-        """
-        Find the grid that contains the maximum page size for each row/col.
-        Returns the grid dimensions as a tuple of two lists.
-        """
-        col_width = [0] * self.cols
-        row_height = [0] * self.rows
-
-        if self.col_major:
-            for c in range(self.cols):
-                col_width[c] = max(pw[c * self.rows : c * self.rows + self.rows]) - (
-                    trim[0] + trim[1]
-                )
-
-            for r in range(self.rows):
-                row_height[r] = max(ph[r : n_tiles : self.cols]) - (trim[2] + trim[3])
-        else:
-            for r in range(self.rows):
-                row_height[r] = max(ph[r * self.cols : r * self.cols + self.cols]) - (
-                    trim[2] + trim[3]
-                )
-
-            for c in range(self.cols):
-                col_width[c] = max(pw[c : n_tiles : self.rows]) - (trim[0] + trim[1])
-
-        if self.right_to_left:
-            col_width.reverse()
-
-        if self.bottom_to_top:
-            row_height.reverse()
-
-        return col_width, row_height
+        n_tiles = len(page_names)
 
-    def calc_rows_cols(self, n_tiles: int) -> bool:
-        """
-        Calculate the number of rows/columns requested based on the number of pages to tile.
-        Returns True if the result is valid, False otherwise.
-        """
+        # check which one is specified
         if self.cols is not None and self.cols > 0:
             self.rows = math.ceil(n_tiles / self.cols)
             if self.rows == 1 and self.cols > n_tiles:
                 print(
                     _("Warning: requested {} columns, but there are only {} pages").format(
                         self.cols, n_tiles
                     )
@@ -330,114 +313,87 @@
                 )
                 self.rows = n_tiles
         else:
             # try for square
             self.cols = math.ceil(math.sqrt(n_tiles))
             self.rows = math.ceil(n_tiles / self.cols)
 
-        # Make sure there are no empty columns or rows
-        if self.col_major:
-            return self.cols * self.rows - n_tiles < self.rows
-        else:
-            return self.cols * self.rows - n_tiles < self.cols
-
-    def run(
-        self,
-        rows=None,
-        cols=None,
-        target_width=None,
-        target_height=None,
-        vertical_align=None,
-        horizontal_align=None,
-    ):
-        """
-        The main function for tiling pages.
-        """
-
-        if self.in_doc is None:
-            print(_("Input document not loaded"))
-            return
-
-        # First, go through the pages and normalize the various boxes
-        for page in self.in_doc.pages:
-            utils.normalize_boxes(page)
-
-        if rows or cols:
-            self.rows = rows
-            self.cols = cols
-
-        if target_width is not None:
-            self.target_width = Config.general["units"].units_to_px(target_width)
-        if target_height is not None:
-            self.target_height = Config.general["units"].units_to_px(target_height)
-
-        if vertical_align is not None:
-            self.vertical_align = vertical_align
-        if horizontal_align is not None:
-            self.horizontal_align = horizontal_align
+        # after calculating rows/cols but before reordering trim, show the user the selected options
+        self.show_options()
 
-        # initialize a new document
-        new_doc = utils.init_new_doc(self.in_doc)
+        # swap the trim order
+        # default: left,right,top,bottom
+        order = [0, 1, 2, 3]
 
-        # get the user unit from the first page (either 1 or 10, if it's a huge page)
-        user_unit = 1
-        first_page = self.in_doc.pages[self.page_range[0] - 1]
-        if "/UserUnit" in first_page.keys():
-            user_unit = float(first_page.UserUnit)
-
-        # define the trim in pdf units, then build the page list
-        px_trim = [Config.general["units"].units_to_px(t / user_unit) for t in self.trim]
-        content_dict, pw, ph, page_names = self.build_pagelist(new_doc, px_trim)
-        n_tiles = len(page_names)
-        if not self.calc_rows_cols(n_tiles):
-            error_msg = _(
-                "Error: cannot tile {} pages with {} rows and {} columns".format(
-                    n_tiles, self.rows, self.cols
-                )
-            )
-            if self.col_major:
-                error_msg += "\n" + _("filling columns first, the last column would be empty.")
-            else:
-                error_msg += "\n" + _("filling rows first, the last row would be empty.")
-            print(error_msg)
-            return
+        if self.rotation == SW_ROTATION.CLOCKWISE:
+            order = [3, 2, 0, 1]
+        if self.rotation == SW_ROTATION.COUNTERCLOCKWISE:
+            order = [2, 3, 1, 0]
+        if self.rotation == SW_ROTATION.TURNAROUND:
+            order = [1, 0, 3, 2]
 
-        # after calculating rows/cols but before reordering trim, show the user the selected options
-        self.show_options()
-        self.adjust_trim_order(px_trim)
+        trim = [Config.general["units"].units_to_px(t / user_unit) for t in self.trim]
+        trim = [trim[o] for o in order]
 
         if self.rotation in (SW_ROTATION.CLOCKWISE, SW_ROTATION.COUNTERCLOCKWISE):
             # swap width and height of pages
             ph, pw = pw, ph
 
+        width = 0
+        height = 0
+        col_width = [0] * self.cols
+        row_height = [0] * self.rows
+
         if self.target_width and self.target_height:
             # determine size of each page based on requested dimensions
             width = self.target_width
             height = self.target_height
             page_box_width = self.target_width / self.cols
             page_box_height = self.target_height / self.rows
             page_box_defined = True
         else:
-            col_width, row_height = self.compute_target_size(n_tiles, pw, ph, px_trim)
+            # Find the grid that contains the maximum page size for each row/col
+            if self.col_major:
+                for c in range(self.cols):
+                    col_width[c] = max(pw[c * self.rows : c * self.rows + self.rows]) - (
+                        trim[0] + trim[1]
+                    )
+
+                for r in range(self.rows):
+                    row_height[r] = max(ph[r : n_tiles : self.cols]) - (trim[2] + trim[3])
+            else:
+                for r in range(self.rows):
+                    row_height[r] = max(ph[r * self.cols : r * self.cols + self.cols]) - (
+                        trim[2] + trim[3]
+                    )
+
+                for c in range(self.cols):
+                    col_width[c] = max(pw[c : n_tiles : self.rows]) - (trim[0] + trim[1])
+
+            if self.right_to_left:
+                col_width.reverse()
+
+            if self.bottom_to_top:
+                row_height.reverse()
+
             width = sum(col_width)
             height = sum(row_height)
             page_box_defined = False
 
         # create a new document with a page big enough to contain all the tiled pages, plus requested margin
         margin = Config.general["units"].units_to_px(self.margin / user_unit)
         media_box = [
-            float(first_page.MediaBox[0]),
-            float(first_page.MediaBox[1]),
+            float(new_page.MediaBox[0]),
+            float(new_page.MediaBox[1]),
             width + 2 * margin,
             height + 2 * margin,
         ]
 
         utils.print_media_box(media_box)
 
-        # TODO: Refactor this giant loop into two functions (scale to fit and no scaling)
         i = 0
         content_txt = ""
         performed_scale = False
 
         # loop through all the page xobjects and place the non-empty ones
         for i in range(n_tiles):
             if not page_names[i]:
@@ -462,21 +418,21 @@
                 # calculate scaling factors based on source page size
                 source_width = pw[i]
                 source_height = ph[i]
                 scalef_width = page_box_width / source_width
                 scalef_height = page_box_height / source_height
                 # take the smaller scaling factor so that the page will fit into its box
                 scale_factor = min(scalef_width, scalef_height)
-                cpos_x0 = c * page_box_width - c * (px_trim[0] + px_trim[1])
+                cpos_x0 = c * page_box_width - c * (trim[0] + trim[1])
                 cpos_y0 = (self.rows - r - 1) * page_box_height - (self.rows - r - 1) * (
-                    px_trim[2] + px_trim[3]
+                    trim[2] + trim[3]
                 )
             else:
-                cpos_x0 = sum(col_width[:c]) - px_trim[0]
-                cpos_y0 = sum(row_height[r + 1 :]) - px_trim[3]
+                cpos_x0 = sum(col_width[:c]) - trim[0]
+                cpos_y0 = sum(row_height[r + 1 :]) - trim[3]
 
                 # store the page box height/width for convenience if rotation is needed
                 page_box_height = ph[i]
                 page_box_width = pw[i]
 
             # define the xobject position with reference to the origin at bottom left of page.
             x0 = margin + cpos_x0
@@ -564,14 +520,15 @@
 
         new_doc.pages.append(tiled_page)
 
         return new_doc
 
 
 def main(args):
+
     utils.setup_locale()
 
     # first try opening the document
     try:
         in_doc = pikepdf.Pdf.open(args.input)
     except:
         print(_("Unable to open") + " " + args.input)
@@ -580,33 +537,36 @@
     tiler = PageTiler(in_doc)
 
     if args.pages is not None:
         tiler.page_range = utils.parse_page_range(args.pages)
     else:
         tiler.page_range = [i + 1 for i in range(len(in_doc.pages))]
 
-    if args.units == "cm":
-        Config.general["units"] = utils.UNITS.CENTIMETERS
-
     if args.margin is not None:
+        # all the docs/examples seem to assume 72 dpi all the time
         tiler.margin = utils.txt_to_float(args.margin)
 
     if args.trim is not None:
         trim = [utils.txt_to_float(t) for t in args.trim.split(",")]
-        tiler.trim = trim
+        tiler.set_trim(trim)
 
-    r = int(args.rotate)
-    if r == 0:
-        tiler.rotation = SW_ROTATION.NONE
-    elif r == 90:
-        tiler.rotation = SW_ROTATION.CLOCKWISE
-    elif r == 180:
-        tiler.rotation = SW_ROTATION.TURNAROUND
-    elif r == 270:
-        tiler.rotation = SW_ROTATION.COUNTERCLOCKWISE
+    if args.rotate is not None:
+        failed = False
+        r = int(args.rotate)
+        if r == 0:
+            tiler.rotation = SW_ROTATION.NONE
+        elif r == 90:
+            tiler.rotation = SW_ROTATION.CLOCKWISE
+        elif r == 180:
+            tiler.rotation = SW_ROTATION.TURNAROUND
+        elif r == 270:
+            tiler.rotation = SW_ROTATION.COUNTERCLOCKWISE
+        else:
+            print(_("Invalid rotation value"))
+            sys.exit()
 
     tiler.cols = 0
     tiler.rows = 0
     if args.columns is not None:
         tiler.cols = int(args.columns)
 
     if args.rows is not None:
@@ -656,47 +616,35 @@
     parser.add_argument(
         "-c",
         "--columns",
         type=int,
         help=_("Number of columns in tiled grid."),
     )
     parser.add_argument(
-        "-u",
-        "--units",
-        choices=["in", "cm"],
-        default="in",
-        help=_("Units for margin and trim values."),
-    )
-    parser.add_argument(
         "-m",
         "--margin",
-        help=_("Margin size in selected units."),
+        help=_("Margin size in inches."),
     )
     parser.add_argument(
         "-t",
         "--trim",
-        help=_("Amount to trim from edges in selected units")
+        help=_("Amount to trim from edges")
         + " "
-        + _("given as left,right,top,bottom (e.g. 0.5,0,0.5,0 would trim 0.5 from left and top)"),
+        + _(
+            "given as left,right,top,bottom (e.g. 0.5,0,0.5,0 would trim half an inch from left and top)"
+        ),
     )
     parser.add_argument(
         "-R",
         "--rotate",
         type=int,
-        default=0,
-        choices=[0, 90, 180, 270],
-        help=_("Rotate pages"),
-    )
-    parser.add_argument(
-        "--col-major",
-        type=bool,
-        default=False,
-        help=_("Fill columns before rows (default is rows first)"),
+        help=_("Rotate pages (90, 180, or 270 degrees)"),
     )
 
     return parser.parse_args()
 
 
 if __name__ == "__main__":
+
     utils.setup_locale()
     args = parse_arguments()
     new_doc, success = main(args)
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/ui/dialogs.py` & `pdfstitcher-0.8b1/pdfstitcher/ui/dialogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import wx, wx.adv
 from pdfstitcher import utils
 from pdfstitcher.utils import Config
 from pdfstitcher import updater
 from pdfstitcher import bug_info
-from pathlib import Path
 from babel import Locale
 import webbrowser
 import yaml
 
 
 class UpdateDialog(wx.Dialog):
     """
@@ -225,44 +224,20 @@
             wx.TheClipboard.SetData(wx.TextDataObject(self.bug_report.GetValue()))
             wx.TheClipboard.Close()
         else:
             wx.MessageBox(_("Could not copy to clipboard"), _("Error"))
 
     def create_mangled_pdf(self, event):
         """Creates a mangled version of the input PDF."""
-        pdf = self.main_gui.in_doc
-        save_path = Path(pdf.filename).parent
-        with wx.DirDialog(
-            self,
-            _("Choose a location to save the mangled PDF"),
-            defaultPath=str(save_path),
-            style=wx.DD_DEFAULT_STYLE | wx.DD_DIR_MUST_EXIST,
-        ) as dlg:
-            if dlg.ShowModal() == wx.ID_OK:
-                save_path = Path(dlg.GetPath())
-            else:
-                return
-
-        progress_win = wx.ProgressDialog(
-            _("Mangling PDF with {} pages".format(len(pdf.pages))),
-            _("This may take some time, please wait"),
-            style=wx.PD_CAN_ABORT | wx.PD_AUTO_HIDE,
-        )
-        try:
-            pdf_path = bug_info.mangle_pdf(pdf, save_path, progress_win)
-        except InterruptedError:
-            print(_("Mangling PDF cancelled by user."))
-            progress_win.Update(progress_win.GetRange())
-            return
-
+        pdf_path = bug_info.mangle_pdf(self.main_gui.in_doc)
         if pdf_path:
             wx.MessageBox(
-                _("Mangled PDF saved to {}.".format(pdf_path))
-                + "\n\n"
-                + _("Please attach to GitHub issue or email."),
+                _("Mangled PDF saved to {}.\n\nPlease attach to GitHub issue or email.").format(
+                    pdf_path
+                ),
                 _("Success"),
             )
         else:
             wx.MessageBox(_("Failed to mangle PDF"), _("Error"))
 
     def open_issue(self, event):
         """
@@ -440,11 +415,11 @@
         Config.general["check_updates"] = self.check_updates.IsChecked()
 
         # save config
         Config.save()
 
         msg = _("Preferences saved to {}").format(Config.config_dir / Config.config_file)
         if language_change:
-            msg += "\n\n" + _("Please restart to switch to {}.".format(self.lang_combo.GetValue()))
+            msg += _("\n\nPlease restart to switch to {}.".format(self.lang_combo.GetValue()))
 
         wx.MessageBox(msg, _("Preferences saved"), wx.OK | wx.ICON_INFORMATION)
         self.Destroy()
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/ui/io_tab.py` & `pdfstitcher-0.8b1/pdfstitcher/ui/io_tab.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/pdfstitcher/ui/layers_tab.py` & `pdfstitcher-0.8b1/pdfstitcher/ui/layers_tab.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/pdfstitcher/ui/main_frame.py` & `pdfstitcher-0.8b1/pdfstitcher/ui/main_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,67 +166,90 @@
 
             # trim
             trim = [0.0] * 4
             trim[0] = utils.txt_to_float(self.tt.left_trim_txt.GetValue())
             trim[1] = utils.txt_to_float(self.tt.right_trim_txt.GetValue())
             trim[2] = utils.txt_to_float(self.tt.top_trim_txt.GetValue())
             trim[3] = utils.txt_to_float(self.tt.bottom_trim_txt.GetValue())
-            self.tiler.trim = trim
+            self.tiler.set_trim(trim)
             self.tiler.actually_trim = bool(self.tt.trim_overlap_combo.GetSelection())
             self.tiler.override_trim = self.tt.override_trim.GetValue()
 
             # rows/cols
             cols = self.tt.columns_txt.GetValue().strip()
             cols = int(cols) if cols else None
             rows = self.tt.rows_txt.GetValue().strip()
             rows = int(rows) if rows else None
 
         # do it
         try:
             if do_layers:
-                progress_win = wx.ProgressDialog(
-                    _("Processing layers"),
-                    _("Processing layers, please wait"),
-                    style=wx.PD_CAN_ABORT | wx.PD_AUTO_HIDE,
+                self.progress_win = wx.ProgressDialog(
+                    "Processing layers",
+                    "Processing layers, please wait",
+                    style=wx.PD_CAN_ABORT,
+                )
+                filtered = self.layer_filter.run(
+                    self.set_progress_range,
+                    self.update_progress,
+                    self.progress_was_cancelled,
                 )
-                filtered = self.layer_filter.run(progress_win)
             else:
                 filtered = self.in_doc
 
+            if self.progress_win:
+                self.update_progress(self.progress_win.GetRange())
+
             if filtered is None:
                 return
 
             if do_tile:
                 self.tiler.in_doc = filtered
                 new_doc = self.tiler.run(rows, cols)
-                if new_doc:
-                    print(_("Tiling successful"))
+                print(_("Tiling successful"))
             else:
                 # extract the requested pages
                 page_filter = PageFilter(filtered)
                 page_filter.page_range = page_range
                 page_filter.margin = utils.txt_to_float(self.io.margin_txt.GetValue())
                 new_doc = page_filter.run()
 
         except Exception as e:
             print(_("Something went wrong"))
             traceback.print_exc()
             return
 
         try:
-            if new_doc:
-                new_doc.save(self.out_doc_path)
-                print(_("Successfully written to") + " " + self.out_doc_path)
+            new_doc.save(self.out_doc_path)
+            print(_("Successfully written to") + " " + self.out_doc_path)
         except Exception as e:
             print(
                 _("Something went wrong") + ", " + _("unable to write to") + " " + self.out_doc_path
             )
             print(e)
             print(_("Make sure " + self.out_doc_path + " isn't open in another program"))
 
+    def progress_was_cancelled(self):
+        if self.progress_win != None:
+            return self.progress_win.WasCancelled()
+
+    def update_progress(self, val):
+        if self.progress_win != None:
+            p_range = self.progress_win.GetRange()
+            if p_range:
+                if val == p_range:
+                    # Hit the max, we're done
+                    self.progress_win = None
+                else:
+                    self.progress_win.Update(val)
+
+    def set_progress_range(self, val):
+        if self.progress_win != None:
+            self.progress_win.SetRange(val)
+
     def make_menu_bar(self):
         """
         Make and populate the menubar.
         """
         menu_bar = wx.MenuBar()
 
         # Make a file menu with load and exit items
@@ -332,14 +355,15 @@
         with wx.FileDialog(
             self,
             _("Save output as"),
             defaultDir=Config.general["save_dir"],
             wildcard="PDF files (*.pdf)|*.pdf",
             style=wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT,
         ) as fileDialog:
+
             if fileDialog.ShowModal() == wx.ID_CANCEL:
                 return
 
             pathname = fileDialog.GetPath()
             self.set_output_filename(pathname)
 
     def set_output_filename(self, pathname):
@@ -386,14 +410,15 @@
         with wx.FileDialog(
             self,
             _("Select input PDF"),
             defaultDir=Config.general["open_dir"],
             wildcard="PDF files (*.pdf)|*.pdf",
             style=wx.FD_OPEN | wx.FD_FILE_MUST_EXIST,
         ) as fileDialog:
+
             if fileDialog.ShowModal() == wx.ID_CANCEL:
                 return
 
             # Proceed loading the file chosen by the user
             pathname = fileDialog.GetPath()
             self.load_file(pathname)
 
@@ -467,21 +492,17 @@
     """
     Create the app and run it.
     """
     app = wx.App()
 
     # Fix the size for high-resolution displays on windows
     if sys.platform.startswith("win32"):
-        try:
-            from ctypes import OleDLL
+        from ctypes import OleDLL
 
-            OleDLL("shcore").SetProcessDpiAwareness(1)
-        except Exception:
-            # Probably Windows 7, or some other non-DPI aware issue
-            pass
+        OleDLL("shcore").SetProcessDpiAwareness(1)
 
     disp_size = wx.DisplaySize()
     app_size = wx.Size(min(int(disp_size[0] * 0.6), 700), min(int(disp_size[1] * 0.85), 800))
 
     frm = PDFStitcherFrame(None, title="PDF Stitcher" + " " + utils.VERSION_STRING, size=app_size)
     frm.SetSize(frm.FromDIP(app_size))
     frm.reset_sash_position()
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/ui/tile_tab.py` & `pdfstitcher-0.8b1/pdfstitcher/ui/tile_tab.py`

 * *Files identical despite different names*

### Comparing `pdfstitcher-0.8.5/pdfstitcher/update_loc.py` & `pdfstitcher-0.8b1/pdfstitcher/update_loc.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 def compile():
     print("**compile**")
     run(f"pybabel compile -D pdfstitcher -d {T}", shell=True)
 
 
 if __name__ == "__main__":
+
     args = parse_args()
 
     do_all = False
     if args.all or len(sys.argv) < 2:
         do_all = True
 
     if args.extract or do_all:
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/updater.py` & `pdfstitcher-0.8b1/pdfstitcher/updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,26 @@
 import requests
 from pdfstitcher import utils
 import os
 import packaging
 
 __version__ = importlib.metadata.version("pdfstitcher")
 
-
 def is_flatpak() -> bool:
     """
     Returns True if the app is running in a Flatpak sandbox.
     """
     return "FLATPAK_ID" in os.environ
 
-
 def update_available() -> str:
     """
     Checks whether there's a new release of PDFStitcher.
     Returns a string containing the latest version if there's a new one,
     or None if the current version is up to date.
-    """
+    """ 
     response = requests.get(utils.PYPI_HOME + "/json")
     if not response.ok:
         raise requests.HTTPError(response.status_code, response.url, response.reason)
 
     pypi_version = response.json()["info"]["version"]
 
     if packaging.version.parse(pypi_version) > packaging.version.parse(__version__):
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher/utils.py` & `pdfstitcher-0.8b1/pdfstitcher/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,36 +214,35 @@
         lang = lang
     # Then check just the language without country code
     elif lang[:2] in valid_langs:
         lang = lang[:2]
     elif lang[:2] == "sk":
         # fallback to Czech if Slovak is not available
         lang = "cs"
-        # Google Translate to Slovak, this might be kind of awful
-        language_warning = "Slovenský preklad nie je k dispozícii, predvolená je čeština"
+        language_warning = _("Slovak translation not available, defaulting to Czech")
     else:
         # check if there's a country code variant for the language
         for valid_lang in valid_langs:
             if lang[:2] in valid_lang:
                 lang = valid_lang
                 break
 
     try:
         translate = gettext.translation(
             "pdfstitcher", resource_path("locale"), languages=[lang], fallback=True
         )
         translate.install()
 
-        Config.general["language"] = lang
-        if not isinstance(translate, gettext.GNUTranslations) and "en" not in lang:
+        if isinstance(translate, gettext.GNUTranslations):
+            Config.general["language"] = lang
+        elif lang != "en":
             language_warning = f"Could not find translation for language {Locale(*lang.split('_')).display_name}, defaulting to English"
             Config.general["language"] = "en"
     except Exception as e:
         language_warning = e
-        Config.general["language"] = "en"
 
     return language_warning
 
 
 def txt_to_float(txt):
     """
     Convert a string to a float, or return None if it can't be converted.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher.egg-info/PKG-INFO` & `pdfstitcher-0.8b1/pdfstitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfstitcher
-Version: 0.8.5
+Version: 0.8b1
 Summary: The open source PDF stitching software for sewists, by sewists.
 Author: Charlotte Curtis
 Author-email: c.f.curtis@gmail.com
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
@@ -394,18 +394,17 @@
 
 Since version 0.4, it is also possible to select layers for inclusion/exclusion in the final output. Additionally, line properties can be modified for each layer if the input PDF is compatible.
 
 For up-to-date information, also check out https://www.pdfstitcher.org.
 
 ## Download the latest release
 * [Windows (7 or 10, 64-bit)](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/pdfstitcher.exe)
-* [macOS - Intel Processor](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-InstallerX64.dmg)
-* [macOS - M1/M2 Processor](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-InstallerARM64.dmg)
+* [macOS (High Sierra or higher)](https://github.com/cfcurtis/pdfstitcher/releases/latest/download/PDFStitcher-Installer.dmg)
 * <a href='https://flathub.org/apps/details/com.github.cfcurtis.pdfstitcher'><img width='120' alt='Download on Flathub' src='https://flathub.org/assets/badges/flathub-badge-en.svg'/></a>
-* Using pip: `pip install pdfstitcher` **Note: Requires Python <= 3.11**. As of November 2022, there is no wheel available for wxPython for 3.11+.
+* Using pip: `pip install pdfstitcher` **Note: Requires Python <= 3.9.13**. As of February 2022, there is no wheel available for wxPython for 3.10.
 
 ## Translations:
 
 <a href="https://hosted.weblate.org/engage/pdfstitcher/">
 <img src="https://hosted.weblate.org/widgets/pdfstitcher/-/287x66-grey.png" alt="Translation status" /></a>
 
 PDFStitcher will detect system language settings and change localisation if supported. 
@@ -424,12 +423,12 @@
 * Exclude layers (either deactivate or remove)
 * Modify line properties (colour, thickness, style (solid, dashed, dotted))
 
 ## Development Installation
 Most people probably want to just use the executable links above. However, to edit the code, clone this repo and install in editable mode using the command:
 
 ```console
-$ pip install -e ".[dev]"
+$ pip install -e .
 ```
 
 ## Help!
 Found a bug, or have an idea for a great new feature? Check out the [Issues](https://github.com/cfcurtis/pdfstitcher/issues) tab to see if it's an open issue, or submit a new one if it's not on the list.
```

### Comparing `pdfstitcher-0.8.5/pdfstitcher.egg-info/SOURCES.txt` & `pdfstitcher-0.8b1/pdfstitcher.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pdfstitcher/__init__.py
 pdfstitcher/__main__.py
-pdfstitcher/app.py
 pdfstitcher/bug_info.py
 pdfstitcher/layerfilter.py
 pdfstitcher/pagefilter.py
 pdfstitcher/pdf_operators.py
+pdfstitcher/pdfstitcher.py
 pdfstitcher/tile_pages.py
 pdfstitcher/update_loc.py
 pdfstitcher/updater.py
 pdfstitcher/utils.py
 pdfstitcher.egg-info/PKG-INFO
 pdfstitcher.egg-info/SOURCES.txt
 pdfstitcher.egg-info/dependency_links.txt
@@ -34,23 +34,20 @@
 pdfstitcher/locale/hu_HU/LC_MESSAGES/pdfstitcher.po
 pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.mo
 pdfstitcher/locale/it/LC_MESSAGES/pdfstitcher.po
 pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.mo
 pdfstitcher/locale/nb_NO/LC_MESSAGES/pdfstitcher.po
 pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.mo
 pdfstitcher/locale/nl_NL/LC_MESSAGES/pdfstitcher.po
-pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.mo
-pdfstitcher/locale/pt/LC_MESSAGES/pdfstitcher.po
 pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.mo
 pdfstitcher/locale/pt_BR/LC_MESSAGES/pdfstitcher.po
 pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.mo
 pdfstitcher/locale/tr/LC_MESSAGES/pdfstitcher.po
 pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.mo
 pdfstitcher/locale/zgh/LC_MESSAGES/pdfstitcher.po
 pdfstitcher/resources/stitcher-icon.ico
 pdfstitcher/ui/__init__.py
 pdfstitcher/ui/dialogs.py
 pdfstitcher/ui/io_tab.py
 pdfstitcher/ui/layers_tab.py
 pdfstitcher/ui/main_frame.py
-pdfstitcher/ui/tile_tab.py
-tests/test_tile_pages.py
+pdfstitcher/ui/tile_tab.py
```

### Comparing `pdfstitcher-0.8.5/pyproject.toml` & `pdfstitcher-0.8b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdfstitcher"
-version = "0.8.5"
+version = "0.8b1"
 description = "The open source PDF stitching software for sewists, by sewists."
 readme = "README.md"
 requires-python = ">=3.8, <3.11"
 license = {file = "LICENSE"}
 keywords = ["pdf", "sewing", "utility", "stitch", "n-up", "page imposition"]
 authors = [
     {name = "Charlotte Curtis"},
@@ -18,15 +18,15 @@
 dependencies = [
     "pikepdf >= 2.2.0",
     "wxPython >= 4.1",
     "Babel",
     "PyYAML",
     "appdirs",
     "requests",
-    "pdf-mangler >= 0.1.4",
+    "pdf-mangler",
     "psutil",
     "pyobjc ; platform_system=='Darwin'"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
@@ -35,15 +35,15 @@
 ]
 
 [project.urls]
 homepage = "https://www.pdfstitcher.org/"
 repository = "https://github.com/cfcurtis/pdfstitcher"
 
 [project.scripts]
-pdfstitcher = "pdfstitcher.app:main"
+pdfstitcher = "pdfstitcher.pdfstitcher:main"
 
 [build-system]
 requires = ["setuptools", "Babel"]
 # use legacy to force setup.py to run
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
```

### Comparing `pdfstitcher-0.8.5/setup.py` & `pdfstitcher-0.8b1/setup.py`

 * *Files identical despite different names*

